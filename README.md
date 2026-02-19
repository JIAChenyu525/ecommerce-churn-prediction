# E-commerce 用户流失预测与营销优化

## 📌 项目背景
随着电商平台的快速增长，用户流失已成为关键问题。  
本项目旨在通过数据驱动的洞察识别高风险用户，并设计精准营销策略，以提高用户留存率并最大化投资回报率（ROI）。

## 🎯 项目目标
- 预测用户流失概率
- 识别高风险用户
- 设计针对性营销策略
- 评估营销ROI
- 构建自动化数据分析流水线

## 📊 数据集
数据集来自Kaggle，包含以下用户行为数据：
- 页面浏览量
- 加入购物车行为
- 购买记录
- 时间戳
- 商品类别与价格

## 🔍 项目流程
1. 数据清洗与预处理
2. 探索性数据分析（EDA）
3. 特征工程
4. 流失标签定义
5. 模型训练与评估
6. 用户分群
7. 营销策略与ROI分析
8. 可视化与报告
9. 自动化流水线

## 🛠 技术栈
- Python（pandas, numpy, sklearn, xgboost）
- SQL
- 数据可视化（matplotlib, seaborn）
- Tableau / PowerBI

## 📈 模型表现
- 逻辑回归
- 随机森林
- XGBoost

最佳AUC得分：0.78

## 💡 关键洞察
- 最近购买时间（Recency）和购买频率是预测流失的重要指标
- 高价值用户流失概率较低
- 精准优惠券策略可提升留存率

## 🚀 业务价值
- 识别高风险用户群体
- 提升营销效率
- 提高投资回报率（ROI）

## 📂 项目结构
```plaintext
ecommerce-churn-prediction/
│
├── data/
│   ├── raw/          # 原始数据集
│   └── processed/    # 清洗后数据
│
├── notebooks/        # Jupyter Notebook
│   ├── 01_eda.ipynb  # 探索性数据分析
│   ├── 02_feature_engineering.ipynb  # 特征工程
│   └── 03_model.ipynb  # 模型训练
│
├── src/              # 核心代码
│   ├── data_cleaning.py
│   ├── feature_engineering.py
│   ├── churn_model.py
│   ├── evaluation.py
│   ├── marketing_strategy.py
│   └── pipeline.py
│
├── visualization/    # 可视化图表
│
├── reports/          # 项目报告
│   ├── analysis_report.pdf
│   └── project_ppt.pptx
│
├── dashboard/        # 交互式仪表盘
│
├── README.md         # 项目说明
├── requirements.txt  # 依赖包
└── run_pipeline.py   # 自动化流水线入口
```

## ▶ 如何运行
```bash
pip install -r requirements.txt

python run_pipeline.py
```

> **运行说明**  
> `run_pipeline.py` 会自动执行完整流程：  
> ✅ 数据清洗 → ✅ 特征工程 → ✅ 模型训练 → ✅ 营销策略生成  
> 生成的营销策略可直接用于实际业务场景，如向高风险用户发送精准优惠券。

## 🔮 Future Work
- **深度学习模型**：探索LSTM/Transformer等模型提升预测精度
- **实时预测系统**：构建实时用户行为监控与流失预警机制
- **A/B测试框架**：设计科学实验验证营销策略有效性，持续优化ROI
