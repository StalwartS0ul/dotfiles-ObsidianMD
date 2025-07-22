# used with vimrc plugin, filename is .obsidian.vimrc

" row navigation
nmap j gj
nmap k gk

" remove search highlights
nmap <F9> :nohl<CR>

" yank to clipboard
set clipboard=unnamed

" join lines
unmap <Space>
nmap <Space>j :join<CR>

" NOTE obcommand needs to end in <CR> as of Obsidian 1.7.2

" [g]oto [f]ile (= Follow Link under cursor)
exmap followLinkUnderCursor obcommand editor:follow-link
nmap gf :followLinkUnderCursor<CR>

" Emulate Folding https://vimhelp.org/fold.txt.html#fold-commands
exmap togglefold obcommand editor:toggle-fold
nmap zo :togglefold<CR>

exmap unfoldall obcommand editor:unfold-all
nmap zR :unfoldall<CR>

exmap foldreduce obcommand editor:fold-less
nmap zr :foldreduce<CR>

exmap foldall obcommand editor:fold-all
nmap zM :foldall<CR>

exmap foldmore obcommand editor:fold-more
nmap zm :foldmore<CR>

" Toggle checkbox
exmap checkListStatus obcommand editor:toggle-checklist-status
nmap tt :checkListStatus<CR>

" Split vertical
exmap splitVertical obcommand workspace:split-vertical
nmap <Space>v :splitVertical<CR>

" Search files
exmap seachFiles obcommand global-search:open
nmap <Space>sf :searchFiles<CR>
