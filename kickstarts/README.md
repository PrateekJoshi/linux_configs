# Kickstart 

1. Install vsftpd

```
sudo apt-get install vsftpd
```

2. Enable Anonymous login at `/etc/vsftpd.conf`

```
anonymous_enable=YES
```

3. Restart the vsftpd service

```
sudo systemctl restart vsftpd
```

4. Create a VM using iso image and then during installation `press TAB` when boot from live-cd and add ks=<KICKSTART_FILE_LOCATION>

Example (FTP kickstart)

```
vmlinuz initrd=initrd.img inst.stage2=hd:LABEL=CentOS quiet ks=ftp://192.168.0.1/ks.cfg
```

## Reference
[Youtube](https://www.youtube.com/watch?v=EGBvtWEr65I)
[CentOS Community Kickstarts](https://github.com/CentOS/Community-Kickstarts)
