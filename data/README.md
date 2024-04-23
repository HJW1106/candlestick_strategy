# 訓練資料集

## 資料準備

2019~2022台灣股市上市櫃所有股票(不包含ETF)每日開盤價、收盤價、最高價、最低價

## 產生訓練圖形

將資料欄位整理成mplfinance package欄位格式Data、Open、High、Low、Close

年月日:Date

開盤價(元):Open

最高價(元):High

最低價(元):Low

收盤價(元):Close

`winner_data.ipynb`[Winner](../winner_data.ipynb): 篩選2019年至2022年中，120日內最低及最高價格上漲150%以上之股票，依據篩選出標未來120日內上漲超過100%且預測日為最低價之前120日K線圖，並將路徑儲存於`Winner_path`。

`loser_data.ipynb`[Loser](../loser_data.ipynb): 篩選2019年至2022年中，120日內最高及最低價格下跌60%以上之股票，依據篩選出標未來120日內下跌超過30%且預測日為最高價之前120日K線圖，並將路徑儲存於`Loser_path`。

