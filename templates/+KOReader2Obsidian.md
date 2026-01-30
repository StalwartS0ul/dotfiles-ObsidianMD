<%*
// The KOReader defined highlight styles vs callout mapping. Leave the keys as is, but you can edit the values to create your own convention.
const NOTE_STYLES = {
  lighten: {
	type: "quote",
	title: "Quote",
  },
  invert: {
	type: "important",
	title: "Resonance",
  },
  strikeout: {
	type: "danger",
	title: "Discord",
  },
  underscore: {
	type: "question",
	title: "Musings",
  },
};

function format_koreader_percentages(page, total) {
	if (page && total) {
		return `${((page / total) * 100).toFixed(2)}%`;
	}
	return "";
}

function format_koreader_json_highlights(content) {
	const data = JSON.parse(content);
    let output = `---
title: "${data.title}"
aliases: ["Notes from ${data.title}"]
author: "${data.author}"
---
# ${data.title}
##### ${data.author}`;
	let current_chapter = "";
	for (const entry of data.entries) {
	  if (entry.text) {
		if (entry.chapter != current_chapter) {
		  output += `\n\n## ${entry.chapter}\n`;
		  current_chapter = entry.chapter;
		}
		output += `\n### Page: ${
		  entry.page
		} (${format_koreader_percentages(
		  entry.page,
		  data.number_of_pages
		)}) @ ${window.moment.unix(entry.time).format("DD MMM YYYY hh:mm:ss A")}\n`;
		output += `\n${entry.text}`;
		const note_type = NOTE_STYLES[entry.drawer];
		output += `\n\n> [!${note_type.type}] ${note_type.title}`;
		if (entry.note) {
		  if (entry.note.length > 50) {
			output += `\n> ${entry.note}`;
		  } else {
			output += `: ${entry.note}`;
		  }
		  output += "\n";
		}
		output += "\n";
	  }
	}
	return output;
}

const content = await tp.system.prompt("Paste the JSON content", null, true, true);
const output = format_koreader_json_highlights(content);
let file = app.workspace.getActiveFile();
await app.vault.modify(file, output);
%>