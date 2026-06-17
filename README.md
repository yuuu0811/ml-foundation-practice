# ML Foundation Practice

這個 repository 是一個機器學習基礎實作專案，目標是建立一套完整、可展示的機器學習工作流程。

本專案不只追求模型分數，而是希望透過多個經典任務，系統化練習從資料理解、前處理、特徵工程、模型選擇、交叉驗證、評估指標到模型解釋的完整流程。

## 專案目標

本專案主要用於：

1. 補強傳統機器學習基礎。
2. 建立可放在 GitHub 上展示的 ML portfolio。
3. 養成標準化 ML workflow 的實作習慣。
4. 為未來進一步實作 ECG / PhysioNet 或其他進階資料科學專案做準備。

## 預計涵蓋能力

本 repository 會逐步練習以下能力：

- 探索性資料分析，也就是 EDA。
- 資料清理與缺失值處理。
- 類別特徵編碼。
- 數值特徵轉換與標準化。
- 特徵工程。
- 訓練集、驗證集與測試集切分。
- Baseline model 建立。
- 多模型比較。
- Cross-validation。
- 分類與回歸任務的評估指標。
- 不平衡資料處理。
- 模型可解釋性分析，例如 SHAP。
- 實驗結果整理與限制說明。

## 專案內容

### 1. Titanic classification

這是入門分類任務，用來練習：

- 資料載入與初步檢查。
- 缺失值處理。
- 類別特徵編碼。
- 分類模型 baseline。
- Accuracy、precision、recall、F1-score 等指標。

### 2. House price regression

這是房價預測回歸任務，用來練習：

- 回歸問題定義。
- 數值與類別特徵處理。
- 目標變數分布觀察。
- 特徵轉換。
- MAE、RMSE、R² 等回歸指標。
- Cross-validation。

### 3. Credit card fraud detection

這是不平衡分類任務，用來練習：

- 類別不平衡問題分析。
- Class weight。
- Under-sampling / over-sampling。
- Threshold tuning。
- Confusion matrix。
- Precision、recall、F1-score、ROC-AUC、PR-AUC。

### 4. Model interpretability with SHAP

這是模型可解釋性任務，用來練習：

- Global explanation。
- Local explanation。
- Feature importance。
- SHAP value 解讀。
- 模型決策邏輯說明。

## 建議開發流程

每個子專案原則上都應該遵循以下流程：

1. 定義問題。
2. 載入資料。
3. 進行 EDA。
4. 處理缺失值。
5. 處理類別特徵。
6. 處理數值特徵。
7. 切分資料集。
8. 建立 baseline model。
9. 比較多個模型。
10. 使用 cross-validation。
11. 使用合適的指標評估模型。
12. 進行模型解釋。
13. 撰寫結果總結與限制。

## 使用工具

建議使用：

- Python
- pandas
- numpy
- matplotlib
- scikit-learn
- imbalanced-learn
- SHAP
- Jupyter Notebook

除非任務明確需要，否則本 repository 優先使用傳統機器學習方法，不優先使用深度學習框架。

## 學習定位

這個專案的重點不是單純追求 leaderboard 分數，而是展示完整且正確的 ML 思考流程。

- 你如何理解資料。
- 你如何避免 data leakage。
- 你如何選擇模型。
- 你如何評估模型。
- 你如何處理模型限制。
- 你如何解釋模型結果。
