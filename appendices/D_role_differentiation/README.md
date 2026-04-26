# 附录 D · 角色分化的完整证据

> 📄 完整内容见 [`../../docs/appendix.pdf`](../../docs/appendix.pdf) 第 D 部分（约 5 页）。

---

## 章节速览

### D.1 · Causal SHAP 完整数值分解

**附表 D1**：9 项核心特征的标准 SHAP / 直接贡献 / 传导贡献 / 总贡献完整数值表。

核心结果：

| 作用类型 | 特征 | 直接占比 |
|:---|:---|:---:|
| **驱动主导** | 累积惊奇度 | 95% |
|  | 宿主词位置 | 100% |
|  | 平均惊奇度 | 95% |
|  | 嵌套深度 | 94% |
|  | 词汇密度 | 99% |
|  | 上下文重叠度 | 96% |
|  | 成分至宿主距离 | 93% |
| **传导主导** | 内部平均依存距离 | **34%**（即 66% 经传导） |
| **刚性边界** | 是否核心论元 | 99%（直接，但量级小） |

### D.2 · DAG 稳健性 + 不对称扰动

**[附图 D1](../../figures/figD1_dag_robustness_heatmap.png)**：9 项特征在 13 种替代 DAG 下的作用类型分类热力图。

- 7/9 特征在全部 13 种 DAG 下保持一致
- 仅内部平均依存距离与成分至宿主距离在个别替代 DAG 下出现类别漂移
- 即便最激进设定（移除跨层边、反转因果方向），三类核心特征均未发生逆转

**[附图 D2](../../figures/figD2_robustness_summary.png)**：稳健性检验汇总。

**5% 标签不对称扰动**（100 次重复，模拟 95% 精确率）：

- 8/9 特征 100% 类型稳定
- Intra_MDD 稳定率 98%（从未转为直接主导）
- MDD 直接占比均值 41.9%，95% CI [36.3%, 48.7%]
- 距 70% 阈值有 **28 个百分点**的余量

### D.3 · 配价类别细分

**附表 D2**：核心论元内部各配价类别的破框率。

### D.4 · 偏相关检验（独立于 DAG）

**附表 D3**：非拓扑特征与破框的原始相关 vs 控制拓扑后的偏相关对比。

控制拓扑后，仅内部平均依存距离的关联强度出现显著跃升（Δr = 0.183），其余非拓扑特征基本不变 —— 与 Causal SHAP 路径分类完全一致。

---

## 相关图

- [`figD1_dag_robustness_heatmap.png`](../../figures/figD1_dag_robustness_heatmap.png) · 附图 D1
- [`figD2_robustness_summary.png`](../../figures/figD2_robustness_summary.png) · 附图 D2
- [`fig04_causal_shap_decomposition.png`](../../figures/fig04_causal_shap_decomposition.png) · 正文图 4（Causal SHAP 六面板分解）
- [`table02_direct_share_comparison.png`](../../figures/table02_direct_share_comparison.png) · 正文表 2（直接占比对照）
