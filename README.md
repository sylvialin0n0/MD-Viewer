# MD Viewer

一個純前端、免安裝的 Markdown 檔案瀏覽與編輯工具。只需用瀏覽器開啟，即可拖拉 `.md` / `.yaml` 檔案或整個資料夾來瀏覽與編輯。

## 功能

- **拖拉匯入** — 支援單一檔案、多檔案、整個資料夾
- **樹狀側欄** — 資料夾結構可展開收合，快速切換檔案
- **Markdown 渲染** — 支援 GFM（表格、checkbox、程式碼高亮）
- **即時編輯** — 點選「編輯」進入 Rich Text 模式，工具列支援標題、粗體、清單、引用、連結等
- **儲存** — 透過 File System Access API 直接寫回原始檔案，或下載為新檔案
- **跨 session 還原** — 重新整理頁面後自動還原上次載入的檔案（同一 session），或點選「↩ 還原上次的檔案」重新授權
- **YAML 預覽** — `.yaml` / `.yml` 檔案以程式碼區塊顯示
- **可調整側欄寬度** — 拖拉分隔線調整

## 使用方式

1. 用瀏覽器開啟 `MD-Viewer.html`（或前往線上版）
2. 將 `.md` 檔案或資料夾拖拉至左側區域，或點選「+ 檔案」／「+ 資料夾」
3. 點選側欄中的檔案即可預覽
4. 點選右上角「編輯」進入編輯模式，完成後按「儲存」


## 技術

- 純 HTML / CSS / JavaScript，無需任何框架或後端
- [marked.js](https://marked.js.org/) — Markdown 解析
- [highlight.js](https://highlightjs.org/) — 程式碼高亮
- [Turndown](https://github.com/mixmark-io/turndown) — HTML 轉 Markdown（儲存時使用）
- File System Access API — 直接讀寫本機檔案
- IndexedDB — 跨 session 記憶載入過的檔案

## 瀏覽器支援

建議使用 **Chrome** 或 **Edge**（需支援 File System Access API）。Safari 可瀏覽但部分功能（直接儲存、跨 session 還原）不支援。

## 作者

Built by Sylvia Lin, 2026
