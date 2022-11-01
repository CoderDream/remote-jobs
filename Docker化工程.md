



# Docker登录并上传镜像到docker hub中

### 打包命令

```
# 一步到位
docker build . -t coderdream/remote-jobs:1.0.0

# 或者分步骤
docker build . -t remote-jobs:1.0.0
docker tag remote-jobs:1.0.0 coderdream/remote-jobs:1.0.0
```

### 推送命令

```
docker run -p 49162:8080 -d coderdream/remote-jobs:1.0.0
```

### 本地使用

#### 命令

```
docker run -p 49162:8080 -d coderdream/remote-jobs:1.0.0
```

#### 部署

![image-20221101174401791](assets\image-20221101174401791.png)

#### 访问

```
http://192.168.3.4:49162/
```

![image-20221101174555572](assets\image-20221101174555572.png)



# END