#### Linux常用操作

- Ctrl + D 退出cat

#### 新的centos各种命令没有

1. vi /etc/sysconfig/network-scripts/ifcfg-ens33
2. 将`ONBOOT=no`改为`ONBOOT=yes`
3. 输入:wq命令保存后执行`systemctl restart network`
4. 没有ifconfig和netstat ,yum install net-tools

#### xshell 中 screen 操作

- 修改终端类型为vt100用来辨别是否在screen中