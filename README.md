# AICUP_STAS_Segmentation

# 介紹
#### 以下為 AICUP 肺腺癌病理切片影像之腫瘤氣道擴散偵測競賽中所使用的程式代碼
#### 採用的是 DeepLabV3+ 搭配 eca_nfnet_l2 所組成的模型

# 環境與函式庫
#### 訓練環境
```
TWCC : cm.2xsuper (TWCC 4 GPU + 16 cores + 240GB memory + 120GB share memory)
映像檔 : pytorch-22.02-py3:latest
```
#### 函式庫
```
!pip3 install monai
!pip3 install -U Setuptools
!pip install torch
!pip install torchvision
!pip install optuna
!pip install git+https://github.com/qubvel/segmentation_models.pytorch
!pip install adabelief-pytorch==0.2.0
```

# 模型與權重

類別|訓練Jupyter Notebook|權重|結果圖片|
--|--|--|--|
Data Process|[Data_preprocess](https://github.com/yungchang310514077/AICUP_STAS_Segmentation/blob/main/datapreprocess.ipynb)|-|-
ECA-NFNet|[ECA-NFNet](https://github.com/yungchang310514077/AICUP_STAS_Segmentation/blob/main/Finally_eca_nfnet_l2_ver3_DeepLabV3Plus.ipynb)|[Weight](https://drive.google.com/file/d/1Ybb1UDdhyX1QzX-EXkuX4scclWH5Xfaj/view?usp=sharing)|Zip 位置|
