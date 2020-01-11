# Dell-Latitude-7480-Hackintosh

Don't forget after install or upgrade to **Catalina 10.15** to copy files from `/EFI/CLOVER/kexts/Other/ToLE` folder to `/Library/Extentions` and change permission then rebuild cache

```
 sudo cp -r Copy2LE/* /L*/E*/

 sudo chmod -Rf 755 /L*/E*

 sudo chown -Rf 0:0 /L*/E*

 sudo kextcache -i /
 ```


And of course don't forget completely turn off hibernate for a quick wakeup after lid open. 

```
sudo pmset hibernatemode 0

sudo rm -f /var/vm/sleepimage

sudo pmset hibernatefile /dev/null
```

---
## Credit:
https://osxlatitude.com/forums/topic/12379-dell-latitude-7480-catalina/