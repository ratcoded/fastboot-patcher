## `fastboot-patcher`
### Halt! Read this first:
> This repository is basically a fork of [Johx22/Patch-Recovery](https://github.com/Johx22/Patch-recovery)  
> Which is then based off of this script: [phhusson/samsung-galaxy-a51-gsi-boot](https://github.com/phhusson/samsung-galaxy-a51-gsi-boot)  
> So, the only thing I really did is revamp the scripts! All credit goes to them.
> 
> For now, there's no workflow, so you have to clone this repo and run the script yourself,  
> Meaning you have to use linux to run the script! (unless you get magiskboot.exe and run the script on windows with some edits)


### Instructions for patching!
> Note: you're going to need the packages *(git, wget, lz4, tar, openssl, & python3)*,  
> and *recovery.img.lz4 or recovery.img.* Personally, I unzipped the AP archive of a stock rom and got my recovery image from that.

If you have those, then clone the repository, and move your recovery image to it.
```bash
git clone github.com/engineer4t/fastboot-patcher.git && mv recovery.img.lz4 ./fastboot-patcher/ && cd fastboot-patcher
```
Then, just simply run the script with this command and wait for it to finish, it shouldn't take longer than a minute.
```bash
chmod a+x ./magiskboot && chmod a+x ./patcher && ./patcher
```
You'll find the original recovery image and 2 new images *(.img and .tar.md5 for odin)* in the top directory if successful.
