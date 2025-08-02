<!--
  🌟 n8n • Telegram AI Agent • 🚀
  A friendly, voice-aware AI bot that handles customer queries, recommends products,
  and logs every interaction—powered by n8n (latest), Telegram & OpenAI.
-->

# 🤖 n8n Telegram AI Sales Assistant

[![n8n](https://img.shields.io/badge/n8n-latest-blue.svg)](https://n8n.io/) [![Telegram](https://img.shields.io/badge/Telegram-Bot-blue.svg)](https://core.telegram.org/bots) [![OpenAI](https://img.shields.io/badge/OpenAI-GPT-00acee.svg)](https://openai.com/)

## 🚀 Overview

Turn Telegram into a 24/7 AI-powered sales desk! This n8n workflow:  
- **Listens** for text & voice messages  
- **Transcribes** audio via OpenAI’s speech-to-text  
- **Processes** queries with a GPT agent (contextual memory included)  
- **Logs** every chat in Google Sheets  
- **Responds** instantly with personalized recommendations  

## 📋 Workflow Nodes

| Step | Node                                      | Function                                                                                 |
|------|-------------------------------------------|------------------------------------------------------------------------------------------|
| 1    | **Telegram Trigger**                      | Captures incoming messages (text & voice)                                                |
| 2    | **Switch**                                | Routes to text or audio branch                                                           |
| 3    | **HTTP Request**                          | Downloads voice file from Telegram API                                                  |
| 4    | **Transcribe Recording**                  | Converts speech → text using OpenAI                                                      |
| 5    | **AI Agent (GPT)**                        | Generates context-aware responses; remembers past interactions                           |
| 6    | **Google Sheets – Append/Update Row**     | Logs `chat_id`, `user_name`, `query`, `timestamp`, and `bot_response`                    |
| 7    | **Send Telegram Message**                 | Returns AI’s reply back to the user                                                      |

---

## 📂 Additional Resources

- **n8n Official Documentation**  
  https://docs.n8n.io/  
- **n8n Nodes Reference**  
  https://docs.n8n.io/nodes/  
- **Telegram Bot API Guide**  
  https://core.telegram.org/bots/api  
- **OpenAI API Reference**  
  https://platform.openai.com/docs/api-reference  
- **Google Sheets Node (n8n)**  
  https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-google-sheets/  
- **Sample Workflow JSON (IA AGENT.json)**  
  [Download on GitHub](./IA%20AGENT.json)  


## 🤝 Community & Support

- **Join the n8n Community Forum**  
  https://community.n8n.io/  
- **Telegram Bot Developers Chat**  
  https://t.me/botdevelopers  
- **OpenAI Discord**  
  https://discord.gg/openai  

---

> “Automate the mundane. Focus on the magic.” ✨  

