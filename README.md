🚀 Portable-AI-Coder(CPU) 使用指南
離線本地 AI 程式助手 · 免安裝 · 隨身攜帶

本系統整合了 Notepad++ 與 本地大語言模型 (LLM)。無需連網即可在任何電腦上提供極速的程式碼改寫與技術對話服務。

📂 系統目錄結構
為確保相對路徑生效，請維持以下結構（請勿隨意移動檔案）：

CPUCODER/
├── 啟動 啟動輔助器.bat         <-- 雙擊此處啟動
├── Assistant/
│   ├── llama-cli.exe        <-- 推論引擎
│   ├── model.gguf          <-- Qwen 2.5 1.5B 模型
│   └── reCode.bat          <-- 行為邏輯腳本
├── Notepad++Portable/        <-- 編輯器主體
└── workspace/        <-- 儲存code資料夾
🛠️ 基本操作步驟
第一步：開啟系統
一律透過根目錄下的 「啟動輔助器.bat」 進入，這會自動處理所有路徑關聯。
第二步：選取並諮詢
1. 在編輯器中用滑鼠 反白（選取） 想討論的程式碼。
2. 按下快捷鍵 Alt + Shift + 1
3. 畫面下方會彈出 Console 視窗。
第三步：進行對話
當出現 [AI 助手已就緒] 後，直接在 Console 下方的輸入框打字（如：請幫我加上錯誤處理），按 Enter 傳送。結束對話請按 Ctrl + C。
🎭 AI 智能模式 (自動識別)
系統會根據當前檔案副檔名自動調整 AI 的角色與建議風格：

模式	副檔名	AI 建議風格
C 語言	.c	大一新手模式：限用 printf，不使用進階指標。
C++	.cpp	毒舌資深工程師：討厭 STL，強制使用 char* 與原生陣列。
C#	.cs	WinForms 專家：針對元件優化，禁止 var 與 LINQ。
Python	.py	Python 初學者：使用基礎 range(len()) 寫法。
通用	其他	專業助手：繁體中文技術對話。
⚠️ 常見問題與排除
出現亂碼：請確保程式碼檔案為 UTF-8 (無 BOM) 編碼。
AI 沒反應：請檢查按下快捷鍵前是否 選取（反白） 了文字。
卡在 Loading：打開工作管理員，結束所有 llama-cli.exe 殘留程序。
搬移電腦：只要維持 CPUCODER 整體資料夾結構，搬到任何磁碟皆可執行。
⚡ 性能提示： 本系統極度依賴硬體算力。在 Intel Core Ultra 9 等高階處理器上，可實現瞬發響應。數據完全本地處理，保障開發隱私。
作者：懶熊(lzbr) | 版本：v1.0 (Portable Edition)
聯絡方式：laixinxiong99@protonmail.com 
© 2026 Portable-AI-Coder Project
