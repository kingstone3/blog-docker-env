From centos:7.6.1810

MAINTAINER WangDaLei <1244513986@qq.com>

RUN yum install -y wget

# Enable EPEL for Node.js
RUN yum install -y epel-release
RUN yum install -y nodejs

# RUN exec when build image,
# But mount volumes while runing container(after built),
# So can not use RUN CD website/src (website/src not mount that time)

# CMD exec when run container,
# Use '&&' to connect multi commends
CMD cd website/src && npm run start-website-admin-dev
