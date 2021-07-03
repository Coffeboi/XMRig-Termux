# XMRig-Termux
XMRig for Termux on Android.
 
```
pkg install update
apt-get update
apt-get install git 
apt install wget 
```
XMRig

```
apt update 
apt upgrade
apt-get install git build-essential cmake libuv1-dev libmicrohttpd-dev   
git clone https://github.com/xmrig/xmrig.git 
cd xmrig 
mkdir build
cd build 
cmake -DWITH_HWLOC=OFF .. 
make
```
Enter this to start the miner.
./xmrig -a cn-pico -o norpool.org:3333 -u SEKRaddressHere -p x -t numberOfCores
