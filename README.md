# XMRig-Termux
This is the big boi compile-it-yourself version of XMRig for Termux on Android. 

It is recommended to get the latest version of termux <a href="https://wiki.termux.com/wiki/Installing_from_F-Droid">here</a>.
 
```
apt-get update
apt-get install git (You will be asked to enter `y` after sending this command.)
pkg install cmake   (You will be asked to enter `y` after sending this command.)
```
Now on to cloning XMRig repo.

```
apt update 
apt upgrade  
git clone https://github.com/xmrig/xmrig.git 
cd xmrig
```
It should look something like this now.

![image](https://user-images.githubusercontent.com/84473858/124390827-94fe8480-dced-11eb-9f5e-1d53497e8aa4.png)
``` 
mkdir build
cd build
cmake -DWITH_HWLOC=OFF .. 
```

![image](https://user-images.githubusercontent.com/84473858/124390943-430a2e80-dcee-11eb-95f0-2d2645faae26.png)

After running cmake you have to make it. NOTE: This step might take a while depending on what phone you are on!
```
make
```
![image](https://user-images.githubusercontent.com/84473858/124390954-5f0dd000-dcee-11eb-8d4b-e47add3f8230.png)

Enter this to start the miner.
```
./xmrig -a cn-pico -o norpool.org:3333 -u SEKRaddressHere -p x -t numberOfThreads
```
![image](https://user-images.githubusercontent.com/84473858/124391157-8f09a300-dcef-11eb-8294-144837e7b641.png)
