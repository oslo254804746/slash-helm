
## 介绍
这是一个部署`slash`的 `helm chart`

对应仓库[yourselfhosted-slash](https://github.com/yourselfhosted/slash)


## 配置项

### volume
默认是`hostPath`, 挂载地址为`/var/opt/slash`, 请根据实际情况修改类型
```yaml
volumes:
 - name: slash-volume
   hostPath:
     path: /data/slash
     type: DirectoryOrCreate
```

