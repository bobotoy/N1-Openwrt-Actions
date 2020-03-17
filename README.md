# N1-Openwrt-Actions
默认ip已更换为192.168.2.1
食用方法
下载并导入openwrt镜像包
----①.将docker-img-openwrt-aarch64-****.gz文件上传至N1的/root目录
----②.ssh到N1
----③.导入软路由docker包：
----gzip -dc docker-img-openwrt-aarch64-r9.10.24.gz | docker load
----或者docker pull bobotoy/openwrt-aarch64:****
----docker run  -d --restart always --network macnet --ip 192.168.2.1  --privileged bobotoy/openwrt-aarch64:****  /sbin/init
借鉴引用以下代码，感谢各位大佬付出

https://github.com/fyglinfo/actions-openwrt-passwall

https://github.com/P3TERX/Actions-OpenWrt

https://github.com/Lienol/openwrt-package

https://github.com/coolsnowwolf/lede

https://github.com/zorzcc/openwrt-actions
