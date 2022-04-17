# Error facing add second slave in aws

# timezone eroor
```
timedatectl

timedatectl list-timezones 

sudo timedatectl set-timezone "Asia/Kolkata" 

```

# cron job won't run

```
systemctl restart cron.service
```


# s3 bucket error key not validating
```
aws s3 cp  --recursive /mysqlbackup/${filename} s3://tendercuts-databackup/
```
