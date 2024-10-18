# DB-GPT 部署相关(AutoDL)

## 模型管理

- 目前模型管理好像是基于内存的, 重启后需要重新配置, 没办法持久化

## 路径相关

```shell
# 将知识库文件路径设置到数据盘
mkdir -p /root/autodl-tmp/DB-GPT/pilot/data
ln -s /root/autodl-tmp/DB-GPT/pilot/data /root/DB-GPT/pilot/data
```

### chroma 向量数据存储路径配置 [可选]

> 这只影响向量数据路径, 影响不了上传的文件路径, 要影响整个存储路径就按上面的软链方法配置

```ini
### Chroma vector db config
#CHROMA_PERSIST_PATH=/root/DB-GPT/pilot/data
CHROMA_PERSIST_PATH=/root/autodl-tmp/DB-GPT/pilot/data
```
