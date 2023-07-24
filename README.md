![logo-blue](https://user-images.githubusercontent.com/51039935/197520391-f35db354-6071-4c12-86ea-fc450f04bc85.png)
# NAS媒体库管理工具

[![GitHub stars](https://img.shields.io/github/stars/NAStool/nas-tools?style=plastic)](https://github.com/c939984606/Nas_Tools_Pro/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/NAStool/nas-tools?style=plastic)](https://github.com/c939984606/Nas_Tools_Pro/network/members)
[![GitHub issues](https://img.shields.io/github/issues/NAStool/nas-tools?style=plastic)](https://github.com/c939984606/Nas_Tools_Pro/issues)
[![GitHub license](https://img.shields.io/github/license/NAStool/nas-tools?style=plastic)](https://github.com/c939984606/Nas_Tools_Pro/blob/main/LICENSE.md)
[![Docker pulls](https://img.shields.io/docker/pulls/c939984606/nas_tools_pro?style=plastic)](https://hub.docker.com/r/c939984606/nas_tools_pro)
[![Platform](https://img.shields.io/badge/platform-amd64/arm64-pink?style=plastic)](https://hub.docker.com/r/c939984606/nas_tools_pro)


Docker：
* https://hub.docker.com/r/c939984606/nas_tools_pro

API: http://localhost:3000/api/v1/


## 功能：

NAS媒体库管理工具。基于3.2.2版本最后一次Commit，增加修复了一些功能（移除认证，域名修复，豆瓣图片修复，签到修复）等。

（PS:由于3.2.3要关闭之前删除了部分功能，所以暂时不会更新到3.2.3版本。）


## 安装
### 1、Docker
```
docker pull c939984606/nas_tools_pro:latest
```
教程见 [这里](docker/readme.md) 。

如无法连接Github，注意不要开启自动更新开关(NASTOOL_AUTO_UPDATE=false)，将NASTOOL_CN_UPDATE设置为true可使用国内源加速安装依赖。

### 2、本地运行
python3.10版本，需要预安装cython，如发现缺少依赖包需额外安装：
```
git clone -b main https://github.com/c939984606/Nas_Tools_Pro --recurse-submodule 
python3 -m pip install -r requirements.txt
export NASTOOL_CONFIG="/xxx/config/config.yaml"
nohup python3 run.py & 
```

### 3、可执行文件
下载打包好的执行文件运行即可，会自动生成配置文件目录：

https://github.com/c939984606/Nas_Tools_Pro/releases

### 4、群晖套件
暂不支持

## 免责声明
1) 本软件仅供学习交流使用，软件本身不提供任何内容，仅作为辅助工具简化用户手工操作，对用户的行为及内容毫不知情，使用本软件产生的任何责任需由使用者本人承担。
2) 本软件代码开源，基于开源代码进行修改，人为去除相关限制导致软件被分发、传播并造成责任事件的，需由代码修改发布者承担全部责任。本项目的用户认证机制是项目长期生存下去的基础，建议不要修改用户认证并公开发布。
3) 本项目没有在任何地方发布捐赠信息页面，也不会接受捐赠或进行收费，请仔细辨别避免误导。
