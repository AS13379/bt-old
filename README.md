## 原版本内容
#### 宝塔开源许可协议：https://www.bt.cn/kyxy.html
#### 原版使用手册：http://docs.bt.cn
#### 原版论坛地址：https://www.bt.cn/bbs
#### 原版反馈建议： https://www.bt.cn/bbs/forum-43-1.html
#### 原版Bug提交：https://www.bt.cn/bbs/forum-39-1.html

## 请先使用如下命令安装最新版本：
#### Centos
```bash
yum install -y wget && wget -O install.sh http://download.bt.cn/install/install_6.0.sh && sh install.sh
```
#### Ubuntu/Debian
```bash
wget -O install.sh http://download.bt.cn/install/install-ubuntu_6.0.sh && sudo bash install.sh
```
### 请使用如下方法将您的版本回退为您想要的版本的版本:
##### 所有系统通用
```bash
cd /root
```
##### 获取旧版宝塔zip文件
#### 通过官方链接
```bash
wget http://download.bt.cn/install/update/LinuxPanel-5.9.1.zip //（配php7.2的开心版）
wget http://download.bt.cn/install/update/LinuxPanel-7.4.2.zip //（有pma漏洞）
wget http://download.bt.cn/install/update/LinuxPanel-7.4.5.zip //（会有绑定提醒）
wget http://download.bt.cn/install/update/LinuxPanel-版本号.zip
```
#### 通过本仓库
```bsah
wget https://github.com/Charlie894/bt-old/releases/download/Updete01/LinuxPanel-5.9.1.zip //配php7.2的开心版
wget https://github.com/Charlie894/bt-old/releases/download/Updete01/LinuxPanel-7.4.3.zip //有pma漏洞版本的下一版本
wget https://github.com/Charlie894/bt-old/releases/download/Updete01/LinuxPanel-7.4.5.zip //开始有强制绑定的版本
wget https://github.com/Charlie894/bt-old/releases/download/Updete01/LinuxPanel-版本号.zip //请先前往Updete01查看已经上传的版本,如果您有特殊需求,请发is或pull,我将会下载并上传
//注意,为提供下载便利,所有包均在Update01发，其它均会发后续版本
```
##### ps:我并不懂如何正确注释,因此建议删除注释部分运行
##### 如果报错,请执行以下代码:
##### CentOS
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
unzip LinuxPanel-*
cd panel
bash update.sh
cd .. && rm -f LinuxPanel-*.zip && rm -rf panel
echo '127.0.0.1 bt.cn' >>/etc/hosts
```
