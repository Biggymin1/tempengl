# File Editing Rules
- NEVER use PowerShell, bash, python, or terminal commands (`Set-Content`, `Out-File`, `sed`, etc.) to create, modify, or delete files.
- ALWAYS use the built-in `replace_in_file` or `write_to_file` tools for all code and text edits.
- Only use the terminal for running builds, tests, git commands, or installing packages.

- **NEVER** use `execute_command` (PowerShell) to read, search, inspect, or edit files.
- **ALWAYS** use Cline's built-in file tools:
  - `read_file` to inspect files or check line counts.
  - `search_files` to find text or patterns in files.
  - `replace_in_file` for targeted edits and `write_to_file` for new files or full rewrites.
- Only use `execute_command` for running build/dev servers or `git` commands.
- Note: This environment runs on Windows (`win32`). Never use Linux/bash syntax or pass `$variables` inside double-quoted strings in PowerShell commands.

-Never delete whole file or write anything from scratch