<div align="center">

# 幻灵终端 (LiteMask)

**轻量级 Android 代码运行与文件管理工具**
An open-source & forever-free Android code runner toolkit — no root required.

混合架构单包 APK：原生 Java + Android SDK，**源码级内置液态玻璃 UI 与本地 Java 代码执行环境**，不依赖任何外部 App，即可完成代码编辑与本地运行。

### 项目状态 · 许可

<a href="https://github.com/nanci-dev/LiteMask/issues"><img src="https://img.shields.io/badge/状态-开发中-brightgreen.svg" alt="状态"></a>
<a href="https://github.com/nanci-dev/LiteMask/blob/main/LICENSE"><img src="https://img.shields.io/badge/许可-MIT-blue.svg" alt="许可"></a>
<a href="https://github.com/nanci-dev/LiteMask/stargazers"><img src="https://img.shields.io/badge/stars-0-brightgreen.svg" alt="stars"></a>
<a href="https://github.com/nanci-dev/LiteMask/network/members"><img src="https://img.shields.io/badge/forks-0-blue.svg" alt="forks"></a>
<a href="https://github.com/nanci-dev/LiteMask/issues"><img src="https://img.shields.io/badge/issues-0%20open-orange.svg" alt="issues"></a>
<a href="https://github.com/nanci-dev/LiteMask/pulls"><img src="https://img.shields.io/badge/PRs-welcome-blueviolet.svg" alt="PRs"></a>

### 构建环境

<a href="https://www.java.com"><img src="https://img.shields.io/badge/Java-100%25-orange.svg" alt="Java"></a>
<a href="https://developer.android.com"><img src="https://img.shields.io/badge/minSdk-26%20(Android%208.0)-green.svg" alt="minSdk"></a>
<a href="https://www.android.com"><img src="https://img.shields.io/badge/Platform-Android-brightgreen.svg" alt="Platform"></a>
<a href="https://github.com/nanci-dev/LiteMask"><img src="https://img.shields.io/badge/AIDE-Pro-red.svg" alt="AIDE Pro"></a>

### 技术栈

<a href="https://www.java.com" target="_blank"><img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" height="28"></a>
<a href="https://developer.android.com" target="_blank"><img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android" height="28"></a>
<a href="https://github.com/nanci-dev/LiteMask" target="_blank"><img src="https://img.shields.io/badge/AIDE_Pro-FF5722?style=for-the-badge&logo=androidstudio&logoColor=white" alt="AIDE Pro" height="28"></a>
<a href="https://github.com/nanci-dev/LiteMask" target="_blank"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" height="28"></a>

### 快速跳转

<a href="#项目简介"><img src="https://img.shields.io/badge/项目简介-blue.svg?style=flat-square" alt="项目简介"></a>
<a href="#开发状态"><img src="https://img.shields.io/badge/开发状态-brightgreen.svg?style=flat-square" alt="开发状态"></a>
<a href="#构建环境"><img src="https://img.shields.io/badge/构建环境-orange.svg?style=flat-square" alt="构建环境"></a>
<a href="#重要声明"><img src="https://img.shields.io/badge/重要声明-red.svg?style=flat-square" alt="重要声明"></a>
<a href="#相关链接"><img src="https://img.shields.io/badge/相关链接-blueviolet.svg?style=flat-square" alt="相关链接"></a>

</div>

---

## 项目简介

“幻灵终端”是一款面向 Android 平台的轻量级代码编辑器与文件管理工具。内置 Java 代码运行环境，支持纯本地编译与输出，配备了全新的“液态玻璃”风格 UI。本项目完全开源、免费，不依赖任何外部 App。

## 开发状态

- **当前版本**：v1.0.0（正式版）
- **核心功能**：代码编辑器、文件管理、液态玻璃 UI 参数调节均已实现
- **更新频率**：随缘更新，欢迎在 Issues 提交反馈
- **开发环境**：AIDE Pro（手机端）

## 构建环境

| 项目 | 版本 |
| --- | --- |
| 开发工具 | AIDE Pro（手机端） |
| 开发语言 | Java |
| 最低 SDK | Android 8.0 (API 26) |
| 主题 | Theme.Material.NoActionBar |
| 外部依赖 | 原生 SDK，无第三方依赖 |

## 重要声明

> **⚠️ 重要声明：当前为 v1.0.0 正式版**

本项目为个人开源项目，目前源码结构稳定，可编译出 APK 直接运行：

- 请在 Android 8.0 及以上系统使用，需授予存储读写权限。
- 源码仅供学习与交流使用，请遵循 MIT 开源协议。
- **AIDE 编译避坑**：如果遇到编译报错，请先检查 R.java 生成情况，或删除 `build/` 和 `gen/` 目录后重新编译。若 `BuildConfig.java` 卡死，同样删除构建目录重新编译。
- 如果遇到无法编译的情况，欢迎提交 Issue，但请附上具体的报错日志。

## 项目结构

```text
LiteMask/
├── app/
│   └── src/
│       └── main/
│           ├── java/com/huanling/application/  <-- 核心 Java 代码
│           │   ├── mainactivity.java
│           │   ├── homefragment.java
│           │   ├── filefragment.java
│           │   ├── minefragment.java
│           │   ├── splashactivity.java
│           │   └── globalapplication.java
│           ├── res/                            <-- UI 资源文件
│           │   ├── layout/
│           │   ├── drawable/
│           │   └── values/
│           └── AndroidManifest.xml
├── .gitignore
├── LICENSE
└── README.md
