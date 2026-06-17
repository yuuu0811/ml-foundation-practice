# Codex Task Backlog

這份文件用來記錄 Codex 可以協助完成的工作。任務應優先服務兩個目標：

1. 幫助使用者建立完整機器學習基礎。
2. 讓這個 repository 逐步成為可展示的 ML portfolio。

## 立即任務

1. 建立乾淨的 repository 架構。
2. 若資料夾目前是空的，加入 `.gitkeep`，讓 Git 可以追蹤空資料夾。
3. 新增 `requirements.txt`。
4. 若使用者決定採用開源授權，新增 MIT License。
5. 為每個子專案建立 starter notebook。
6. 補強 `README.md`，清楚說明專案目標、學習路徑與 repository 架構。
7. 確認所有檔案命名一致，避免資料夾名稱與文件描述不一致。

## Titanic classification 任務

- 載入 Titanic dataset。
- 進行資料初步檢查。
- 進行 EDA。
- 檢查 missing values。
- 處理缺失值。
- 編碼類別變數。
- 建立 baseline models：
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
- 使用 train/validation split 或 cross-validation。
- 評估分類指標：
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion matrix
- 撰寫結果摘要。
- 說明模型限制與下一步改善方向。

## House price regression 任務

- 載入 house price dataset。
- 進行資料初步檢查。
- 進行 EDA。
- 檢查目標變數分布。
- 視需求對目標變數進行 log transform。
- 處理數值特徵與類別特徵。
- 建立 preprocessing pipeline。
- 建立 baseline models：
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
- 使用 cross-validation。
- 評估回歸指標：
  - MAE
  - RMSE
  - R²
- 撰寫結果摘要。
- 說明模型限制與下一步改善方向。

## Credit card fraud detection 任務

- 載入 credit card fraud dataset。
- 檢查 class distribution。
- 明確說明不平衡資料問題。
- 避免 data leakage，特別是在 resampling 與 scaling 階段。
- 比較以下方法：
  - 原始資料 baseline。
  - Class weight。
  - Under-sampling。
  - Over-sampling。
  - SMOTE，如果適合。
  - Threshold tuning。
- 評估分類指標：
  - Confusion matrix
  - Precision
  - Recall
  - F1-score
  - ROC-AUC
  - PR-AUC
- 說明 precision 與 recall 的 trade-off。
- 從實務角度說明 false positive 與 false negative 的成本差異。
- 撰寫結果摘要與限制。

## SHAP model interpretability 任務

- 從已訓練的模型中選擇一個適合解釋的模型。
- 計算 SHAP values。
- 產生 global explanation。
- 產生 local explanation。
- 解釋重要特徵如何影響模型預測。
- 說明 SHAP 的限制。
- 將解釋結果整理成適合作品集展示的文字。

## 文件任務

- 更新 `README.md`，讓讀者能快速理解專案目的。
- 補上每個子專案的簡短說明。
- 為每個 notebook 補上：
  - 問題定義。
  - Dataset 說明。
  - 方法摘要。
  - 評估結果。
  - 結論與限制。
- 建立 `docs/LEARNING_ROADMAP.md`，整理學習路徑。
- 建立 `docs/NOTES.md`，紀錄重要 ML 觀念。

## 程式品質任務

- 檢查 imports 是否完整。
- 移除未使用的 imports。
- 確認 notebook cell 順序可由上到下執行。
- 確認 preprocessing 沒有使用 test data 資訊。
- 確認模型評估指標與任務類型相符。
- 確認結果可重現，例如設定 `random_state`。
- 將重複程式碼整理成 helper functions，但避免過度抽象化。

## Codex 工作原則

Codex 在處理這個 repository 時，應該優先：

1. 先讀取 `README.md`、`AGENTS.md` 與 `docs/PROJECT_CONTEXT.md`。
2. 確認目前 repository 狀態。
3. 提出最小且明確的修改計畫。
4. 一次處理一個清楚的任務。
5. 修改後說明改了哪些檔案，以及為什麼這樣改。
6. 避免一次產生大量未驗證的程式碼。
7. 優先保證 correctness，再追求複雜度與分數。

## 建議第一輪 Codex Prompt

可以在 Codex 中輸入：

```text
請協助我繼續開發 `ml-foundation-practice` repository。

請先閱讀：
- README.md
- AGENTS.md
- docs/PROJECT_CONTEXT.md
- docs/CODEX_TASKS.md

然後請你摘要：
1. 這個 repository 的目標。
2. 目前的資料夾架構。
3. 目前缺少或需要改善的檔案。
4. 下一步最值得做的 3 個任務。

請先不要修改檔案，只做檢查與提出計畫。
```
