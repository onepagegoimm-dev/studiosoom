# 資安須知(Security)

完整規範:`one_page_go/gitlab/docs/security-standard.md`(範本庫)。

前端重點:**所有插入 `innerHTML` 的資料欄位都用 `esc()` 轉義**(已內含於 `booking/` 與 `admin/` 頁,
擋顧客輸入造成的後台儲存型 XSS)。改前端 → `git push` 才生效。
