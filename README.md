# build-live-event-raffle

一份給 coding agent 的 Skill：幫婚禮、meetup 或小型活動搭一個「掃碼加入、手機加油、投影揭曉、主持人控場」的現場抽獎網站。

來自 DevDay Exchange Taipei 分享〈自己的婚禮自己寫〉（DinDin，2026-11-18）。

## 怎麼用

1. 下載這個 repo（Code → Download ZIP），或 `git clone https://github.com/peter6601/build-live-event-raffle`
2. 把 `build-live-event-raffle/` 資料夾放進你專案的 skills 目錄
   - Codex：`.agents/skills/`
   - Claude Code：`.claude/skills/`
3. 對你的 coding agent 說：「用 build-live-event-raffle 做一個掃碼加入的活動抽獎網站」

不想裝也可以：直接把 [`SKILL.md`](build-live-event-raffle/SKILL.md) 的內容貼給 agent。

## 它會幫你做什麼

- 三個頁面：手機前台（賓客）、大螢幕前台（投影）、後台（主持人）
- 沒有現成專案時的預設組合：純 HTML 前端放 Vercel、Supabase 資料庫函式當後端、本機 PGlite 彩排，全部在免費方案內
- 伺服器決定計票與加權抽獎，動畫只負責表演
- 一套彩排清單：重送、刷新、斷線、缺席補抽
