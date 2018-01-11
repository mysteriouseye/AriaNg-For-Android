Static binary can't not get local DNS server,that means you need to specify dns server by using:
```shell
aria2c --async-dns --async-dns-server=`getprop net.dns1`,`getprop dnet.dns2`
```
And when you change your network environment such as swich wifi to mibile network or change another wifi.DNS server changes too.
So aria2c will stop working with a wrong DNS server,you need to reboot aria2c after change network environment.
