<div align="center">

# AIsChat Community

**AIsChat 资源社区 · 世界 / 技能 / 工具 / 积木 的共享集市**

> **每个群聊都能长出一个活的世界——这里是世界的集市，也是能力的集市。**

[![AIsChat](https://img.shields.io/badge/AIsChat-主仓库-blue)](https://github.com/Coprexist/AIsChat)
[![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
[![Worlds](https://img.shields.io/badge/worlds-在线同步-brightgreen)](https://github.com/Coprexist/AIsChat-Community/tree/main/worlds)

</div>

<br>

---

<br>

## 这是什么？

**AIsChat Community 是 AIsChat 的共享资源社区仓库。**

[AIsChat](https://github.com/Coprexist/AIsChat) 是一个开源 AI 群聊框架——AI 拥有自己的状态、记忆和节奏，「群视界」能力让任何群聊都能绑定一个**活的世界**。而驱动这一切的，不只是世界本身，还有让 AI 与世界变强的**技能（skills）、工具（tools）和积木（blocks）**。

这个仓库就是**资源的集市**，收录四类资产：

| 资产 | 是什么 | 存放位置 |
|------|--------|----------|
| 🌍 **世界** | 完整世界包：页面 + 数据 + 代码，绑定群聊即成活的世界（2D 冒险、卡牌、小说互动…） | `worlds/` |
| 🧠 **技能 Skills** | AI 的能力说明书 + 执行代码：平台技能、世界 AI 技能、世界侧技能 | `skills/` |
| 🔧 **工具 Tools** | 可复用的工具定义：聊天社交、文件、群管理、记忆、网络、自我配置… | `tools/` |
| 🧩 **积木 Blocks** | 世界积木库：可组合的现成模块，拼出你的世界 | `blocks/` |

任何 AIsChat 实例都可以通过**同步机制**从这个仓库**发布资源、获取资源**——你造的会被所有人看见和使用，别人的也能一键进你的实例。

<br>

---

<br>

## 目录结构

```
├── worlds/                    # 🌍 世界包
│   ├── world-{id}/            # 每个世界一个目录
│   │   ├── meta.json          #   元数据（标题/描述/标签/作者…）
│   │   └── world.zip          #   完整包（页面+数据+代码，经安全过滤）
│   └── index.json             # 世界索引
├── skills/                    # 🧠 技能包
│   └── skill-{slug}/          #   技能卡（说明） + 执行代码 + manifest
├── tools/                     # 🔧 工具定义
│   └── tool-{name}/           #   工具描述 + 实现
├── blocks/                    # 🧩 世界积木
│   └── block-{name}/          #   积木定义与资源
└── index.json                 # 顶层索引（四类资源分节）
```

**`index.json`** 是同步的入口——商城/资源中心读取它获得资源列表，再按需下载。

<br>

---

<br>

## 快速开始

### 发布你的资源

1. 部署 [AIsChat](https://github.com/Coprexist/AIsChat)，造好你的世界 / 技能 / 工具 / 积木
2. 在资源中心（世界商城）点击**发布**，填写标题、描述、标签
3. 点击**同步到 GitHub**——资源包自动推送到本仓库对应目录，进入公共索引

### 获取别人的资源

1. 在 AIsChat 管理后台配置 GitHub 同步：仓库填 `Coprexist/AIsChat-Community`（或任何社区仓库），填入有写权限的 Token
2. 资源中心自动加载本仓库的资源列表（可开启"自动获取最新"或手动刷新）
3. 点击**导入**——资源一键进入你的实例，立即可用

<br>

---

<br>

## 现有资源

| 类型 | 资源 | 作者 | 说明 |
|------|------|------|------|
| 🌍 世界 | **诗の子** | ShuAICFR | 诗歌，AIsChat 的第一个世界 |

> 完整列表见 [index.json](index.json)，持续更新中。

<br>

---

<br>

## 关联项目

| 项目 | 说明 |
|------|------|
| [**AIsChat**](https://github.com/Coprexist/AIsChat) | 主项目——开源 AI 群聊框架，群聊即世界的入口 |
| [**AIsChat Client**](https://github.com/Coprexist/AIsChat-Client) | 桌面客户端（Tauri 2）——原生桌面应用，打开即达你的 AI 世界 |

<br>

---

<br>

## 许可证

MIT License · 资源内容版权归各自作者所有，代码与索引自由使用。

<br>

---

<br>

起步不久，资源会越来越多。欢迎你来贡献第一个。

**作者**:Coprexist 团队 · 提交 [Issue](https://github.com/Coprexist/AIsChat/issues) 或 Pull Request 分享你的资源。
