# XMRig-Termux
XMRig for Termux on Android.
 
```
pkg install update && upgrade
apt-get install git 
apt install wget 
apt install proot
```
This is for Ubuntu.

```
git clone https://github.com/Neo-Oli/termux-ubuntu 
cd termux-ubuntu 
chmod +x ubuntu.sh 
sh ubuntu.sh 
./start-ubuntu.sh
```
XMRig

```
apt update 
apt upgrade  
build-essential cmake libuv1-dev libmicrohttpd-dev libssl-dev 
git clone https://github.com/xmrig/xmrig.git 
cd xmrig 
mkdir build
cd build 
cmake -DWITH_HWLOC=OFF .. 
make
