# 经藏 PAR2 灾难恢复数据

这里保存真实的 PAR2 / Reed–Solomon 恢复块，配合以下仓库的经文数据使用：

- https://github.com/Chanray-May9/dharma-archive
- https://github.com/Chanray-May9/dharma-archive-data-001
- https://github.com/Chanray-May9/dharma-archive-data-002

将各仓库的 `data/` 合并到同一个恢复目录，执行 `par2 repair -B. data/recovery/dharma.par2`，再用主仓库的 SHA-256 清单核验。实际创建参数及“丢失一个整包、损坏另一个包”的修复实测见 `data/recovery/PROTECTION.json`。

纠错能力按剩余恢复块计算。此仓库单独不能恢复全部经文，须保留尽可能多的源文件、索引和恢复块。
