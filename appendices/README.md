# 在线补充材料目录 / Online Appendices

> 📌 本目录提供附录 A–E 的结构化导航。完整排版版本（含全部图表与数学表达）见 [`../docs/appendix.pdf`](../docs/appendix.pdf)。

> *This directory provides structured navigation for Appendices A–E. For the fully formatted version with all figures and mathematical notation, see [`../docs/appendix.pdf`](../docs/appendix.pdf).*

---

## 整体结构 / Overall Structure

```
appendices/
├── A1_terminology_boundary.md             ← Ausklammerung/Extraposition 概念边界
├── A2_cross_study_positioning.md          ← 破框率的跨研究定位
├── A3_density_vs_weight.md                ← 信息密度与物理重量的可分离性
│
├── B_data_and_methods/                    ← 数据基础与方法
├── C_synergy_evidence/                    ← 协同结构的完整证据
├── D_role_differentiation/                ← 角色分化的完整证据
└── E_frame_organization/                  ← 框型组织的完整证据
```

---

## 附录 A · 术语与分布讨论 / Appendix A · Terminology & Distribution

A 部分为相对独立的论辩章节，已转录为 Markdown 格式以便在线阅读。

| 章节 | 主题 | 链接 |
|:---:|:---|:---:|
| **A.1** | Ausklammerung 与 Extraposition 的概念边界 — 论证传统术语二分实为同一约束结构在不同句框配置下的行为分化 | [📖 阅读](A1_terminology_boundary.md) |
| **A.2** | 破框率的跨研究定位 — 与既有德语研究（李媛等 2021、Cortés Rodríguez et al. 2024、Dubenion-Smith 2024 等）的发生率比对 | [📖 阅读](A2_cross_study_positioning.md) |
| **A.3** | 信息密度与物理重量的可分离性 — 论证累积惊奇度与成分长度的统计独立性 | [📖 阅读](A3_density_vs_weight.md) |

---

## 附录 B · 数据基础与方法 / Appendix B · Data and Methods

含语料预处理、变量操作化、模型设置、超参搜索、稳健性检验等技术性章节。

| 章节 | 主题 | 包含图表 |
|:---:|:---|:---|
| **B.1** | 破框分布统计（识别流程 + 人工核验） | 附表 B1–B3 |
| **B.2** | 特征筛选过程（18 项 → 9 项） | 附图 B1–B3，附表 B4–B6 |
| **B.3** | 模型比较与消融设计 | — |

> 完整内容见 [`../docs/appendix.pdf`](../docs/appendix.pdf) 第 B 部分。

---

## 附录 C · 协同结构的完整证据 / Appendix C · Full Synergy Evidence

| 章节 | 主题 | 包含图表 |
|:---:|:---|:---|
| **C.1** | 5 类分类器对比与维度消融完整结果 | 附表 C1–C2，附图 C1–C2 |
| **C.2** | SHAP 阈值行为与配对交互 | 附图 C3–C4，附表 C3–C4 |
| **C.3** | 极端位置稳健性 | 附表 C5 |
| **C.4** | 个案分析（HDT 第 20071 句、第 33842 句、第 35053 句） | — |

> 完整内容见 [`../docs/appendix.pdf`](../docs/appendix.pdf) 第 C 部分。

---

## 附录 D · 角色分化的完整证据 / Appendix D · Full Role Differentiation Evidence

| 章节 | 主题 | 包含图表 |
|:---:|:---|:---|
| **D.1** | Causal SHAP 完整数值分解 | 附表 D1 |
| **D.2** | DAG 稳健性 + 不对称扰动 | 附图 D1–D2 |
| **D.3** | 配价类别细分 | 附表 D2 |
| **D.4** | 偏相关检验 | 附表 D3 |

> 完整内容见 [`../docs/appendix.pdf`](../docs/appendix.pdf) 第 D 部分。

---

## 附录 E · 框型组织的完整证据 / Appendix E · Full Frame Organization Evidence

| 章节 | 主题 | 包含图表 |
|:---:|:---|:---|
| **E.1** | 成分类型子集对比（短语 vs 从句） | 附表 E1，附图 E1 |
| **E.2** | 句框配置的独立预测力 + 控制位置后的破框率分布 | 附表 E2–E5，附图 E2–E3，附表 E6 |
| **E.3** | 跨语言对比（德语 vs 荷兰语） | 附表 E7–E10，附图 E4 |
| **E.4** | 跨语体验证（HDT vs GSD） | 附表 E11，附图 E5–E7 |
| **E.5** | 瑞典语探索性分析 | 附图 E8–E9 |
| **E.6** | 操作化敏感性检验 | 附表 E12 |

> 完整内容见 [`../docs/appendix.pdf`](../docs/appendix.pdf) 第 E 部分。

---

## 状态 / Status

✅ **附录 A** ：A.1 / A.2 / A.3 已完成 Markdown 转录，可在线阅读。

📄 **附录 B–E** ：技术细节集中（公式、表格、多面板图），完整版仅在 `docs/appendix.pdf` 中提供。本目录文件夹下的 `README.md` 提供章节速览与图表索引。
