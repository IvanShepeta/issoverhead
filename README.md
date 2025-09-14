# ISS Overhead Notifier 🚀✨

A Python script that sends you an email notification when the **International Space Station (ISS)** is passing above your location **at night**, so you can go outside and spot it in the sky!

---

## 🌍 How It Works

1. Fetches the current position of the ISS from the [Open Notify API](http://api.open-notify.org/iss-now.json).  
2. Compares the ISS latitude/longitude with your location.  
   - If the ISS is within ±5 degrees of your coordinates → it’s overhead.  
3. Uses the [Sunrise-Sunset API](https://sunrise-sunset.org/api) to check if it is currently night at your location.  
4. If both conditions are true, the program sends you an email saying:  
   **"LOOK UP! The ISS is above you in the sky"**.  
5. The script checks every **60 seconds**.

---

## 🛠 Requirements

- Python 3  
- `requests` library  
- Gmail account (or another SMTP-supported email service)


