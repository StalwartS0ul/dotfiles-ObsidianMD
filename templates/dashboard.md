---
cssclasses:
  - table-wrap
  - table-wide
  - table-center
---

<div style="display: flex; justify-content: center; padding: 80px 0 40px 0"><pre style ="font-family: monospace; margin: 0; line-height: 1; display: inline-block; color: #8A5CF6; background: none; border: none;">
 ██████╗ ██████╗ ███████╗██╗██████╗ ██╗ █████╗ ███╗   ██╗
██╔═══██╗██╔══██╗██╔════╝██║██╔══██╗██║██╔══██╗████╗  ██║
██║   ██║██████╔╝███████╗██║██║  ██║██║███████║██╔██╗ ██║
██║   ██║██╔══██╗╚════██║██║██║  ██║██║██╔══██║██║╚██╗██║
╚██████╔╝██████╔╝███████║██║██████╔╝██║██║  ██║██║ ╚████║
 ╚═════╝ ╚═════╝ ╚══════╝╚═╝╚═════╝ ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝
</pre></div>

##   Commands

<!-- Please choose which version you prefer nerd font or emoji -->
<!-- You can remove lines like this after you are done. They are not shown when in reading mode -->
<!-- Nerd font version, first row has description to guide you -->
<!-- You can also refer to https://i.imgur.com/yRNgeDI.png -->
<table style="width: 100%; border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><span style="color: #8A5CF6;">  </span> <span style="color: #DCD7BA;">Find File</span> </td><!-- icon color, icon, description -->
    <td style="text-align: right; border: none;"><code>⌘-F</code></td> <!-- shortcut command in code block -->
  </tr>
  <tr>
    <td style="border: none;"><span style="color: #8A5CF6;">  </span> <span style="color: #DCD7BA;">Quick Switch</span></td>
    <td style="text-align: right; border: none;"><code>⌘-o</code></td>
  </tr>
  <tr>
    <td style="border: none;"><span style="color: #8A5CF6;">  </span> <span style="color: #DCD7BA;">New File</span></td>
    <td style="text-align: right; border: none;"><code>⌘-N</code></td>
  </tr>
  <tr>
    <td style="border: none;"><span style="color: #8A5CF6;"> 󱁻 </span> <span style="color: #DCD7BA;">New File (Templater)</span></td>
    <td style="text-align: right; border: none;"><code>⌘-n</code></td>
  </tr>
  <tr>
    <td style="border: none;"><span style="color: #8A5CF6;">  </span> <span style="color: #DCD7BA;">Settings</span></td>
    <td style="text-align: right; border: none;"><code>⌘-,</code></td>
  </tr>
  <tr>
    <td style="border: none;"><span style="color: #8A5CF6;">  </span> <span style="color: #DCD7BA;">Quit</span></td>
    <td style="text-align: right; border: none;"><code>⌘-q</code></td>
  </tr>
</table>

<!-- Emoji version, first row has description to guide you -->
<table style="width: 100%; border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"> 🔍 <span style="color: #DCD7BA;">Find File</span> </td><!-- icon and description -->
    <td style="text-align: right; border: none;"><code>⌘-F</code></td> <!-- shortcut command in code block -->
  </tr>
  <tr>
    <td style="border: none;"> 🔄 <span style="color: #DCD7BA;">Quick Switch</span></td>
    <td style="text-align: right; border: none;"><code>⌘-o</code></td>
  </tr>
  <tr>
    <td style="border: none;"> 📝 <span style="color: #DCD7BA;">New File</span></td>
    <td style="text-align: right; border: none;"><code>⌘-N</code></td>
  </tr>
  <tr>
    <td style="border: none;"> 🗒️ <span style="color: #DCD7BA;">New File (Templater)</span></td>
    <td style="text-align: right; border: none;"><code>⌘-n</code></td>
  </tr>
  <tr>
    <td style="border: none;"> ⚙️ <span style="color: #DCD7BA;">Settings</span></td>
    <td style="text-align: right; border: none;"><code>⌘-,</code></td>
  </tr>
  <tr>
    <td style="border: none;"> ❌ <span style="color: #DCD7BA;">Quit</span></td>
    <td style="text-align: right; border: none;"><code>⌘-q</code></td>
  </tr>
</table>

##   Recent Files

```dataview
TABLE WITHOUT ID link(file.link, file.path) as " "
FROM "" WHERE file.name != this.file.name
SORT file.mtime DESC 
LIMIT 5
```

<div style="text-align: center; padding: 20px 0; color: #727169; font-size: 0.9em; opacity: 0.8; letter-spacing: 1px; font-style: italic;">
  [󱐋 One tool for one thing.]
</div>
