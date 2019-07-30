# 目的
> 偶尔我们只是想运行模拟器，并不想打开AndroidStudio，这时我们可以从终端找到emulator，通过emulator来启动指定名称的模拟器

# 步骤
1.找到emulator所在位置
```
find . -name emulator
```
2.查看已创建的模拟器列表
```
./emulator -list-avds
```
3.启动模拟器
```
./emulator @Nexus_5X_API_27_x86
或
./emulator -avd Nexus_5X_API_27_x86
```

# 参考链接
- [单独启动android模拟器 如何从命令行启动Android模拟器?](https://code-examples.net/zh-CN/q/4be7e8)