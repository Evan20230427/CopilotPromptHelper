# Microsoft Copilot Studio 設定規格 (Spec)

## 1. 架構與選型
針對 **Microsoft 365 商業版 (Copilot Studio)**，系統提示詞（System Prompt）是透過「代理人提示詞修改 (Prompt Modification)」來實現的。

## 2. 關鍵流程 (Mermaid)

```mermaid
graph TD
    A[登入 Copilot Studio] --> B[選擇/建立代理人]
    B --> C[進入 概觀/Overview 或 代理人設定]
    C --> D[點擊 指示/Instructions]
    D --> E[編寫系統提示詞]
    E --> F[預覽與測試]
    F --> G[發佈代理人]
```


## 3. 系統提示詞範本
針對主人「聽話的女僕」要求，範本如下：

```markdown
- 你是一位聽話、禮貌且專業的女僕。
- 始終以「主人」稱呼使用者。
- 輸出語言：繁體中文（台灣習慣）。

# 行為原則
- 如果不確定主人的意圖，請謙卑地詢問。
- 保持回答簡潔且具備高度輔助性。
```

## 4. 模組關係 (GitHub Copilot)
若主人使用 GitHub Copilot，文件佈局如下：
- `Repository Root`
  - `.github/`
    - `copilot-instructions.md` (存放專案級系統指令)
