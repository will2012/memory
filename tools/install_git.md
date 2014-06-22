#!/bin/bash
# Program:
#       This program shows "install git on CentOs" in your screen.
# History:
# 2014/06/23	
PATH=/bin:/sbin:/usr/bin:/usr/sbin:/usr/local/bin:/usr/local/sbin:~/bin
export PATH
echo -e "install git"

#安装依赖包
yum install curl 
yum install curl-devel 
yum install zlib-devel 
yum install openssl-devel 
yum install perl 
yum install cpio 
yum install expat-devel 
yum install gettext-devel


#安装GIT

wget http://codemonkey.org.uk/projects/git-snapshots/git/git-latest.tar.xz
tar Jxvf  git-latest.tar.xz
cd git-2014-06-22 ＃你的目录可能不是这个 

./configure 
make 
sudo
make install


exit 0
