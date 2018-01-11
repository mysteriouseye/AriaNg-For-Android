Install this by using command folowing.or install it manually

```shell
su
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
