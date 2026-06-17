# AGENTS.md

## 專案身分

這個 repository 是 `ml-foundation-practice`。

專案目標是建立一個完整的機器學習實作作品集，涵蓋以下內容：

- 探索性資料分析，也就是 EDA。
- 資料前處理。
- 特徵工程。
- 模型選擇。
- Cross-validation。
- 不平衡分類處理。
- 模型評估。
- 使用 SHAP 進行模型可解釋性分析。

使用者過去已有深度學習專案經驗，尤其是訊號預測、空間預測與類似 computer vision workflow 的實作經驗。不過，目前這個 repository 的重點是補強傳統機器學習基礎。

## Repository 架構

- `00_environment/`：環境設定、套件需求、安裝檢查與開發環境說明。
- `01_titanic_classification/`：使用 Titanic 資料集練習基礎分類 workflow。
- `02_house_price_regression/`：使用房價預測資料集練習回歸 workflow。
- `03_credit_card_fraud/`：練習不平衡分類問題。
- `04_model_interpretability/`：使用 SHAP 練習模型解釋。
- `docs/`：專案脈絡、Codex 任務清單與學習規劃文件。

## 工作方式

在這個 repository 中工作時，請遵守以下原則：

- 優先提供清楚且具教學價值的說明。
- 不只寫出程式，也要解釋每個 ML 步驟為什麼需要做。
- 避免過度工程化。
- 程式碼應該維持 beginner-to-intermediate friendly。
- Notebook 或 Python script 都應保持可讀性，必要時加入簡短註解。
- 除非任務明確需要深度學習，否則優先使用 scikit-learn workflow。
- 新增程式碼時，應簡要說明假設、限制與下一步。

## 預期機器學習流程

每個子專案原則上都應該遵循以下流程：

1. 定義問題。
2. 載入並檢查資料。
3. 進行 EDA。
4. 處理缺失值。
5. 編碼類別特徵。
6. 視需求標準化或轉換數值特徵。
7. 正確切分 train、validation 與 test 資料。
8. 建立 baseline model。
9. 比較多個模型。
10. 使用 cross-validation。
11. 使用適合任務的指標評估模型。
12. 解釋模型行為。
13. 撰寫簡短的結果摘要與限制說明。

## 偏好的工具

請優先使用：

- Python
- pandas
- numpy
- matplotlib
- scikit-learn
- imbalanced-learn，用於不平衡資料任務。
- SHAP，用於模型可解釋性分析。
- Jupyter Notebook，適合展示學習與實驗流程。

## 避免事項

請避免：

- 在基礎 ML 任務中不必要地使用深度學習框架。
- 在 preprocessing 階段洩漏 test data 資訊。
- 在不平衡分類問題中只看 accuracy。
- 在建立簡單 baseline 之前就使用過度複雜的 pipeline。
- 只給出程式碼，不說明設計理由。

## 驗證要求

在判定任務完成前，請確認：

- 程式碼可以執行。
- 必要 imports 已包含。
- 沒有 train/test data leakage。
- 評估指標符合任務類型。
- 分類任務應包含 confusion matrix 與合適的分類指標。
- 不平衡分類任務應包含 precision、recall、F1、PR-AUC 或 ROC-AUC 等指標。
- 回歸任務應包含 MAE、RMSE 與 R² 等指標。
- 結果摘要應說明模型表現與限制。

## 使用者學習目標

使用者希望這個 repository 同時作為：

1. 機器學習基礎學習路徑。
2. 能展示實作能力的 portfolio project。

當需要提出任務建議時，請優先選擇同時提升學習價值與 portfolio 價值的工作。
