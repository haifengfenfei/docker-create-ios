# 基于linux使用docker构建CentOS基础镜像
=======================================
## 安装docker
```
yum install docker-ce docker-ce-cli containerd.io
```

## 启动 Docker
```
systemctl start docker
```
## 运行 hello-world 映像来验证是否正确安装了 Docker
```
docker run hello-world
```

## 基于Dockerfile开始构建镜像

在 Dockerfile 文件的存放目录下执行,构建一个 centos7:test（镜像名称:镜像标签）
```
docker build -t centos7:test .
```
### 指令最后一个 . 是上下文路径

## 运行镜像
```
docker run  centos7:test
```
