<div align="center">
  
# Nebula Lab

**面向科研数据预处理、批处理执行与 Origin 交接的 Windows 桌面工作站**

从原始实验数据到最终作图前的数据整理，统一完成导入、归组、处理、批量复用与导出；同时提供样品与配方记录，以及连接课题组实验室服务器的数据中心。

[🇨🇳 简体中文](./README.md) · [🇺🇸 English](./README_EN.md)

[![Latest Release](https://img.shields.io/github/v/release/ptjworks/NebulaLab-Releases?display_name=tag&sort=semver&style=for-the-badge&color=2e4c70)](https://github.com/ptjworks/NebulaLab-Releases/releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20x64-0A66C2?style=for-the-badge&logo=windows)](https://github.com/ptjworks/NebulaLab-Releases/releases/latest)
[![Channels](https://img.shields.io/badge/Channels-Stable%20%7C%20Beta-C97A1A?style=for-the-badge)](https://github.com/ptjworks/NebulaLab-Releases/releases)

[**📥 下载正式版**](https://github.com/ptjworks/NebulaLab-Releases/releases/latest) &nbsp;&nbsp;•&nbsp;&nbsp; [**📄 查看发版记录**](https://github.com/ptjworks/NebulaLab-Releases/releases) &nbsp;&nbsp;•&nbsp;&nbsp; [**📖 文档站**](https://nebulalab.app/)

</div>

> **Nebula Lab 的定位：** 为组级数据（Group-level Data）和多谱图序列提供稳定、可重复的预处理流程，减少实验数据在进入 Origin 或其他绘图工具前的重复手工整理。

## 工作流概览

| 导入 | 归组 | 处理 | 批量复用 | 预览 | 导出 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `.csv` `.txt` `.xlsx` `.xls` `.dat` `.xy` `.asc` | 多个文件合并为一组，或拆成多个分组 | 裁剪、平滑、基线扣除、归一化 | 在一个样品上调好流程，再从原始数据重放到整组 | 在真实样品上预览每一步处理 | Origin 工作簿与图形、CSV、PNG / JPG / SVG、Nebula 工程文件 |

## 核心能力

| 能力 | 说明 |
| :--- | :--- |
| 预处理优先 | 在正式作图前先统一数据质量与结构，减少后续分析和制图返工。 |
| 组级批量复用 | 将单个样品上验证过的处理流程推广到同组数据；处理步骤、参数、轴映射和绘图默认设置可以保存，套用到相似数据。 |
| 分支独立控制 | 单个异常样品可以拆成独立流程，单独调整处理步骤，不影响同组其他样品。 |
| 交给 Origin | 把选中的样品组连同 Origin 图形模板和主题发送到 Origin 继续作图（需要本机已安装 Origin）。 |
| 插件与社区 | 从插件商店安装官方或社区插件；浏览和发布社区共享的处理流程、Origin 模板、主题和科研脚本。 |
| 样品与配方 | 样品管理集中查看概览、外观形貌、测试与表征、附件和历史，可生成报告；配方库支持版本保存与差异查看，物料库支持 PubChem 查询。 |
| 实验室数据中心 | 连接课题组的实验室服务器后，可上传样品记录，跨样品、测试和指标检索，并按样品设置共享；管理员在实验室管理中处理成员、设备和操作审计。部分数据中心功能仍在验证中，以各版本更新说明为准。 |
| 本地优先 | 作为独立 Windows 应用运行，实验数据保存在本机；数据中心使用课题组自己的实验室服务器。 |

## 快速开始

1. 从 [Releases 页面](https://github.com/ptjworks/NebulaLab-Releases/releases/latest) 下载 `NebulaLab-<版本>-windows-x64-setup.exe`，运行安装向导。
2. 导入仪器导出的数据文件，在导入配置中核对编码、跳过行数、表头行和工作表，再整理成样品组。
3. 在一个样品上添加裁剪、平滑、基线扣除、归一化等处理步骤，逐步预览结果。
4. 确认无误后把同一套步骤应用到整组，并可保存为处理流程，供相似数据复用。
5. 把整理好的样品组导出到 Origin，或导出 CSV、图片和 Nebula 工程文件。

> 账号、登录与授权方式请以应用内提示和 [文档站](https://nebulalab.app/) 的说明为准。

## 下载与安装

> 系统要求：Windows 10 / Windows 11（x64）

| 通道 | 安装包 | 说明 |
| :--- | :--- | :--- |
| 正式版 | `NebulaLab-<版本>-windows-x64-setup.exe` | 标记为 Latest 的发布，推荐日常使用。 |
| Beta | `NebulaLabBeta-<版本>-windows-x64-setup.exe` | 标记为 Pre-release 的发布，供内测用户提前验证新功能；重要日常工作请继续使用正式版。Beta 与正式版相互隔离，可以在同一台电脑上并存。 |

- 自 0.8.8 起只提供 `setup.exe` 安装包，不再提供 `.msi`。
- `.sig` 与 `latest.json` 是应用内更新使用的签名与清单文件，手动安装时可以忽略；名为 `beta-channel` 的发布只存放 Beta 通道的更新清单，不含安装包。
- 安装包目前没有代码签名，浏览器或 Windows SmartScreen 可能提示风险；放行步骤见[用户手册](https://nebulalab.app/manual/)。

## 更新

- 正式版和 Beta 分别从各自的通道获取更新。检测到新版本时，应用会先征求确认，再显示下载与安装进度。
- 每个版本的更新内容、数据兼容说明和已知限制写在对应 [Release](https://github.com/ptjworks/NebulaLab-Releases/releases) 的说明里，升级前建议先阅读。

## 文档与反馈

- 文档站：[nebulalab.app](https://nebulalab.app/)（用户手册与教程）
- 问题反馈与功能建议：[Issues](https://github.com/ptjworks/NebulaLab-Releases/issues)，请选择“报告问题”或“功能建议”模板。
- 附上样例数据、日志或截图前，请先去掉未公开的科研数据和个人信息。
