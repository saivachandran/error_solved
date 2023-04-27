# step 1

cat /proc/sys/vm/swappiness

# step 2 
sudo sysctl vm.swappiness=60

# step 3

Check space: # free -m 
Disable swap: # swapoff -a 

Wait approx 30 sec 
(use free -m to see the amount of swap used/available decrease over time)

Enable swap: # swapon -a 
