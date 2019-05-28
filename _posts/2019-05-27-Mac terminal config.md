### Proxy

```
export http_proxy="http://127.0.0.1:1080"
export https_proxy="http://127.0.0.1:1080"
export all_proxy="socks5://127.0.0.1:1086"
```


### Git

```
git config --global http.proxy "http://127.0.0.1:1080"
git config --global https.proxy "http://127.0.0.1:1080"

git config --global --unset http.proxy
git config --global --unset https.proxy
```

### Python

```
sudo pip install --user module
sudo pip install --upgrade module
sudo pip install --user module --proxy 127.0.0.1:1080
```

