# XMRig-Termux
语言选择: [英文](./README.md) | 简体中文

这是用于 Android 上的 Termux 的 XMRig 的 big boi 自行编译版本。

建议获取最新版本的termux
 <a href="https://wiki.termux.com/wiki/Installing_from_F-Droid">这里
</a>.
 
```
apt-get update
apt-get install git -y
pkg install cmake -y
```
现在开始克隆 XMRig 存储库。

```
apt update 
apt upgrade  
git clone https://github.com/xmrig/xmrig.git 
cd xmrig
```
它现在应该看起来像这样。

![image](https://user-images.githubusercontent.com/84473858/124390827-94fe8480-dced-11eb-9f5e-1d53497e8aa4.png)
``` 
mkdir build
cd build
cmake -DWITH_HWLOC=OFF .. 
```

![image](https://user-images.githubusercontent.com/84473858/124390943-430a2e80-dcee-11eb-95f0-2d2645faae26.png)

运行 cmake 后，您必须“制作”它。注意：此步骤可能需要一段时间，具体取决于您使用的手机！
```
make
```
![image](https://user-images.githubusercontent.com/84473858/124390954-5f0dd000-dcee-11eb-8d4b-e47add3f8230.png)

现在你应该已经设置好了所有东西。 （您可以输入 `clear` 清除屏幕以获得更好的概览。）
进入 `ls` 您将获得您所在文件夹中所有内容的列表。

![image](https://user-images.githubusercontent.com/84473858/124391996-a185db80-dcf3-11eb-8455-8c0360cffa20.png)

输入这个来启动矿工。
```
./xmrig -a cn-pico -o norpool.org:3333 -u SEKR地址在这里 -p x -t 线程数
```
![image](https://user-images.githubusercontent.com/84473858/124391157-8f09a300-dcef-11eb-8294-144837e7b641.png)

