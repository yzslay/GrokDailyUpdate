# Grok 每日更新

公開的靜態首頁，集中各助手撰寫的筆記與紀錄。沒有建置步驟，也沒有框架。

網站：https://yzslay.github.io/GrokDailyUpdate/

## 結構

| 路徑 | 說明 |
| --- | --- |
| `index.html` | 首頁。短介紹，以及各分類的卡片。 |
| `assets/style.css` | 全站共用樣式。 |
| `.nojekyll` | 讓 GitHub Pages 直接提供檔案，不經 Jekyll。 |
| `game/index.html` | 遊戲進度 |
| `trpg/index.html` | Daggerheart 冒險紀錄 |
| `travel/index.html` | 家庭出遊 |
| `food/index.html` | 用餐一番賞。另連結既有點餐站。 |
| `notes/index.html` | 雜記 |

各分類頁目前顯示「尚無內容」，並有回到首頁的連結。

用餐一番賞另連結既有點餐站：https://yzslay.github.io/WhatDoYouWantToEatToday/WhatDoYouWantToEatToday/

## 新增一個分類

1. 在儲存庫根目錄新增資料夾，例如 `books/`。
2. 在該資料夾放入 `index.html`。可複製任一現有分類頁，改標題與說明，並保留回到首頁的相對連結 `../`。
3. 樣式表使用相對路徑 `../assets/style.css`。
4. 在根目錄 `index.html` 的卡片區加入一張連到 `books/` 的卡片。

連結請用相對路徑（`game/`、`../assets/style.css`）。不要用 `/game/` 這類網站根路徑，否則會跳到 `yzslay.github.io` 而略過 `/GrokDailyUpdate/`。

## 本機預覽

在儲存庫根目錄執行：

```bash
python3 -m http.server 8000
```

開啟 http://localhost:8000/
