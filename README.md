<div align="center">

# WangmiaoGit

**轻量、原生的 macOS Git 图形客户端**

基于 SwiftUI 构建，不内置浏览器运行时，不需要 WangmiaoGit 账户，不收集遥测数据。

[![Release](https://img.shields.io/github/v/release/wangmiaozero/WangmiaoGit?color=blue)](https://github.com/wangmiaozero/WangmiaoGit/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/wangmiaozero/WangmiaoGit/total?color=blue)](https://github.com/wangmiaozero/WangmiaoGit/releases)
[![macOS](https://img.shields.io/badge/macOS-14%2B-black?logo=apple)](#系统要求)
[![SwiftUI](https://img.shields.io/badge/SwiftUI-Native-orange?logo=swift&logoColor=white)](#项目介绍)

[下载最新版](https://github.com/wangmiaozero/WangmiaoGit/releases/latest) · [查看全部版本](https://github.com/wangmiaozero/WangmiaoGit/releases)

</div>

## 项目介绍

WangmiaoGit 是一款面向 macOS 的原生 Git 客户端。它直接调用系统中已经安装的
`git`，因此终端里已有的 SSH 密钥、凭据助手、Git 配置和 Hooks 都可以继续使用。

应用覆盖日常 Git 工作流，并通过原生界面提供提交图、文件差异、分支管理、暂藏、
工作树、子模块和冲突处理等能力。

## 核心功能

- **提交历史**：彩色提交图、分支与标签定位、提交搜索、文件历史、文本与图片差异。
- **工作区管理**：暂存、取消暂存、提交、修订上一次提交、丢弃更改、创建补丁和暂藏。
- **分支工作流**：创建、重命名、切换、合并、变基、快进、重置、删除和上游管理。
- **高级 Git 能力**：Cherry-pick、Worktree、Submodule、Git LFS 和内置冲突编辑器。
- **多仓库体验**：仓库仪表盘、多标签页和仓库活跃度概览。
- **托管平台集成**：配合 `gh` 或 `glab` 查看和创建 Pull Request、Merge Request 与 Issue。
- **可选 AI 能力**：按需生成提交说明或 Pull Request 文案，服务商和接口地址由用户配置。
- **原生体验**：SwiftUI + AppKit、系统深浅色外观、键盘导航和界面缩放。

## 安装

1. 从 [GitHub Releases](https://github.com/wangmiaozero/WangmiaoGit/releases/latest)
   下载最新 DMG。
2. 打开 DMG，将 WangmiaoGit 拖入“应用程序”文件夹。
3. 首次启动后，通过“文件 → 打开仓库”选择本地 Git 仓库。

当前公开版本尚未经过 Apple 公证。如果 macOS 阻止首次启动，请前往
“系统设置 → 隐私与安全性”，选择“仍要打开”。

## 可选工具

WangmiaoGit 的基础 Git 功能无需额外安装工具。以下功能需要相应命令行程序：

| 工具 | 用途 |
|---|---|
| [`git-lfs`](https://git-lfs.com) | Git LFS 状态、文件追踪、指针预览和对象下载 |
| [`gh`](https://cli.github.com) | GitHub Pull Request 与 Issue |
| [`glab`](https://gitlab.com/gitlab-org/cli#installation) | GitLab Merge Request、Issue 和实例头像 |

## 隐私与网络

WangmiaoGit 不收集遥测数据。网络访问仅发生在功能本身需要联网时，包括访问 Git
远程仓库、检查 GitHub Release 更新、运行用户触发的 `gh`/`glab` 命令、请求用户配置的
AI 服务，以及可选的作者头像查询。AI API Key 存储在 macOS 登录钥匙串中。

## 系统要求

- macOS 14 Sonoma 或更高版本
- `git` 命令可通过 `PATH` 使用

## 关于本仓库

本仓库用于发布 WangmiaoGit 安装包、版本说明和更新信息。请前往
[Releases](https://github.com/wangmiaozero/WangmiaoGit/releases) 获取公开版本。
