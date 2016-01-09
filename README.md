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
sudo apt-get install bzip2 gcc g++ binutils make autoconf  \
          libssl-dev openjdk-7-jdk openjdk-7-jre ant \
          libpcre3 libpcre3-dev build-essential \
          libc6-i386 libstdc++6 zlib1g

```
./prepare-build-system
./build
```

## License

    Copyright (C) 2015 Aleksandar Gotev

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
