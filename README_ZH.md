# VIGÍA — 学术文档（研究存档）

**语言：** 中文 · [English](README.md) · [Español](README_ES.md) · [Русский](README_RU.md)

> **状态：维护中，内容已过时。** 本仓库是主仓库 [`vigia-intent-analysis`](https://github.com/annatchijova/vigia-intent-analysis) 中 `docs/academic/` 文件夹在 **2026 年 11 月 5 日** 的快照（直接复制粘贴，不含 git 历史记录）。VIGIA 目前已拥有超过 500 个 Python 模块，其内部逻辑已经超越了这些文档中许多内容所描述的状态。它们不一定反映引擎当前的实际状态——发布它们是作为研究材料和理论参考,而非现行的技术文档。

## 为什么要设立这个独立仓库

VIGIA 主仓库迭代很快,其内部学术文档(位于 `docs/academic/`)在各次修订之间会变得过时。与其让这约 198 份文档被埋没、无法公开访问,不如把它们单独拆分到这里,以便分享给研究者——尤其是为了继续推广将 **查尔斯·桑德斯·皮尔士(Charles Sanders Peirce)** 的符号学(以及艾柯、格赖斯和卡内基的理论)应用于取证推理系统,这正是 VIGIA 的理论核心。

随着时间推移,这个存档会被更新和扩充,以便更好地反映目前超过 500 个模块的架构及其设计理由。目前它只是一个快照,而非持续更新的文档。

## 从这里开始

- **[VIGIA_RESEARCH_REPORT.md](VIGIA_RESEARCH_REPORT.md)**([英文版](VIGIA_RESEARCH_REPORT_EN.md))——关于 VIGIA 存在之理由的长篇研究:传统 DFIR(数字取证与事件响应)所面临的危机、EDR 作为“黑箱”的问题,以及提出一个将证据与 LLM 叙述相分离的确定性溯因推理引擎。该文档最初由 Kimi K2 智能体集群生成,并由 Claude 对照实时仓库进行了核实与修正——完整的作者信息详见文档开头。
- **[ACADEMIC_DOCS_MASTER_INDEX_ZH.md](ACADEMIC_DOCS_MASTER_INDEX_ZH.md)**——192 个已记录模块的总索引,按领域分类(`core`、`tools`、`sift`、`forensics`、`inference`、`pipeline`、`security`、`scripts`、`governance`、`specialized`)。另有[英文版](ACADEMIC_DOCS_MASTER_INDEX_EN.md)、[西班牙文版](ACADEMIC_DOCS_MASTER_INDEX.md)和[俄文版](ACADEMIC_DOCS_MASTER_INDEX_RU.md)。

## 目录结构

```
.
├── VIGIA_RESEARCH_REPORT.md / _EN.md       ← VIGIA 存在之理由(ES/EN)
├── ACADEMIC_DOCS_MASTER_INDEX.md           ← 总索引(ES)
│                        _EN.md / _RU.md / _ZH.md   ← 同一索引的英/俄/中文版本
├── core/            — 38 篇文档 — 核心流水线、符号学、信号、校准
├── tools/           — 22 篇文档 — CAIE、对抗性 NLP、MITRE、模式识别、EML
├── sift/            —  9 篇文档 — MFT、prefetch、shellbag、注册表、网络、浏览器、内存
├── forensics/       —  5 篇文档 — PDF、PKI、RFC3161、图像分析、证据链
├── inference/       —  5 篇文档 — 溯因推理、行为指纹
├── pipeline/        —  4 篇文档 — 数据包、报告、SIFT 桥接、证据登记
├── security/        —  4 篇文档
├── governance/       —  2 篇文档
├── specialized/      —  2 篇文档
├── scripts/          — 10 篇文档
├── root/             — 13 篇文档 — 原始语料库根目录下的杂项内容
└── unclassified/     — 78 篇文档 — 按旧有分类方案尚待重新归类
```

每份文档都会就皮尔士、艾柯和格赖斯的符号学理论对其所述模块作出科学说明,部分文档还附有多语种技术术语表——各文件具体支持哪些语言,请参见该文件的文档头部说明。

## 许可证

**Apache License 2.0** —— 详见 [LICENSE](LICENSE)。与主仓库 [`vigia-intent-analysis`](https://github.com/annatchijova/vigia-intent-analysis) 使用相同的许可证,因为本存档是同一项目的一部分,采用不同的许可证并不合理。

## 作者署名

与 VIGIA 项目采用相同的署名规则:架构、理论决策与设计均归 **Anna Tchijova** 所有;其中多篇文档由一组 AI 模型(Kimi K2、Claude,以及视具体文档而定的其他模型——详见各文件文档头部)在她的指导下撰写,并对照实时仓库进行了核实与修正。完整细节请见主仓库中的 [`AUTHORS.md`](https://github.com/annatchijova/vigia-intent-analysis/blob/main/AUTHORS.md)。

## 主仓库

代码、测试以及现行有效的技术文档均位于 [`github.com/annatchijova/vigia-intent-analysis`](https://github.com/annatchijova/vigia-intent-analysis)。本仓库仅为学术文档的存档。
