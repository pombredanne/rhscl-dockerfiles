FROM rhel6
MAINTAINER docker@softwarecollections.org
RUN yum update -y && yum clean all
RUN yum install -y yum-utils && yum clean all
RUN yum-config-manager --enable rhel-server-rhscl-6-rpms
RUN yum-config-manager --enable rhel-6-server-optional-rpms
RUN yum install -y --setopt=tsflags=nodocs perl516 && yum clean all

ADD ./enableperl516.sh /etc/profile.d/