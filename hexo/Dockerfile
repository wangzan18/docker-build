# Version 0.0.1
FROM centos:7.7.1908
MAINTAINER wangzan18
ENV PATH $PATH:/usr/local/node/bin
WORKDIR /opt/
RUN yum install wget git -y \
    && wget https://nodejs.org/dist/v12.13.0/node-v12.13.0-linux-x64.tar.xz \
    && tar xf node-v12.13.0-linux-x64.tar.xz \
    && mv node-v12.13.0-linux-x64 /usr/local/node \
    && mkdir hexo \
    && cd hexo \
    && npm install -g hexo \
    && hexo init \
    && npm install hexo-deployer-git --save \
    && rm -rf /opt/node-v12.13.0-linux-x64.tar.xz
WORKDIR /opt/hexo/
EXPOSE 4000
ENTRYPOINT ["hexo","server"]
