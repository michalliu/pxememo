pxememo
=======

1. U盘安装debian,root登陆
2. 配置静态ip 192.168.2.2
> iface eth0 inet static
>   address 192.168.2.2
>   netmask 255.255.255.0
>   gateway 192.168.2.1
>   dnsnameservers 211.162.78.1 211.162.78.3
3.安装基本工具包
> apt-get install openssh-server sudo  lm-sensors
