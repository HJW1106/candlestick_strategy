# Candlestick Strategy with Image Recognition Model
K線圖為歷史悠久之金融商品分析工具，雖然概念簡單易懂，但其完整反應市場所有投資人對金融商品交易價格的共識，要在金融商品市場中獲利，最重要的獲利來源為資本利得及利息收入，而交易價格為賺取資本利得中最重要的因子，因此此專案希望透過深度學習方式經由電腦掌握K線圖提供的資訊，藉由預測交易價格走勢以增進投資報酬率。
## 資料蒐集
2019年到2022年間市場經歷了自2015年中國股災後4到5年的多頭，及2020年3月份新冠疫情的股災，到疫情後股市迅速的復甦，期間包含了多次市場大漲大跌，股市波動較過去時間都大，預期有許多資訊可以獲取，因此選擇此段期間作為模型訓練的資料。

**訓練資料集**

* 資料期間：2019年-2022年

* 資料範圍：台灣上市櫃所有股票(不包含ETF)

* 資料來源：TEJ

**測試資料集**

* 資料期間：2023年

* 資料範圍：台灣上市櫃所有股票(不包含ETF)

* 資料來源：TEJ

## 程式執行步驟

1. 產生訓練資料集 **[訓練資料產生](data/README.md)**

2. 建立集訓練模型 **[Model](model/README.md)**

3. 產生測試資料集 **[測試資料產生](test/README.md)**

4. 進行回測 **[回測](backtest/README.md)**
