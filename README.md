##### 宝塔开源许可协议：https://www.bt.cn/kyxy.html
##### 原版使用手册：http://docs.bt.cn
##### 原版论坛地址：https://www.bt.cn/bbs
##### 原版反馈建议： https://www.bt.cn/bbs/forum-43-1.html
##### 原版Bug提交：https://www.bt.cn/bbs/forum-39-1.html

#### 请先使用如下命令安装最新版本：
##### Centos
```bash
yum install -y wget && wget -O install.sh http://download.bt.cn/install/install_6.0.sh && sh install.sh
```
##### Ubuntu/Debian
```bash
wget -O install.sh http://download.bt.cn/install/install-ubuntu_6.0.sh && sudo bash install.sh
```
#### 请使用如下方法将您的版本回退/更新为目前支持的版本:
##### 所有系统通用
```bash
cd /root
```
##### 如果报错,请执行以下代码:
```bash
yum install -y wget
```
##### Ubuntu/Debian
```bash
apt-get install wget
```
##### 继续执行以下代码:
##### 所有系统通用
```bash
http://download.bt.cn/install/update/LinuxPanel-7.6.0.zip
unzip LinuxPanel-*
cd panel
bash update.sh
cd .. && rm -f LinuxPanel-*.zip && rm -rf panel
echo '127.0.0.1 bt.cn' >>/etc/hosts
```
