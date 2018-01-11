Install this by using command folowing.or install it manually.

Attention: get root access before runing command.


用下面的代码安装，或者手动安装。

注意:执行前必须获取root权限。

```shell
cd data
mkdir Project
chmod -R 755 Project
cd Project
if [[ `which curl` == '' ]];then
   echo 'curl not found.'
   exit 1
fi
if [[  `which busybox` == '' ]];then
   echo 'busybox not found.'
   exit 1
fi
curl -k -o ./Aria2.zip 'https://raw.githubusercontent.com/Saint-Theana/AriaNg-For-Android/master/For-Android/Aria2.zip'
busybox unzip Aria2.zip
chmod -R 755 Aria2
ln -s Aria2/bin/aria2 /system/xbin/aria2
echo 'complete!'

sleep 2

aria2

```


手动安装方法:(Manual Installation)
1: 下载Aria2.zip  链接:https://raw.githubusercontent.com/Saint-Theana/AriaNg-For-Android/master/For-Android/Aria2.zip

2:解压后把Aria2文件夹放到/data/Project下面，没有该目录就自己新建一个。

3:修改整个目录的权限为755.






