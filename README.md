pxememo
=======

基本系统
----
1. U盘安装debian,root登陆
1. 配置静态ip 192.168.2.2
> iface eth0 inet static  
        address 192.168.2.2  
        netmask 255.255.255.0  
        gateway 192.168.2.1  
        dnsnameservers 211.162.78.1 211.162.78.3
        
1. 安装基本工具包
> apt-get install openssh-server sudo patch lm-sensors

配置
----
1. 默认用户加入sudo组
> usermod xx -a -G sudo

1. sudo无密码启动
> wget --no-check-certificate -O - https://raw.github.com/mmplayer/fsupdate/base/common/etc/sudoers.patch | patch /etc/sudoers

1. 定时备份系统
> TODO

网络启动
----
1. 安装dhcp,tftp服务器
>  apt-get install isc-dhcp-server tftp-hpa

