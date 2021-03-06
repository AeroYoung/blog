# 概述
Android Studio自带的SDK管理器升级的时候花费大量时间，可以将SDK相关文件手动下载后，释放到SDK对应目录，然后启动SDK Manager完成更新。路劲中的版本号替换为想要下载的版本即可，可以实现在SDK Manager中查看选择

# 镜像地址
将google的地址改成镜像地址即可手动下载，我一般用腾讯：

	http://android-mirror.bugly.qq.com:8080
	腾讯镜像使用方法: http://android-mirror.bugly.qq.com:8080/include/usage.html

# 直接覆盖
1. Android SDK：Android SDK主安装包，包含SDK Manager、AVD Manager、工具包tools，释放到根文件夹(android-sdk-windows)
	http://dl.google.com/android/android-sdk_r24.4.1-windows.zip
2. tools：Android SDK的工具包，释放到android-sdk-windows下，文件夹tools覆盖android-sdk-windows/tools
	https://dl-ssl.google.com/android/repository/tools_r25.1.7-windows.zip

# 通过SDK Manager自动安装释放到相应位置
可以将安装包放在文件夹android-sdk-windows/temp下，通过SDK Manager自动安装释放到相应位置. 然后启动SDK Manager选中刚才下载的文件，点击install。这时候其实已经下载好了，Manager会自动解压并安装。

1. platform-tools：Android平台工具包，释放到android-sdk-windows下，产生文件夹platform-tools
	https://dl-ssl.google.com/android/repository/platform-tools_r24-windows.zip

2. build-tools：释放到android-sdk-windows下，产生文件夹build-tools，各版本都可能用到
	https://dl-ssl.google.com/android/repository/build-tools_r24.0.1-windows.zip

3. platforms (各种版本的Android平台，释放到android-sdk-windows/platforms下)
	https://dl-ssl.google.com/android/repository/platform-24_r01.zip

4. system-images (Android系统镜像，释放到android-sdk-windows/system-images/android-xx下[xx对应api版本数字])
	https://dl-ssl.google.com/android/repository/sys-img/android-tv/sysimg_atv_x86-24_r05.zip

	https://dl-ssl.google.com/android/repository/sys-img/android-wear/sysimg_wear_armeabi-v7a-24_r01.zip

	https://dl-ssl.google.com/android/repository/sys-img/android-wear/sysimg_wear_x86-24_r01.zip

	https://dl-ssl.google.com/android/repository/sys-img/android/sysimg_armeabi-v7a-24_r05.zip

	https://dl-ssl.google.com/android/repository/sys-img/android/sysimg_x86-24_r05.zip

	https://dl-ssl.google.com/android/repository/sys-img/android/sysimg_x86_64-24_r05.zip

5. docs (文档，释放到android-sdk-windows下，会产生文件夹docs)
	https://dl-ssl.google.com/android/repository/docs-23_r01.zip

6. samples (应用实例，释放到android-sdk-windows/samples下)
	https://dl-ssl.google.com/android/repository/samples-23_r02.zip

7. sources (Android SDK源程序，释放到android-sdk-windows/sources/android-xx下[xx对应api版本数字])
	https://dl-ssl.google.com/android/repository/sources-23_r01.zip

8. extras (扩展应用，释放到android-sdk-windows/extras下)
	* GPU Debugging tools 3.1
	https://dl-ssl.google.com/android/repository/extras/gapid/gapid_r01_windows.zip

	* Android Support Library(extras/android/support)
	https://dl-ssl.google.com/android/repository/support_r23.2.1.zip

	* Android Auto Desktop Head Unit emulator
	https://dl-ssl.google.com/android/repository/extras/auto/desktop-head-unit-windows_r01.1.zip

	* Google AdMob Ads SDK(extras/google/admob_ads_sdk) (Obsolete)
	https://dl-ssl.google.com/googleadmobadssdk/googleadmobadssdkandroid-6.4.1.zip

	* Google Analytics App Tracking SDK(extras/google/analytics_sdk_v2) (Obsolete)
	https://dl.google.com/gaformobileapps/GoogleAnalyticsAndroid_2.0beta5.zip

	* Google Cloud Messaging for Android Library(extras/google/gcm) (Obsolete)
	https://dl-ssl.google.com/android/repository/gcm_r03.zip

	* Google Play services for Froyo
	https://dl-ssl.google.com/android/repository/google_play_services_3265130_r12.zip

	* Google Play services(extras/google/google_play_services)
	https://dl-ssl.google.com/android/repository/google_play_services_9256000_r31.zip

	* Google Repository(extras/google/m2repository)
	https://dl-ssl.google.com/android/repository/google_m2repository_r31.zip

	* Google Play APK Expansion Library(extras/google/play_apk_expansion)
	https://dl-ssl.google.com/android/repository/market_apk_expansion-r03.zip

	* Google Play Billing Library(extras/google/play_billing)
	https://dl-ssl.google.com/android/repository/play_billing_r05.zip

	* Google Play Licensing Library(extras/google/play_licensing)
	https://dl-ssl.google.com/android/repository/market_licensing-r02.zip

	* Android Auto API Simulators
	https://dl-ssl.google.com/android/repository/simulator_r01.zip

	* Google USB Driver(extras/usb_driver)
	https://dl-ssl.google.com/android/repository/usb_driver_r11-windows.zip

	* Google Web Driver(extras/google/webdriver)
	https://dl-ssl.google.com/android/repository/webdriver_r02.zip

9. add-ons (google手机api,释放到android-sdk-windows/add-ons/)
	https://dl-ssl.google.com/android/repository/google_apis-19_r20.zip  

10. Google APIs (ARM System Image)
	https://dl-ssl.google.com/android/repository/sys-img/x86/google_apis_x86-19_r13.zip  

11. Google APIs (x86 System Image)
	https://dl-ssl.google.com/android/repository/google_apis-23_r01.zip
