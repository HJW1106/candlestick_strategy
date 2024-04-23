# Model Description

* 使用 **python tensorflow package application**中影像辨識模型ResNet152

* 將K線圖路徑資料`Winner_path.csv`和`Loser_path.csv`匯入

* 考量GPU記憶體及ResNet模型是224*224的尺寸訓練之模型，將訓練資料尺寸重新定義為323 * 172.

* 加入Noise Value及Dropout層降低Overfitting可能性

* 儲存訓練後之模型`model_V2.h5`
