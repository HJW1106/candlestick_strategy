# Test Data

* [`test_data.ipynb`](test_data.ipynb)以120筆資料為一組，每次往後移動一日並產生一組圖片樣本資料且連續產生生成樣本數後，建立卷積神經網路訓練樣本。

* 因訓練使用的電腦GPU記憶體不足將資料以每100筆做為分段預測，再使用[`test_path.ipynb`](test_path.ipynb)合併資料。

* 最後產出測試資料路徑`test_path.csv`
