### 简介
> Use rbenv to pick a Ruby version for your application and guarantee that your development environment matches production. 

### 安装rbenv

```
$ brew install rbenv
```

```
$ rbenv init
---------------------------------------
# Load rbenv automatically by appending
# the following to ~/.zshrc:

eval "$(rbenv init -)"
```


```
$ vi .zshrc 
add eval "$(rbenv init -)" to .zshrc 
$ source .zshrc 
```


```
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash
---------------------------------------------------
Checking for `rbenv' in PATH: /usr/local/bin/rbenv
Checking for rbenv shims in PATH: OK
Checking `rbenv install' support: /usr/local/bin/rbenv-install (ruby-build 20190423)
Counting installed Ruby versions: none
  There aren't any Ruby versions installed under `/Users/luoxiaolei/.rbenv/versions'.
  You can install Ruby versions like so: rbenv install 2.2.4
Checking RubyGems settings: OK
Auditing installed plugins: OK
```

### 安装ruby

```
# list all available versions:
$ rbenv install -l
```

```
# install a Ruby version:
$ rbenv install 2.6.3
---------------------------------------------------
ruby-build: use openssl from homebrew
Downloading ruby-2.6.3.tar.bz2...
-> https://cache.ruby-lang.org/pub/ruby/2.6/ruby-2.6.3.tar.bz2
Installing ruby-2.6.3...
Installed ruby-2.6.3 to /Users/luoxiaolei/.rbenv/versions/2.6.3
```

```
$ rbenv version
system (set by /Users/luoxiaolei/.rbenv/version)
```

```
$ rbenv local 2.6.3
$ rbenv version    
2.6.3 (set by /Users/luoxiaolei/.ruby-version)
```

### 安装Ruby gems

```
# 切换版本后需要刷新一下，否则安装报错
-----------------------------------------------
gem install bundler
Fetching: bundler-2.0.1.gem (100%)
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /Library/Ruby/Gems/2.3.0 directory.
-----------------------------------------------
$ rbenv rehash
```

```
$ gem install bundler
--------------------------------------------------
Fetching bundler-2.0.1.gem
Successfully installed bundler-2.0.1
Parsing documentation for bundler-2.0.1
Installing ri documentation for bundler-2.0.1
Done installing documentation for bundler after 2 seconds
1 gem installed
```

```
# 查看gem安装位置
gem env home
/Users/luoxiaolei/.rbenv/versions/2.6.3/lib/ruby/gems/2.6.0
```

### 参考连接
- [rbenv](https://github.com/rbenv/rbenv#how-rbenv-hooks-into-your-shell)

