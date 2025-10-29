# Adult数据集分析项目

## 项目概述

本项目基于Adult数据集，实现收入水平（predclass）的准确分类预测以及对教育程度（education）的可靠回归预测。通过机器学习方法分析人口普查数据中的关键特征与收入水平、教育程度之间的关系。

## 数据集说明

Adult数据集包含48,843条记录，16个特征，主要包括：

### 特征变量
- **人口统计学特征**：age（年龄）、sex（性别）、race（种族）
- **社会经济特征**：workclass（工作类别）、education（教育程度）、education-num（教育年限）、occupation（职业）、relationship（家庭关系）
- **经济指标**：capital-gain（资本收益）、capital-loss（资本损失）、hours-per-week（每周工作时间）
- **其他特征**：fnlwgt（权重）、marital-status（婚姻状况）、native-country（国籍）

### 目标变量
- **predclass**：收入水平分类（<=50K 或 >50K）
- **education**：教育程度（用于回归预测）

## 技术栈

- **编程语言**：Python
- **数据处理**：Pandas, NumPy
- **机器学习**：Scikit-learn
- **可视化**：Matplotlib

## 主要功能

### 1. 数据预处理
- 数据清洗和缺失值处理
- 特征工程和编码转换
- 数据标准化

### 2. 分类任务 - 收入水平预测
- 使用多种分类算法预测收入水平
- 模型包括：随机森林、逻辑回归、支持向量机等
- 评估指标：准确率、混淆矩阵、分类报告、ROC曲线

### 3. 回归任务 - 教育程度预测
- 使用回归算法预测教育年限
- 模型包括：线性回归、岭回归、Lasso回归、随机森林回归等
- 评估指标：均方误差、R²分数

### 4. 模型优化
- 超参数调优
- 交叉验证
- 特征重要性分析

## 项目文件结构

```
Adult-dataset-analysis-main/
├── README.md                    # 项目说明文档
├── 基于adult数据集分析.ipynb     # 主要分析代码（Jupyter Notebook）
├── 基于adult数据集分析.docx      # 详细分析报告
├── 流程图.jpg                   # 项目流程图
└── adult.csv                    # 原始数据集
```

## 使用方法

1. **环境准备**
   ```bash
   pip install pandas numpy scikit-learn matplotlib jupyter
   ```

2. **运行分析**
   - 打开 `基于adult数据集分析.ipynb`
   - 按顺序执行代码单元格
   - 查看模型训练结果和可视化图表

3. **数据集**
   - 确保 `adult.csv` 文件位于项目根目录

## 预期结果

- 收入水平分类的准确率分析
- 教育程度回归预测的精度评估
- 关键特征对收入和教育的影响分析
- 模型性能比较和优化建议

## 贡献

欢迎提交问题和改进建议！

## 许可证

本项目仅供学习和研究使用。
