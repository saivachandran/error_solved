

# error

Can not install on Ubuntu 22.04 (jammy) due to libssl1.1 dependency
#24759 


# solution
```
wget http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.1_1.1.1-1ubuntu2.1~18.04.20_amd64.deb
Then install
sudo dpkg -i libssl1.1_1.1.1-1ubuntu2.1~18.04.20_amd64.deb
```
