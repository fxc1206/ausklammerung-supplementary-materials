# 数据来源与许可证 / Data Sources and Licensing

本研究全部基于公开发布的依存树库。本仓库**不重新分发**任何原始数据；用户应从下列官方来源直接获取，并遵守各自的许可证条款。

> *This study uses publicly available dependency treebanks. This repository does **not** redistribute any of the original data; users should obtain them directly from the official sources listed below and comply with the respective license terms.*

---

## 主语料 / Primary Corpus

### Hamburg Dependency Treebank (HDT) v2.13 — 德语 / German

| 属性 / Attribute | 内容 / Detail |
|:---|:---|
| **下载地址** | https://github.com/UniversalDependencies/UD_German-HDT |
| **UD 主页** | https://universaldependencies.org/treebanks/de_hdt/index.html |
| **语体** | 科技新闻（heise online IT news portal） |
| **规模** | 153,035 句（本研究使用全集） |
| **许可证** | CC-BY-NC-SA 4.0 |
| **本研究破框发生率** | 12.21%（含破框句 18,691，破框成分 21,518） |

**引用格式（GB/T 7714）**：

> BORGES VÖLKER E, WENDT M, HENNIG F, et al. HDT-UD: A very large Universal Dependencies treebank for German [C] // Proceedings of the Third Workshop on Universal Dependencies (UDW 2019). Paris: ACL, 2019: 46-57.

---

## 跨语言验证 / Cross-Linguistic Validation

### UD_Dutch-Alpino — 荷兰语 / Dutch

| 属性 | 内容 |
|:---|:---|
| **下载地址** | https://github.com/UniversalDependencies/UD_Dutch-Alpino |
| **UD 主页** | https://universaldependencies.org/treebanks/nl_alpino/index.html |
| **角色** | 框型结构较松的对照语种（V2 但 VP-final 较弱） |
| **许可证** | CC-BY-SA 4.0 |

**引用格式**：

> BOUMA G, VAN NOORD G. Increasing return on annotation investment: the automatic construction of a Universal Dependency treebank for Dutch [C] // Proceedings of the NoDaLiDa 2017 Workshop on Universal Dependencies (UDW 2017). Gothenburg: ACL, 2017: 19-26.

### UD_German-GSD — 德语（跨语体验证）/ German (Cross-Genre Validation)

| 属性 | 内容 |
|:---|:---|
| **下载地址** | https://github.com/UniversalDependencies/UD_German-GSD |
| **UD 主页** | https://universaldependencies.org/treebanks/de_gsd/index.html |
| **语体** | 维基百科为主，兼含新闻与评论 |
| **角色** | 检验科技新闻语体外的稳健性 |
| **本研究破框发生率** | 7.24% |
| **许可证** | CC-BY-SA 4.0 |

**引用格式**：

> MCDONALD R, NIVRE J, QUIRMBACH-BRUNDAGE Y, et al. Universal dependency annotation for multilingual parsing [C] // Proceedings of the 51st Annual Meeting of the Association for Computational Linguistics (ACL 2013). Sofia: ACL, 2013: 92-97.

### UD_Swedish-Talbanken — 瑞典语 / Swedish

| 属性 | 内容 |
|:---|:---|
| **下载地址** | https://github.com/UniversalDependencies/UD_Swedish-Talbanken |
| **UD 主页** | https://universaldependencies.org/treebanks/sv_talbanken/index.html |
| **角色** | 非框型 V2 北日耳曼语对照（无 VL 配置） |
| **许可证** | CC-BY-SA 4.0 |

**引用格式**：

> NIVRE J, MEGYESI B. Bootstrapping a Swedish treebank using cross-corpus harmonization and annotation projection [C] // Proceedings of the 6th International Workshop on Treebanks and Linguistic Theories (TLT 2007). Bergen: Northern European Association for Language Technology, 2007: 97-102.

---

## 许可证合规性说明 / License Compliance Note

本仓库内容（含分析所得的图表、数值表与方法描述）以 CC-BY-4.0 许可发布。但**树库原始数据不在本仓库内**——使用本研究路径复制实验时，请：

1. 自行从上述官方来源下载所需树库；
2. 遵守各树库的非商业、传染或署名要求；
3. 在派生工作中按各自规定提供归属署名。

> *The contents of this repository (figures, numerical tables, and method descriptions derived from the analysis) are released under CC-BY-4.0. The **original treebank data are not included in this repository**. When reproducing the analysis pipeline, please:*
>
> 1. *Download the required treebanks directly from the official sources listed above;*
> 2. *Comply with each treebank's non-commercial, share-alike, or attribution requirements;*
> 3. *Provide proper attribution in any derivative work as specified by each license.*
