# 将标准Anthropic Claude请求转发至VertexAI Claude
代码来自[VertexAI Claude](https://github.com/TheValkyrja/Anthropic2Vertex)，使用Github进行编译，并上传至Docker Hub

**注意：**

auth.json文件需从GCP获取

.env文件需完善

**运行方法：**

```
# 创建名为nginx的Docker网络
sudo docker network create nginx

# 启动Docker容器
sudo docker compose up -d
```