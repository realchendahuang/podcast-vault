# 播客金库 · Podcast Vault

> 全球精选硬核播客与深度长谈的开源知识库：高精度时间戳逐字稿、核心认知速读、底层心智模型与高光金句索引。  
> Open-source repository of curated high-signal podcast transcripts, mental models & key insights from world-class dialogues.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/realchendahuang/podcast-vault?style=social)](https://github.com/realchendahuang/podcast-vault)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Episodes](https://img.shields.io/badge/Episodes-1%2B-orange.svg)](episodes/)
[![Follow @realchendahuang](https://img.shields.io/badge/Follow-%40realchendahuang-1DA1F2?logo=x&logoColor=white)](https://x.com/realchendahuang)

---

## 设立宗旨

声音是当下时代最具真实感与思想厚度的载体，但动辄数小时的长音频往往存在三大阅读痛点：
1. **时间成本高昂**：两到四个小时的长篇对谈，往往伴随着漫长的前期客套与寒暄；
2. **难以精准检索**：音频和视频无法直接用 `Ctrl + F` 快速定位具体的代码选型、商业数据或关键结论；
3. **缺乏结构化沉淀**：听完即忘，未能转化为能进入个人知识库、随时供调用与启发的心智模型。

**Podcast Vault（播客金库）** 致力于将全球最前沿、最高信噪比的技术、商业、哲思与创始人对谈，全面转化并沉淀为**结构化、可检索、可溯源的纯文本开源资产**。

### 四大交付标准
* ✂️ **剥离寒暄，交付纯净信号**：为每期节目提炼高浓度核心速读与底层机制拆解；
* ⏱️ **全量时间戳逐字稿**：保留真实发言人的完整对话，所有核心结论均可随时回溯原片核验；
* 💡 **底层心智模型与金句库**：提炼反直觉认知、数学决策框架与工程经验，摘录现场高光原话；
* 📂 **纯文本与本地优先**：全部采用干净标准的 Markdown 格式，天然适配 Obsidian、Cursor、本地搜索与大模型分析。

---

## 精选单集目录 · Episode Catalog

| 编号 | 单集标题 | 嘉宾 / 主持 | 时长 | 核心认知与标签 | 精读导读 | 完整逐字稿 | 原片一手链接 |
|:---:|---|---|:---:|---|:---:|:---:|:---:|
| **001** | **对话孙宇晨：年轻人如何抓住 AI 时代的机会？** | 孙宇晨（Justin Sun）<br>邵艾伦（Allen Shao） | 04:22:26 | `AI 生产力` `Crypto` `孙学` `身体健康` `黄毛心智` `创造哲学` | [📖 导读与金句](./episodes/001-justin-sun-allen-shao-ai-opportunities/README.md) | [📝 24万字逐字稿](./episodes/001-justin-sun-allen-shao-ai-opportunities/transcript.md) | [📺 YouTube](https://www.youtube.com/watch?v=0Z-vhBvBmUY) |

> 完整目录与筹备中的单集计划请查看 [episodes/README.md](./episodes/README.md)。

---

## 仓库架构

```text
podcast-vault/
├── README.md               # 仓库首页、单集大盘索引与项目愿景
├── CONTRIBUTING.md         # 社区贡献指南（收录标准、逐字稿规范与 PR 流程）
├── LICENSE                 # MIT 开源协议
├── episodes/               # 播客单集核心归档
│   ├── README.md           # 完整单集索引列表
│   └── 001-justin-sun-allen-shao-ai-opportunities/
│       ├── README.md       # 单集精读导读（元数据、4小时核心速读、心智模型、金句库、时间轴）
│       ├── transcript.md   # 完整高精度时间戳逐字稿（纯文本 Markdown）
│       └── metadata.json   # 机器可读结构化元数据
└── templates/              # 单集收录脚手架模板
    └── episode-template/
        ├── README.md
        ├── transcript.md
        └── metadata.json
```

---

## 如何使用本仓库

### 1. 网页端与移动端阅读
直接点击对应单集的导读页面，通过金句库与主题时间轴掌握脉络；遇到感兴趣的段落，点击对应时间戳跳转回 YouTube 听取原片现场表达。

### 2. 本地检索与知识库挂载
将本仓库 Clone 到本地，直接作为独立知识库或子模块挂载到你的个人知识库（如 Obsidian、Logseq、Cursor）中：

```bash
git clone https://github.com/realchendahuang/podcast-vault.git
```

使用编辑器全局搜索功能，即可瞬间检索特定技术专有名词、商业决策或观点出处。

### 3. 驱动大模型深度分析
每份 `transcript.md` 均为清洗规范的 Markdown 纯文本，你可以直接将文件路径或文本丢给你的本地大模型或编程 Agent（Claude Code、Codex、Gemini 等），进行针对性提问、反事实推演或交叉对比。

---

## 正在筹备的单集方向

欢迎关注并推荐以下全球高信噪比播客专栏的内容：

* **Dwarkesh Podcast**（Ilya Sutskever, Sholto Douglas 等顶级模型架构长谈）
* **Latent Space**（AI 工程师、Coding Agent 落地与上下文工程）
* **The Changelog**（开源系统设计、本地优先 Local-First 架构）
* **Lenny’s Podcast**（独立产品冷启动、一人公司与商业化变现）
* **Lex Fridman Podcast**（前沿科技、物理学与思想领袖长程对谈）
* **中文深度对谈专栏**（海内外华人科技领袖、创造者与极客实战）

如果你希望将某期高价值播客贡献入库，请阅读 [CONTRIBUTING.md](./CONTRIBUTING.md) 并提交 Pull Request！

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=realchendahuang/podcast-vault&type=Date)](https://star-history.com/#realchendahuang/podcast-vault&Date)

---

## 社区与作者

* **作者**：[@realchendahuang](https://x.com/realchendahuang)
* **反馈与交流**：欢迎在 [GitHub Issues](https://github.com/realchendahuang/podcast-vault/issues) 中提出建议或推荐优质单集。

---

## License

本仓库的精读总结、心智模型分析、索引大纲与项目组织结构基于 [MIT License](./LICENSE) 开源。逐字稿文本受原节目创作者知识产权保护，仅供学习、研究与非商业性学术引证使用，引用请保留原片一手出处。
