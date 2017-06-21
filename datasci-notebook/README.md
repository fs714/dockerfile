---
Run as

```
docker run -d --restart=always --name datasci --hostname datasci -e PASSWORD=<Password> -v /root/projects:/root/projects -p 8888:8888 daocloud.io/fs714/datasci-notebook
```
or
```
docker run -d --restart=always --name datasci --hostname datasci -e PASSWORD=<Password> -p 8888:8888 daocloud.io/fs714/datasci-notebook
```

