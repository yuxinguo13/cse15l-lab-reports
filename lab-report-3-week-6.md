# Lab Report3 Week6
[Other reports here](https://yuxinguo13.github.io/cse15l-lab-reports/)

### Streaminglining ssh Configuration

- Open the config file in textEditor, and set the content of it.

<img src = "image_report3/show_config.png" width = 500>

- After changing the the config, and use an alis to represent my ieng6 account, I could log into the account using ssh + alis name

<img src = "image_report3/log_into_account.png" width = 500>

- These are files in my ieng6 account before I copy files into the account

<img src = "image_report3/before_scp.png" width = 500>

- Files in my ieng6 account after copying files

<img src = "image_report3/scp_file.png" width = 500>

By changing the .ssh config and set a alis name to my ieng6 account, I could easily log into the account and do operations over the account.

<br>

### Setuo Github Access from ieng6
- This is the public key that I settled for my ieng6 account

<img src = "image_report3/public_ssh.png" width = 500>

- This is where I stored my private key on my computer

<img src = "image_report3/private_ssh.png" width = 500>

- This is how I git commit the command, and push it into the github

<img src = "image_report3/git_commit.png" width = 500>

- [Link to commit](https://github.com/yuxinguo13/markdown-parser/commit/577b5adab7815024d536f72aa8047445b7cc2938)


<br>

### Copy whole directory using scp -r
- By using the scp -r, I could directly copy the whole directory to ieng6 account.

<img src = "image_report3/copy_all_files.png" width = 500>

- Then I log into account to check the folder.

<img src = "image_report3/run_files.png" width = 500>

- I could also compile the program and run the test on my ieng6 account

<img src = "image_report3/scp_file.png" width = 500>

- This is how to copying and loging into account in one step

<img src = "image_report3/copy_log_in_one_line.png" width = 500>


