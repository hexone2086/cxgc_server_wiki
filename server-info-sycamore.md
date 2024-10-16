# 服务器 Sycamore 说明

## 硬件配置
* CPU: 2x Intel(R) Xeon(R) Gold 5218R CPU @ 2.10GHz 20c40t
* GPU: 4x Nvidia GA102GL\[A40\] 48G
* RAM: 251GB (available)
* HDD: 27TB (available) SSD RAID 

## 软件配置
* OS: ubuntu 22.04
* Desktop: KDE-plasma
* Cuda Version: 12.6
* Muti User: support

## 管理策略
服务器采用单系统多用户模式运行，用户策略：

* 禁用 root 用户
* 管理员用户 cxgc_a40
* 其他用户为普通组，无 sudo 权限