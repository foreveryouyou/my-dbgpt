# DB-GPT 部署相关

## 模型管理

- 目前模型管理好像是基于内存的, 重启后需要重新配置, 没办法持久化

## chroma 配置

### 向量数据存储路径

```ini
### Chroma vector db config
#CHROMA_PERSIST_PATH=/root/DB-GPT/pilot/data
CHROMA_PERSIST_PATH=/root/autodl-tmp/DB-GPT/pilot/data
```
