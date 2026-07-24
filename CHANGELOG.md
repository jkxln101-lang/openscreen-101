# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2026-07-24

openscreen-101 第一个增强版本！基于 [openscreen](https://github.com/siddharthvaddem/openscreen) 继续开发与维护。

### ✨ 新增功能

- **2K/4K 高分辨率导出** — 新增 1440p (2K) 和 2160p (4K) 导出选项，码率自适应最高 100Mbps
- **MP4 视频导入** — 支持将外部 MP4 视频文件导入到项目中编辑
- **选择区域优化** — 隐藏预设框，默认缩放比例调整为 1.25x，体验更流畅
- **13 种语言完整翻译** — Arabic, English, Español, Français, Italiano, 日本語, 한국어, Português (Brasil), Русский, Türkçe, Tiếng Việt, 简体中文, 繁體中文

### 🐛 修复问题

- 修复语言选择对话框在悬浮窗体中被截断的问题
- 修复导出分辨率选择器 UI 样式与整体不协调的问题
- 修复导出分辨率下拉面板被父容器裁剪导致无法点击的问题

### 🎨 界面改进

- 导出分辨率选择器改为自定义下拉面板（毛玻璃暗色主题）
- 下拉面板使用 portal 渲染，避免被父容器裁剪
- 选中项绿色高亮，悬停效果优化

###  技术改进

- 配置 GitHub Actions 全自动发布流程（推送 tag 即自动构建三平台）
- 修改 appId 为 `com.jkxln101.openscreen101`
- 更新所有 CI/CD 工作流适配 fork 版本
- 升级 GitHub Actions 依赖到 v4

### ️ 已知问题

- macOS 版本未签名，首次打开需在「系统设置 > 隐私与安全性」中允许
- winget 包管理器安装暂不可用（待审核）
- Homebrew 安装需要额外配置 tap 仓库
