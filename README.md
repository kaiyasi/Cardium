# Cardium - 個人資料卡生成與展示平台

> **由 Serelix Studio 開發的多平台個人檔案整合工具，讓你的數位身份更有型。**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Build](https://img.shields.io/badge/build-passing-brightgreen.svg)]()
[![Docker](https://img.shields.io/badge/docker-ready-%230db7ed.svg?style=flat\&logo=docker\&logoColor=white)](https://www.docker.com/)
[![Version](https://img.shields.io/badge/version-0.1--alpha-blue.svg)]()

---

## 💡 專案概念 | Project Overview

**Cardium** 是一款致力於打造「數位名片新形態」的應用。
在這個資訊過載的時代，每個人都有多個平台帳號、專案連結與作品展示頁，而 Cardium 讓你能在同一張互動式卡片中呈現個人風格與專業形象。

**你可以：**

* ✨ 建立屬於自己的個人檔案卡片（支援多語與主題自訂）
* 🌐 整合社群帳號、GitHub、Discord、Instagram、ForumKit 個人頁等
* 🔗 一鍵生成公開連結（cardium.serelix.xyz/@username）
* 🪄 使用 API 或嵌入代碼將卡片整合到網站、部落格、Discord Bot
* 📊 內建統計與互動資料分析（瀏覽次數、連結點擊來源等）

Cardium 不只是展示，更是「你的數位身份中樞」。

---

## 🧩 系統架構 | System Design (預計規劃)

```
Cardium/
├── 📁 core/              # 主應用程式與 API
│   ├── auth/             # 使用者登入與驗證模組
│   ├── profile/          # 個人卡片生成邏輯
│   └── analytics/        # 瀏覽與互動統計
├── 🌐 web/               # 前端展示平台 (Next.js + Tailwind)
├── 🧠 docs/              # 開發文檔（即將推出）
├── 🐳 docker/            # Docker 環境設定
└── ⚙️ tests/             # 自動化測試模組
```

* 後端：FastAPI + PostgreSQL
* 前端：Next.js + Tailwind + ShadCN UI
* 容器：Docker + Nginx（統一使用內部 port 80）
* 認證：JWT-based Auth（支援 Serelix SSO 整合）
* 通訊：Socket.IO (即時卡片互動事件)

---

## 🧭 使用情境 | Use Cases

| 使用情境              | 功能展示                        |
| ----------------- | --------------------------- |
| 🧑‍💻 學生/開發者個人頁   | 展示專案連結、技術堆疊與社群帳號            |
| 🎨 設計師名片          | 加入 Behance、IG、作品集、配色主題      |
| 💬 校園社群           | 結合 ForumKit 讓使用者能點擊名片查看發文紀錄 |
| 🤖 Discord Bot 整合 | 使用 `/card @user` 直接顯示使用者卡片  |

---

## 📅 專案進度 | Development Status

| 階段                                 | 說明         |
| ---------------------------------- | ---------- |
| ✅ 概念與資料架構定稿                        | 完成         |
| 🔄 前端介面開發中                         | 進行中        |
| 🔜 API 整合 (ForumKit / Serelix SSO) | 預計 2025 Q4 |
| ⏳ 公開測試版                            | 2026 Q1    |

---

## 📖 文件與支援 | Documentation & Support

* 開發文件（即將推出）
* [ForumKit 官方支援群](https://discord.gg/serelix)
* Email：[cardium.serelix@gmail.com](mailto:cardium.serelix@gmail.com)
* IG：[@serelix.studio](https://www.instagram.com/serelix.studio)

如欲參與開發、測試或設計主題模板，請透過上述管道聯繫我們。

---

## 💬 結語 | Final Note

Cardium 是一張卡片，但更像是一種身份的延伸。
它不只是展示資料，而是記錄「你在數位世界留下的足跡」。
我們相信，每個人都該有屬於自己的數位名片。

> Cardium — Your Identity, Simplified.
