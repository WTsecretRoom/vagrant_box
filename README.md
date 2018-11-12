# vagrant box 
vagrant php5开发环境   php7的详见 [php7分支](https://github.com/zhu2688/vagrant_box/tree/php7)

## box 文件保存在file分支
github上超过100M大文件必须用[LFS](https://git-lfs.github.com) 来上传

## 下载box后本地安装
- 下载box [https://github.com/zhu2688/vagrant_box/releases/download/0.0.2/centos-6.9-x64.box](https://github.com/zhu2688/vagrant_box/releases/download/0.0.2/centos-6.9-x64.box) 
- 下载Vagrantfile [Vagrantfile](https://raw.githubusercontent.com/zhu2688/vagrant_box/master/centos/Vagrantfile)
- 下载centos69.sh [centos69.sh](https://raw.githubusercontent.com/zhu2688/vagrant_box/master/centos/centos69.sh)


```shell
## 把上面三个脚本放到当前目录
vagrant box add dev1 centos-6.9-x64.box
vagrant up
```

## 软件环境
-  vagrant 2.1.4
-  VirtualBox 5.2.18
-  GuestAdditions 5.2.18

## 简介
  vagrant 一个完整的box文件都特别大,所以使用base文件加上provision来初始化开发环境

```shell
  ├── centos
  │   ├── centos-6.9-x64.box  基本box
  │   ├── centos69.sh    初始化脚本
  │   ├── Vagrantfile    Vagrantfile 文件
```
  
## php环境

```shell
* Php5.6
* Mysql 5.6
* Redis 3.2
* Tengine 2.2.1
```