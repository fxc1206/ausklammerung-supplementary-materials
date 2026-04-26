# 附录 E · 框型组织的完整证据

> 📄 完整内容见 [`../../docs/appendix.pdf`](../../docs/appendix.pdf) 第 E 部分（约 12 页，附录中规模最大）。

---

## 章节速览

### E.1 · 成分类型子集对比（短语 vs 从句）

**附表 E1**：从句类与短语类子集的模型比较、五维贡献占比与 Causal SHAP 路径分解。

**[附图 E1](../../figures/figE1_dimension_contribution_subsets.png)**：五维度约束贡献占比 —— 全量 vs 从句类 vs 短语类。

核心发现：两类成分共享信息 × 拓扑协同架构，仅约束权重系统性不同。

### E.2 · 句框配置的独立预测力

**附表 E2**：控制宿主词位置后句框类型的独立预测力（PR-AUC，十折交叉验证）。

| 模型 | PR-AUC（无句框） | PR-AUC（加句框） | p 值 |
|:---|:---:|:---:|:---:|
| 仅宿主词位置 | 0.137 | **0.147** | < 1e-6 |
| 9 项核心变量 | 0.925 | **0.937** | < 1e-6 |

**结论**：控制物理空间后句框类型仍保留独立预测力 —— 拓扑许可不能归约为物理空间。

**附表 E3 / E4**：控制宿主词归一化位置后从句/短语的破框率（V2 vs VL）。方向反转最大达 +34.5 个百分点。

**[附图 E2](../../figures/figE2_satzklammer_shap_distribution.png)**：句框类型的 SHAP 值分布（短语类 vs 从句类独立模型）。

**[附图 E3](../../figures/figE3_constituent_type_heatmap.png) + 附表 E5–E6**：V2/VL × 短语/从句四格的五维贡献占比，逐特征 SHAP 偏移热力图。

### E.3 · 跨语言对比（德语 vs 荷兰语）

**附表 E7**：五种日耳曼语言的维度贡献占比与传导路径对比（正文图 7 的数值底表）。

**附表 E8 / E9 / E10**：德语 ↔ 荷兰语模型比较、Causal SHAP 完整数值、9 项特征作用类型对比。

**[附图 E4](../../figures/figE4_cross_linguistic_heatmap.png)**：作用类型跨语言一致性热力图 —— 8/9 特征跨语一致。

### E.4 · 跨语体验证（HDT vs GSD）

**[附图 E5](../../figures/figE5_cross_genre_comparison.png)**：跨语体模型比较（科技新闻 vs 维基百科）。

**附表 E11**：德语 GSD Causal SHAP 完整数值表。

**[附图 E6](../../figures/figE6_german_gsd_decomposition.png)**：GSD Causal SHAP 效应拆解。

**[附图 E7](../../figures/figE7_cross_genre_total_contributions.png)**：HDT vs GSD 总贡献并排对比。

### E.5 · 瑞典语探索性分析

**[附图 E8](../../figures/figE8_swedish_decomposition.png)**：瑞典语 Causal SHAP 效应拆解（Talbanken 树库）。

**[附图 E9](../../figures/figE9_cross_typology_dimensions.png)**：跨类型学维度占比对比（德语 / 荷兰语 / 瑞典语）。

核心发现：非框型 V2 语言中传导路径**消失**（MDD 传导占比 0%）。

### E.6 · 操作化敏感性检验

**附表 E12**：正文基线与操作化放宽版的九特征路径分类对照。

---

## 相关图

- [`figE1_dimension_contribution_subsets.png`](../../figures/figE1_dimension_contribution_subsets.png) · 附图 E1
- [`figE2_satzklammer_shap_distribution.png`](../../figures/figE2_satzklammer_shap_distribution.png) · 附图 E2
- [`figE3_constituent_type_heatmap.png`](../../figures/figE3_constituent_type_heatmap.png) · 附图 E3
- [`figE4_cross_linguistic_heatmap.png`](../../figures/figE4_cross_linguistic_heatmap.png) · 附图 E4
- [`figE5_cross_genre_comparison.png`](../../figures/figE5_cross_genre_comparison.png) · 附图 E5
- [`figE6_german_gsd_decomposition.png`](../../figures/figE6_german_gsd_decomposition.png) · 附图 E6
- [`figE7_cross_genre_total_contributions.png`](../../figures/figE7_cross_genre_total_contributions.png) · 附图 E7
- [`figE8_swedish_decomposition.png`](../../figures/figE8_swedish_decomposition.png) · 附图 E8
- [`figE9_cross_typology_dimensions.png`](../../figures/figE9_cross_typology_dimensions.png) · 附图 E9
- [`fig07_cross_linguistic.png`](../../figures/fig07_cross_linguistic.png) · 正文图 7（5 语种汇总）
- [`fig06_v2_vl_dual_modulation.png`](../../figures/fig06_v2_vl_dual_modulation.png) · 正文图 6（V2/VL 双重调节）
