From centos:7.6.1810

MAINTAINER WangDaLei <1244513986@qq.com>

RUN curl -sL https://rpm.nodesource.com/setup_10.x | bash -
RUN yum install -y nodejs
RUN npm upgrade npm -g

RUN npm install nodemon -g

CMD cd website/src/servers && npm run start-account-dev
