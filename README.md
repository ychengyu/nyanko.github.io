# Nyanko-Sama Portfolio

可直接部署至 GitHub Pages 的純靜態單頁作品集，使用 HTML、CSS、JavaScript，不需建置工具、後端、API 金鑰或付費服務。

## 專案內容

- 首頁主視覺、品牌定位與作品導覽
- 經來源核對的個人簡介
- 3 件 Pixiv / YouTube 對應 MMD 作品
- 官方 YouTube 精選影片入口
- 已確認的主要社群連結
- 響應式導覽、櫻花動畫、捲動顯示效果
- 鍵盤焦點、跳至內容、語意化標記與 reduced-motion 支援
- 圖片 lazy loading、固定比例與載入失敗占位

## 本機預覽

直接開啟 `index.html` 即可。建議在專案資料夾執行：

```bash
python -m http.server 8000
```

再開啟 `http://localhost:8000/`。

## 部署至 GitHub Pages

1. 在 GitHub 建立新的公開儲存庫。
2. 將本專案根目錄內的 `index.html`、`style.css`、`script.js`、`README.md` 上傳至預設分支根目錄。
3. 開啟儲存庫的 **Settings → Pages**。
4. **Build and deployment** 選擇 **Deploy from a branch**。
5. Branch 選預設分支（通常為 `main`），資料夾選 `/ (root)`，按 **Save**。
6. 等候 GitHub 顯示網站網址。所有站內資源均使用 `./` 相對路徑，可部署於專案子路徑。

## 來源與素材策略

- 個人資料與社群：Lit.link、Pixiv 公開個人頁。
- 作品標題及作者：各 Pixiv 作品頁，並連回原作品。
- 影片與縮圖：官方 YouTube 頻道及影片網址。縮圖使用 YouTube 遠端網址，不納入本專案、不重新託管。
- 裝飾視覺均由 CSS 繪製，專案沒有第三方角色圖片、模型、音樂或字型檔；字型若無法連線會回退至系統字型。
- Pixiv 原圖因平台存取與授權限制未下載、未重託管。若遠端縮圖失效，卡片仍保留標題、占位與 Pixiv / YouTube 入口。

## 維護

替換作品時，請同步核對 Pixiv 作者頁、作品網址、YouTube 頻道歸屬與影片 ID。請勿把無授權內容加入 `assets` 或重新託管。
