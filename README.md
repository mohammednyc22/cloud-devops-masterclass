# 🚀 Cloud & DevOps Masterclass: Ubuntu & WSL Essentials Cheatsheet

## 1. Quick WSL & Terminal Shortcuts (From PowerShell)
* `wsl` — Instantly jump into your default Ubuntu environment from PowerShell.
* `wsl -l -v` — List all installed Linux distributions and check their WSL versions.
* `wsl --shutdown` — Instantly restart/stop all background WSL virtual machines if something gets stuck.
* `exit` — Close out of your current Ubuntu session and return to Windows.

## 2. Moving Around the File System (Inside Ubuntu)
* `pwd` (*Print Working Directory*) — Shows the exact folder path you are currently sitting in.
* `ls` (*List*) — Shows all files and folders in your current location (`ls -la` shows hidden files too).
* `cd [folder_name]` (*Change Directory*) — Moves you into a specific folder.
* `cd ..` — Moves you *backward* one folder level up.

## 3. Managing Files & Folders
* `mkdir [folder_name]` — Creates a brand new folder.
* `touch [file_name]` — Creates a clean, empty file.
* `rm [file_name]` — Deletes a file.
* `cat [file_name]` — Prints the text contents of a file directly onto your screen.

## 4. Keeping Ubuntu Up-to-Date
* `sudo apt update && sudo apt upgrade -y` — Refreshes and updates all your system software packages in one go.
==============================================================================================
Here is a clean, well-formatted guide written in Markdown that you can directly copy, paste into your README.md file in VS Code, and commit to Git!

🚀 Setting Up Ubuntu (WSL) with VS Code
A step-by-step documentation of connecting the Ubuntu Linux environment (WSL) to Visual Studio Code for local DevOps development.

Step 1: Navigate to the Project Directory
First, open your Ubuntu Terminal (via Windows Terminal or the Ubuntu App) and navigate to your working repository:

Bash
cd ~/cloud-devops-masterclass
Step 2: Launch VS Code via WSL Bridge
From inside the project directory, trigger VS Code to open attached to the current directory using the dot (.) flag:

Bash
code .
Note: The . tells VS Code to launch and automatically open the current folder (~/cloud-devops-masterclass).

Step 3: Grant Host Trust & Permission
When opening VS Code via WSL for the first time:

A security popup will appear asking: "The host 'wsl.localhost' was not found in the list of allowed hosts. Do you want to allow it anyway?"   

Check the box "Permanently allow host 'wsl.localhost'".   

Click Allow.   

When prompted in VS Code, click "Trust Folder" to grant full access for running scripts and terminal extensions.   
+ 1

Step 4: Configure Integrated Ubuntu Terminal inside VS Code
Press Ctrl + ` (backtick) to open the integrated terminal panel inside VS Code.

If it opens in PowerShell by default:   

Click the + dropdown arrow in the top-right of the terminal pane.   

Select Ubuntu (WSL) / wsl.   

Select Select Default Profile 
→ Ubuntu (WSL) to ensure it always launches in Linux mode.

Verify that your prompt displays the Linux path:

Bash
mohammed_howladermgabbari@Toaha-Alienware:~/cloud-devops-masterclass$
🛠️ How to Commit & Push This to GitHub
Now, open your integrated terminal in VS Code (where you see your green Linux prompt) and run these commands to record your update:   

1. Check Repository Status
Bash
git status
(You will see modified files listed in red, such as README.md)

2. Stage the Changes
Bash
git add .
3. Commit the Changes
Bash
git commit -m "docs: add WSL and VS Code setup guide to README"
How does this documentation look for your repository? Ready to run git status in your integrated terminal?For example, if you want your file to be named my-notes.md and you want the text inside to say something like "Learning Cloud DevOps and pushing to GitHub!", just copy and paste this command into your VS Code terminal and hit Enter:
=======================
Hi Mr Gemini, how are you doing my professor?
