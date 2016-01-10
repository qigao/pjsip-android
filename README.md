# PJSIP Android Builder
This is revised script from https://github.com/alexbbb/pjsip-android-builder 

Easily build PJSIP with: x264,ffmpeg,opus for Android, by using a Linux virtual machine.

## Easy setup
Install [vagrant](https://www.vagrantup.com/), then open a terminal and execute:
```
git clone https://github.com/qigao/pjsip-android
cd pjsip-android
vagrant up
```

then you can SSH into the VM and build PJSIP:
```
vagrant ssh
cd /pjsip-android
```
install  necessary  libs as :
```
sudo apt-get install bzip2 gcc g++ binutils make autoconf  \
          libssl-dev openjdk-7-jdk openjdk-7-jre ant \
          libpcre3 libpcre3-dev build-essential \
          libc6-i386 libx32stdc++6 zlib1g
```
finally, you can build pjsip now
```
./prepare-build-system
./build
```

## License
    Licensed under the Apache License, Version 2.0 (the "License");

