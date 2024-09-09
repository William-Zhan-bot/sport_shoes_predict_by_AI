# sport_shoes_predict

以Kaggle2020~20235之球鞋基本資料，訓練模型進行球鞋售價預測
Kaggle: 

資料庫欄位: 品牌 款式名稱 出產年份 主打族群 尺寸 功能類別 材質 主要顏色 售價 
數量: 100筆

選用 Feature: 品牌 主打族群 尺寸 功能類別 材質 主要顏色
Label: 售價(USD)

算法選用:
以線性回歸成效過低，r平方僅為0.15
改以決策樹回歸進行評估，r平方達到0.7

資料清理:
皆為類別資料，先對所有feature進行one-hot encoding後開始以決策樹回歸進行訓練

模型輸出後檔案為: decision_tree_model.pkl
啟動predict.ipynb必須先跑過預測產生模型才可順利執行
