如果是用邏輯來判斷是否是ai產生的code，要規避就不能用這個（廢棄掉



🚀 Portable-AI-Coder (CPU) 使用指南

離線本地 AI 程式助手 · 免安裝 · 隨身攜帶
📖 簡介與安裝建議

本系統為 Windows 環境整合了 Notepad++ 與 本地大語言模型 (LLM)。無需連網即可在任何電腦上提供極速的程式碼改寫與對話服務。

    💡 建議用法：
    下載後存入 USB (建議容量 ≥ 4GB)，至學校電腦插入後，務必複製進 C 槽 (C:\) 解壓縮使用 以獲得最佳效能。

📂 系統目錄結構

請維持以下結構以確保相對路徑生效，請勿隨意移動檔案：
Plaintext

CPUCODER/
├── 啟動輔助器.bat        <-- 雙擊此處啟動系統 (自動處理路徑)
├── Assistant/
│   ├── llama-cli.exe    <-- AI 推論引擎
│   ├── model.gguf       <-- Qwen 2.5 1.5B 權重模型
│   └── reCode.bat       <-- 行為邏輯腳本
├── Notepad++Portable/   <-- 編輯器主體
└── workspace/           <-- 預設程式碼儲存資料夾

🛠️ 基本操作步驟

    開啟系統：一律透過根目錄下的 「啟動輔助器.bat」 進入。

    選取並諮詢：

        在編輯器中用滑鼠 反白（選取） 想討論的程式碼段落。

        按下快捷鍵 Alt + Ctrl + 1。

    進行對話：

        下方 Console 出現 [AI 助手已就緒] 後，直接在輸入框打字（如：請幫我加上錯誤處理）。

        按 Enter 傳送需求；結束對話請按 Ctrl + C。

🤖 AI 智能模式（自動識別）

系統會根據檔案副檔名自動調整 AI 的角色與風格：
模式	副檔名	AI 建議風格
C 語言	.c	大一新手：限用 printf，不使用進階指標。
C++	.cpp	毒舌資深工程師：討厭 STL，強制使用 char* 原生陣列。
C#	.cs	WinForms 專家：針對元件優化，禁止 var 與 LINQ。
Python	.py	Python 初學者：使用基礎 range(len()) 寫法。
通用	其他	專業助手：繁體中文技術對話。
⚠️ 常見問題排除

    出現亂碼：請確保程式碼檔案為 UTF-8 (無 BOM) 編碼。

    AI 沒反應：請檢查按下快捷鍵前，是否已 選取（反白） 文字。

    卡在 Loading：打開工作管理員，結束所有 llama-cli.exe 殘留程序。

    搬移電腦：只要維持 CPUCODER 整體資料夾結構，搬到任何磁碟皆可執行。

⚡ 性能與隱私提示

    極速響應：本系統極度依賴硬體算力。在 Intel Core Ultra 9 等高階處理器上，可實現瞬發響應。

    絕對隱私：所有數據完全在本地處理，保障開發隱私。

作者：懶熊 (lzbr) | 版本：v1.0 (Portable Edition)

聯繫方式：laixinxiong99@protonmail.com

© 2026 Portable-AI-Coder Project
