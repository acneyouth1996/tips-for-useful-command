# tips-for-useful-command
### Part 1: ssh connection
###### 1.connect using username and password authentication: ssh username@clould_ip
###### 2.connect using key files: step1: cd [keydir]
######                            step2: chmod 400 keyfilename.pem
######                            step3: ssh -i keyfilename.pem@cloud_ip
### Part 2: transfer file
###### 1.upload files from local machine to cloud machine: scp [local dir] username@cloud_ip:[cloud dir]
###### 2.download files from cloud machine to local machine scp username@cloud_ip:[cloud dir] [local_dir]
### part 1: check files
###### 1.count how many files in current dir: 
