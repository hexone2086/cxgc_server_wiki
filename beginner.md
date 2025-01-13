# 新手上路
> 目前该部分仅针对 Sycamore-A40 服务器

## 用户注册
~~服务器采用 LDAP 方式管理用户~~ 暂时还没实现

目前，对于 `Sycamore-A40`，暂时请按照以下模板发送邮件至 [<CaoWangrenbo>cao.wangrenbo@yandex.com](mailto:cao.wangrenbo@yandex.com)：

```
姓名*：
微信id或者手机号*：
拟申请的账户名称*： (尽量短小，避免user、admin等。例如 alley9527)
邮件地址*：
工作单位：
申请原因：
```
收到邮件后一般会在 24h 内回复并返回初始帐号、密码和登录方式，如有问题也会尽快回复，请关注邮件列表（此外有可能被误识别为垃圾邮件/spam，烦请关注一下）。

## 本地软件配置



## 修改默认密码
当您收到确认邮件之后，请尽快按照随附的登录方式登录服务器（因为可能产生变动），并且第一时间设置您自己的高强度密码

1. 设置密码，请将 <username> 替换成您的登录名
```shell
passwd <username>
```
2. 根据提示输入密码和确认密码（为保证强度，建议至少有一个大写字母、一个小写字母、数字和特殊符号，总长不小于 8 位）

## 添加用户密钥
为了确保服务器安全，尽管并未禁止密码登录，但是还请尽量采用密钥登录

## conda 环境配置
由于服务器采用多用户模型，所以 conda 也仅为当前用户安装。conda 采用 Miniconda

1. 最新 Miniconda 版本可以从服务器以下路径获得，建议复制到用户目录

```
/public/Resources/software/Miniconda3-latest-Linux-x86_64.sh
```

2. 如果复制过来的安装文件不具备执行权限，可运行以下命令（假设文件位于 `~/Download/` 目录下）

```shell
chmod 755 ~/Download/Miniconda3-latest-Linux-x86_64.sh
```

3. 赋予权限后可直接执行，按照提示阅读并同意 EULA，最后完成安装

```shell
~/Download/Miniconda3-latest-Linux-x86_64.sh
```