# 云编译N1 Openwrt固件 Docker
默认ip已更换为192.168.2.1

# 食用方法
1.将docker-img-openwrt-aarch64-r9.10.24.gz文件上传至N1的/root目录  
2.gzip -dc docker-img-openwrt-aarch64-r9.10.24.gz | docker load 或者 docker pull bobotoy/openwrt-aarch64:****  
3.docker run  -d --restart always --network macnet --ip 192.168.2.1  --privileged bobotoy/openwrt-aarch64:****  /sbin/init  

# 鸣谢
借鉴引用以下代码，感谢各位大佬付出
https://github.com/fyglinfo/actions-openwrt-passwall

https://github.com/P3TERX/Actions-OpenWrt

https://github.com/Lienol/openwrt-package

https://github.com/coolsnowwolf/lede

https://github.com/zorzcc/openwrt-actions
