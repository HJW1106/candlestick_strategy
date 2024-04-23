# Backtest

* 測試台灣股市每檔上市櫃股票，每檔股票以預測率最高之買進訊號及**預測率**最高之賣出訊號為一組，算取其報酬率，若賣出訊號較買進訊號先出現則不計算其報酬率。

* 因訓練使用的電腦GPU記憶體不足將資料以每50筆做為分段預測如[`backtest.ipynb`](../backtest.ipynb)，再使用[`backtest_data.ipynb`](../backtest_data.ipynb)合併資料。(可依使用訓練之設備調整訓練筆數)

* 若需依2023年台灣股票市場所有上市櫃股票(不包含ETF)整年平均成交值作為篩選標的之基準可使用[`backtest_consider_vol.ipynb`](../backtest_consider_vol.ipynb)
