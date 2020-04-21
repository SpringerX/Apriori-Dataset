## Ubuntu 18.04 安装 Docker 

更新ubuntu的apt源索引 

```bash
sudo apt-get update
```

安装包允许apt通过HTTPS使用仓库 

```bash
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
```

添加Docker官方GPG key 

```bash
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```
设置Docker稳定版仓库 

```bash
#注意下面两行其实是一条命令
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```

添加仓库后，更新apt源索引 

```bash
sudo apt-get update
```

安装最新版Docker CE（社区版） 

```bash
sudo apt-get install docker-ce
```

检查Docker CE是否安装正确 

```bash
sudo docker run hello-world
```

出现如下信息，表示安装成功 

![docker](C:\Users\kaixu\Desktop\docker.jpg)

为了避免每次命令都输入sudo，可以设置用户权限，**注意执行后须注销重新登录**

```bash
sudo usermod -a -G docker $USER
```

## Docker服务的启动与停止 

安装完成Docker后，默认已经启动了docker服务，如需手动控制docker服务的启停，可执行如下命令 

启动docker

```bash
sudo service docker start
```
停止docker

```bash
sudo service docker stop
```

重启docker

```bash
sudo service docker restart
```