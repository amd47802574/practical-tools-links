# 🧰 实用工具链接收藏夹（Practical Tools Links）

> 一个极简的「实用工具导航」仓库：用 Windows 原生 `.url` 快捷方式文件收藏好用的小工具网站，双击即达，无需书签同步、无需注册账号。

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows-lightgrey)](#使用方法)
[![Links](https://img.shields.io/badge/工具链接-3%2B-green)](#工具清单)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#贡献指南)

---

## 📖 项目简介

日常冲浪时总会遇到一些「用完想收藏」的在线小工具：视频去水印、无损音乐下载、背单词……但浏览器书签一多就乱，换台电脑也带不走。

这个仓库的思路很简单：

- **每个工具 = 一个 `.url` 文件**，Windows 双击直接用默认浏览器打开；
- 放在 GitHub 上，**克隆即用、多端同步**，还能持续补充新工具；
- 文件名即说明（`视频下载.url`、`背单词.url`），一眼可辨，也可以直接在资源管理器里搜索。

适合谁：不想装浏览器同步账号、喜欢用文件管理器整理东西、或者只想快速拿到一批「已验证可用」的工具链接的人。

---

## 🗂️ 工具清单

| 工具 | 文件 | 链接 | 简介 |
|------|------|------|------|
| 🎬 视频下载 | [视频下载.url](./工具链接/视频下载.url) | [hellotik.app/zh/douyin](https://www.hellotik.app/zh/douyin) | 抖音短视频去水印下载，粘贴链接即可解析，支持无水印原视频/封面 |
| 🎵 音乐下载 | [音乐下载.url](./工具链接/音乐下载.url) | [music.zyfx6.xyz](https://music.zyfx6.xyz/) | 在线音乐搜索与下载工具，支持试听和多种音质 |
| 📚 背单词 | [背单词.url](./工具链接/背单词.url) | [typewords.cc/words](https://typewords.cc/words) | 打字式背单词网站，边打字边记忆，适合日常碎片时间练习 |
| 🔍 IP纯净度查询 | [IP纯净度查询.url](./工具链接/IP纯净度查询.url) | [ping0.cc](https://ping0.cc/) | 查询 IP 纯净度/风险值，检测代理与原生 IP 质量 |

> 🔗 链接失效或站点改版？欢迎提 [Issue](../../issues) 告知，会及时更新。

---

## ✨ 特性

- **零依赖**：不需要安装任何软件，Windows 系统原生支持 `.url` 文件
- **双击即用**：资源管理器里双击，默认浏览器直接打开对应站点
- **可搜索**：直接在文件管理器搜索栏输入工具名（如「背单词」）快速定位
- **易扩展**：添加新工具 = 新建一个 `.url` 文件，格式两行搞定
- **版本管理**：Git 管理，链接改版历史可追溯

---

## 🚀 使用方法

### 方式一：直接使用

```bash
# 1. 克隆本仓库（或直接下载 ZIP）
git clone https://github.com/<你的用户名>/practical-tools-links.git

# 2. 进入目录，双击任意 .url 文件即可在默认浏览器打开
cd practical-tools-links
```

### 方式二：把链接放进「快速启动」

把整个文件夹固定到任务栏 / 开始菜单，或者把 `.url` 文件发送到桌面快捷方式，随点随开。

### 添加一个新工具

1. 在资源管理器里 **右键 → 新建 → 快捷方式**，填入网址并命名；或者手动新建文本文件，改扩展名为 `.url`，内容如下：

```ini
[InternetShortcut]
URL=https://example.com/
```

2. 文件名用工具名命名（如 `截图工具.url`）；
3. 提交并推送，README 的「工具清单」表格里补一行说明即可。

---

## 📁 目录结构

```
practical-tools-links/
├── 工具链接/              # 所有 .url 快捷方式
│   ├── 视频下载.url      # 抖音视频去水印下载
│   ├── 音乐下载.url      # 在线音乐搜索下载
│   ├── 背单词.url        # 打字式背单词
│   └── IP纯净度查询.url  # IP 纯净度/风险值查询
└── README.md
```

`.url` 文件格式说明（INI 格式，Windows Internet Shortcut）：

```ini
[{000214A0-0000-0000-C000-000000000046}]
Prop3=19,11
[InternetShortcut]
URL=https://目标网址
HotKey=0
```

---

## 🛣️ 计划中

- [ ] 按分类建立子目录（视频 / 音乐 / 学习 / 效率 / 设计…）
- [ ] 增加更多常用工具（截图、OCR、PDF 处理、格式转换等）
- [ ] 定期巡检链接可用性
- [ ] 提供跨平台 `.webloc`（macOS）/ `.desktop`（Linux）版本

---

## 🤝 贡献指南

欢迎补充好用的工具链接！

1. Fork 本仓库
2. 新建分支：`git checkout -b add-new-tool`
3. 添加你的 `.url` 文件，并在 README「工具清单」表格中补充一行
4. 提交：`git commit -m "feat: 添加 xx 工具链接"`
5. 推送并提交 Pull Request

也可以直接提 [Issue](../../issues) 推荐工具，我来补充。

---

## ⭐ 支持一下

如果这个合集对你有帮助，欢迎点个 **Star** ⭐ 让更多人看到！

## 📄 License

[MIT](./LICENSE)
