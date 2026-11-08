# 📱 FC 坦克大战 (100关掌机版) — 安卓 App 打包与安装指南

本工程已为你配置好完整的**原生安卓横屏沉浸式工程 (`com.retro.battlecity`)**，内置自动横屏锁定 (`sensorLandscape`)、隐藏状态栏/导航栏全屏掌机模式、零延迟 8-bit 音效解锁、震动反馈以及安卓返回键拦截（在战斗界面按返回键自动退回选关大厅）。

你可以任选以下 **3 种方式** 在安卓手机上安装成独立 App：

---

## 方式一：免编译 · 手机端一键安装成全屏桌面 App（最快，10秒完成）
无需电脑，直接在安卓手机上用 **Chrome** 或 **Edge** 浏览器打开 `app/src/main/assets/index.html`：
1. 点击游戏选关大厅顶部的绿色按钮 **「📱 安卓全屏横屏」** 即可立即锁定横屏全屏；
2. 点击浏览器右上角菜单 `⋮` -> 选择 **「添加到主屏幕 (Add to Home screen)」** 或 **「安装应用」**；
3. 手机桌面上就会生成独立的 **《FC 坦克大战》App 图标**，点开即直接以无地址栏的全屏横屏掌机模式运行。

---

## 方式二：使用 Android Studio 一键打包 `.apk` 安装包
1. 解压本压缩包 `FC_Battle_City_Android_App_Project.zip`；
2. 打开 **Android Studio** -> 选择 **Open** -> 选中解压后的文件夹；
3. 等待 Gradle 同步完成后，点击顶部菜单 **Build -> Build Bundle(s) / APK(s) -> Build APK(s)**；
4. 在 `app/build/outputs/apk/debug/app-debug.apk` 即可拿到生成的安卓安装包，发到手机上点击即可安装！

---

## 方式三：免装软件 · 利用 GitHub Actions 云端自动编译 `.apk`
本工程已内置 `.github/workflows/build-apk.yml` 自动打包脚本：
1. 在 GitHub 新建一个仓库，将解压后的全部文件上传上去；
2. 点击仓库顶部的 **Actions** 标签页，云端服务器会自动为你编译安卓工程；
3. 约 2 分钟编译完成后，在 Actions 页面底部 **Artifacts** 处直接下载编译好的 `FC-Battle-City-100Stages-Android-APK.zip` 即可！
