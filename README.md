
# AI-CUP-2023多模態病理嗓音分類
## 作品說明
* [前言](#前言)
* [資料處理](#資料處理)
* [訓練流程](#訓練流程)
* [預測](#預測)

前言
------
環境介紹
1. numpy  1.22.4 
2. sklearn  0.0.post1 
3. xgboost 0.90
4. pandas 1.5.2 
5. pandasq l0.7.3
6. cx-Orcle 8.3.0 
7. dill  0.3.6
8.  librosa 0.10.0.post2 
9.  tqdm  4.64. 

資料處理
------
Oversampling:利用excel的篩選功能將聲帶腫瘤、聲帶正常的資料複製之後貼在csv末尾或者利用以下程式實現:

      for i in range(len(train_X)):
    if train_Y[i][0] == 3:
        to_add.append(i)
    elif train_Y[i][0] == 4:
        to_add.append(i)

訓練流程
-------
直接開啟
