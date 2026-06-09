# Studio Soom — 前端(GitHub Pages)

公開靜態網站。部署到 GitHub Pages 即可上線。
**範圍:首頁(形象 + 單堂/套餐方案)+ 預約系統 + 管理後台**。客戶原站(studiosoom.co.uk)放一個連結連到首頁即可。

## 網址(GitHub Pages 啟用後)

| 用途 | 網址 |
|------|------|
| **首頁(對外入口)** | <https://onepagegoimm-dev.github.io/studiosoom/> |
| 線上預約 | <https://onepagegoimm-dev.github.io/studiosoom/booking/> |
| 管理員行程表(不公開) | <https://onepagegoimm-dev.github.io/studiosoom/admin/> |

## 頁面

| 路徑 | 說明 |
|------|------|
| `index.html` | 首頁:品牌形象 + 單堂(Services)/ 套餐(PackageProducts)方案展示,動態讀取 |
| `booking/index.html` | 線上預約系統(登入、套餐/剩餘次數、預約、取消/改期、24h 規則) |
| `admin/index.html` | 管理員行程表(`noindex`,不公開連結) |

> `booking` 與 `admin` 為自包含單檔(樣式、程式都內嵌),不依賴任何共用 assets。

## 上線重點

1. `booking/index.html` 與 `admin/index.html` 的 `API_URL` 已填入正式 Apps Script 部署網址。
2. **原站加入口**:在 studiosoom.co.uk 放一個「Book」按鈕,連到 `https://<帳號>.github.io/studiosoom/booking/`。
3. 兩頁左上的返回連結已指向客戶原站 `https://studiosoom.co.uk/`。
4. 後台(`admin/`)新增 Services、批次產生 Time slots、為顧客建立 Packages。

詳見 `../gitlab/docs/setup-guide.md`。
