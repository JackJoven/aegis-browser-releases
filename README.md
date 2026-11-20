<div align="center">
  <img src="./logo.png" alt="AegisBrowser Logo" width="96" height="96" />
  <h1>AegisBrowser 官方安装包下载中心</h1>
  <p><strong>超轻量双 C++ 内核防关联指纹浏览器工作台 · 安装包仅 3~6 MB · 支持 Windows 10/11 与 macOS</strong></p>
  <p>
    <a href="https://github.com/JackJoven/aegis-browser-releases/releases/latest">
      <img src="https://img.shields.io/github/v/release/JackJoven/aegis-browser-releases?style=flat-square&label=%E6%9C%80%E6%96%B0%E6%AD%A3%E5%BC%8F%E7%89%88&color=4f46e5" alt="最新正式版" />
    </a>
  </p>
  <p>
    <a href="https://github.com/JackJoven/aegis-browser-releases/releases/latest"><strong>👉 点击前往下载最新正式版安装包（免登录直链）</strong></a>
  </p>
</div>

---

## AegisBrowser 解决什么问题？

- **解决多账号关联封店难题**：面向跨境电商（Amazon / TikTok Shop / Shopee / Etsy）与海外社媒多账号矩阵运营，为每个环境提供物理隔离的本地存档与 C++ 引擎级独立硬件指纹（Canvas / WebGL / 声卡 / 字体 / 屏幕特征），彻底告别同机多登串号关联。
- **解决代理断连漏真机 IP 与时区穿帮**：每次启动窗口前强制执行 **Kill-Switch 出口预检**，代理不通或意外暴露国内 IP 时立即熔断拦截，并根据真实出口 IP 自动对齐对应国家的时区、语言与地理位置。
- **解决传统指纹浏览器臃肿吃内存与风控识别**：告别动辄数百 MB 的套壳客户端；人工开窗采用 **Zero-CDP 纯净模式**（不暴露自动化调试端口痕迹，从容应对 Cloudflare Turnstile / DataDome 等严苛站点），所有环境共享单一只读内核，关窗自动清理冗余视频与图片缓存。
- **解决多设备协同泄密与同号撞车**：核心店铺 Cookie 与免密箱在本地经零知识端到端加密（`AES-256-GCM`）后再同步，云端零明文，并配备防异地同时在线的会话互斥锁。

---

## 核心优势亮点

- **🪶 极致轻量 & 免卸载静默升级**：基于 `Rust` + `Tauri` 原生构建，安装包仅 `3 ~ 6 MB`；支持软件内自动检测更新并一键原地静默覆盖重启，无需反复手动卸载重装，环境与内核数据完整保留。
- **🧠 双 C++ 防关联引擎 + 老号版本锁定**：按需一键下载 `Fingerprint Chromium`（完整兼容 Chrome `.crx` 扩展）或 `Camoufox`（Firefox 深度反检测内核）；内置国内多源加速、断点续传与本地离线压缩包一键导入，并支持老店铺内核版本永久锁定（`Version Pinning`）。
- **🛡️ 默认纯净 + Mihomo 链式代理按需启用**：安装后默认保持纯净零冗余进程，需要时可在界面一键按需安装或移除 `Mihomo (Clash.Meta)` 核心，支持机场订阅导入与 **「前置专线中转 ➔ 静态住宅 IP 落地」** 链式代理及端口池热切换。
- **📱 随身远程流控 & 云手机矩阵**：内置手机扫码随身中控与纯 Rust 原生 ADB 云手机多宫格群控，兼顾桌面店铺与移动端矩阵协同。

---

## 下载与选型指南（Windows & macOS）

请点击进入 **[最新正式版发布页 (Releases Latest)](https://github.com/JackJoven/aegis-browser-releases/releases/latest)**，根据您的电脑系统选择对应文件下载（各文件对应的 `SHA-256` 校验值均随附于每个版本的发布说明中）：

| 操作系统 | 适用设备架构 | 文件后缀标识 | 说明 |
| --- | --- | --- | --- |
| **Windows 10 / 11** | 64-bit 通用推荐 | `*_x64-setup.exe` | 一键安装向导（推荐，支持后续软件内自动静默覆盖升级） |
| **Windows 10 / 11** | 64-bit 企业部署 | `*_x64_en-US.msi` | Windows 原生 MSI 安装包 |
| **macOS** | Apple Silicon（M1 / M2 / M3 / M4） | `*_aarch64.dmg` | 新款苹果自研芯片 Mac 专用 |
| **macOS** | Intel 芯片 | `*_x64.dmg` | 老款 Intel 处理器 Mac 专用 |

---

## 首次安装放行说明

由于桌面端安装包未附加商业 EV 硬件证书签名，首次安装或打开时若遇到系统安全拦截，按以下步骤放行即可：

- **Windows（SmartScreen 提示）**：  
  若弹出 *“Windows 已保护你的电脑”*，点击弹窗上的 **「更多信息」→「仍要运行」** 即可正常安装。
- **macOS（Gatekeeper 隔离提示）**：  
  打开 `.dmg` 将 `AegisBrowser.app` 拖入 **「应用程序（Applications）」** 后，若首次启动提示 *“无法验证开发者”* 或 *“已损坏，无法打开”*，请打开「终端（Terminal）」执行以下命令解除隔离标记：
  ```bash
  sudo xattr -rd com.apple.quarantine /Applications/AegisBrowser.app
  ```

---

## 首次启动 3 步快速上手

1. **按需下载浏览器内核**：打开软件进入左侧 **「双内核中心」**，任选 `Chromium`（电商扩展首选）或 `Camoufox`（强风控过盾首选）一键加速下载，也支持直接导入网盘离线 `.zip` / `.dmg` 内核包。
2. **配置网络（可选）**：若需使用代理池，进入 **「Clash 与代理池」** 一键按需安装 `Mihomo` 核心，即可导入 Clash 订阅或添加静态住宅代理节点。
3. **创建环境与授权解锁**：新装机默认免费享 `Starter` 基础额度，在 **「环境工作台」** 新建环境即可独立开窗；如持有 `AEGIS1.*` 离线激活码，可在 **「💎 会员与激活」** 一键离线解锁更高并发配额、多端加密云同步与云手机矩阵。
