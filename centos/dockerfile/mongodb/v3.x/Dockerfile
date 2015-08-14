#
# MongoDB Dockerfile
#
# https://github.com/cowpanda/MyFavorites
#

FROM centos:centos7

RUN 
yum -y update && \
yum -y install wget && \
wget https://raw.githubusercontent.com/CowPanda/cowpanda.github.io/master/packages/centos/yum/mongodb-org-3.0.repo -P /etc/yum.repos.d/ && \
yum -y install mongodb-org && \
yum clean all

# Define mountable directories(map host).
VOLUME ["/data/db"]

EXPOSE 27017
EXPOSE 28017
ENTRYPOINT ["/usr/bin/mongod"]