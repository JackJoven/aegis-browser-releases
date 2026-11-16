<div align="center">
  <img src="./logo.png" alt="AegisBrowser Logo" width="96" height="96" />
  <h1>AegisBrowser 官方安装包下载中心</h1>
  <p><strong>超轻量防关联指纹浏览器工作台 · 安装包仅 3~6 MB · 支持 Windows 10/11 与 macOS</strong></p>
  <p>当前最新版本：<code>v0.1.1</code></p>
</div>

---

## `v0.1.1` 核心更新亮点

- **⚡ 内置国内智能多源加速**：内置 5 个经实测可用（`HTTP 200` + 二进制直链校验）的国内 GitHub Release 加速节点（`ghfast.top` / `gh-proxy.com` / `ghproxy.net` / `gh-proxy.org` / `edgeone.gh-proxy.com`），支持防假 `200 OK` HTML 拦截与 25s 流式超时自动切换，也支持 **GitHub 官方直连** 与 **自定义镜像前缀 / 私有 OSS·COS·R2 直链**。
- **📦 网盘离线包一键导入 (`.zip` / `.dmg`)**：严格内网或无代理环境下，可在内核卡片直接粘贴网盘下载的 `.zip`（Windows/Mac）或 `.dmg`（Mac）本地压缩包路径，自动剥离引号、安全解压并校验入库，无需手动折腾目录。

---

## 一键直链下载 (`v0.1.1`)

无需登录 GitHub，点击下方对应平台的安装包即可直接下载：

| 平台 | 适用版本 / 架构 | 安装包大小 | 直链下载 |
| --- | --- | --- | --- |
| **Windows 10/11** | 64-bit 一键安装版（推荐） | ~3.1 MB | [AegisBrowser_0.1.1_x64-setup.exe](https://github.com/JackJoven/aegis-browser-releases/releases/download/v0.1.1/AegisBrowser_0.1.1_x64-setup.exe) |
| **Windows 10/11** | 64-bit MSI 企业安装包 | ~4.1 MB | [AegisBrowser_0.1.1_x64_en-US.msi](https://github.com/JackJoven/aegis-browser-releases/releases/download/v0.1.1/AegisBrowser_0.1.1_x64_en-US.msi) |
| **macOS** | Apple Silicon（M1 / M2 / M3 / M4） | ~6.0 MB | [AegisBrowser_0.1.1_aarch64.dmg](https://github.com/JackJoven/aegis-browser-releases/releases/download/v0.1.1/AegisBrowser_0.1.1_aarch64.dmg) |
| **macOS** | Intel（老款芯片） | ~6.3 MB | [AegisBrowser_0.1.1_x64.dmg](https://github.com/JackJoven/aegis-browser-releases/releases/download/v0.1.1/AegisBrowser_0.1.1_x64.dmg) |

> 更多历史版本（如 `v0.1.0`）或完整发布附件，请访问 [Releases 页面](https://github.com/JackJoven/aegis-browser-releases/releases)。

---

## SHA-256 校验值 (`v0.1.1`)

下载完成后可核对文件哈希值以确保安装包完整无篡改：

```text
7000bc6e7cf78f169f7af06324ee03beb8e5f4c34cd90fb62d5184734e10a26a  AegisBrowser_0.1.1_x64-setup.exe
3f573db4c0d95864ed7e3ea44af7cf9502132fd53103785dc0c38ebff00d42f4  AegisBrowser_0.1.1_x64_en-US.msi
29a6517dfcf06df6faec6a5aab5b49efb0b37c8893f6db4b368ac82ba4887afb  AegisBrowser_0.1.1_aarch64.dmg
0499ab35e2d02738c29d725af81bf1068cc53e422202c793bdbb761903ecd302  AegisBrowser_0.1.1_x64.dmg
```

---

## 首次安装放行说明

由于当前版本尚未附加商业 EV 代码签名证书，首次安装或启动时操作系统可能会弹出安全提示，按以下方式放行即可：

- **Windows（SmartScreen 拦截）**：
  若提示 *“Windows 已保护你的电脑”*，点击弹窗上的 **「更多信息」→「仍要运行」** 即可继续安装。
- **macOS（Gatekeeper 隔离提示）**：
  打开 `.dmg` 并将 `AegisBrowser.app` 拖入「应用程序（Applications）」文件夹后，若首次双击提示 *“无法验证开发者”* 或 *“已损坏，无法打开”*，请打开「终端（Terminal）」执行以下命令解除隔离属性：
  ```bash
  sudo xattr -rd com.apple.quarantine /Applications/AegisBrowser.app
  ```

---

## 首次启动 2 步上手

1. **获取浏览器内核**：打开软件后，进入左侧 **「内核管理」**，一键在线下载 `fingerprint-chromium` 或 `Camoufox` 内核（也支持直接挂载本地离线内核包）。
2. **开始使用与会员激活**：新安装默认免费享 `Starter` 基础额度；如您持有 `AEGIS1.*` 离线激活码，可进入 **「💎 会员与激活」** 一键离线解锁更高环境并发数、云同步与云手机矩阵功能。
