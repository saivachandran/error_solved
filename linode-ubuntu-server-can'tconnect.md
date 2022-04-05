 # error
 
 systemd-resolved.service - Network Name Resolution
   Loaded: loaded (/lib/systemd/system/systemd-resolved.service; enabled; vendor
   Active: active (running) since Tue 2022-04-05 14:32:17 IST; 1h 5min ago
     Docs: man:systemd-resolved.service(8)
           https://www.freedesktop.org/wiki/Software/systemd/resolved
           https://www.freedesktop.org/wiki/Software/systemd/writing-network-con
           https://www.freedesktop.org/wiki/Software/systemd/writing-resolver-cl
 Main PID: 888 (systemd-resolve)
   Status: "Processing requests..."
    Tasks: 1 (limit: 4915)
   CGroup: /system.slice/systemd-resolved.service
           └─888 /lib/systemd/systemd-resolved

Apr 05 15:00:20 jenkins systemd-resolved[888]: Using degraded feature set (TCP) 
Apr 05 15:00:30 jenkins systemd-resolved[888]: Using degraded feature set (TCP) 
Apr 05 15:10:26 jenkins systemd-resolved[888]: Using degraded feature set (UDP) 
Apr 05 15:11:31 jenkins systemd-resolved[888]: Using degraded feature set (UDP) 
Apr 05 15:11:36 jenkins systemd-resolved[888]: Using degraded feature set (TCP) 
Apr 05 15:12:11 jenkins systemd-resolved[888]: Using degraded feature set (TCP) 
Apr 05 15:31:16 jenkins systemd-resolved[888]: Using degraded feature set (UDP) 
Apr 05 15:31:16 jenkins systemd-resolved[888]: Using degraded feature set (UDP) 
Apr 05 15:31:31 jenkins systemd-resolved[888]: Using degraded feature set (TCP) 
Apr 05 15:31:37 jenkins systemd-resolved[888]: Using degraded feature set (TCP)




  vim  /etc/systemd/resolved.conf
   
    DNSSEC=no
 
 
sudo systemctl restart systemd-resolved.service
