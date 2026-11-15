<div align="center">
  <img src="./logo.png" alt="AegisBrowser Logo" width="96" height="96" />
  <h1>AegisBrowser 官方安装包下载中心</h1>
  <p><strong>超轻量防关联指纹浏览器工作台 · 安装包仅 3~6 MB · 支持 Windows 10/11 与 macOS</strong></p>
  <p>当前最新版本：<code>v0.1.0</code></p>
</div>

---

## 一键直链下载 (`v0.1.0`)

无需登录 GitHub，点击下方对应平台的安装包即可直接下载：

| 平台 | 适用版本 / 架构 | 安装包大小 | 直链下载 |
| --- | --- | --- | --- |
| **Windows 10/11** | 64-bit 一键安装版（推荐） | ~3.1 MB | [AegisBrowser_0.1.0_x64-setup.exe](https://github.com/JackJoven/aegis-browser-releases/releases/download/v0.1.0/AegisBrowser_0.1.0_x64-setup.exe) |
| **Windows 10/11** | 64-bit MSI 企业安装包 | ~4.0 MB | [AegisBrowser_0.1.0_x64_en-US.msi](https://github.com/JackJoven/aegis-browser-releases/releases/download/v0.1.0/AegisBrowser_0.1.0_x64_en-US.msi) |
| **macOS** | Apple Silicon（M1 / M2 / M3 / M4） | ~6.0 MB | [AegisBrowser_0.1.0_aarch64.dmg](https://github.com/JackJoven/aegis-browser-releases/releases/download/v0.1.0/AegisBrowser_0.1.0_aarch64.dmg) |
| **macOS** | Intel（老款芯片） | ~6.3 MB | [AegisBrowser_0.1.0_x64.dmg](https://github.com/JackJoven/aegis-browser-releases/releases/download/v0.1.0/AegisBrowser_0.1.0_x64.dmg) |

> 更多历史版本或完整发布附件，请访问 [Releases 页面](https://github.com/JackJoven/aegis-browser-releases/releases)。

---

## SHA-256 校验值

下载完成后可核对文件哈希值以确保安装包完整无篡改：

```text
065ccbb8bdda73bef0bb1a4487dea2b664b4fb67c6918204b9e9f7fa9247d3c0  AegisBrowser_0.1.0_x64-setup.exe
2bc4bb8d7f7518e0268d592b07f4c25c3380ed03f03a3dc118d186c191e9e2d0  AegisBrowser_0.1.0_x64_en-US.msi
68455d2503b41fe95cfb04b3ab68586790567bbf16ab6e31d6561f53398dd35c  AegisBrowser_0.1.0_aarch64.dmg
73f53ad96001bfd089253cbc187cc20ddcf220e55f11e3553b7a341c22d7f49b  AegisBrowser_0.1.0_x64.dmg
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
