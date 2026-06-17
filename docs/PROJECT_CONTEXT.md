# Project Context

## 背景

這個 repository 是使用者機器學習學習計畫的一部分。

使用者過去已有一些深度學習專案經驗。先前的專案名稱為：

「基於深度學習技術之高人流訊號盲區預測系統」

該系統主要包含兩個核心部分：

1. 人流分類。
2. 空間訊號預測。

使用者過去曾接觸深度學習、模型訓練與系統整合相關概念，但目前希望透過更基礎、結構化的實作，補強傳統機器學習能力。

## 目前學習方向

目前的學習規劃為：

1. 補強機器學習基礎。
2. 透過結構化專案練習完整 ML workflow。
3. 後續進一步實作 ECG / PhysioNet 類型專案。
4. 未來再深化或重新設計原本的訊號預測專案方向。

## Repository 目標

這個 repository 的目標是建立一個結構清楚的 ML practice portfolio。

本專案的重點不是單純追求最高分，而是展示完整機器學習流程：

- 資料理解。
- 資料前處理。
- 特徵工程。
- 模型建立。
- 模型驗證。
- 模型評估。
- 模型解釋。
- 文件化與結果總結。

## 預計專案

### 1. Titanic classification

目的：

- 學習基礎分類問題。
- 練習缺失值處理。
- 練習類別特徵編碼。
- 建立 baseline model。
- 比較多個分類模型。
- 使用 accuracy、precision、recall、F1-score 等指標。

### 2. House price regression

目的：

- 學習回歸問題。
- 練習數值與類別特徵處理。
- 練習目標變數轉換，例如 log transform。
- 使用 regression metrics。
- 使用 cross-validation。

### 3. Credit card fraud detection

目的：

- 學習不平衡分類問題。
- 比較 class weighting、resampling 與 threshold tuning。
- 使用 precision、recall、F1-score、ROC-AUC 與 PR-AUC。
- 理解不同錯誤類型的實務成本。

### 4. Model interpretability with SHAP

目的：

- 理解 feature importance。
- 比較 global explanation 與 local explanation。
- 使用 SHAP 解釋模型預測。
- 練習用清楚文字說明模型行為與限制。

## 重要設計原則

這個 repository 應該呈現出：

- 清楚的資料科學流程。
- 正確的資料切分觀念。
- 避免 data leakage。
- 適當的模型選擇理由。
- 與任務相符的評估指標。
- 對結果的反思，而不只是展示分數。

## 使用者目前狀態

使用者不是完全初學者，已具備深度學習與專案開發經驗；但在傳統機器學習流程、模型評估、cross-validation、特徵工程與不平衡資料處理方面，希望建立更完整的基礎。

因此，這個 repository 的內容應避免過度簡略，也不應直接跳到過度複雜的工程架構。最佳方向是：清楚、完整、可執行、可解釋。
