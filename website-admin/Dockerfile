From centos:7.6.1810

MAINTAINER WangDaLei <1244513986@qq.com>

RUN curl -sL https://rpm.nodesource.com/setup_12.x | bash -
RUN yum install -y nodejs
RUN npm upgrade npm -g

RUN npm install nodemon -g

# RUN exec when build image,
# But mount volumes while runing container(after built),
# So can not use RUN CD website/src (website/src not mount that time)

# CMD exec when run container,
# Use '&&' to connect multi commends
CMD ln -sf /website/src/servers/common /website/src/servers/website-admin/common \
    && cd website/src/servers \
    && npm run start-admin-dev
