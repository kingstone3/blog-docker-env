From centos:7.6.1810

MAINTAINER WangDaLei <1244513986@qq.com>

RUN yum install -y wget

RUN curl -sL https://rpm.nodesource.com/setup_10.x | bash -
RUN yum install -y nodejs
RUN npm upgrade npm -g

CMD cd website/src && npm run start-website-account-dev
