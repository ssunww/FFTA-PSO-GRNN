# FFTA-PSO-GRNN 入侵检测模型

本项目实现了一种基于 FFTA（模糊故障树分析）、PSO（粒子群优化）和 GRNN（广义回归神经网络）的网络入侵检测方法。

该方法主要包含三个阶段：

1. **FFTA 特征重要性分析**：利用模糊故障树分析计算各特征的失效概率和重要度，并完成特征选择。
2. **PSO 参数优化**：采用粒子群优化算法自动搜索 GRNN 的最优平滑因子。
3. **GRNN 分类识别**：使用优化后的 GRNN 对网络流量进行分类，实现正常流量与攻击流量识别。

本项目可用于网络入侵检测研究，并支持特征选择实验、消融实验和对比实验。

---

## 项目结构

FFTA-PSO-GRNN/<br>
│<br>
├── FFTA_PSO_GRNN.ipynb      # 主程序 Notebook<br>
├── requirements.txt         # Python 依赖环境<br>
├── README.md                # 项目说明文件<br>
├── shuju/<br>
&emsp;└── sample.csv         # 示例数据<br>

---

## 运行环境

- Python 3.10 及以上
- Jupyter Notebook

主要依赖库：

- numpy
- pandas
- scikit-learn
- matplotlib
- scipy
