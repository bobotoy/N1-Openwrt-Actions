FROM scratch
#FROM multiarch/ubuntu-debootstrap:arm64-bionic-slim
#ENV ARCH=arm64
ADD openwrt-armvirt-64-default-rootfs-patched.tar /
EXPOSE 22 80 443
# using exec format so that /sbin/init is proc 1 (see procd docs)
ENTRYPOINT ["/sbin/init"]
