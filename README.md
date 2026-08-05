<div align="center">

# TermX

**为现代运维而生的桌面 SSH 工作台**

终端 · 监控 · 文件 · 片段 — 同一窗口，一气呵成

[![Website](https://img.shields.io/badge/%E5%AE%98%E7%BD%91-termx.cn-4f7cff?style=flat-square)](https://termx.cn/)
[![Platform](https://img.shields.io/badge/%E5%B9%B3%E5%8F%B0-Windows%2010%2B-0078D4?style=flat-square)](#下载)
[![Version](https://img.shields.io/badge/version-1.0.24-24292e?style=flat-square)](../../releases)
[![QQ Group](https://img.shields.io/badge/QQ%E7%BE%A4-1095707034-EB1923?style=flat-square)](#社区)

[官网](https://termx.cn/) · [下载最新版](../../releases) · [QQ 群 1095707034](#社区)

</div>

<img src="doc/screenshots/01-home.png" alt="TermX 主界面">

---

## 为什么是 TermX

服务器日常运维的真正痛点从不是某一条命令，而是**工具切换**——终端开一个窗口、监控面板开一个、SFTP 工具开一个、命令片段记在便签里。TermX 把这些能力合并到同一个桌面应用，让一屏之内能看清楚、操作完所有事。

- **一站式工作台** — 终端、SFTP、监控、片段四模块同屏协作，告别多窗口切换
- **生产环境就绪** — 实时性能监控走 SSH 通道直采，服务端无需安装任何 Agent
- **键盘优先工作流** — 命令面板 `Ctrl+P` 键盘可达一切操作，手不离键盘
- **国产中文优先** — 界面、文档、社区均为中文，符合国内运维使用习惯

---

## 核心特性

### 多窗格终端

支持多标签 + 任意水平 / 垂直分屏组合。同一会话下开多个 shell，对比日志、调试进程、并发操作多台服务器——所有终端共享同一窗口，分屏可拖拽调整大小。

### 实时性能监控

接入会话即刻采集：CPU（总览 + 每核心使用率）、内存与 Swap、系统负载、磁盘容量与 IO、网络吞吐、Top 进程。提供 1 分钟 / 5 分钟 / 30 分钟三档趋势曲线，远程资源健康度一目了然。

### SFTP 文件浏览器

图形化远程文件管理。双栏树 + 列表布局，支持上传、下载、新建、删除、重命名、权限修改、拖拽上传与传输队列管理。从 Windows 资源管理器拖文件即可上传。

### 命令片段库

把常用命令按分类保存——运维、安装、网站、其他，分类可自定义。底部状态栏一键插入到当前终端光标位置，告别重复输入。

### 命令面板

按下 `Ctrl+P` 召唤类 VSCode 的快速命令入口。模糊搜索、键盘导航，新建会话、分屏、重连、切换主题、打开设置等所有操作一气呵成。

### 多服务器管理

左侧边栏统一管理所有服务器配置。支持分组、搜索、最近连接、快速重连，运维一台到几十台服务器都顺手。

---

## 界面预览

<table>
  <tr>
    <td width="50%" align="center"><b>主界面 · 四模块同屏</b></td>
    <td width="50%" align="center"><b>多窗格分屏工作流</b></td>
  </tr>
  <tr>
    <td width="50%"><img src="doc/screenshots/01-home.png" alt="主界面"></td>
    <td width="50%"><img src="doc/screenshots/02-multi-pane.png" alt="多窗格"></td>
  </tr>
  <tr>
    <td width="50%" align="center"><b>命令面板（Ctrl+P）</b></td>
    <td width="50%" align="center"><b>SFTP 文件浏览器</b></td>
  </tr>
  <tr>
    <td width="50%"><img src="doc/screenshots/03-command-palette.png" alt="命令面板"></td>
    <td width="50%"><img src="doc/screenshots/04-sftp.png" alt="SFTP"></td>
  </tr>
  <tr>
    <td width="100%" align="center" colspan="2"><b>命令片段管理</b></td>
  </tr>
  <tr>
    <td width="100%" colspan="2"><img src="doc/screenshots/05-snippets.png" alt="命令片段"></td>
  </tr>
</table>

---

## 下载

到 [Releases](../../releases) 页下载最新版安装包：

```
TermX-Setup-1.0.24-x64.exe    约 82 MB · Windows 10 1809+ / Windows 11 (x64)
```

或访问 [官网 termx.cn](https://termx.cn/) 获取最新版本与产品信息。

### 安装步骤

1. 双击 `TermX-Setup-1.0.24-x64.exe` 启动安装向导
2. 按向导完成：欢迎 → 许可协议 → 安装目录 → 数据目录 → 安装 → 完成
3. 安装完成后自动启动；之后可从开始菜单或桌面快捷方式启动
4. 首次启动时添加第一台服务器，开始使用

> 安装无需管理员权限，默认安装到用户目录。

---

## 快速上手

| 任务 | 操作 |
|------|------|
| **添加服务器** | 左侧边栏「+ 新建会话」或 `Ctrl+P` → 「新建会话」 |
| **连接服务器** | 双击会话卡片，右侧监控面板自动开始采集 |
| **打开 SFTP** | 会话内点击路径栏「打开 SFTP 浏览器」 |
| **分屏** | `Ctrl+P` → 「水平分割」/「垂直分割」 |
| **保存命令** | 底部状态栏「+ 管理」打开片段管理面板 |
| **快捷键** | `Ctrl+P` 打开命令面板，所有快捷键可达 |

---

## 技术架构

| 层 | 选型 |
|----|------|
| 桌面框架 | Electron 32 |
| 渲染层 | React 18 · TypeScript · Tailwind CSS |
| 状态管理 | Zustand |
| 终端 | xterm.js |
| SSH 协议 | ssh2 + 原生模块（设备指纹与授权） |
| 数据可视化 | Recharts |
| 打包 | electron-builder · Inno Setup |

---

## 社区

<table>
  <tr>
    <td width="50%" align="center" valign="middle">
      <h3>官方网站</h3>
      <p><a href="https://termx.cn/">termx.cn</a></p>
      <p>产品介绍 · 下载中心 · 商务合作</p>
    </td>
    <td width="50%" align="center" valign="middle">
      <h3>QQ 交流群 · 1095707034</h3>
      <img src="doc/screenshots/qq-group.jpg" width="180" alt="QQ 群二维码"><br>
      <sub>扫码加群 · 或 QQ 搜索群号</sub>
    </td>
  </tr>
</table>

加入 QQ 群可获得：

- 第一时间版本更新通知
- 使用问题与排障答疑
- 功能建议与产品路线图参与
- 与同行交流最佳实践

---

## 反馈

- **Bug 与功能建议**：[提交 Issue](../../issues)，附版本号、复现步骤、截图与日志
- **商务合作 / 企业版咨询**：访问 [官网](https://termx.cn/) 联系方式
- **加群交流**：QQ 群 **1095707034**

---

<div align="center">

**TermX** · [termx.cn](https://termx.cn/) · QQ 群 1095707034

</div>
