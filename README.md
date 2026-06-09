# Studio Soom — 前端(GitHub Pages)

公開靜態網站。部署到 GitHub Pages 即可上線,不需編譯、不需後端伺服器。

## 頁面

| 路徑 | 說明 |
|------|------|
| `index.html` | 首頁(Hero、About Gyrotonic、About Studio、預約入口、Hours/Location) |
| `about-us.html` | 關於我們 / 總監介紹 |
| `about-gyrotonic.html` | 關於 Gyrotonic 方法 |
| `pricing.html` | 價格方案 / 套餐 |
| `contact.html` | 地址、電話、WhatsApp、Email、IG |
| `booking/index.html` | 線上預約系統 |
| `admin/index.html` | 管理員行程表(`noindex`,不公開連結) |
| `assets/styles.css` | 共用設計 token 與元件樣式 |

## 上線前一定要改

1. `booking/index.html` 與 `admin/index.html` 最上方的 `const API_URL = "..."` → 換成你的 Apps Script 部署網址。
2. 全站 placeholder 圖片(`picsum.photos` 灰階佔位)→ 換成 Studio Soom 自有照片。
3. 聯絡資訊、營業時間、地址等 → 換成正式內容。

詳見 `../gitlab/docs/setup-guide.md`。
