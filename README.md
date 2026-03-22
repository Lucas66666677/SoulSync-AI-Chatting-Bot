# 🔒 SoulSync - AI 陪伴私密日記
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
**SoulSync** 是一個結合 AI 對話與情緒監測的私密日記系統。透過 Groq 的高速推論引擎與 Streamlit 互動介面，為使用者提供一個安全、溫暖的情緒出口。

## ✨ 核心功能

* **🤖 AI 引導式對話**：採用 `Llama 3.3-70B` 模型，提供具有同理心的互動，幫助釐清思緒。
* **📊 即時情緒監測**：透過 `Llama 3.1-8B` 分析日記內容，並以燈號（綠、黃、紅）同步顯示給房間好友。
* **👥 好友狀態監測**：在不洩露具體內容的前提下，讓好友了解彼此的心情狀態。
* **🔥 一鍵銷毀**：支援隨時清除所有對話紀錄與房間資料，保護個人隱私。
* **🌐 遠端存取**：整合 Ngrok 技術，即使在 Google Colab 執行也能輕鬆對外連線。

## 🛠️ 技術架構

* **模型引擎**：Groq Cloud API
* **主要模型**：Llama-3.3-70b-versatile, Llama-3.1-8b-instant
* **網頁框架**：Streamlit
* **網路穿透**：Ngrok
* **開發語言**：Python 3

## 🚀 快速開始 (Google Colab 版)

1.  **取得金鑰**：
    * 至 [Groq Console](https://console.groq.com/keys) 取得 API Key。
    * 至 [Ngrok Dashboard](https://dashboard.ngrok.com/tunnels/authtokens) 取得 Authtoken。
2.  **設定 Colab Secrets**：
    * 在 Colab 左側點擊「鑰匙」圖示。
    * 新增 `GROQ_KEY` 並貼入您的 Groq 金鑰。
    * 新增 `NGROK_TOKEN` 並貼入您的 Ngrok Token。
3.  **執行腳本**：
    * 執行專案中的 `.ipynb` 檔案。
    * 等待暖機完成後，點擊輸出的 `ngrok-free.dev` 連結即可開始使用。

## ⚠️ 安全警告
* **隱私保護**：本專案預設將日記資料存於 `shared_diary_data.json`，請務必將此檔案加入 `.gitignore`。

## 📝 授權協議

本專案採用 [MIT License](LICENSE) 授權。
