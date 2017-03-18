# Introduction to Linux

## Link
- http://tldp.org/LDP/intro-linux/html/

## 2.2. Absolute basics
### 2.2.1. The commands
- ls: displays a list of files in the current working directory
- cd directory: change directories
- passwd: change the password for the current user
- file filename: display file type of file with name filename
- cat textfile: throws content of textfile on the screen
- pwd: display present working directory
- exit or logout: leave this session
- man command: read man pages on command
- info command: read info pages on command
- apropos string: search the whatis database for strings
- whatis command: display short description of command

### 2.2.2. General remarks
- option
- argument

### 2.2.3. Using Bash Features
- Ctrl+A: Move cursor to the beginning of the comman line.
- Ctrl+C: End a running program and return the prompt.
- Ctrl+D: Log out of the current shell session, equal to typing exit or logout.
- Ctrl+E: Move cursor to the end of the command line.
- Ctrl+H: Generate backspace character.
- Ctrl+L: Clear this terminal.
- Ctrl+R: Search command history.
- Ctrl+Z: Suspend a program.
- ArrowLeft and ArrowRight: Move the cursor one place to the left or right on the command line, so that you can insert characters at other places than just at the beginning and the end.
- ArrowUp and ArrowDown: Browse history. Go to the line that you want to repeat, edit details if necessary, and press Enter to save time.
- Shift+PageUp and Shift+PageDown: Browse terminal buffer.
- Tab: Command or filename completion; when multiple choices are possible, the system will either signal with an audio or visual bell, or, if too many choices are possible, ask you if you want to see them all.
- Tab Tab: Shows file or command completion possibilities.

## 2.3. Getting help
### 2.3.2. The man pages
- man man
- Browse to the next page using the space bar.
- You can go back to the previous page using the b.
- Type q if you want to leave the man page.
- In man pages, press h can show SUMMARY of LESS command, which will show how to navigate man page.
- man 5 passwd
- man -a passwd: see all man pages about a command, one after the other.
- man intro

### 2.3.3. More info
#### 2.3.3.1. The Info pages
- These usually contain more recent information and are somewhat easier to use. The man pages for some commands refer to the Info pages.

#### 2.3.3.2. The whatis and apropos commands
- A short index of explanations for commands is available using the whatis command.
- If you do not know where to get started and which man page to read, apropos gives more information.

#### 2.3.3.3. The --help option
- Gives a short explanation about how to use the command and a list of available options.

#### 2.3.3.5. Exceptions
- Some commands do not have separate documentation, because they are part of another command. cd, exit, logout and pwd are such exceptions. They are part of your shell program and are called shell built-in commands.
- If you have been changing your original system configuration, it might also be possible that man pages are still there, but not visible because your shell environment has changed. In that case, you will need to check the MANPATH variable.
- Some programs or packages only have a set of instructions or references in the directory /usr/share/doc.
