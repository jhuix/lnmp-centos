FROM freecat888/centos-sshd:7
MAINTAINER freecat888<jhuix0117@gmail.com>
RUN yum -y install epel-release; \
  rpm --import https://www.elrepo.org/RPM-GPG-KEY-elrepo.org; \
  rpm -Uvh https://www.elrepo.org/elrepo-release-7.0-2.el7.elrepo.noarch.rpm; \
  rpm -Uvh https://li.nux.ro/download/nux/dextop/el7/x86_64/nux-dextop-release-0-5.el7.nux.noarch.rpm; \
  yum clear all; \
  yum makecache; \
  yum -y install redhat-lsb; \
  yum -y install ksh; \
  yum -y install libXext.so.6; \
  yum -y install libXtst.so.6; \
  yum -y install libXt.so.6; \ 
  yum -y install libGLU*; \
  yum -y install libelf.so.1; \ 
  yum -y install libXrender.so.1; \
  yum -y install libXp.so.6; \ 
  yum -y install libXrandr.so.2; \
  yum -y install *xorg*; \  
  yum -y install libXp; \ 
  yum -y install ld-linux.so.2; \
  yum -y install openmotif; \ 
  yum -y install libstdc++.so.5v; \
  yum -y install libstdc++.so.6; \
  yum -y install xterm; \
  yum -y install gcc gcc-c++ csh compat-libstdc++-33.i686; \
  yum -y install alliance-libs alliance glibc-devel.i686 glibc; \
  ln -s /bin/gunzip /bin/uncompress; \
  cd /lib64; \
  ln -s libreadline.so.6 libreadline.so.5; \
  ln -s libcrypto.so.10 libcrypto.so.6; \
  cd /usr/lib64; \
  ln -s libhistory.so.6 libhistory.so.5
EXPOSE 22
CMD ["/usr/sbin/init"]
