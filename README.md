# 讓綠能觸手可及-根據區域微氣候資料預測發電量競賽
# AI-CUP-2024-Competition-to-predict-power-generation-based-on-regional-microclimate-data
## TEAM_5729
## Private leaderboard：554811.0 / Rank 18
**使用資料與程式碼皆放在同一層資料夾，使用資料皆為CSV，且程式碼皆為ipynb，下載後RUN ALL即可**

###### 1.程式執行環境說明
* Python：3.9.12
* 使用套件：requirements.txt
    ```js
    pip install -r requirements.txt
    ```
###### 2.Data processing(資料前處理)
* TEAM_5729_L1.ipynb
* TEAM_5729_L2.ipynb
* TEAM_5729_L3.ipynb......

執行檔案後輸出L1-17_Train_Revise.csv

* TEAM_5729_LALL.ipynb

執行檔案將合併L1-17_Train_Revise.csv，輸出LALL_Train_Revise.csv，該csv為模型訓練所使用的資料集，該csv在Model training和主目錄皆有備份

###### 3.Model training(模型訓練)
* TEAM_5729_RF.ipynb
* TEAM_5729_XGB.ipynb
* TEAM_5729_CatBoost.ipynb

執行檔案訓練模型，內容包括特徵選擇、資料切割、初始模型績效和超參數模型績效

###### 4.Final Model and Submission(最終模型和提交)
* TEAM_5729_Stacking.ipynb
* TEAM_5729_upload.ipynb

由於主目錄也有模型訓練所使用的csv，因此可直接執行TEAM_5729_Stacking.ipynb，Stacking Model訓練完成，透過joblib輸出模型檔，方可執行TEAM_5729_upload.ipynb
