sudo apt update -y
Hit:1 http://eu-west-1.ec2.archive.ubuntu.com/ubuntu bionic InRelease
Hit:2 http://eu-west-1.ec2.archive.ubuntu.com/ubuntu bionic-updates InRelease
Hit:3 http://eu-west-1.ec2.archive.ubuntu.com/ubuntu bionic-backports InRelease
Get:4 http://security.ubuntu.com/ubuntu bionic-security InRelease [88.7 kB]
Get:5 http://repo.mysql.com/apt/ubuntu bionic InRelease [20.0 kB]                            
Err:5 http://repo.mysql.com/apt/ubuntu bionic InRelease                                      
  The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 467B942D3A79BD29
Reading package lists... Done
W: GPG error: http://repo.mysql.com/apt/ubuntu bionic InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 467B942D3A79BD29
E: The repository 'http://repo.mysql.com/apt/ubuntu bionic InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.


  
  
  # command
  
         sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys  467B942D3A79BD29
