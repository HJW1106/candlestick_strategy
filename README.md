# Candlestick Strategy with ''Image recognition'' Model
K線圖為歷史悠久之金融商品分析工具，簡單易懂，其完整反應金融商品交易價格走勢
要在金融商品市場中獲利，最重要的獲利來源為資本利得及利息收入，而要賺取資本利得交易價格為最重要的因子，交易價格為所有投資人集體共識，與其實質價值並不一定相關，因此若能透過深度學習方式經由電腦掌握K線圖提供的資訊，能增進報酬率。
## Data
2019年到2022年間市場經歷了自2015年中國股災後4到5年的多頭，及2020年3月份新冠疫情的股災，到疫情後股市迅速的復甦，期間包含了多次市場大漲大跌，股市波動較過去時間都大，預期有許多資訊可以獲取，因此選擇此段期間作為模型訓練的資料。

**訓練資料集**

資料期間：2019年-2022年

資料範圍：台灣上市櫃所有股票(不包含ETF)

資料來源：TEJ

**測試資料集**

資料期間：2023年

資料範圍：台灣上市櫃所有股票(不包含ETF)

資料來源：TEJ

## Create Candlestick Graph

繪製包含預測日之前120日日K線圖，加入模型進行判斷。

**Loser**： 篩選2019年至2022年中，120日內最高及最低價格下跌60%以上之股票，依據篩選標的繪製未來120日內下跌超過30%且預測日之最高價為K線圖內最高價。

**Winner**： 篩選2019年至2022年中，120日內最低及最高價格上漲150%以上之股票，依據篩選標的繪製未來120日內上漲超過100%且預測日之最低價為K線圖內最低價。

**Note**:使用`loser_data.ipynb` 繪製大跌股票K線圖，使用`winner_data.ipynb` 繪製大漲股票K線圖
