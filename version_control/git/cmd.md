# Command

#### 保存用户名密码

```shell
git config credential.helper store
```

输入上述命令，然后第一次拉取代码的时候输入用户名、密码，就会记录到系统中。

这样保存的密码是明文的，保存在用户目录~的.git-credentials文件中

