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


1、首先打开 windows功能，若存在Windows Hypervisor Platform，则将其勾选上，否则转下步

2、重启电脑

### Run flutter doctor

在终端输入：flutter docker 检查缺少的依赖并安装，成功后重启vscode

android studio 下载地址：https://developer.android.google.cn/studio?hl=zh_cn

android sdk 安装教程：https://blog.csdn.net/lilongwei000/article/details/88870272

环境变量名：ANDROID_HOME

#### Android license status unknown

### 设置 Android emulator

1、启用 VM acceleration

2、启动 Android Studio > Tools > Android > AVD Manager and select Create Virtual Device

3、在vscode终端中输入: flutter create myappp

4、cd myapp

5、 ctrl+shift+p 打开command pallet,输入Flutter:Select Device

6、flutter run



