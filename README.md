# kenjiong-japan-trip-2027

日本中部・關西家族旅行 2027 規劃網站的 source authority。

- **Live 網站**：https://kenjiong-japan-trip-2027.pages.dev
- **內容**：7 天 6 夜家庭旅行行程（名古屋 → 白川鄉 → 高山 → 大阪），2027/1/20（三）出發
- **語言**：繁體中文

## 檔案

| 檔案 | 說明 |
|---|---|
| `index.html` | 網站本體，單檔自帶 CSS/JS，無外部相依 |
| `AI_CONTENT.md` | 供 AI 讀取的結構化行程內容（不含任何私人資訊） |
| `.source_provenance.json` | source 與線上版本的位元組等價證據 |

## Source 等價性

`index.html` 經 SHA256 驗證與線上 production 版本**位元組完全相同**
（33159 bytes / `8db30abaac189d99f...`）。這個 repo 是該線上版本的 source authority：
改這個 repo 的 `index.html` 就代表改線上內容，部署請走
`~/.hermes/scripts/deploy-pages.sh`（Cloudflare Pages 治理流程）。

## 隱私

本 repo 刻意**不收錄**任何下列資料：訂位碼／訂房確認碼、機票票號、護照或身分證號碼、
信用卡號、帳號密碼、API token、個人 email 或手機號碼。

內容中出現的 `0577-35-1300` 是 KOKO HOTEL 飛驨高山的**公開商家聯絡電話**（公開旅遊資訊），
`1900` 是日本旅客服務電話代碼，兩者皆非個人資料。

## 維護

- 行程內容由人（建智大人）維護，網站為靜態產物。
- 任何 production deploy 必須先通過 registry gate
  （`ACTIVE` + `LINKED` + `ai_readable_paths` 非空），否則 fail closed。

行程檔最後更新：2026-08-09
