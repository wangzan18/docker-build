## create hexo container,just run:
```
# docker run -d --name wz-hexo -p 4000:4000 -v <local-dir>:/opt/hexo/source/_posts/ wangzan18/hexo
```
## enter the hexo container ,just run:
```
# docker exec -it wz-hexo bash
```
## visit the Hexo website
```
just visit http://127.0.0.1:4000 through your web browser. or curl http://127.0.0.1:4000
```
## 配置 git
```
git config --global user.name "wangzan18"// 你的github用户名，非昵称
git config --global user.email  "wangzan18@126.com"// 填写你的github注册邮箱
```
## 配置秘钥
```
ssh-keygen -t rsa -C "wangzan18@126.com"
```

## 小技巧
```
# 简要显示文章内容，在文档中输入下面字符，上下各留一行
<!--more-->
```
