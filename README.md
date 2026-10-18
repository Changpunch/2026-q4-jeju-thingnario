# 濟州員旅 2026/11/6–11/8（8 人）

投票頁：https://claude.ai/artifact/JFBz6sJYosi9fLTK1FG7Lq
行程網頁「敢不敢去濟州島打醫美」：單檔 index.html（含 Naver 地圖截圖底圖），發佈在 GitHub Pages（Public repo）。
結構：交通住宿（機票／住宿／租車）｜無腦跟玩（旅遊大地圖／行程詳情）｜自己帶腦（出發前須知）｜分帳（明細／結算）。

## 網頁維護
- 未加密原始檔：claude/jeju-site-source.html（改內容改這份，已含 Apps Script 網址）
- 上傳到 GitHub 的是 StatiCrypt 3.5.4 加密版：`npx staticrypt@3.5.4 index.html -p <密碼> --short --remember 30 --salt de53ed50bee302c5063dc45f43b5baf4`，中文提示文字＋橘色 #E26A1F；加密後在 <head> 補 `<meta name="robots" content="noindex,nofollow">`
- 沿用同一個 salt，大家勾過「記住我」就不用重新輸入；密碼由 Sonia 保管

## 分帳
- 後端：Google Apps Script（claude/jeju-expense-apps-script.gs），綁在行程試算表，只讀寫「Expenses-明細」「Expense-設定」分頁；API token 寫在 script 和網頁裡
- 10/18 已部署：https://script.google.com/macros/s/AKfycbxe1q2E9F2XdR5wRaBiSdyPAQtPuDvMwlCfVr9ZLG2j3aCrCH3vvXkpPOD6NCTrs4le/exec（勿外流）
- 改 Apps Script 程式後要「部署 → 管理部署作業 → 編輯 → 版本：新版本」，網址才會維持不變
- 明細欄位：日期｜項目｜幣值｜總花費｜墊付人｜攤分人｜類型（支出/還款，取代原本的「是否已收款」）｜備註｜ID
- 有網頁密碼的人都能新增、修改、刪除；KRW 依「Expense-設定」B1 的固定匯率換成台幣後一起結算；還款會記成類型＝還款的一筆
- 名字：試算表用 WT，網頁顯示 Wanting

## 基本資訊
- 去 11/6 Jin Air LJ942 TPE T1 02:45 → CJU 06:05（01:00 桃園集合）；回 11/8 LJ941 CJU 22:15 → TPE T1 23:45
- 行李：託運 15kg、手提 1 件 10kg、個人物品 1 件
- 租車（KLOOK）The Safe Rent A Car，제주시 용문로 36，營業 07:00–22:00；現代 Staria 2024 9 人座（行李標示 3 件）
  - 取車 11/6 07:00、還車 11/8 20:00；接駁：入境 5 號門 → 過馬路右轉 → 租車接駁停車場 4 區 3 號線，每 20 分一班
  - 駕駛：護照＋台灣駕照正本＋紙本 IDP；26 歲以上、駕齡 1 年以上；已加購多人駕駛
  - 押金：主駕駛實體信用卡預授權約 ₩300,000；等量取還油；加強保障自負額 0（不含玻璃/底盤/輪胎/車頂）
- 住：Airbnb Sogobae Summer（Summer's House），機場 5 分鐘，3 房 10 床 3 衛；入住 16:00、退房 10:00
- 行程以 Google Sheet「261106-261108 Jeju Island 三天兩夜遊」Schedule 分頁為準
  - 10/18 Day 2 整體提早：09:20 出門、09:30 鹽工廠、11:00 楓葉、12:00 滿足の商會（Sonia 會去改訂位）、13:45 Osulloc、15:30 9.81 Park、17:20 夕陽、19:05 醬蟹
- 11/8：10:00 退房後自由活動（醫美團找 Alice、逛街團找 Sonia），中午／晚餐是否集合留到行前會討論
- 慧景科技贊助每人 NT$2,000

## 注意
- Google Sheet Basic Info 分頁含護照資料，勿公開分享；網頁不放訂位代號、機票號碼、KLOOK 確認編號與個人聯絡資料
