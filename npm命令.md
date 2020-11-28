# npm 命令

```shell
# 安装
npm install 包名
#简写
npm i 包名
#安装指定版本的包
npm install 包名@版本号   -> npm install moment@2.22.2

#初始化
npm init -y
#安装所有的包
npm install

#卸载包
npm uninstall 包名

#安装开发依赖
npm install 包名 -D

#安装全局包
npm install 包名 -g
#卸载全局包
npm uninstall 包名 -g
```

# 解决 nrm 不能使用问题

```shell
1.使用管理员 权限打开 cmd 或者powershell
2.set-ExecutionPolicy RemoteSigned 输入Y
3.get-ExecutionPolicy 
4.Set-ExecutionPolicy RemoteSigned -Scope Process 输入Y
```

# nrm的使用

```shell
#展示列表
nrm ls
#切换镜像
nrm use 镜像名字 -> nrm use taobao
```



# 发布包

```shell
#1.切换原版镜像
nrm use npm
#2.登陆(一定要在包文件夹路径下登陆)
npm login
#3.发布包
npm publish
#4.删除包(72小时以内)
npm unpublish 包名 --force

```

