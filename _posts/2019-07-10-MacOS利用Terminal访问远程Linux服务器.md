# 常用命令
默认22端口访问
```
ssh x.x.x.x
```

指定端口访问
```
ssh x.x.x.x -p port
```

指定用户访问(默认是MacOS当前用户)
```
ssh user@x.x.x.x [-p port]
```

# 设置主机别名，快捷访问
```
vi ~/.ssh/config
```
复制如下内容粘贴至config文件末尾(按需修改)
```
# xx Server
Host alias
        HostName x.x.x.x
        Port port
        User root
```
使用
```
ssh alias
```

# 参考链接
- [使用mac自带ssh连接远程服务器](https://blog.csdn.net/qq_34581118/article/details/77132208)

