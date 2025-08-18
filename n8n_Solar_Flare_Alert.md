# ☀️ n8n Solar Flare Alert (NASA DONKI + Postbin)

This is a **space-weather alert workflow** built on **n8n (web app)**.  
It connects to **NASA’s DONKI API**, checks for **solar flares**, and posts an alert message to **Postbin** (or any webhook).

---

## 🎥 Demo
- Video: [YouTube Video](https://youtu.be/5FH7AtSz5QY)

---

## ✨ Features
- **NASA DONKI API** integration for real-time space weather  
- **Filter with IF node** → only pick major flares (e.g., X-class)  
- **Webhook alerts** via Postbin (can be swapped with Slack/Discord/Telegram)  
- Fully automated on **n8n Cloud**  

---

## 🚀 How it works
1. **Schedule Trigger** runs the workflow (e.g., every Monday at 9 AM)  
2. **NASA node** fetches solar flare data  
3. **IF node** checks if `classType` contains `"X"`  
4. **Send Request / Postbin node** posts a message like:  
   > “There was a solar flare of class X1.1 starting 2025-08-17T10:22Z (peak 2025-08-17T10:27Z)”

---

## 🔗 Links
- LinkedIn Demo: [Automating Space Weather Alerts with n8n + NASA DO](https://www.linkedin.com/posts/muhammad-bodla_n8n-nasa-donki-activity-7363014514725826560-M_jH?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAAEik8fwBOKdNioqtq_1h96yRgPY2ZpVpAMk) 
- n8n: [https://n8n.io](https://n8n.io)  
- NASA API: [https://api.nasa.gov](https://api.nasa.gov)  

---

## 📜 License
MIT
