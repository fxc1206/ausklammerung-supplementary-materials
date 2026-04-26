# 框型结构对约束分工的组织作用——基于德语"破框"的可解释机器学习研究

> The Organizing Role of the Sentential Frame in Constraint Division of Labor:
> An Interpretable Machine Learning Study of German Ausklammerung

本仓库为论文的在线补充材料，含术语与分布讨论（附录 A）、数据基础与方法（附录 B），以及协同结构（C）、角色分化（D）、框型组织（E）三组完整证据。正文中"附录 X"或"附表 X"均指本仓库对应部分。

*This repository provides online supplementary materials for the paper, comprising terminology and distribution discussions (Appendix A), data basis and methods (B), and full evidence for synergy structure (C), role differentiation (D), and frame organization (E).*

---

## 论文文档 / Paper Documents

| 文件 | PDF | DOCX |
|:---|:---|:---|
| 正文 / Main Paper | [main_paper.pdf](docs/main_paper.pdf) | [main_paper.docx](docs/main_paper.docx) |
| 附录 / Appendix | [appendix.pdf](docs/appendix.pdf) | [appendix.docx](docs/appendix.docx) |

---

## 摘要 / Abstract

破框（Ausklammerung）集中体现了德语框型结构中的多重约束交互，但其协同机制尚缺乏系统实证。本文基于汉堡依存树库（HDT）153,035 句科技新闻语料，运用可解释机器学习发现：各约束以信息负荷与拓扑条件的非线性协同为核心，分化为"驱动—传导—边界"三重角色。信息负荷连续直接驱动，认知压力经拓扑条件间接传导，配价关系构成刚性边界。德语 V2/VL 配置对短语与从句产生相反调节；荷兰语及三种非框型北日耳曼语的对比进一步表明，传导路径随框型结构有无而出现或消失，驱动与边界跨语言稳定。本文将破框解释单位由单个约束转向框型结构所组织的约束分工，为"人驱复杂适应系统"所论生物普遍性与语言特殊性的区分提供句法实证。

**关键词** ：德语破框 · 框型结构 · 约束分工 · 作用路径 · 可解释机器学习

---

## 核心发现 / Key Findings

<table>
  <tr>
    <td align="center" width="33%">
      <b>F1 · 非线性协同</b><br>
      <i>Non-linear Synergy</i>
    </td>
    <td align="center" width="33%">
      <b>F2 · 驱动—传导—边界</b><br>
      <i>Three-Role Division</i>
    </td>
    <td align="center" width="33%">
      <b>F3 · 框型结构组织</b><br>
      <i>Frame Organization</i>
    </td>
  </tr>
  <tr>
    <td align="center"><img src="figures/fig02_synergy_pr_auc.png" alt="F1: PR-AUC comparison" /></td>
    <td align="center"><img src="figures/fig04_causal_shap_decomposition.png" alt="F2: Causal SHAP path decomposition" /></td>
    <td align="center"><img src="figures/fig07_cross_linguistic.png" alt="F3: Cross-linguistic comparison" /></td>
  </tr>
  <tr>
    <td valign="top">
      信息负荷与拓扑许可的二维联合 PR-AUC 达 0.804，约为五维全集模型（0.886）的 89%；其余二维组合均不超过 0.73。两个维度单独时分别为 0.46 与 0.32，联合后的跃升远超叠加预期。
    </td>
    <td valign="top">
      Causal SHAP 路径分解显示三类作用方式：信息负荷直接连续驱动（直接占比 ≥ 94%）；内部平均依存距离（MDD）经拓扑条件间接传导（传导占比 70.2%）；配价关系构成刚性边界（核心论元直接占比 99%）。
    </td>
    <td valign="top">
      德语 V2/VL 配置对短语与从句的破框率施加方向相反的调节；MDD 传导占比在框型语言内部呈梯度递减（德语 66% → 荷兰语 49%），在三种非框型 V2 语言中均为 0%。
    </td>
  </tr>
</table>

---

## 研究概览 / Research at a Glance

| 项目 / Item | 内容 / Detail |
|:---|:---|
| 主语料 / Primary Corpus | 汉堡依存树库 HDT 2.13，153,035 句科技新闻 |
| 跨语言验证 / Cross-Linguistic | 荷兰语 Alpino · 德语 GSD（维基百科）· 瑞典语 Talbanken · 丹麦语 DDT · 挪威语 Bokmaal |
| 核心方法 / Core Method | XGBoost + SHAP + Causal SHAP 路径分解 + mGPT 惊奇度 + PC 算法 DAG |
| 特征维度 / Features | 5 维 9 项（拓扑 / 加工 / 信息 / 形式 / 角色） |
| 破框发生率 / Extraposition Rate | 12.21%（HDT 全集）· 7.24%（GSD） |
| 路径分类阈值 / Path Threshold | 70%（直接 / 传导主导分界） |
| 稳健性 / Robustness | 5% 标签不对称扰动下 8/9 特征作用类型 100% 稳定 |

---

## 仓库结构 / Repository Structure

```
ausklammerung-supplementary-materials/
├── README.md
├── LICENSE                                CC-BY-4.0
├── CITATION.cff
│
├── docs/                                  论文与附录原文 / Paper and appendix
│   ├── main_paper.{pdf,docx}
│   └── appendix.{pdf,docx}
│
├── appendices/                            附录章节结构化导航 / Appendix navigation
│   ├── A1_terminology_boundary.md
│   ├── A2_cross_study_positioning.md
│   ├── A3_density_vs_weight.md
│   ├── B_data_and_methods/
│   ├── C_synergy_evidence/
│   ├── D_role_differentiation/
│   └── E_frame_organization/
│
├── figures/                               正文与附录全部图 / 400 DPI PNG
├── results/                               关键数值表 / Key numerical tables (CSV)
└── data/                                  数据集来源与许可证说明 / Data sources
```

---

## 在线补充材料目录 / Online Appendices

### 附录 A · 术语与分布讨论 / Terminology and Distribution

| 章节 | 内容 |
|:---:|:---|
| A.1 | [Ausklammerung 与 Extraposition 的概念边界](appendices/A1_terminology_boundary.md) |
| A.2 | [破框率的跨研究定位](appendices/A2_cross_study_positioning.md) |
| A.3 | [信息密度与物理重量的可分离性](appendices/A3_density_vs_weight.md) |

### 附录 B–E · 数据 / 方法 / 完整证据 / Data, Methods, and Full Evidence

| 章节 | 主题 |
|:---:|:---|
| [B](appendices/B_data_and_methods/) | 数据基础与方法（语料处理、变量操作化、模型设置） |
| [C](appendices/C_synergy_evidence/) | 协同结构的完整证据（模型对比、消融、交互效应） |
| [D](appendices/D_role_differentiation/) | 角色分化的完整证据（Causal SHAP 路径分解、稳健性） |
| [E](appendices/E_frame_organization/) | 框型组织的完整证据（V2/VL 对比、跨语言、跨语体） |

完整附录 PDF（含全部排版图表与数学表达）见 [`docs/appendix.pdf`](docs/appendix.pdf)。

---

## 数据来源 / Data Sources

本仓库不重新分发任何原始树库数据。如需获取原始数据，请按下表至各原始仓库下载并遵循其许可证条款。

| 树库 | 语言 | 许可证 |
|:---|:---|:---|
| [UD_German-HDT 2.13](https://github.com/UniversalDependencies/UD_German-HDT) | 德语 / German | CC-BY-NC-SA 4.0 |
| [UD_Dutch-Alpino](https://github.com/UniversalDependencies/UD_Dutch-Alpino) | 荷兰语 / Dutch | CC-BY-SA 4.0 |
| [UD_German-GSD](https://github.com/UniversalDependencies/UD_German-GSD) | 德语 / German | CC-BY-SA 4.0 |
| [UD_Swedish-Talbanken](https://github.com/UniversalDependencies/UD_Swedish-Talbanken) | 瑞典语 / Swedish | CC-BY-SA 4.0 |

详情参见 [`data/README.md`](data/README.md)。

---

## 源代码 / Source Code

Source code (data extraction, feature engineering, modeling, and the Causal SHAP analysis pipeline) will be released upon publication of this work.

本研究的源代码（含数据抽取、特征工程、建模与 Causal SHAP 分析全流程）将在论文正式发表后公开。完整方法描述见正文第二章及附录 B；变量操作化、模型选择、路径分解的全部技术细节均在附录中给出，足以支撑独立实现。

---

## 引用 / Citation

```bibtex
@unpublished{fu2026ausklammerung,
  author = {Fu, Xuchen},
  title  = {框型结构对约束分工的组织作用——基于德语"破框"的可解释机器学习研究},
  year   = {2026},
  note   = {Supplementary materials available at
            https://github.com/fxc1206/ausklammerung-supplementary-materials}
}
```

---

## 联系方式 / Contact

- 作者 / Author：付栩辰 Xuchen Fu
- 指导教师 / Supervisor：刘海涛 Haitao Liu
- 机构 / Institution：复旦大学 Fudan University
- 联系邮箱 / Email：[fxc1206@qq.com](mailto:fxc1206@qq.com)

---

## 许可证 / License

本仓库内容（论文文本、附录、图表、数据表）采用 [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) 许可证。

The contents of this repository (paper text, appendices, figures, and data tables) are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Datasets themselves are not redistributed in this repository; please comply with the license terms of the respective original treebanks.
