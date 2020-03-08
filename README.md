# flutter-doc

## 使用vscode创建第一个App

### vscode下载flutter和dart插件

### 安装Flutter SDK

1、打开 https://flutter.dev/docs/get-started/install/windows，找到Get the Flutter SDK并下载

2、设置bin文件夹路径的环境变量，

### 安装硬件加速

需要安装HAXM


修改模拟器虚拟化技术为Hyper-V：

windows 版本需要是 Windows10 2018 April（Windows 1803）及以上版本

Android Studio 3.2 beta 及以上版本

Android Emulator v27.3.8 及以上版本

$ winver 查看电脑版本

1、首先打开 windows功能，若存在Windows Hypervisor Platform，则将其勾选上，否则转下步

2、重启电脑

### Run flutter doctor -v

在终端输入：flutter docker 检查缺少的依赖并安装，成功后重启vscode

若是使用vscode编译的话，也强烈建议安装android studio，因为由于墙的原因以及android studio内置的AVD支持Hyper-V硬件加速。

android studio 下载地址：https://developer.android.google.cn/studio?hl=zh_cn

android sdk 安装教程：https://blog.csdn.net/lilongwei000/article/details/88870272

<<<<<<< HEAD
环境变量名：ANDROID_HOME
=======
android sdk: 环境变量设置

%ANDROID_HOME%\tools

%ANDROID_HOME%\platforms

%ANDROID_HOME%\platform-tools
>>>>>>> 147d6531c64e3e9702f037f062945b36a48539f4

#### Android license status unknown

$ flutter doctor --android-licenses

若是有报错：Exception in thread "main" java.lang.UnsupportedClassVersionError: 

一般是JDK版本过高，无法兼容，降级到1.8可行

#### SDK 升级失败

在SDK Manager下Tools->Options打开了SDK Manager的Settings，选中“Force https://… sources to be fetched using http://…”，强制使用http协议。

Windows在C:\WINDOWS\system32\drivers\etc打开/etc/hosts文件，添加

#google_android更新

203.208.46.146 dl.google.com

203.208.46.146 dl-ssl.google.com

#### sdkmanager 代理地址

mirrors.neusoft.edu.cn:80

### 设置 Android emulator

配置模拟器教程： https://blog.csdn.net/zha6476003/article/details/80785344

1、启用 VM acceleration

2、启动 Android Studio > Tools > Android > AVD Manager and select Create Virtual Device

3、在vscode终端中输入: flutter create myappp

4、cd myapp

5、 ctrl+shift+p 打开command pallet,输入Flutter:Select Device

6、flutter run



