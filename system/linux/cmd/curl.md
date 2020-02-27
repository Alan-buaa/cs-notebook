# curl

https://tecadmin.net/curl-command-with-proxy/

**curl使用代理**

利用环境变量

```shell
Without Authentication 

export http_proxy="http://proxy.server:port"
export https_proxy="https://proxy.server:port"

With Authentication 

export http_proxy="http://username:password@proxy.server:port"
export https_proxy="https://username:password@proxy.server:port"
```

去掉环境变量

```shell
unset http_proxy
unset https_proxy
```



不使用环境变量

```shell
curl -x "http://username:password@proxy.server:port" http://example.com
```

