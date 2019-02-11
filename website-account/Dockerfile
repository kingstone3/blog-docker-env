From centos:7.6.1810

MAINTAINER WangDaLei <1244513986@qq.com>

RUN yum install -y wget

RUN yum install -y epel-release
RUN yum install -y nodejs

CMD cd website/src && npm run start-website-account-dev
