<div align="center">

# AIsChat Community

**世界分享社区 · AIsChat 世界商城的 GitHub 数据源**

> **每个群聊都能长出一个活的世界——这里是世界的集市。**

[![AIsChat](https://img.shields.io/badge/AIsChat-主仓库-blue)](https://github.com/Coprexist/AIsChat)
[![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
[![Worlds](https://img.shields.io/badge/worlds-在线同步-brightgreen)](https://github.com/Coprexist/AIsChat-Community/tree/main/worlds)

</div>

<br>

---

<br>

## 这是什么？

**AIsChat Community 是 AIsChat 的世界分享社区仓库。**

[AIsChat](https://github.com/Coprexist/AIsChat) 是一个开源 AI 群聊框架——它的「群视界」能力让任何群聊都能绑定一个**活的世界**：有自己的网页、自己的世界 AI、自己的时间流速、甚至自己的运行代码。世界可以是 2D 冒险、卡牌对战、小说互动、剧本杀……任何你能描述的形态。

**这个仓库就是世界的集市**：任何 AIsChat 实例的世界商城，都可以通过 GitHub 同步机制从这个仓库**发布世界、拉取世界**——你造的世界能被所有人看见和使用，别人造的世界也能一键进你的商城。

<br>

---

<br>

## 目录结构

```
├── worlds/                    # 世界包
│   ├── world-8/               # 每个世界一个目录（world-{商品id}）
│   │   ├── meta.json          # 世界元数据（标题/描述/标签/作者…）
│   │   └── world.zip          # 世界完整包（页面+数据+代码，经安全过滤）
│   └── index.json             # 世界索引（商城同步用，含全部世界条目）
└── LICENSE
```

**`worlds/index.json`** 是商城同步的入口——AIsChat 商城读取它获得世界列表，再按需下载各世界的 `world.zip` 导入。

### meta.json 字段

| 字段 | 说明 |
|------|------|
| `id` | 商品 ID（发布实例内唯一） |
| `kind` | 商品类型 |
| `title` | 世界名称 |
| `description` | 世界介绍 |
| `tags` | 标签数组 |
| `author_name` | 发布者 |
| `source_world_id` | 源世界 ID |
| `package_size` | 包大小（字节） |
| `updated_at` | 更新时间（ISO 8601） |
| `download_url` | 世界包下载路径 |

<br>

---

<br>

## 快速开始

### 作为世界作者：发布你的世界

1. 部署 [AIsChat](https://github.com/Coprexist/AIsChat)，在「群视界」里造好你的世界
2. 打开 **世界商城 → 发布**，填写标题、描述、标签
3. 点击 **同步到 GitHub**——世界包自动推送到本仓库 `worlds/`，进入公共索引

### 作为世界玩家：获取别人的世界

1. 在 AIsChat 管理后台配置 GitHub 同步：仓库填 `Coprexist/AIsChat-Community`（或任何社区仓库），填入有写权限的 Token
2. 商城自动加载本仓库的世界列表（可开启"自动获取最新"或手动刷新）
3. 点击 **导入**——世界一键进入你的实例，立即可绑定群聊使用

<br>

---

<br>

## 现有世界

| 世界 | 作者 | 说明 |
|------|------|------|
| 🌸 **诗の子** | ShuAICFR | 诗歌，AIsChat 的第一个世界 |

> 完整列表见 [worlds/index.json](worlds/index.json)，持续更新中。

<br>

---

<br>

## 关联项目

| 项目 | 说明 |
|------|------|
| [**AIsChat**](https://github.com/Coprexist/AIsChat) | 主项目——开源 AI 群聊框架，群聊即世界的入口 |

<br>

---

<br>

## 许可证

MIT License · 世界内容版权归各自作者所有，代码与索引自由使用。

<br>

---

<br>

起步不久，世界会越来越多。欢迎你来造第一个。

**作者**:Coprexist 团队 · 提交 [Issue](https://github.com/Coprexist/AIsChat/issues) 或 Pull Request 分享你的世界。
