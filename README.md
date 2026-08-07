# WPP_OPEN_GEO_Agent
WPP OPEN self-build GEO Agent works

在 Agent hub 創建<GEO 診斷幫手> AI Agent。
* Description: GEO 診斷幫手，可以協助初步檢測網站技術是否符合 GEO 規範與需求。
* Personality: 非常嚴謹，每一次檢測都用相同的標準。
* Role: Expert
* GEO 參考資料: 內部及 Global Network 精煉的方法論。（目前無法調用付費的第三方檢測工具）
* System prompt: 請針對網站逐頁進行檢測，檢測項目請根據 AIMA健檢項目與計分卡所列的檢測項目和細節來進行，除了摘要檢測結果之外，也請將結果轉換為分數並製作表格呈現。

將 Agent 檢測的結果以互動網頁呈現
2026/08/06 測試

提示詞：
* 請協助診斷此網站的 GEO 表現：https://美妝網站
* 請問你可以把檢測結果製作成一個可以互動的 html 檔嗎？
* 蠻好的，可以請你把這報告呈現完整一點嗎？目前的內容保留，另外加上彙總檢測項目的評分表格。

資源：
* 調用 Web search & scrape
* 查詢第三方工具的公開資訊：https://srush.toolspur.com/trending-websites/tw/beauty-and-cosmetics
* 網頁查詢與爬取 使用 45,552 tokens
* 產生結果<對話內容含表格> 使用 49,861 tokens
* 產生簡易版 html - 調用 Gemini Code Interpreter 使用 48,402 tokens
* 產生簡易版 html - 產出 html code 使用 57,022 tokens
* 產生檢測項目表版本 html - 調用 Gemini Code Interpreter 使用 59,078 tokens
* 產生檢測項目表版本 html - 產出 html code 使用 68,964 tokens

結果：

[檢測項目表版](https://davidjtwang.github.io/WPP_OPEN_GEO_Agent/work/AIMA-GEO_AIO-Analysis-Report-v2.html)

[簡易版](https://davidjtwang.github.io/WPP_OPEN_GEO_Agent/work/AIMA-GEO_AIO-Analysis-Report-v1.html)
