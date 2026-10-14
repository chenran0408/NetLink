# NetLink

Android 代理客户端，支持订阅导入、规则分流、应用代理、流量查看和备份恢复。

## 下载

前往 [发行版](https://github.com/chenran0408/NetLink/releases/latest) 下载 APK。大多数手机选择 `arm64-v8a`，旧款 32 位设备选择 `armeabi-v7a`，x86 设备或模拟器选择 `x86_64`。

- 应用名：NetLink
- Android 包名：`io.github.chenran0408.netlink`
- 可与原版同时安装，配置通过备份导入。
- 应用更新从本仓库获取；此版本未配置 Firebase 云端统计或崩溃上报。

## 构建

安装 Flutter 3.47.6、Go 1.27.1、Rust、JDK 17 和 Android SDK/NDK 后：

```sh
git clone --recursive https://github.com/chenran0408/NetLink.git
cd NetLink
flutter pub get
dart run intl_utils:generate
dart setup.dart android --env stable
```

正式发行使用仓库的 Android release 工作流，签名密钥通过 GitHub Secrets 提供。

## 许可与来源

本项目基于 [上游项目](https://github.com/chen08209/FlClash) 修改，保留原作者版权与贡献者声明，遵循 [GPL-3.0](LICENSE)。源码与修改记录在本仓库公开。