### 简介
> pyenv lets you easily switch between multiple versions of Python. It's simple, unobtrusive, and follows the UNIX tradition of single-purpose tools that do one thing well.

### 手动安装

```
git clone https://github.com/pyenv/pyenv.git ~/.pyenv
```

### 自动安装

```
curl https://pyenv.run | bash
------------------------------
% Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:--  0:00:10 --:--:--     0
curl: (35) LibreSSL SSL_connect: SSL_ERROR_SYSCALL in connection to pyenv.run:443 
➜  ~ curl https://pyenv.run | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   259  100   259    0     0      4      0  0:01:04  0:01:00  0:00:04    64
Cloning into '/Users/luoxiaolei/.pyenv'...
remote: Enumerating objects: 643, done.
remote: Counting objects: 100% (643/643), done.
remote: Compressing objects: 100% (484/484), done.
remote: Total 643 (delta 317), reused 244 (delta 68), pack-reused 0
Receiving objects: 100% (643/643), 371.66 KiB | 13.00 KiB/s, done.
Resolving deltas: 100% (317/317), done.
Cloning into '/Users/luoxiaolei/.pyenv/plugins/pyenv-doctor'...
warning: You appear to have cloned an empty repository.
Cloning into '/Users/luoxiaolei/.pyenv/plugins/pyenv-installer'...
remote: Enumerating objects: 16, done.
remote: Counting objects: 100% (16/16), done.
remote: Compressing objects: 100% (13/13), done.
remote: Total 16 (delta 1), reused 8 (delta 0), pack-reused 0
Unpacking objects: 100% (16/16), done.
Cloning into '/Users/luoxiaolei/.pyenv/plugins/pyenv-update'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 10 (delta 1), reused 6 (delta 0), pack-reused 0
Unpacking objects: 100% (10/10), done.
Cloning into '/Users/luoxiaolei/.pyenv/plugins/pyenv-virtualenv'...
remote: Enumerating objects: 57, done.
remote: Counting objects: 100% (57/57), done.
remote: Compressing objects: 100% (51/51), done.
remote: Total 57 (delta 11), reused 21 (delta 0), pack-reused 0
Unpacking objects: 100% (57/57), done.
Cloning into '/Users/luoxiaolei/.pyenv/plugins/pyenv-which-ext'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 10 (delta 1), reused 6 (delta 0), pack-reused 0
Unpacking objects: 100% (10/10), done.

WARNING: seems you still have not added 'pyenv' to the load path.

# Load pyenv automatically by adding
# the following to ~/.bashrc:

export PATH="/Users/luoxiaolei/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"

```

### 配置环境变量
#### bash
```
$ echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
$ echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
$ echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bash_profile
```

#### Zsh
```
$ echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshenv
$ echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshenv
$ echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.zshenv
```

### 参考链接
- [pyenv](https://github.com/pyenv/pyenv#installation)
- [automatic installer](https://github.com/pyenv/pyenv-installer)