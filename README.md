# File Editing Rules
- NEVER use PowerShell, bash, python, or terminal commands (`Set-Content`, `Out-File`, `sed`, etc.) to create, modify, or delete files.
- ALWAYS use the built-in `replace_in_file` or `write_to_file` tools for all code and text edits.
- Only use the terminal for running builds, tests, git commands, or installing packages.


-Never delete whole file or write anything from scratch