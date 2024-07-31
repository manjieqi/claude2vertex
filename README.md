# 将标准Anthropic Claude请求转发至VertexAI Claude
代码来自[VertexAI Claude](https://github.com/TheValkyrja/Anthropic2Vertex)，使用Github进行编译，并上传至Docker Hub

**注意：**

auth内json文件需从GCP获取，命名为项目名

.env文件需完善

**运行方法：**

```
# 创建名为nginx的Docker网络
sudo docker network create nginx

# 构建镜像(可选，需修改compose文件中对应镜像)
sudo docker build -t claude2vertex ./build

# 启动Docker容器
sudo docker compose up -d
```