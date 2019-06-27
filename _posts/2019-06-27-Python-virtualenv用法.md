# 简介
> virtualenv就是用来为一个应用创建一套“隔离”的Python运行环境。

# 安装
```
pip3 install virtualenv
```

# 使用
创建运行环境
```
mkdir myproject
cd myproject
virtualenv --no-site-packages venv
```
Linux进入运行环境
```
source venv/bin/activate
```
Windows进入运行环境
```
cd venv
cd Scripts
activate
-------------
(venv) E:\project\python\venv\venv\Scripts>deactivate
```

退出当前的venv环境
```
deactivate 
```

