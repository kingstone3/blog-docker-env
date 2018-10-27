From centos:7.5.1804

MAINTAINER WangDaLei <1244513986@qq.com>

RUN yum install -y wget

# Enable EPEL for Node.js
RUN yum install -y epel-release

RUN yum install -y nodejs

RUN wget https://dl.yarnpkg.com/rpm/yarn.repo -O /etc/yum.repos.d/yarn.repo
RUN yum install -y yarn

# RUN exec when build image,
# But mount volumes while runing container(after built),
# So can not use RUN CD website/src (websit/src not mount that time)

# CMD exec when run container,
# Use '&&' to connect multi commend
CMD cd website/src && npm start
