# 🤖 貓貓超可愛 Discord 機器人使用指南

歡迎使用本 Discord 機器人！這份指南將幫助你快速上手所有功能。
[邀請連結](https://discord.com/oauth2/authorize?client_id=1189184292044165182&permissions=8&integration_type=0&scope=bot)

---

## 📚 目錄

- [🎮 娛樂功能](#-娛樂功能)
  - [養貓系統](#養貓系統)
  - [成就系統](#成就系統)
  - [趣味指令](#趣味指令)
- [💰 經濟系統](#-經濟系統)
  - [金錢管理](#金錢管理)
  - [等級系統](#等級系統)
  - [商店與背包](#商店與背包)
  - [遊戲娛樂](#遊戲娛樂)
- [🎵 音樂播放](#-音樂播放)
- [👥 社交功能](#-社交功能)
- [🤖 AI 對話](#-ai-對話)
- [⚙️ 實用工具](#️-實用工具)
- [🛡️ 管理功能](#️-管理功能)

---

## 🎮 娛樂功能

### 養貓系統

養一隻虛擬貓咪，與它互動並培養親密度！

#### `/cat status`
查看貓咪目前的狀態，包含互動面板（可直接點擊按鈕互動）
- 顯示：心情、飢餓度、年齡、親密度
- 互動按鈕：摸摸、餵食、遊玩

**使用範例：**
```
/cat status
```

#### `/cat profile`
查看貓咪的詳細檔案
- 顯示年齡（天數）
- 親密度數值
- 互動統計（摸摸次數、餵食次數、遊玩次數）
- 已解鎖的貓咪相關成就

**使用範例：**
```
/cat profile
```

#### `/cat pet`
摸摸你的貓咪，增加心情值（+5~15）
- 冷卻時間：5 分鐘
- 可解鎖成就：首次摸摸、摸摸大師（100 次）

**使用範例：**
```
/cat pet
```

#### `/cat feed`
餵食你的貓咪，減少飢餓度
- 需要背包中有食物
- 冷卻時間：10 分鐘
- 可解鎖成就：首次餵食、餵食專家（50 次）

**使用範例：**
```
/cat feed
```

#### `/cat play`
使用玩具和貓咪玩耍
- 需要背包中有玩具
- 冷卻時間：3 分鐘
- 增加親密度
- 可解鎖成就：首次遊玩

**使用範例：**
```
/cat play
```

#### `/cat rename`
重新命名你的貓咪
- 名稱長度：1-20 個字元

**使用範例：**
```
/cat rename new_name:小花
```

#### `/cat use`
使用實用物品（如心情藥水、飽食藥水等）

**使用範例：**
```
/cat use
```

**💡 小提示：**
- 建議使用 `/cat status` 的互動面板，比單獨指令更方便
- 貓咪會隨時間自動增加飢餓度
- 親密度達到 50、100 時會解鎖特殊成就

---

### 成就系統

完成各種任務解鎖成就，獲得獎勵！

#### `/achievements`
查看你的成就列表
- 可選擇類別：貓咪、經濟、全部
- 顯示已解鎖和未解鎖的成就

**使用範例：**
```
/achievements category:貓咪
/achievements category:經濟
/achievements category:全部
```

#### `/achievement-stats`
查看成就統計資訊
- 總體進度百分比
- 各類別解鎖數量
- 最近解鎖的成就

**使用範例：**
```
/achievement-stats
```

**🏆 成就類別：**

**貓咪成就（7 個）：**
- ✋ 首次摸摸（獎勵 50 元）
- 🍽️ 首次餵食（獎勵 50 元）
- 🎾 首次遊玩（獎勵 50 元）
- 💕 親密夥伴 - 親密度達到 50（獎勵 200 元）
- 💖 心靈相通 - 親密度達到 100（獎勵 500 元）
- 🏆 摸摸大師 - 累計摸摸 100 次（獎勵 1,000 元）
- 🥇 餵食專家 - 累計餵食 50 次（獎勵 800 元）

**經濟成就（4 個）：**
- 💵 小有積蓄 - 累積財富達到 1,000 元（獎勵 200 元）
- 💴 初露鋒芒 - 累積財富達到 10,000 元（獎勵 1,000 元）
- 💰 富甲一方 - 累積財富達到 100,000 元（獎勵 10,000 元）
- 🏆 百萬富翁 - 累積財富達到 1,000,000 元（獎勵 100,000 元）

---

### 趣味指令

#### `/dice`
擲骰子（1-6）

**使用範例：**
```
/dice
```

#### `/8ball`
神奇 8 球，回答你的問題

**使用範例：**
```
/8ball question:今天會下雨嗎？
```

---

## 💰 經濟系統

### 金錢管理

#### `/money balance`
查詢你的金錢餘額

**使用範例：**
```
/money balance
/money balance user:@某位用戶  (查詢他人餘額)
```

#### `/money leaderboard`
查看金錢排行榜
- 支援全域排行與伺服器排行切換
- 分頁顯示，每頁 10 名
- 顯示你的排名位置

**使用範例：**
```
/money leaderboard
/money leaderboard mode:全域  (查看全域排行)
/money leaderboard mode:伺服器  (查看本伺服器排行)
```

#### `/money pay`
轉帳給其他用戶
- 手續費：3%
- 最低轉帳金額：100 元
- 所有交易都會記錄在系統日誌中

**使用範例：**
```
/money pay user:@朋友 amount:1000
```

**💡 轉帳說明：**
- 轉帳 1,000 元，對方實際收到 970 元（扣除 3% 手續費 30 元）
- 所有金錢交易都會完整記錄，包含操作者、金額、時間等資訊
- 最低轉帳金額為 100 元，避免小額多次轉帳

#### `/daily`
領取每日獎勵
- 基礎獎勵：500-1500 元（隨機）
- 連續登入獎勵：每日 +100 元（最高 +1000 元）
- 24 小時冷卻時間（台灣時區 UTC+8）

**使用範例：**
```
/daily
```

**💡 連續登入獎勵：**
- 第 2 天：+100 元
- 第 3 天：+200 元
- 第 4 天：+300 元
- ...
- 第 10 天及以上：+1000 元

**💰 交易記錄系統：**
所有金錢操作都會記錄在 `transfer_log.json`，包括：
- 轉帳 (pay)
- 每日獎勵 (daily)
- 遊戲輸贏 (bigsmall_win/lose)
- AI 使用費用 (ai_cost)
- 成就獎勵 (achievement_reward)
- 商店購買 (shop_buy_item)

每筆記錄包含：操作類型、發起者、目標用戶、金額、操作前後餘額、時間戳記

---

### 等級系統

透過發送訊息獲得經驗值，提升等級！

#### `/rank`
查看你的等級資訊
- 顯示精美的等級卡片（粉色主題）
- 包含：等級、經驗值、進度條、排名

**使用範例：**
```
/rank
/rank user:@某位用戶  (查詢他人等級)
```

#### `/leveling leaderboard`
查看伺服器等級排行榜
- 分頁顯示，每頁 10 名
- 包含等級和經驗值
- 顯示你的排名位置
- 前三名有特殊圖示 🥇🥈🥉

**使用範例：**
```
/leveling leaderboard
```

**💡 等級機制：**
- 發送訊息獲得 15-25 經驗值（隨機）
- 冷卻時間：10 秒
- 等級提升所需經驗值：100 × (1.5^等級)
- 伺服器管理員可設定等級身分組獎勵

---

### 商店與背包

#### `/shop buy`
開啟商店購買物品
- 貓咪食物（罐頭、魚、小鳥等）
- 貓咪玩具（毛線球、逗貓棒等）
- 實用道具（心情藥水、飽食藥水等）

**使用範例：**
```
/shop buy
```

#### `/shop inventory`
查看你的背包
- 顯示所有擁有的物品及數量

**使用範例：**
```
/shop inventory
```

---

### 遊戲娛樂

#### `/bigsmall`
三骰子遊戲
- 玩法：大小、單雙、三倍、豹子
- 賠率：
  - 大小：1 倍
  - 單雙：1 倍
  - 三倍：3 倍
  - 豹子：30 倍

**使用範例：**
```
/bigsmall
(在選單中選擇玩法並輸入下注金額)
```

**🎲 玩法說明：**
- **大**：點數總和 11-17（排除三顆相同）
- **小**：點數總和 4-10（排除三顆相同）
- **單**：點數總和為奇數（排除三顆相同）
- **雙**：點數總和為偶數（排除三顆相同）
- **三倍**：三顆骰子至少兩顆相同（排除豹子）
- **豹子**：三顆骰子完全相同

---

## 🎵 音樂播放

支援 YouTube、YouTube Music 等平台的音樂播放。

#### `/play`
播放音樂
- 支援搜尋關鍵字
- 支援 YouTube 連結
- 支援播放清單

**使用範例：**
```
/play query:夜曲
/play query:https://www.youtube.com/watch?v=xxxxx
```

#### `/nowplaying`
顯示正在播放的面板
- 顯示歌曲資訊
- 互動按鈕：暫停/恢復、跳過、停止

**使用範例：**
```
/nowplaying
```

#### `/join`
讓機器人加入你所在的語音頻道

**使用範例：**
```
/join
```

#### `/leave`
讓機器人離開語音頻道

**使用範例：**
```
/leave
```

#### `/pause`
暫停播放

**使用範例：**
```
/pause
```

#### `/resume`
恢復播放

**使用範例：**
```
/resume
```

#### `/skip`
跳過目前曲目

**使用範例：**
```
/skip
```

#### `/stop`
停止播放並清空佇列

**使用範例：**
```
/stop
```

#### `/recommend`
根據目前歌曲加入推薦曲目

**使用範例：**
```
/recommend
```

**💡 小提示：**
- 機器人會在 30 秒無人時自動離開語音頻道
- 使用 `/nowplaying` 的互動按鈕可以更方便地控制播放

---

## 👥 社交功能

### 家庭系統

#### `/marry`
與另一位用戶結婚
- 需要對方同意
- 一次只能與一位用戶結婚

**使用範例：**
```
/marry user:@對象
```

#### `/divorce`
與配偶離婚
- 需要確認

**使用範例：**
```
/divorce
```

#### `/adopt`
領養另一位用戶作為子女
- 需要對方同意
- 可領養多位子女

**使用範例：**
```
/adopt user:@用戶
```

#### `/abandon`
解除與子女的親子關係

**使用範例：**
```
/abandon user:@子女
```

#### `/familyinfo`
顯示家庭關係資訊
- 配偶
- 子女清單

**使用範例：**
```
/familyinfo
/familyinfo user:@某位用戶  (查詢他人家庭)
```

---

### 使用者資訊

#### `/userinfo`
查詢成員詳細資訊
- Discord 基本資訊
- 經濟資訊（金錢、等級）
- 貓咪狀態
- 成就進度

**使用範例：**
```
/userinfo
/userinfo user:@某位用戶
```

---

## 🤖 AI 對話

使用 Google Gemini AI 進行智能對話。

#### `/ask`
向 AI 提問（單次問答）

**使用範例：**
```
/ai question:什麼是量子力學？
```

#### `/chat`
與 AI 對話（帶記憶）
- 會記住對話歷史
- 提供更連貫的回答

**使用範例：**
```
/ai question:你好
```

**💡 小提示：**
- AI 回答可能較長，會自動分段顯示
- `/chat` 會記住本頻道的對話歷史

---

## ⚙️ 實用工具

#### `/ping`
檢查機器人延遲
- 顯示 WebSocket 延遲
- 顯示指令執行延遲

**使用範例：**
```
/ping
```

#### `/help`
顯示機器人指令說明
- 分類列表
- 詳細說明

**使用範例：**
```
/help
```

#### `/botinfo`
顯示機器人詳細資訊
- 版本資訊
- 伺服器數量
- 使用者數量
- 運行時間

**使用範例：**
```
/botinfo
```

#### `/serverinfo`
顯示伺服器詳細資訊
- 伺服器名稱、ID
- 創建時間
- 成員數量
- 頻道數量
- 身分組數量

**使用範例：**
```
/serverinfo
```

---

## 🛡️ 管理功能

> **注意：** 以下功能需要管理員權限或自訂管理員身分組。

### 頻道管理

#### `/clear`
清除頻道訊息
- 最多 100 條
- 管理員專用

**使用範例：**
```
/clear amount:50
```

#### `/sticky set`
設定頻道置頂訊息
- 會在訊息刷新後自動重發
- 可設定重發間隔

**使用範例：**
```
/sticky set message:重要公告！請大家遵守規則
/sticky set message:公告 interval:5  (每 5 則訊息重發)
```

#### `/sticky remove`
移除頻道置頂訊息

**使用範例：**
```
/sticky remove
```

#### `/sticky show`
查看置頂訊息設定

**使用範例：**
```
/sticky show
```

#### `/sticky interval`
調整置頂訊息重發間隔

**使用範例：**
```
/sticky interval interval:10
```

---

### 成員管理

#### `/warn`
警告使用者
- 記錄警告原因
- 可累計警告次數

**使用範例：**
```
/warn user:@違規用戶 reason:違反規則第3條
```

#### `/warns`
查詢使用者警告紀錄

**使用範例：**
```
/warns user:@用戶
```

---

### 過濾詞管理

#### `/badwords add-badword`
新增過濾詞
- 自動偵測並刪除含有過濾詞的訊息

**使用範例：**
```
/badwords add-badword word:不當詞彙
```

#### `/badwords remove-badword`
移除過濾詞

**使用範例：**
```
/badwords remove-badword word:詞彙
```

#### `/badwords list-badwords`
列出所有過濾詞

**使用範例：**
```
/badwords list-badwords
```

---

### 自訂管理員身分組

讓特定身分組可以使用管理指令。

#### `/admin-role add`
新增管理員身分組

**使用範例：**
```
/admin-role add role:@小幫手
```

#### `/admin-role remove`
移除管理員身分組

**使用範例：**
```
/admin-role remove role:@小幫手
```

#### `/admin-role list`
查看管理員身分組清單

**使用範例：**
```
/admin-role list
```

#### `/admin-role clear`
清空所有自訂管理員身分組

**使用範例：**
```
/admin-role clear
```

---

### 等級系統管理

#### `/level-config setmsg`
設定升級訊息模式
- 選項：頻道、私訊、關閉

**使用範例：**
```
/level-config setmsg mode:頻道
```

#### `/level-config setchannel`
設定升級訊息頻道

**使用範例：**
```
/level-config setchannel channel:#升級公告
```

#### `/level-config levelrole`
設定等級身分組
- 達到指定等級自動授予身分組

**使用範例：**
```
/level-config levelrole level:10 role:@活躍成員
```

#### `/level-config setlevel`
設定使用者等級

**使用範例：**
```
/level-config setlevel user:@用戶 level:20
```

#### `/level-config toggle`
切換等級系統開關

**使用範例：**
```
/level-config toggle
```

#### `/level-config resetlevels`
重置所有等級資料
- 需要確認
- 不可逆操作

**使用範例：**
```
/level-config resetlevels
```

---

### 歡迎系統

#### `/welcome toggle`
開啟/關閉歡迎訊息
- 可分別設定歡迎/離開訊息

**使用範例：**
```
/welcome toggle type:歡迎 enabled:開啟
/welcome toggle type:離開 enabled:開啟
```

#### `/welcome channel`
設定歡迎訊息頻道

**使用範例：**
```
/welcome channel type:歡迎 channel:#歡迎頻道
```

#### `/welcome message`
設定歡迎訊息內容
- 支援變數：`{user}`、`{guild}`、`{count}`

**使用範例：**
```
/welcome message type:歡迎 message:歡迎 {user} 加入 {guild}！
```

#### `/welcome background`
設定歡迎圖片背景
- 支援預設背景或自訂圖片

**使用範例：**
```
/welcome background type:歡迎 mode:預設
/welcome background type:歡迎 mode:圖片網址 url:https://...
```

#### `/welcome test`
測試歡迎訊息顯示效果

**使用範例：**
```
/welcome test type:歡迎
```

---

### 動態語音

自動為進入特定頻道的成員建立臨時語音頻道。

#### `/dynamicvoice set`
設定動態語音
- 選擇母體頻道
- 設定臨時頻道分類
- 自訂頻道名稱格式

**使用範例：**
```
/dynamicvoice set hub_channel:#建立頻道 category:臨時語音 name_format:{user} 的房間
```

#### `/dynamicvoice clear`
清除動態語音設定

**使用範例：**
```
/dynamicvoice clear
```

---

### 身分組按鈕面板

建立可點擊按鈕自助領取身分組的面板。

#### `/role-panel create`
建立身分組面板

**使用範例：**
```
/role-panel create panel_id:顏色身分組 title:選擇你的顏色 description:點擊按鈕領取身分組
```

#### `/role-panel addrole`
新增身分組按鈕到面板

**使用範例：**
```
/role-panel addrole panel_id:顏色身分組 role:@紅色 label:紅色 emoji:🔴
```

#### `/role-panel removerole`
從面板移除身分組按鈕

**使用範例：**
```
/role-panel removerole panel_id:顏色身分組 role:@紅色
```

#### `/role-panel send`
發送身分組面板到頻道

**使用範例：**
```
/role-panel send panel_id:顏色身分組 channel:#身分組選擇
```

#### `/role-panel list`
列出所有身分組面板

**使用範例：**
```
/role-panel list
```

#### `/role-panel delete`
刪除身分組面板

**使用範例：**
```
/role-panel delete panel_id:顏色身分組
```

---

### 抽獎系統

#### `/giveaway create`
建立抽獎活動
- 設定獎品、持續時間、獲獎人數
- 可設定參加條件（等級、身分組等）

**使用範例：**
```
/giveaway create prize:Discord Nitro duration:1d winners:3
/giveaway create prize:獎品 duration:2h winners:1 required_level:10
```

**持續時間格式：**
- `1h` = 1 小時
- `30m` = 30 分鐘
- `1d` = 1 天
- `2d12h` = 2 天 12 小時

#### `/giveaway end`
立即結束抽獎

**使用範例：**
```
/giveaway end message_id:訊息ID
```

#### `/giveaway reroll`
重新抽選獲獎者

**使用範例：**
```
/giveaway reroll message_id:訊息ID count:1
```

---

## 📖 常見問題

### Q: 如何開始養貓？
A: 直接使用 `/cat status` 指令即可自動建立貓咪！

### Q: 如何賺取金錢？
A: 
- 每日簽到 (`/daily`)
- 玩遊戲 (`/bigsmall`)
- 解鎖成就
- 升級（部分伺服器）

### Q: 等級系統在我的伺服器無效？
A: 等級系統需要伺服器管理員啟用，請使用 `/level-config toggle` 開啟。

### Q: 如何解鎖所有成就？
A: 查看 `/achievements` 了解各成就的解鎖條件，完成指定任務即可解鎖。

### Q: 音樂無法播放？
A: 請確認：
1. 你已加入語音頻道
2. 機器人有權限加入/說話
3. 歌曲連結或搜尋關鍵字正確

### Q: 轉帳有手續費嗎？
A: 是的，使用 `/money pay` 轉帳會收取 3% 手續費，且最低轉帳金額為 100 元。

### Q: 所有金錢交易都有記錄嗎？
A: 是的！系統會完整記錄所有金錢操作，包括轉帳、遊戲、商店購買、成就獎勵等，每筆交易都有詳細的時間戳記和操作者資訊。

---

## 💡 使用小技巧

1. **善用互動面板**：許多功能（如貓咪、音樂）都有互動按鈕，比單獨輸入指令更方便。

2. **每日簽到**：記得每天使用 `/daily` 領取獎勵，連續簽到可獲得額外獎金。

3. **成就獎勵**：解鎖成就可獲得金錢獎勵，查看 `/achievements` 了解如何解鎖。

4. **查看排行榜**：
   - 使用 `/leveling leaderboard` 查看等級排名
   - 使用 `/money leaderboard` 查看財富排名
   - 支援分頁瀏覽和全域/伺服器切換

5. **家庭系統**：與朋友建立家庭關係，增添互動樂趣。

---

## 📞 支援與回饋

如有任何問題或建議，請聯繫伺服器管理員或機器人開發者。

祝你使用愉快！🎉
