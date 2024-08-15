# Guide to the Windows Command Line

The command line is a text-based interface for interacting with your computer. It can be useful for file management, automation of repetitive tasks, and running open source software you install.

This guide covers basic commands for both Command Prompt (CMD) and PowerShell (PS).

## Opening the Command Line
- Press `Win + R`, type `cmd` or `powershell`, hit Enter.
- Or search for "Command Prompt" or "PowerShell" in the Start menu.

## Command Prompt vs PowerShell
- Command Prompt: Simpler, good for basic tasks.
- PowerShell: More powerful, better for complex operations and scripting.

For most tasks, either will work. PowerShell offers more advanced features if needed.

Remember: Be cautious with delete commands. Always double-check before deleting files.

## Essential Commands

| Action | CMD Command | PowerShell Command | Description |
|--------|-------------|---------------------|-------------|
| Current location | `cd` | `pwd` | Show current directory |
| List files | `dir` | `ls` or `dir` | List files in current directory |
| Change directory | `cd folder_name` | `cd folder_name` | Move to specified folder |
| Go up a directory | `cd ..` | `cd ..` | Move to parent folder |
| Create folder | `mkdir folder_name` | `mkdir folder_name` | Create a new folder |
| Create file | `type nul > file.txt` | `New-Item file.txt` | Create a new file |
| Copy file | `copy file.txt copy.txt` | `Copy-Item file.txt copy.txt` | Copy a file |
| Move/rename | `move old.txt new.txt` | `Move-Item old.txt new.txt` | Move or rename a file |
| Delete file | `del file.txt` | `Remove-Item file.txt` | Delete a file |
| View file contents | `type file.txt` | `Get-Content file.txt` | Display file contents |
| Append to file | `echo text >> file.txt` | `Add-Content file.txt "text"` | Add text to end of file |

## Tips
1. Use `cd` to navigate to your story folders.
2. `dir` or `ls` to check what files you have.
3. `type` or `Get-Content` to quickly view text file contents.
4. Use `mkdir` to create folders for organizing research.
5. `copy` or `Copy-Item` to backup important documents.
6. `echo` or `Add-Content` to append notes or new information to existing files.
