## git配置

## 代理
* 普通代理

git config --global https.proxy http://127.0.0.1:1080

git config --global https.proxy https://127.0.0.1:1080

* socks5代理

git config --global http.proxy socks5://127.0.0.1:1080

git config --global https.proxy socks5://127.0.0.1:1080

* 取消代理

git config --global --unset http.proxy

git config --global --unset https.proxy

* 设置网络缓存

设置缓存500MB：git config --global http.postBuffer 524288000