# Lab Report1 week2

### Installing VScode
- Download the dmg file to the computer and install the vscode application
- Open the application and is will show this page
- In the vscode we are also able to open the file in different format such as markdown, python, and java
- <img src = "Image/VSCode.png" alt = "drawing" width = 700/>
<br>

### Remotely Connecting
- Connect to the remote computer through VSCode
- Open the terminal in VSCode and enter the comment `$ ssh cs15lsp22ael@ieng6.ucsd.edu`
- GIve the password to the account, then we successfully log into the account
- <img src = "Image/LogIntoRemote.png" alt = "drawing" width = 500/>
<br>

### Trying Some Commands
- `cd` or `cd ~` move back to the main root
- `cd..` moves the directory back one directory
- `ls` list the existing files in the current directory
- `ls -a` list all the files in the directory, including all the hidden files (files that start with .)
- `ls -lat` list all the fileshidden files, including the , in the current directory in the descending order or their last open time
- `cp /home/linux/ieng6/cs15lsp22/public/filename.txt ~/` copy the filename.txt file from server public address into own account address
- `cat /home/linux/ieng6/cs15lsp22/public/filename.txt ~/` copy the content in filename.txt file from server public address into own account address
- <img src = "Image/SomeCommand.png" alt = "drawing" width = 500>
<br>

### Moving Files with scp
- Use `javac` to compile the java file and `java` to run the program
- Use `scp fileName.java cs15lsp22ael@ieng6.ucsd.edu:~/` to copy the local java file into the remote computer, and enter the password to ensure the log in status
- To check whether the file is in the remote computer or not, log into the remote account again and `ls` to see the file in the directory
- 
<br>

### Setting an SSH Key
<br>

### Optimizing Remote Running
<br>
