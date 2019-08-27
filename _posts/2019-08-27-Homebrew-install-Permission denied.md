# 解决办法
```
sudo chown -R `whoami` /usr/local/Homebrew/
 
sudo chown -R $(whoami) $(brew --prefix)/*
 
sudo mkdir /usr/local/Frameworks
 
sudo chown -R `whoami` /usr/local/Frameworks/
```


# 参考链接
1. [macOS High Sierra(10.13.6)解决"Error: Running Homebrew as root is extremely dangerous and no longer supported."](https://www.mobibrw.com/2018/13593)