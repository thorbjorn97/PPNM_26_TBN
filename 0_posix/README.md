# POSIX Exercise

## 1. Install a POSIX sytem on your device (box)

I have a Windows machine, so I used the option **Windows Subsystem for Linux (WSL)**.

Steps followed:

- Installed WSL from Administrator PowerShell following Microsoft's officiel guide.
- Chose Ubuntu 24.04 LTS as the POSIX environment.
- Verified terminal access using `wsl` from Administrator PowerShell.

## 2. Learn how to start a terminal in your POSIX system

As I am using Ubuntu via WSL on a Windows machine, there are two options, either

- Open the Windows Start Menu --> search for "Ubuntu" --> click to launch it 

or

- Open the Windows Start Menu --> search for "PowerShell" --> open it as Administrator --> type: wsl

Once the terminal opens, I can optionally verify my environment:

- Check current directory: `pwd`
- Check current user: `whoami`
- List files: `ls`
- Navigate directories: `cd <directory>`

## 3. Read about the man utility. Run man man and read the description of the utility in your system.

- The `man` command displays the **manual page** for other commands in my POSIX system. It is a built-in way to read documentation directly from the terminal.
- It can be used to read manuals for any installed command by typing, for instance:
	- `man ls`
	- `man cp`
	- `man mkdir`
- To read the manual for `man` itself, type:
	- `man man`
- The manual will open using the default pager (`less`). Scrolling is done with the **arrow keys**.
- To search inside the manual, press `/` followed by the search term and Enter.
- To quit the manual and return to the shell, press `q`.

## 4. Learn the following commands (file utilities) from the GNU Core Utilities: cp, ls, mkdir, mv, rm, and the bash built-in command cd.

Here is a brief description of the commands mentioned.

| Command | Description |
|---------|-------------|
| `ls`   | List directory contents |
| `cp`   | Copy files or directories |
| `mv`   | Move or rename files/directories |
| `rm`   | Remove files or directories |
| `mkdir`| Create new directories |
| `cd`   | Change current working directory |


## 5. Install bash-completion with the command "sudo apt install bash-completion". Read about the command-line completion.

- The bash-completion was installed as described
- Bash-completion enhances the shell with **command-line completion**, which allows the user to only type the first few characters of an item (command, program or filename) and have the remaining part filled by pressing `Tab`.

Examples:
-   Type `cd /h` and press Tab → may complete to `/home/`
-   Type `ls --v` and press Tab → may complete to `ls --version`

## 6. Install your favourite text editor.

I chose Visual Studio Code as my text editor, as it is already installed on my sytem.

## 7. Learn to create, save and edit text files with your favourite text editor.

In my setup (Ubuntu via WSL) and editor (VS Code), the workflow is as follows:

1) Start PowerShell as administrator
2) Launch VS Code and navigate to the Linux home director:
	wsl			[redirects to (W)Windows (S)ubsystem for (L)inux]
	cd ~ 			[redirects to my Linux home directory]
	pwd			[prints working directory]
3)  In WSL terminal, verify last output:
	"# /home/thorbj" 		<--- IMPORTANT
4)  In WSL terminal, type:
	code . 			[launches VSC from the currenct directory]
5)  In VSC:
	File -> New File -> Save As -> enter <FILENAME>.txt in the current directory
6)  In VSC:
	edit the file as needed
7)  In VSC:
	Ctrl + S        	[saves changes]
8)  In WSL terminal, type:
	ls                 	[lists files in the directory]
	cat <FILENAME>.txt 	[displays file contents]
9)  In WSL terminal, verify last output:
	<FILECONTENT>thorbj[...]:~$

Now file <FILENAME> is now created, edited to have content <FILECONTENT>, saved, and accessible in the desired directory.


