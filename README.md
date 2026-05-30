# OpenU-LaTeX

## paths
### fonts directory
- Windows: `C:/Windows/Fonts/` or `C:/Users/〈user_name〉/AppData/Local/Microsoft/Windows/Fonts/`
- macOS: `/Library/Fonts` or `/Users/〈user_name〉/Library/Fonts`

### key bindings
To add keyboard shortcuts, create a new file named `user.bind` in LyX user directory
- Windows: `C:\Users\ehud\AppData\Roaming\LyX2.5\bind`
- macOS: `/Users/〈user_name〉/Library/Application Support/LyX-2.5/bind/user.bind`
```
\bind "M-minus" "unicode-insert 0x05be" # Ctrl + -
\bind "C-apostrophe" "unicode-insert 0x201D" # ” Right Double Quotation Mark
\bind "S-Return" "separator-insert" # separator Shift+Enter
\bind "C-M-Return" "separator-insert latexpar" # latexpar separator Ctrl+Alt+Enter
```

## To Do
- [ ] Consider writing custom LaTeX macros to define appearance of titles for chapters, sections, subsections and table of contents
- [ ] Calling font NarkisTam Bold doesn't work. There are few new fonts in overleaf temp project. Implement to our project
- [ ] Consider setting `partopsep` of trivlists to zero: `\partopsep0pt`
- [ ] Create LyX styles from latex macros in `detokenize.tex` in overleaf temp project, for solutions and questions referencing
