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

2、

### Run flutter doctor

在终端输入：flutter docker 检查缺少的依赖并安装，成功后重启vscode

android studio 下载地址：https://developer.android.google.cn/studio?hl=zh_cn

android sdk 安装教程：https://blog.csdn.net/lilongwei000/article/details/88870272

### 使用Hyper-V 和 Windows Hypervisor Platform 替代 HAXM 实现虚拟机加速

使用 Windows Hypervisor Platform 配置虚拟机加速

您的计算机必须满足以下要求，您才能启用 WHPX：

Intel 处理器：支持虚拟化技术 (VT-x)、扩展页表 (EPT) 和无限制访客 (UG) 功能。必须在计算机的 BIOS 设置中启用 VT-x。

AMD 处理器：建议使用 AMD Ryzen 处理器。必须在计算机的 BIOS 设置中启用虚拟化或 SVM。

Android Studio 3.2 Beta 1 或更高版本（从 developer.android.com 下载）

Android 模拟器版本 27.3.8 或更高版本（使用 SDK Manager 下载）

Windows 10 April 2018 Update 或更高版本

要在 Windows 上安装 WHPX，请按以下步骤操作：

在 Windows 桌面上，右键点击 Windows 图标，然后选择应用程序和功能。

在相关设置下，点击程序和功能。

点击打开或关闭 Windows 功能。

选中 Windows Hypervisor Platform。



点击确定。

安装完成后，重启计算机。

### 设置 Android emulator

1、启用 VM acceleration

2、启动 Android Studio > Tools > Android > AVD Manager and select Create Virtual Device

3、在vscode终端中输入: flutter create myapp

4、cd myapp

5、flutter run



