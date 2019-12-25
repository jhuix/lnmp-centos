FROM freecat888/centos-systemd:7
MAINTAINER freecat888<jhuix0117@gmail.com>
RUN yum -y install openssh-server; \
  yum -y install net-tools; \
  yum -y install wget; \
  yum -y install ntp; \
  yum clean all; \
  systemctl enable sshd
EXPOSE 22
CMD ["/usr/sbin/init"]
