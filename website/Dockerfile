From centos:7.5.1804

MAINTAINER WangDaLei <1244513986@qq.com>

# Enable EPEL for Node.js
RUN rpm -Uvh http://download.fedoraproject.org/pub/epel/6/i386/epel-release-6-8.noarch.rpm

# Install Nodejs and NPM
RUN yum install -y nodejs

ENV NODE_ENV production

RUN ls
RUN cd /blog;
RUN npm install

CMD ["npm", "start"]
