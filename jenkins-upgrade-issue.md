jenkins upgrade error 2.375.1 to 2.397
--------------------------------------
error
------
Ign:6 https://pkg.jenkins.io/debian-stable binary/ Release.gpg             
Hit:10 http://repo.zabbix.com/zabbix/4.0/ubuntu bionic InRelease
Reading package lists... Done                      
W: GPG error: https://pkg.jenkins.io/debian-stable binary/ Release: The following signatures were invalid: EXPKEYSIG FCEF32E745F2C3D5 Jenkins Project <jenkinsci-board@googlegroups.com>
E: The repository 'https://pkg.jenkins.io/debian-stable binary/ Release' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.

solution add below repo 
----------------------

Debian/Ubuntu
```
 curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
  
 echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

```
