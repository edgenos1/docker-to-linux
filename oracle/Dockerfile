FROM oraclelinux:7.6@sha256:a6ee3b4c6a52a529a6de77bb25c3d0a99e99e1ad81cd936cd14b100288ffe246
LABEL com.iximiuz-project="docker-to-linux"

RUN mkdir -p /usr/share/info

RUN yum-config-manager --enable ol7_latest
RUN yum -y install deltarpm
RUN yum -y update
RUN yum -y install grub2 kernel-uek dracut-fips dracut-fips-aesni

RUN ln -s /boot/vmlinuz-* /boot/vmlinuz
RUN ln -s /boot/initramfs-* /boot/initramfs
