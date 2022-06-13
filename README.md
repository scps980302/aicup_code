# aicup_code

# 介紹

這是AICUP 肺腺癌病理切片影像之腫瘤氣道擴散偵測競賽 II：運用影像分割作法於切割STAS輪廓 
提供程式碼的地方，我會在這邊提供比賽所需相關資料。我成績最佳的model使用的是DeepLabV3+配上tf_efficientnetv2_m_in21ft1k的模型，細節會逐一講解。



# 安裝環境與套件
環境

```
TWCC : cm.2xsuper 
映像檔 : pytorch-22.02-py3:latest
```

套件

```
pip install monai
pip install -U Setuptools
pip install git+https://github.com/qubvel/segmentation_models.pytorch
pip install adabelief-pytorch==0.2.0
```

# 模型權重

|類別|模型|Jupyter Notebook|最佳模型權重|預測結果圖|
--|--|--|--|--|
最佳模型|EfficientNetv2-m|[tf_efficientnetv2_m_in21ft1k](https://github.com/scps980302/aicup_code/blob/main/Finally_tinghong_tf_efficientnetv2_m_in21ft1k.ipynb)|[EfficientNetV2-m](https://drive.google.com/file/d/1OgITEmRlynHn6ODyTg-ccQpZMfDs3yKk/view?usp=sharing)|[預測結果圖](https://github.com/scps980302/aicup_code/blob/main/Best_tf_efficientnetv2_m_in21ft1k.zip)|

# 使用說明
主要需要修改的部分是圖片路徑`data_path`以及訓練及驗證影像存放的路徑`tempdir`

更改為使用者指定之路徑。





