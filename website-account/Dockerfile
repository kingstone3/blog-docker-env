From centos:7.6.1810

MAINTAINER WangDaLei <1244513986@qq.com>

RUN curl -sL https://rpm.nodesource.com/setup_12.x | bash -
RUN yum install -y nodejs
RUN npm upgrade npm -g

RUN npm install nodemon -g

CMD ln -sf /website/src/servers/common /website/src/servers/website-account/common \
    && cd website/src/servers \
    && npm run start-account-dev
