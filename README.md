# 游婉彤 Grinz Yu｜作品集網站

純 HTML + CSS，不需要安裝任何東西，可以直接放上 GitHub Pages。

## 檔案說明

| 檔案 | 用途 |
|---|---|
| `index.html` | 網站內容（文字、圖片位置都在這裡） |
| `style.css` | 外觀（顏色、字型、間距） |
| `images/` | 放作品圖片 |

## 一、放上 GitHub（第一次）

1. 登入 GitHub，右上角 **+** → **New repository**
2. Repository name 輸入 `portfolio`（或 `你的帳號.github.io`，網址會更短）
3. 選 **Public**，按 **Create repository**
4. 進入新的 repository，點 **uploading an existing file**
5. 把 `index.html`、`style.css`、`README.md` 和 `images` 資料夾裡的檔案拖進去，按 **Commit changes**
6. 到 **Settings → Pages**，Source 選 **Deploy from a branch**，Branch 選 **main**、資料夾選 **/ (root)**，按 **Save**
7. 等 1～2 分鐘，頁面上方會出現你的網址：`https://你的帳號.github.io/portfolio/`

## 二、新增圖片

1. 把圖檔放進 `images/` 資料夾（建議檔名用英文與數字，例如 `tandem-1.png`）
2. 打開 `index.html`，搜尋 `class="gallery"`，每個專案標題下面都有一個
3. 把裡面註解的頭尾 `<!--` 和 `-->` 刪掉，改成你的檔名和說明
4. 想放更多張，就複製整段 `<figure>…</figure>` 往下貼

圖片小提醒：
- 單張建議 **1MB 以下**，網頁才不會慢（可用 squoosh.app 壓縮）
- `alt=""` 請寫簡短說明，視障者的閱讀器會讀出來
- 檔名大小寫要一致，`Photo.jpg` 和 `photo.jpg` 是不同檔案

## 三、修改文字

直接在 GitHub 上點 `index.html` → 右上角鉛筆圖示 → 修改 → **Commit changes**，約 1 分鐘後網站更新。

## 四、新增一個專案

複製 `index.html` 裡任一個 `<section id="…">…</section>`，貼在 `</main>` 前面，改掉 `id` 和內容；再到最上面的導覽列 `<header>` 加一個 `<a href="#新的id">名稱</a>`。

## 五、換顏色

打開 `style.css`，最前面的 `--yellow` 是主色，`--hl` 是螢光筆底色，改色碼即可。
