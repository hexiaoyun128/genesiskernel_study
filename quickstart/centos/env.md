# 环境配置
本配置在VirtualBox下安装centos7虚拟机的桌面版

## 网卡设置(root用户)

* 到 `/etc/sysconfig/network-scripts/` 路径下 
* 执行命令`ls | grep ifcfg`,默认出现两个文件,排除`ifcfg-lo`
* 将另一个文件中的`ONBOOT=no`改为`ONBOOT=yes`
* 重启网卡`/etc/init.d/network restart`

## git安装(root用户)

`yum install git -y`