# 图表索引 / Figures Index

本目录收录论文正文与附录中**全部嵌入图像**（共 27 张），从 `docs/main_paper.docx` 与 `docs/appendix.docx` 中提取并按论文中的图表编号命名。

> *This directory contains all 27 embedded images from the main paper and appendix, named according to their figure numbers.*

---

## 正文图表 / Main Paper Figures

| 编号 | 标题 | 文件 |
|:---:|:---|:---|
| **图 1** | 破框拓扑结构示例（HDT 第 20071 句） | [`fig01_topology_example.png`](fig01_topology_example.png) |
| **图 2** | 非线性协同的定位：单维度、二维组合与多维扩展的 PR-AUC 对比 | [`fig02_synergy_pr_auc.png`](fig02_synergy_pr_auc.png) |
| **图 3** | 信息负荷×拓扑条件联合破框率热力图 | [`fig03_synergy_heatmap.png`](fig03_synergy_heatmap.png) |
| **图 4** | 各特征的直接贡献与间接贡献拆解（六面板：响应形态 + 贡献拆解） | [`fig04_causal_shap_decomposition.png`](fig04_causal_shap_decomposition.png) |
| **图 5** | 核心论元与非核心论元的破框率对信息负荷的响应 | [`fig05_core_argument_response.png`](fig05_core_argument_response.png) |
| **图 6** | 句框配置对约束分工的双重调节：方向反转与权重分化 | [`fig06_v2_vl_dual_modulation.png`](fig06_v2_vl_dual_modulation.png) |
| **图 7** | 五种日耳曼语言中内部平均依存距离的传导占比及五维贡献结构 | [`fig07_cross_linguistic.png`](fig07_cross_linguistic.png) |
| **表 2** | 直接占比对照表（Causal SHAP × 偏相关） | [`table02_direct_share_comparison.png`](table02_direct_share_comparison.png) |

---

## 附录图 / Appendix Figures

> 📌 附录中的"附表"均为 Word 原生表格（非图像），仅在 `docs/appendix.pdf` 中可见。本目录仅收录"附图"（共 19 张）。

> *"附表" (tables) in the appendix are native Word tables (not images) and only visible in `docs/appendix.pdf`. This directory contains only "附图" (figures), 19 in total.*

### 附录 A · 术语与分布讨论

| 编号 | 标题 | 文件 |
|:---:|:---|:---|
| **附图 A1** | 10 特征模型 SHAP 贡献排名：累积惊奇度与成分长度的对比 | [`figA1_density_vs_weight.png`](figA1_density_vs_weight.png) |

### 附录 B · 数据基础与方法

| 编号 | 标题 | 文件 |
|:---:|:---|:---|
| **附图 B1** | 特征筛选流程：从 18 项候选指标到 9 项核心特征 | [`figB1_feature_selection_flow.png`](figB1_feature_selection_flow.png) |
| **附图 B2** | 候选特征的 Pearson 相关矩阵 | [`figB2_pearson_correlation.png`](figB2_pearson_correlation.png) |
| **附图 B3** | 核心特征在破框组与未破框组中的分布比较 | [`figB3_distribution_comparison.png`](figB3_distribution_comparison.png) |

### 附录 C · 协同结构的完整证据

| 编号 | 标题 | 文件 |
|:---:|:---|:---|
| **附图 C1** | 逻辑回归交互项对照实验：交互项与二次项对 PR-AUC 差距的解释比例 | [`figC1_interaction_term_test.png`](figC1_interaction_term_test.png) |
| **附图 C2** | 31 组维度组合的 PR-AUC 热力图（红框标识"拓扑+信息"核心配对） | [`figC2_dimension_combination_heatmap.png`](figC2_dimension_combination_heatmap.png) |
| **附图 C3** | 三项核心特征的 SHAP 依赖图（红色虚线标注阈值位置） | [`figC3_shap_dependence_thresholds.png`](figC3_shap_dependence_thresholds.png) |
| **附图 C4** | SHAP 交互效应热力图（非对角线，颜色越深交互越强） | [`figC4_shap_interaction_heatmap.png`](figC4_shap_interaction_heatmap.png) |

### 附录 D · 角色分化的完整证据

| 编号 | 标题 | 文件 |
|:---:|:---|:---|
| **附图 D1** | 9 项特征在 13 种 DAG 下的作用类型分类热力图 | [`figD1_dag_robustness_heatmap.png`](figD1_dag_robustness_heatmap.png) |
| **附图 D2** | 稳健性检验汇总 | [`figD2_robustness_summary.png`](figD2_robustness_summary.png) |

### 附录 E · 框型组织的完整证据

| 编号 | 标题 | 文件 |
|:---:|:---|:---|
| **附图 E1** | 五维度约束贡献占比：全量 vs 从句类 vs 短语类 | [`figE1_dimension_contribution_subsets.png`](figE1_dimension_contribution_subsets.png) |
| **附图 E2** | 句框类型的 SHAP 值分布：短语类 vs 从句类独立模型 | [`figE2_satzklammer_shap_distribution.png`](figE2_satzklammer_shap_distribution.png) |
| **附图 E3** | 各特征在不同成分类型间的 SHAP 归因差异热力图 | [`figE3_constituent_type_heatmap.png`](figE3_constituent_type_heatmap.png) |
| **附图 E4** | 作用类型跨语言一致性热力图 | [`figE4_cross_linguistic_heatmap.png`](figE4_cross_linguistic_heatmap.png) |
| **附图 E5** | 跨语体模型比较（HDT 科技新闻 vs GSD 维基百科） | [`figE5_cross_genre_comparison.png`](figE5_cross_genre_comparison.png) |
| **附图 E6** | 德语 GSD Causal SHAP 效应拆解（维基百科语体） | [`figE6_german_gsd_decomposition.png`](figE6_german_gsd_decomposition.png) |
| **附图 E7** | 跨语体 Causal SHAP 总贡献对比（HDT vs GSD） | [`figE7_cross_genre_total_contributions.png`](figE7_cross_genre_total_contributions.png) |
| **附图 E8** | 瑞典语 Causal SHAP 效应拆解（Talbanken 树库） | [`figE8_swedish_decomposition.png`](figE8_swedish_decomposition.png) |
| **附图 E9** | 跨类型学维度占比对比（德语/荷兰语/瑞典语） | [`figE9_cross_typology_dimensions.png`](figE9_cross_typology_dimensions.png) |

---

## 字体与配色 / Fonts & Colors

| 项目 | 内容 |
|:---|:---|
| **中文字体** | Noto Sans CJK SC（从 TTC collection 索引 2 提取，via fontTools） |
| **西文字体** | 默认 sans-serif |
| **分辨率** | 400 DPI |
| **背景** | 白色 |
| **盒型** | FancyBboxPatch 圆角 |

**五维统一配色 / Five-dimension unified palette**：

| 维度 | 色值 | 颜色 |
|:---|:---:|:---:|
| 拓扑 / Topology | `#4c72b0` | 🟦 蓝 |
| 加工 / Processing | `#dd8452` | 🟧 橙 |
| 信息 / Information | `#55a868` | 🟩 绿 |
| 形式 / Form | `#c44e52` | 🟥 红 |
| 角色 / Role | `#8172b3` | 🟪 紫 |
