# Kickstart 

Press TAB when boot from live-cd and add ks=<KICKSTART_FILE_LOCATION>

Example (FTP kickstart)

```
vmlinuz initrd=initrd.img inst.stage2=hd:LABEL=CentOS quiet ks=ftp://192.168.0.1/pub/ks.cfg
```

## Reference
![Youtube](https://www.youtube.com/watch?v=EGBvtWEr65I)
