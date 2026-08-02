# IFP Releases

**IFP（发票管理 & 财务解析桌面应用）官方发布仓库**——应用安装包与更新清单的唯一分发源。

> IFP 是一款本地优先的发票管理与财务解析桌面应用：PDF 发票导入 → 结构化解析（MinerU / 税务查验 API / LLM 三层兜底）→ 归档管理 → 报销状态流转，支持导出 Excel / CSV / PDF / Word。

## 下载

| 平台 | 安装包 | 加速下载（国内推荐） |
|------|--------|---------------------|
| macOS | [IFP-latest.dmg](https://github.com/Invoice-Financial-Parser/IFP-releases/releases/latest/download/IFP-latest.dmg) | [xget 加速](https://xget.xi-xu.me/gh/Invoice-Financial-Parser/IFP-releases/releases/latest/download/IFP-latest.dmg) |
| Windows | [IFP-latest-setup.exe](https://github.com/Invoice-Financial-Parser/IFP-releases/releases/latest/download/IFP-latest-setup.exe) | [xget 加速](https://xget.xi-xu.me/gh/Invoice-Financial-Parser/IFP-releases/releases/latest/download/IFP-latest-setup.exe) |

- 链接固定指向最新版本（`releases/latest/download/`），无需随版本更新修改
- macOS 首次安装：应用未签名，请在访达中右键应用 → 「打开」（或系统设置 → 隐私与安全性 → 仍要打开）
- Windows 安装：SmartScreen 提示时选择「更多信息」→「仍要运行」

## 版本历史

| 版本 | 日期 | 说明 |
|------|------|------|
| [v0.0.2](https://github.com/Invoice-Financial-Parser/IFP-releases/releases/tag/v0.0.2) | 2026-08-02 | 发布链路迁移至 GitHub Releases + xget 加速 |
| [v0.0.1](https://github.com/Invoice-Financial-Parser/IFP-releases/releases/tag/v0.0.1) | 2026-08-02 | 首个公测版本 |

## 更新机制

- 应用内置自动更新（electron-updater）：启动时检查 `latest-mac.yml` / `latest.yml`，发现新版本自动下载并提示安装
- 更新清单与安装包同仓库维护，发布新版本后用户端即可检测到更新
- 下载走 xget 加速服务（[xget](https://github.com/xixu-me/xget)），国内网络环境可正常更新

## 本仓库说明

- 本仓库**仅存储发布产物**（安装包 + 更新清单，均通过 GitHub Releases 资产分发，不占用仓库文件空间）
- 源码仓库为私有，不在本仓库公开；本仓库的 README 与 Release 信息即对外发布页面
- 子模块形式挂载于源码仓库（`releases/` 目录），方便从属关系追踪

## 许可

商业软件，保留所有权利。仅用于官方分发，禁止未授权再分发。
