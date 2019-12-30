# 为什么整这个项目？

工作中经常会学习一些新技术，通常情况下，没有实践过，过一段时间就会忘记，徒增学习成本。

dk 本人很喜欢看小说，so，开了这个工程，将遇到的感兴趣的技术、框架都怼一遍实践项目。古代将军练兵讲究以战养兵，进步神速，dk 效仿之。

# 设计

- [x] [原型图设计](https://www.xiaopiu.com/h5/byId?type=project&id=5de61b416b1b5a71bc47eb71)（xiaopiu）

# 技术栈

### 计划开发

- [ ] 公羊阅读跨多端应用 - `uni-app`

### 待重构

- [ ] client_mobile_android
- [ ] client_mobile_rn
- [ ] server_python_flask

### 已完成

**服务端**

- [x] [server_node_express](https://github.com/py-novel/server_node_express) 

**客户端：小程序**

- [x] [client_mobile_miniapp](https://github.com/py-novel/client_mobile_miniapp)
- [x] [client_mobile_taro](https://github.com/py-novel/client_mobile_taro)

**客户端：app**

- [x] [client_mobile_flutter](https://github.com/py-novel/client_mobile_flutter)

**客户端：h5**

- [x] [client_h5_vant](https://github.com/py-novel/client_h5_vant)

**客户端：后管系统**

- [x] [client_admin-antd](https://github.com/py-novel/client_admin_antd)

### 更新日志

[ChangeLog](./CHANGELOG.md)

# 展示

### 二维码

小程序二维码，扫一扫，直接看！

![小程序二维码](./assets/imgs/小程序二维码.jpg)

### 页面展示

![image.png](https://cdn.nlark.com/yuque/0/2019/png/103389/1563444732432-6f9bb2f1-7150-42ad-a6e0-fa887c005ea9.png#align=left&display=inline&height=588&name=image.png&originHeight=588&originWidth=740&size=127097&status=done&width=740)

![image.png](https://cdn.nlark.com/yuque/0/2019/png/103389/1563444718965-e621e1a2-5d4a-4c16-b576-9c61a5d0073f.png#align=left&display=inline&height=590&name=image.png&originHeight=590&originWidth=731&size=81419&status=done&width=731)

![image.png](https://cdn.nlark.com/yuque/0/2019/png/103389/1563585546106-5945fc65-a0f1-40d9-b699-0ad3654ecc63.png#align=left&display=inline&height=589&name=image.png&originHeight=589&originWidth=742&size=181497&status=done&width=742)

![image.png](https://cdn.nlark.com/yuque/0/2019/png/103389/1563444684802-62ea2108-2246-4c76-8881-1177adcf86be.png#align=left&display=inline&height=588&name=image.png&originHeight=588&originWidth=741&size=142410&status=done&width=741)

# 部署

本地写的 shell 脚本，一键部署。有几点需要说明：

- python 服务单独在云主机(centos7)运行 `$ python3 index.py`，当退出 shell 时服务也会断开。解决方法为将 index.py 做成系统服务，使用 `systemctl` 统一管理；[《自定义系统服务》](https://blog.dkvirus.top/ops/linux/systemd.html)
- 一键部署包括将本地文件传输到云主机，使用的是 ssh 协议，但前提要设置免密登录。[《设置 ssh 免密登录》](https://blog.dkvirus.top/ops/linux/ssh.html)