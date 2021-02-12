# InstallNET
DD安装服务器系统脚本

#先运行:
#Debian/Ubuntu:
apt-get update

#RedHat/CentOS:
yum update

#确保安装了所需软件:
#Debian/Ubuntu:
apt-get install -y xz-utils openssl gawk file

#RedHat/CentOS:
yum install -y xz openssl gawk file

# 用法，安装Debian 9：
wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/zhucaidan/InstallNET/main/InstallNET.sh' && chmod a+x InstallNET.sh

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/zhucaidan/InstallNET/main/InstallNET.sh') -d 9 -v 64 -a -firmware
