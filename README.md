# 大同大學博士班設計學特論工作營（2026-11-16）學員學習單

學員頁：https://scatjay.github.io/ttu-claude/

- 入口頁（QR、登入）：`index.html`　學習單：`sheet.html`（登入後才進得去，未登入會導回入口）
- 講師後台：https://scatjay.github.io/ttu-claude/admin.html （進頁要求 Google 登入；只有講師白名單帳號讀得到資料，網頁本身不含任何學員資料）

講師版、學員名單、金鑰都不在這個倉庫。

## 運作方式
- 學員用 Google 登入（名單內的 Gmail 才能使用助教與記錄進度）。
- 助教的提問寫進 Firebase 資料庫，由講師電腦上的程式呼叫 Gemini 後寫回答案；答完即刪除提問全文，只留次數與字數。

## 會後關閉（擇一，最少做第 1 項）
1. 停用 Pages：GitHub → 本倉庫 Settings → Pages → Source 選 None（網址立即失效）。
2. 把倉庫設為私人：Settings → General → Danger Zone → Change visibility → Private。
3. 資料庫：由講師清掉 `dt1116/DT-20261116` 節點，並從規則移除 `dt1116`。
