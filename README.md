# Tips for useful command
### Part 1: ssh connection
1. connect using username and password authentication: **ssh username@clould_ip**
2. connect using key files:
   1.  **cd [keydir]**
   2.  **chmod 400 keyfilename.pem**
   3.  **ssh -i "keyfilename.pem" username@cloud_ip**
### Part 2: transfer file
1. upload files from local machine to cloud machine: **scp [local dir] username@cloud_ip:[cloud dir]**
2. download files from cloud machine to local machine **scp username@cloud_ip:[cloud dir] [local_dir]**
3. upload for aws: **scp -i [path to keyfile] [local dir] username@cloud_ip:[cloud dir]**
4. download for aws: **scp -i [path to keyfile]username@cloud_ip:[cloud dir] [local_dir]**
### Part 3: check files
1. count how many files in current dir: **ls -l | grep -v ^l | wc -l**
2. check if a certain file exist in dir: **(ls x.txt && echo yes) || echo no**
3. check file/dir size: 
   1. check dir size: **du -sh [path to dir]**
   2. check file size: **du -h [path to file]**
4. count file in dir and its subdir :**find . -type f | wc -l**
### Part 4: vim for editting codes:
1.  undo: **u**
### Part 5: using git
1. add all: git add *
2. undo add all: **git reset**
### Part 6: tensorboard 
1.  **tensorboard --logdir='./logs' --port=6006**
$/Omega$
