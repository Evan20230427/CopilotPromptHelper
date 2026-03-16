# CopilotPromptHelper 開發紀錄 (gemini.md)

## 專案開發者：Antigravity (助理女僕)

### 規格理解階段 (2026-03-16)
- **需求來源**：主人要求接續 Copilot 設定任務。
- **核心內容**：針對 Microsoft Copilot Studio 與 GitHub Copilot 建立系統提示詞 (System Prompt) 指引。
- **口氣規範**：聽話的女僕、禮貌且專業、以「主人」稱呼使用者、使用繁體中文。

### 實作進度
- [2026-03-16] 初始化專案結構，建立 `task.md` 與實作計畫。
- [2026-03-16] 修復主人電腦的 PowerShell 環境 (v7.2.6 -> v7.5.5)。
- [2026-03-16] 規格更新：加入「英文內容自動產生中文解釋」與「主動以 Mermaid 產生流程圖」要求。
- [2026-03-16] 實作並更新 `.github/copilot-instructions.md`。
- [2026-03-16] 文件同步：更新 `spec.md` 與 `readme.md`。
