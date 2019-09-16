FROM freecat888/centos-systemd
MAINTAINER freecat888<jhuix0117@gmail.com>
RUN yum -y install openssh-server; yum clean all; systemctl enable sshd
EXPOSE 22
CMD ["/usr/sbin/init"]
