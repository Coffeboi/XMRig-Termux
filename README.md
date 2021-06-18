# XMRig-Termux
XMRig for Termux on Android.
 
```
pkg install update && upgrade
apt-get install git 
apt install wget 
apt install proot
apt install git build-essential libmicrohttpd-dev libssl-dev cmake libhwloc-dev
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
git clone https://github.com/xmrig/xmrig.git 
cd xmrig 
mkdir build
cd build 
cmake -DWITH_HWLOC=OFF .. 
make
