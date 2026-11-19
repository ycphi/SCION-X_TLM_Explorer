# SCION-X TLM Explorer 2.10

SCION-X Telemetry Mapping, SatNOGS Incremental Download and Decoding Tools

Windows 64 位元遙測繪圖與資料更新工具。支援 SatNOGS OGG、捷克地面站 CS16 與 NCU_OC BIN ver1。

## 下載

- [Windows 安裝包](dist/installer/SCIONX_TLM_Setup.exe?raw=true)。首次安裝需連網下載 MATLAB Runtime R2026a。
- [可攜 ZIP](dist/SCIONX_TLM_Explorer_Portable.zip?raw=true)。完整解壓後執行 `SCIONX_TLM_Explorer.exe`，目標電腦需先安裝 MATLAB Runtime R2026a。
- [SHA-256 檢查碼](dist/SHA256SUMS.json)。

兩種套件均包含初始遙測 Excel、各來源 manifest 與兩份 PDF。

## 文件

- [程式設計流程圖](dist/docs/SCION-X_TLM_程式設計流程圖.pdf)說明三種來源、解碼、合併、備份及復原流程。
- [GUI 使用手冊](dist/docs/SCION-X_TLM_GUI_使用手冊.pdf)以實際操作畫面說明繪圖、篩選、匯出和來源更新。

## 資料更新

安裝後可直接使用套件內的 `data`。本儲存庫的 `data` 與 2.10 套件使用同一份初始資料，包含 `SCX_Filter_TLM.xlsx` 及 `sources` 中各來源的 Excel、manifest 與索引。

首次使用 SatNOGS 更新時，在「更新繪圖參數來源」設定 URL 及自己的 API Key。本機 CS16／BIN 更新使用指定的錄音源頭。完成更新後，程式會清除已入庫的本機暫存。更新視窗列出查詢、下載、解碼及合併耗時，並顯示 Excel 的封包欄位用量。
