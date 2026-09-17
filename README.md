# Favicon Generator

一個單一 HTML 檔案的 favicon / PWA 圖示產生器。跟大多數線上工具不同，你可以**自由勾選要輸出的尺寸**，而不是被強迫產生一包「涵蓋所有尺寸」的檔案。

**不需要安裝任何東西** — 沒有 Node.js、沒有 Python、沒有套件相依。下載後直接用瀏覽器打開 `favicon-generator.html` 就能用，在 Mac、Windows、Linux 上都一樣。

This HTML took me 5 minutes with Claude to generate. With just a single prompt.

Serves me better than any other favicon generation webpage.

Hope it serves you well! 

## 特色

- 依用途分類勾選尺寸：瀏覽器 Favicon／Apple・iOS／Android・PWA／Windows 磁貼／高解析度，也可以一鍵全選
- 自動產生多尺寸 `favicon.ico`
- 自動產生 `manifest-icons-snippet.json`（可貼進 PWA 的 `manifest.json`）與 `html-snippet.txt`（可貼進 `<head>`）
- 非正方形來源圖片會自動置中、補透明邊，不會被拉伸變形
- 所有運算（縮圖、打包 zip、封裝 ico）都在瀏覽器本機端完成，圖片不會被上傳到任何伺服器
- 純 Vanilla JavaScript，zip／ico 封裝邏輯是自己手刻的最小實作，沒有任何外部函式庫或 CDN 依賴

## 使用方式

1. 下載 [`favicon-generator.html`](./favicon-generator.html)
2. 用瀏覽器打開它（雙擊即可）
3. 選擇來源圖片（建議正方形、至少 512×512 以上的 PNG）
4. 勾選要輸出的尺寸
5. 按「產生並下載 ZIP」，取得包含所有 PNG、`favicon.ico`、manifest／HTML 片段的 `favicons.zip`

## 授權

[MIT License](./LICENSE)

歡迎發 Issue 或 PR。
