# 概述
Android Studio自带的SDK管理器升级的时候花费大量时间，可以将SDK相关文件手动下载后，释放到SDK对应目录，然后启动SDK Manager完成更新。路劲中的版本号替换为想要下载的版本即可，可以实现在SDK Manager中查看选择

# 镜像地址
将google的地址改成镜像地址即可手动下载，我一般用腾讯：

腾讯Bugly 镜像:
http://android-mirror.bugly.qq.com:8080
腾讯镜像使用方法: http://android-mirror.bugly.qq.com:8080/include/usage.html

北京化工大学镜像服务器地址:
IPv4: http://ubuntu.buct.edu.cn/ 端口：80
IPv4: http://ubuntu.buct.cn/ 端口：80
IPv6: http://ubuntu.buct6.edu.cn/ 端口：80

上海GDG镜像服务器地址:
http://sdk.gdgshanghai.com 端口：8000

中国科学院开源协会镜像站地址:
IPV4/IPV6: http://mirrors.opencas.cn 端口：80
IPV4/IPV6: http://mirrors.opencas.org 端口：80
IPV4/IPV6: http://mirrors.opencas.ac.cn 端口：80

# 直接覆盖
1. Android SDK：Android SDK主安装包，包含SDK Manager、AVD Manager、工具包tools，释放到根文件夹(android-sdk-windows)
	http://dl.google.com/android/android-sdk_r24.4.1-windows.zip

	http://dl.google.com/android/installer_r24.4.1-windows.exe
	http://dl.google.com/android/android-sdk_r24.4.1-macosx.zip
	http://dl.google.com/android/android-sdk_r24.4.1-linux.tgz
2. tools：Android SDK的工具包，释放到android-sdk-windows下，文件夹tools覆盖android-sdk-windows/tools
	https://dl-ssl.google.com/android/repository/tools_r25.1.7-windows.zip

	https://dl-ssl.google.com/android/repository/tools_r25.1.7-linux.zip
	https://dl-ssl.google.com/android/repository/tools_r25.1.7-macosx.zip

# 通过SDK Manager自动安装释放到相应位置
可以将安装包放在文件夹android-sdk-windows/temp下，通过SDK Manager自动安装释放到相应位置.
1. platform-tools：Android平台工具包，释放到android-sdk-windows下，产生文件夹platform-tools
	https://dl-ssl.google.com/android/repository/platform-tools_r24-windows.zip
	https://dl-ssl.google.com/android/repository/platform-tools_r24-linux.zip
	https://dl-ssl.google.com/android/repository/platform-tools_r24-macosx.zip
2. build-tools：释放到android-sdk-windows下，产生文件夹build-tools，各版本都可能用到
	https://dl-ssl.google.com/android/repository/build-tools_r24.0.1-windows.zip
	https://dl-ssl.google.com/android/repository/build-tools_r24.0.1-linux.zip
	https://dl-ssl.google.com/android/repository/build-tools_r24.0.1-macosx.zip