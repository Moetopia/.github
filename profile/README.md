<div align="center">
<img width="664" height="165" alt="L logo" src="https://github.com/user-attachments/assets/a895860c-e042-4131-962a-aca1815f2a16" />

# Moetopia · 萌托邦

**一个 AI 驱动的高性能二次元图片社区平台**

*An AI-powered, high-performance ACG art community platform*

---

我们**不会**拿所有作品训练任何**生成式AI**。

我们的AI功能均为图片识别等功能，并且保存作品的向量以及提供给本地MIT（漫画翻译器）服务器进行多语言翻译等功能。

---

[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?logo=fastapi&logoColor=white&style=flat-square)](https://fastapi.tiangolo.com)
[![Nuxt](https://img.shields.io/badge/Frontend-Nuxt3-00DC82?logo=nuxt.js&logoColor=white&style=flat-square)](https://nuxt.com)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-4169E1?logo=postgresql&logoColor=white&style=flat-square)](https://www.postgresql.org)
[![Qdrant](https://img.shields.io/badge/Vector_DB-Qdrant-FF3A3A?style=flat-square)](https://qdrant.tech)
[![License](https://img.shields.io/badge/License-AGPL--3.0-blue?style=flat-square)](https://www.gnu.org/licenses/agpl-3.0)

</div>

---

## 👋 关于我们 / About Us

**Moetopia（萌托邦）** 是一个专为 ACG 创作者与爱好者打造的图片社区平台。  
我们致力于将 AI 技术深度融入二次元内容的创作、发现与分享体验中——  
让每一位画师都能被看见，让每一幅作品都能找到它的观众。

> *Moetopia is an ACG art community platform built for creators and enthusiasts.  
> We bring AI-powered discovery, automatic tagging, and reverse image search to the world of anime-style art.*

---

## 🚀 核心特性 / Key Features

|  | 功能 | 说明 |
|--|------|------|
| 🤖 | **WD14 AI 自动打标** | 上传即触发，基于 9083 维语义向量零样本识别角色与属性 |
| 🔍 | **以图搜图** | 上传本地图片，毫秒级检索站内相似构图、角色、风格的作品 |
| 🌐 | **Pixiv 分布式同步** | 多节点 `pixiv-agent` 集群，自动追踪并同步 Pixiv 作者作品 |
| 🛡️ | **分级内容隔离** | 服务端强制安全注入，R-18 / AI 作品严格隔离 |
| ✍️ | **接稿系统** | 创作者开放委托接稿，完整稿件状态流转 |
| 📢 | **公告与社区** | 全站公告、评论、点赞、热评排序 |

---

## 🏗️ 项目构成 / Repositories

| 仓库 | 描述 | 技术栈 |
|------|------|--------|
| [**Moetopia**](https://github.com/Moetopia/) | 主仓库：前后端 + Pixiv 采集节点 | FastAPI · Nuxt 3 · PostgreSQL · Qdrant · Meilisearch |

> 更多子项目持续建设中 / More sub-projects coming soon...

---

## 🛠️ 技术栈概览 / Tech Stack

```
Frontend   →  Nuxt 3 + Vue 3 + TailwindCSS
Backend    →  FastAPI + Tortoise ORM + ARQ + PostgreSQL
Search     →  Meilisearch (text) + Qdrant (vector 9083-dim)
AI         →  ONNX Runtime + WD14 ConvNeXt Tagger v2
Sync       →  pixiv-agent (FastAPI + aiosqlite, scalable nodes)
```

---

## 🔬 研究背景 / Research Background

本项目的**以图搜图**系统基于毕业设计研究成果：  
通过对比 CLIP 与 WD14 语义向量方案，在二次元插画领域实现了零样本条件下 **99.0% 特异度** 的角色识别能力，  
彻底解决了通用多模态模型在 ACG 领域的「语义坍塌」问题。

> The reverse image search system is based on original research comparing CLIP vs. WD14 semantic vector approaches,  
> achieving **99.0% specificity** in zero-shot anime character recognition.

---

## 🤝 参与贡献 / Contributing

欢迎任何形式的贡献——无论是功能建议、Bug 反馈还是代码 PR。  
请先阅读对应仓库的 `README.md` 与架构约定。

*All contributions are welcome — feature requests, bug reports, or pull requests.  
Please read the repository README and architecture guidelines first.*

---

<div align="center">

Made with ❤️ for SakuraKoi Society & misaka10843

</div>
