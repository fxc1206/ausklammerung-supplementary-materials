# 关键数值表 / Key Numerical Tables

本目录提供论文核心结论所对应的数值表（CSV 格式，UTF-8 编码），从附录的关键表格转录而来，便于读者直接核查或在自有分析中引用。

> *This directory provides numerical tables (CSV format, UTF-8) underlying the paper's core findings, transcribed from key tables in the appendix.*

---

## 文件清单 / File List

| 文件 | 内容 | 对应附表 | 论据 |
|:---|:---|:---:|:---:|
| [`causal_shap_total_contributions.csv`](causal_shap_total_contributions.csv) | 9 项核心特征的标准 SHAP / 直接贡献 / 传导贡献 / 总贡献 / 作用类型 | 附表 D1 | **F2** |
| [`dimension_ablation.csv`](dimension_ablation.csv) | 31 组维度组合的完整 PR-AUC / ROC-AUC / F1 | 附表 C2 | **F1** |
| [`cross_linguistic_comparison.csv`](cross_linguistic_comparison.csv) | 5 种日耳曼语言的维度贡献占比与 MDD 传导路径对比 | 附表 E7 | **F3** |
| [`model_comparison.csv`](model_comparison.csv) | 5 类分类器（SVM / 逻辑回归 / RF / MLP / XGBoost）默认与优化参数下的完整性能 | 附表 C1 | F1 配套 |

---

## 关键结论锚点 / Key Findings Anchored

### F1 · 非线性协同 / Non-linear Synergy

来源：[`dimension_ablation.csv`](dimension_ablation.csv) + [`model_comparison.csv`](model_comparison.csv)

- 全集 5 维 PR-AUC：**0.886**
- 信息 + 拓扑 二维 PR-AUC：**0.804**（达全集 89%）
- 任何二维组合均不超过 0.73（除信息 + 拓扑外）
- 非线性模型（XGBoost / RF / MLP）整体优于线性模型（SVM / LR）约 30 个百分点

### F2 · 驱动—传导—边界 / Three-Role Division

来源：[`causal_shap_total_contributions.csv`](causal_shap_total_contributions.csv)

| 作用类型 | 特征 | 直接贡献占比 |
|:---|:---|:---:|
| 驱动主导（7 项） | 累积惊奇度、宿主词位置、平均惊奇度、嵌套深度、词汇密度、上下文重叠度、成分至宿主距离 | 93–100% |
| 传导主导（1 项） | 内部平均依存距离 (MDD) | **34%**（即 66% 经拓扑传导） |
| 刚性边界（1 项） | 是否核心论元 | 99%（直接，但量级量化为外置抑制） |

### F3 · 框型结构组织 / Frame Organization

来源：[`cross_linguistic_comparison.csv`](cross_linguistic_comparison.csv)

| 语言 | 框型结构 | MDD 传导占比 | 作用类型 |
|:---|:---:|:---:|:---|
| 德语 | 严格 | **66%** | 传导主导 |
| 荷兰语 | 较宽松 | 49% | 混合偏传导 |
| 瑞典语 | 无 | **0%** | 直接主导 |
| 丹麦语 | 无 | **0%** | 直接主导 |
| 挪威语 | 无 | **0%** | 直接主导 |

核心断点：传导路径在 V2 框型语言（德 / 荷）中存在，在三种非框型 V2 北日耳曼语中**消失** —— 证据指向框型结构对路径分化的组织作用。

---

## 列名英文对照 / Column Name Reference (English)

| 中文列名 | English |
|:---|:---|
| 特征 | Feature |
| 标准 SHAP | Standard SHAP |
| 直接贡献 / 传导贡献 / 总贡献 | Direct / Transmitted / Total Contribution |
| 作用类型 | Action Type |
| 维度组合 / 维度数 | Dimension Combination / Number of Dimensions |
| PR-AUC / ROC-AUC / F1 | (standard ML metrics) |
| 语言 | Language |
| 框型结构 | Sentential Frame |
| 外置率 | Extraposition Rate |
| 拓扑 / 加工 / 信息 / 形式 / 角色 | Topology / Processing / Information / Form / Role |
| MDD 传导占比 | MDD Transmission Share |
| 分类器 / 参数 | Classifier / Setting |
| 精确率 / 召回率 | Precision / Recall |

---

## 完整附录数据 / Full Appendix Data

附录中尚有更多数值表（附表 B1–B6、C3–C5、D2–D3、E1–E12 等）以原生 Word 表格形式呈现，未独立转 CSV。如有需要请直接参照 [`../docs/appendix.pdf`](../docs/appendix.pdf) 或联系作者。
