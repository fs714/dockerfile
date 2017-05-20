---
Run as

```
docker run -d --restart=always --name notebook --hostname notebook -e PASSWORD=<Password> -v /root/projects:/root/projects -p 8888:8888 daocloud.io/fs714/jupyter-notebook
```
or
```
docker run -d --restart=always --name notebook --hostname notebook -e PASSWORD=<Password> -p 8888:8888 daocloud.io/fs714/jupyter-notebook
```

