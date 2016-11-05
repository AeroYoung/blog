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
可以将安装包放在文件夹android-sdk-windows/temp下，通过SDK Manager自动安装释放到相应位置. 然后启动SDK Manager选中刚才下载的文件，点击install。这时候其实已经下载好了，Manager会自动解压并安装。
1. platform-tools：Android平台工具包，释放到android-sdk-windows下，产生文件夹platform-tools
	https://dl-ssl.google.com/android/repository/platform-tools_r24-windows.zip
	https://dl-ssl.google.com/android/repository/platform-tools_r24-linux.zip
	https://dl-ssl.google.com/android/repository/platform-tools_r24-macosx.zip
2. build-tools：释放到android-sdk-windows下，产生文件夹build-tools，各版本都可能用到
	https://dl-ssl.google.com/android/repository/build-tools_r24.0.1-windows.zip
	https://dl-ssl.google.com/android/repository/build-tools_r24.0.1-linux.zip
	https://dl-ssl.google.com/android/repository/build-tools_r24.0.1-macosx.zip
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
	https://dl-ssl.google.com/android/repository/samples-2.1_r01-linux.zip
	https://dl-ssl.google.com/android/repository/samples-2.2_r01-linux.zip
	https://dl-ssl.google.com/android/repository/samples-2.3_r01-linux.zip
	https://dl-ssl.google.com/android/repository/samples-2.3.3_r01-linux.zip
	https://dl-ssl.google.com/android/repository/samples-3.0_r01-linux.zip
	https://dl-ssl.google.com/android/repository/samples-3.1_r01-linux.zip
	https://dl-ssl.google.com/android/repository/samples-3.2_r01-linux.zip
	https://dl-ssl.google.com/android/repository/samples-14_r02.zip
	https://dl-ssl.google.com/android/repository/samples-15_r02.zip
	https://dl-ssl.google.com/android/repository/samples-16_r01.zip
	https://dl-ssl.google.com/android/repository/samples-17_r01.zip
	https://dl-ssl.google.com/android/repository/samples-18_r01.zip
	https://dl-ssl.google.com/android/repository/samples-19_r06.zip
	https://dl-ssl.google.com/android/repository/samples-20_r03.zip
	https://dl-ssl.google.com/android/repository/samples-21_r04.zip
	https://dl-ssl.google.com/android/repository/samples-22_r06.zip
	https://dl-ssl.google.com/android/repository/samples-23_r02.zip
7. sources (Android SDK源程序，释放到android-sdk-windows/sources/android-xx下[xx对应api版本数字])
	https://dl-ssl.google.com/android/repository/sources-14_r01.zip
	https://dl-ssl.google.com/android/repository/sources-15_r02.zip
	https://dl-ssl.google.com/android/repository/sources-16_r02.zip
	https://dl-ssl.google.com/android/repository/sources-17_r01.zip
	https://dl-ssl.google.com/android/repository/sources-18_r01.zip
	https://dl-ssl.google.com/android/repository/sources-19_r02.zip
	https://dl-ssl.google.com/android/repository/sources-20_r01.zip
	https://dl-ssl.google.com/android/repository/sources-21_r01.zip
	https://dl-ssl.google.com/android/repository/sources-22_r01.zip
	https://dl-ssl.google.com/android/repository/sources-23_r01.zip

8. extras (扩展应用，释放到android-sdk-windows/extras下)

GPU Debugging tools 3.1
	https://dl-ssl.google.com/android/repository/extras/gapid/gapid_r01_linux.zip
	https://dl-ssl.google.com/android/repository/extras/gapid/gapid_r01_osx.zip
	https://dl-ssl.google.com/android/repository/extras/gapid/gapid_r01_windows.zip

GPU Debugging tools 1.0.3
https://dl-ssl.google.com/android/repository/extras/gapid/gapid_2994895_windows.zip
https://dl-ssl.google.com/android/repository/extras/gapid/gapid_2994895_linux.zip
https://dl-ssl.google.com/android/repository/extras/gapid/gapid_2994895_osx.zip
Android Support Repository(extras/android/m2repository)
https://dl-ssl.google.com/android/repository/android_m2repository_r35.zip

Android Support Library(extras/android/support)
https://dl-ssl.google.com/android/repository/support_r23.1.1.zip
https://dl-ssl.google.com/android/repository/support_r23.2.1.zip

Android Auto Desktop Head Unit emulator
https://dl-ssl.google.com/android/repository/extras/auto/desktop-head-unit-windows_r01.1.zip
https://dl-ssl.google.com/android/repository/extras/auto/desktop-head-unit-linux_r01.1.zip
https://dl-ssl.google.com/android/repository/extras/auto/desktop-head-unit-macosx_r01.1.zip

Google AdMob Ads SDK(extras/google/admob_ads_sdk) (Obsolete)
https://dl-ssl.google.com/googleadmobadssdk/googleadmobadssdkandroid-6.4.1.zip
Google Analytics App Tracking SDK(extras/google/analytics_sdk_v2) (Obsolete)
https://dl.google.com/gaformobileapps/GoogleAnalyticsAndroid_2.0beta5.zip
Google Cloud Messaging for Android Library(extras/google/gcm) (Obsolete)
https://dl-ssl.google.com/android/repository/gcm_r03.zip

Google Play services for Froyo
https://dl-ssl.google.com/android/repository/google_play_services_3265130_r12.zip

Google Play services(extras/google/google_play_services)
https://dl-ssl.google.com/android/repository/google_play_services_8487000_r29.zip
https://dl-ssl.google.com/android/repository/google_play_services_9080000_r30.zip
https://dl-ssl.google.com/android/repository/google_play_services_9256000_r31.zip

Google Repository(extras/google/m2repository)
https://dl-ssl.google.com/android/repository/google_m2repository_r25.zip
https://dl-ssl.google.com/android/repository/google_m2repository_r26.zip
https://dl-ssl.google.com/android/repository/google_m2repository_r31.zip

Google Play APK Expansion Library(extras/google/play_apk_expansion)
https://dl-ssl.google.com/android/repository/market_apk_expansion-r03.zip

Google Play Billing Library(extras/google/play_billing)
https://dl-ssl.google.com/android/repository/play_billing_r05.zip
Google Play Licensing Library(extras/google/play_licensing)
https://dl-ssl.google.com/android/repository/market_licensing-r02.zip

Android Auto API Simulators
https://dl-ssl.google.com/android/repository/simulator_r01.zip
Google USB Driver(extras/usb_driver)
https://dl-ssl.google.com/android/repository/usb_driver_r10-windows.zip
https://dl-ssl.google.com/android/repository/usb_driver_r11-windows.zip

Google Web Driver(extras/google/webdriver)
https://dl-ssl.google.com/android/repository/webdriver_r02.zip

Intel x86 Emulator Accelerator(HAXM installer)(extras/intel/Hardware_Accelerated_Execution_Manager)
https://software.intel.com/sites/default/files/haxm-windows_r03.zip
https://software.intel.com/sites/default/files/managed/21/5f/haxm-macosx_r05.zip
https://download-software.intel.com/sites/landingpage/android/extra_intel_haxm-windows_r03.zip
https://download-software.intel.com/sites/landingpage/android/extra_intel_haxm-macosx_r03.zip
https://dl-ssl.google.com/android/repository/extras/intel/haxm-windows_r05.zip
https://dl-ssl.google.com/android/repository/extras/intel/haxm-windows_r05.4.zip
https://dl-ssl.google.com/android/repository/extras/intel/haxm-macosx_r04.zip
https://dl-ssl.google.com/android/repository/extras/intel/haxm-macosx_r05.4.zip
https://dl-ssl.google.com/android/repository/extras/intel/haxm-windows_r6_0_3.zip
https://dl-ssl.google.com/android/repository/extras/intel/haxm-macosx_r6_0_3.zip

9. add-ons (google手机api,释放到android-sdk-windows/add-ons/)
addon-google_apis-google-xx[xx对应api版本数字]
https://dl-ssl.google.com/android/repository/google_apis-3-r03.zip
https://dl-ssl.google.com/android/repository/google_apis-4_r02.zip
https://dl-ssl.google.com/android/repository/google_apis-5_r01.zip
https://dl-ssl.google.com/android/repository/google_apis-6_r01.zip
https://dl-ssl.google.com/android/repository/google_apis-7_r01.zip
https://dl-ssl.google.com/android/repository/google_apis-8_r02.zip
https://dl-ssl.google.com/android/repository/google_apis-9_r02.zip
https://dl-ssl.google.com/android/repository/google_apis-10_r02.zip
https://dl-ssl.google.com/android/repository/google_apis-11_r01.zip
https://dl-ssl.google.com/android/repository/google_apis-12_r01.zip
https://dl-ssl.google.com/android/repository/google_apis-13_r01.zip
https://dl-ssl.google.com/android/repository/google_apis-14_r02.zip
https://dl-ssl.google.com/android/repository/google_apis-15_r02.zip
https://dl-ssl.google.com/android/repository/google_apis-16_r03.zip
https://dl-ssl.google.com/android/repository/google_apis-17_r04.zip
https://dl-ssl.google.com/android/repository/google_apis-18_r04.zip
https://dl-ssl.google.com/android/repository/google_apis-19_r20.zip  Google APIs (ARM System Image)
https://dl-ssl.google.com/android/repository/sys-img/x86/google_apis_x86-19_r13.zip  Google APIs (x86 System Image)


https://dl-ssl.google.com/android/repository/google_tv-12_r02.zip
https://dl-ssl.google.com/android/repository/google_tv-13_r01.zip


https://dl-ssl.google.com/android/repository/google_apis-21_r01.zip
https://dl-ssl.google.com/android/repository/google_apis-22_r01.zip
https://dl-ssl.google.com/android/repository/google_apis-23_r01.zip


Glass Development Kit Preview
https://dl.google.com/glass/xe22/google-gdk.zip


addon-intel_atom_x86_system_image-intel_corporation-xx
https://software.intel.com/sites/landingpage/android/addon_intel_sysimg_2.3.7_api-10.zip
addon-dual_screen_apis-kyocera_corporation-xx (Dual Screen api)
http://dl.kyocera-wireless.com/echobykyocera.com/ECHO-SDK-v1-03.zip
http://dl.kyocera-wireless.com/echobykyocera.com/ECHO-SDK-v2-00.zip
addon-sony_xperia_extensions_edk_2_0-sony_mobile_communications_ab-xx
http://dl-developer.sonymobile.com/edk/android/edk_2.0_ver2.zip
addon-real3d-lge-xx
http://developer.lgmobile.com/sdk/android/Real3D_addon_api-8_r01.zip
http://developer.lgmobile.com/sdk/android/Real3D_SDK_api-10_r02.zip
http://developer.lgmobile.com/sdk/android/Real3D_SDK_api-14_r01.zip
addon-htc_opensense_sdk-htc-15
http://dl.htcdev.com/sdk/zip/htc_opensense_sdk.zip
addon-htc_opensense_apis-16
http://dl.htcdev.com/sdk/zip/htc_opensense_apis.zip

10. ADT Plugin for Eclipse
http://dl.google.com/android/ADT-22.2.1.zip
http://dl.google.com/android/ADT-22.3.0.zip
http://dl.google.com/android/ADT-22.6.2.zip
http://dl.google.com/android/ADT-22.6.3.zip
http://dl.google.com/android/ADT-23.0.2.zip

11. Android Developer Tools(基于Eclipse的Android开发环境，已包含Eclipse与ADT).
revision 22.6.2
http://dl.google.com/android/adt/22.6.2/adt-bundle-windows-x86-20140321.zip
http://dl.google.com/android/adt/22.6.2/adt-bundle-windows-x86_64-20140321.zip
http://dl.google.com/android/adt/22.6.2/adt-bundle-mac-x86_64-20140321.zip
http://dl.google.com/android/adt/22.6.2/adt-bundle-linux-x86-20140321.zip
http://dl.google.com/android/adt/22.6.2/adt-bundle-linux-x86_64-20140321.zip
revision 23
http://dl.google.com/android/adt/adt-bundle-windows-x86-20140624.zip
http://dl.google.com/android/adt/adt-bundle-windows-x86_64-20140624.zip
http://dl.google.com/android/adt/adt-bundle-mac-x86_64-20140624.zip
http://dl.google.com/android/adt/adt-bundle-linux-x86-20140624.zip
http://dl.google.com/android/adt/adt-bundle-linux-x86_64-20140624.zip
revision 23.0.2
http://dl.google.com/android/adt/adt-bundle-windows-x86-20140702.zip
http://dl.google.com/android/adt/adt-bundle-windows-x86_64-20140702.zip
http://dl.google.com/android/adt/adt-bundle-mac-x86_64-20140702.zip
http://dl.google.com/android/adt/adt-bundle-linux-x86-20140702.zip
http://dl.google.com/android/adt/adt-bundle-linux-x86_64-20140702.zip

12. Android NDK
revision 9d
http://dl.google.com/android/ndk/android-ndk-r9d-windows-x86.zip
http://dl.google.com/android/ndk/android-ndk-r9d-windows-x86_64.zip
http://dl.google.com/android/ndk/android-ndk-r9d-darwin-x86.tar.bz2
http://dl.google.com/android/ndk/android-ndk-r9d-darwin-x86_64.tar.bz2
http://dl.google.com/android/ndk/android-ndk-r9d-linux-x86.tar.bz2
http://dl.google.com/android/ndk/android-ndk-r9d-linux-x86_64.tar.bz2
http://dl.google.com/android/ndk/android-ndk-r9d-cxx-stl-libs-with-debug-info.zip
revision 10c
http://dl.google.com/android/ndk/android-ndk-r10c-windows-x86.exe
http://dl.google.com/android/ndk/android-ndk-r10c-windows-x86_64.exe
http://dl.google.com/android/ndk/android-ndk-r10c-darwin-x86.bin
http://dl.google.com/android/ndk/android-ndk-r10c-darwin-x86_64.bin
http://dl.google.com/android/ndk/android-ndk-r10c-linux-x86.bin
http://dl.google.com/android/ndk/android-ndk-r10c-linux-x86_64.bin
revision 10d
http://dl.google.com/android/ndk/android-ndk-r10d-windows-x86.exe
http://dl.google.com/android/ndk/android-ndk-r10d-windows-x86_64.exe
http://dl.google.com/android/ndk/android-ndk-r10d-darwin-x86.bin
http://dl.google.com/android/ndk/android-ndk-r10d-darwin-x86_64.bin
http://dl.google.com/android/ndk/android-ndk-r10d-linux-x86.bin
http://dl.google.com/android/ndk/android-ndk-r10d-linux-x86_64.bin

13. Android Studio(The official Android IDE)
revision 1.5.1.0
https://dl.google.com/dl/android/studio/install/1.5.1.0/android-studio-bundle-141.2456560-windows.exe
https://dl.google.com/dl/android/studio/install/1.5.1.0/android-studio-ide-141.2456560-windows.exe
https://dl.google.com/dl/android/studio/ide-zips/1.5.1.0/android-studio-ide-141.2456560-windows.zip
https://dl.google.com/dl/android/studio/install/1.5.1.0/android-studio-ide-141.2456560-mac.dmg
https://dl.google.com/dl/android/studio/ide-zips/1.5.1.0/android-studio-ide-141.2456560-linux.zip
revision 2.1.1.0
https://dl.google.com/dl/android/studio/install/2.1.1.0/android-studio-bundle-143.2821654-windows.exe
https://dl.google.com/dl/android/studio/install/2.1.1.0/android-studio-ide-143.2821654-windows.exe
https://dl.google.com/dl/android/studio/ide-zips/2.1.1.0/android-studio-ide-143.2821654-windows.zip
https://dl.google.com/dl/android/studio/install/2.1.1.0/android-studio-ide-143.2821654-mac.dmg
https://dl.google.com/dl/android/studio/ide-zips/2.1.1.0/android-studio-ide-143.2821654-linux.zip
revision 2.1.2.0
https://dl.google.com/dl/android/studio/install/2.1.2.0/android-studio-bundle-143.2915827-windows.exe
https://dl.google.com/dl/android/studio/install/2.1.2.0/android-studio-ide-143.2915827-windows.exe
https://dl.google.com/dl/android/studio/ide-zips/2.1.2.0/android-studio-ide-143.2915827-windows.zip
https://dl.google.com/dl/android/studio/install/2.1.2.0/android-studio-ide-143.2915827-mac.dmg
https://dl.google.com/dl/android/studio/ide-zips/2.1.2.0/android-studio-ide-143.2915827-linux.zip
