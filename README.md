## Simply simple


### Get the kernel log

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```
/proc/last_kmsg
/data/tombstones/
/data/dontpanic/
/data/system/dropbox/
```

### Log data continuesly

Capture adb log and dmesg log:
```
setsid cat proc/kmsg > /sdcard/kmsg.txt
logcat -v long -f /sdcard/logcat.txt (somehow only works without setsid)
```
