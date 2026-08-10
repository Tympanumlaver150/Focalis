# Focalis 下载

[English](README.md)

Focalis 是面向 Windows 的数字设计分析桌面工作台，在一个应用中提供 Design 层次、语义
RTL Source、VCD/FST 波形、Driver/Load Trace、Schematic、编辑器，以及受权限控制的
Agent/MCP 工作流。

> **Beta 软件：** 在将当前预发布版本用于关键签核工作前，请先用非生产数据完成验证。
> 对正确性或稳定性问题，请提供可复现证据并通过 Support 渠道反馈。

## 下载

当前版本：**Focalis vA-2026.06 Beta 0.1.0**。

[打开 Focalis Releases](https://github.com/DawnCarol/Focalis/releases)

只使用最新 GitHub Release 附带的资产：

| 资产 | 用途 |
| --- | --- |
| `focalis_vA-2026.06_x64_beta-<version>.exe` | Windows x64 安装器 |
| `focalis_vA-2026.06_x64_beta-<version>.exe.blockmap` | 差分更新元数据 |
| `latest.yml` | 自动更新元数据 |
| `SHA256SUMS.txt` | Release 资产完整性校验 |

本仓库有意不包含 Focalis 应用源码。GitHub 自动生成的 source archive 只包含本公开仓库
的发布说明和法律/支持文件，**不是**应用源码包。

## 安装

1. 从同一个 Release 下载安装器和 `SHA256SUMS.txt`。
2. 运行安装器前核对 SHA-256。
3. 运行安装器，并按需创建桌面快捷方式。
4. 启动 Focalis，在 **About Focalis** 中确认版本和 Beta 试用状态。
5. 通过 **Help > User Guide** 阅读随 Focalis 安装的版本匹配离线手册。

Focalis 当前面向 Windows 10/11 x64。大型 RTL 和波形更适合使用较大内存及本地 SSD。
安装包自带示例不需要用户另行安装编译器。

## 首次验证

通过 **Examples** 打开安装包自带设计：

- **Ibex demo system**：最快验证 Design、Source、Wave 和 Trace 闭环；
- **CVA6 CoreMark**：验证更大的层次和 FST 负载；
- **PicoRV32 SoC**：另一套紧凑 RTL 与波形示例。

推荐首次路径：

```text
Load Design -> 选择 instance -> 查看 Source -> 打开 Dump
-> 添加信号到 Wave -> 移动 Cursor -> Trace Driver/Load -> 打开 Schematic
```

## 更新与 Beta 试用

通过 **About Focalis > Check for updates** 检查 Focalis 官方公开更新源。存在未保存文档时不会静默
安装更新。每个 Beta 构建提供两个日历月评估期；到期后该构建必须通过许可证校验。安装新的 Beta
后，按新版本声明的策略重新计算评估期。

## 数据与网络

普通 Debug 和 Code 工作流中的 RTL、filelist、Dump、索引和 workspace session 均保留在
本地。只有用户明确配置的更新检查、AI Provider 或外部 MCP 会使用网络。问题报告中不要
粘贴 API Key。

## 支持

反馈前请记录：

- Focalis 完整版本和 Windows 版本；
- VCD/FST 格式及大致大小；
- Design/Messages 中第一条可执行诊断；
- 最小复现步骤，以及安装版示例能否复现；
- 去除私有路径和 RTL 后的 task log 或截图。

请通过 [GitHub Issues](https://github.com/DawnCarol/Focalis/issues) 反馈已经脱敏且可复现的产品
问题，并遵循 `SUPPORT.md`。安全问题不得直接提交到公开 Issue。

## 许可与声明

Focalis 以闭源软件形式分发。安装前请阅读本仓库的 `EULA.md`、`PRIVACY.md`、`SUPPORT.md`
和 `SECURITY.md`。第三方声明随应用安装，并可离线查看。
