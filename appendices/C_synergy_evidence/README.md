# 附录 C · 协同结构的完整证据

> 📄 完整内容见 [`../../docs/appendix.pdf`](../../docs/appendix.pdf) 第 C 部分（约 8 页）。

---

## 章节速览

### C.1 · 模型比较与维度消融

**模型比较**（附表 C1）：5 类分类器在真实不平衡分布下的完整 PR-AUC 对比

| 类型 | 模型 | PR-AUC 区间 |
|:---|:---|:---:|
| 线性 | SVM、逻辑回归 | 0.61–0.62 |
| 非线性 | RF、MLP、XGBoost | **0.87–0.91** |

非线性模型整体优势 **~30 个百分点** —— 直接证据指向高阶交互。

**维度消融**（附表 C2 + [附图 C2](../../figures/figC2_dimension_combination_heatmap.png)）：31 组完整组合，PR-AUC 从 0.0724（单维度·角色）到 **0.8863**（全集）。

**交互项对照**（[附图 C1](../../figures/figC1_interaction_term_test.png)）：逻辑回归 + 交互项/二次项无法弥合非线性模型的优势。

### C.2 · SHAP 阈值行为与配对交互

**单变量阈值**（[附图 C3](../../figures/figC3_shap_dependence_thresholds.png) + 附表 C3）：

- 宿主词位置在归一化值 ≈ **1.0** 处出现 SHAP 断崖式反转（对应右句框边界）
- 累积惊奇度在 ≈ **30 bits** 处由抑制转为促进
- 内部平均依存距离效应较弱但方向一致

**配对交互**（[附图 C4](../../figures/figC4_shap_interaction_heatmap.png) + 附表 C4）：

- 宿主词位置 × 累积惊奇度（**0.359**，居首）
- 嵌套深度 × 是否核心论元（0.271，第二）

### C.3 · 极端位置稳健性

**附表 C5**：排除极端宿主词位置样本后，信息 × 拓扑的协同增益保持稳定。

### C.4 · 个案分析

正文涉及的三个 HDT 句例（第 20071、33842、35053 句）的完整拓扑展开与归因路径分析。

---

## 相关图

- [`figC1_interaction_term_test.png`](../../figures/figC1_interaction_term_test.png) · 附图 C1
- [`figC2_dimension_combination_heatmap.png`](../../figures/figC2_dimension_combination_heatmap.png) · 附图 C2
- [`figC3_shap_dependence_thresholds.png`](../../figures/figC3_shap_dependence_thresholds.png) · 附图 C3
- [`figC4_shap_interaction_heatmap.png`](../../figures/figC4_shap_interaction_heatmap.png) · 附图 C4
