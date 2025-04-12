- 👋 Hi, I’m @Alerta-accidente
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Alerta-accidente/Alerta-accidente is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import requests

BOT_TOKEN = "7808474978:AAF8jh2aqeDbux9hmVEGRZ0eCO5X_eNde_I"
CHAT_ID = "6458331173"
TEST_MESSAGE = "✅ TEST ALERTĂ: Acesta este un test de funcționare pentru botul BMSY.\nLocație fictivă: https://www.waze.com/livemap?lon=26.1&lat=44.45&zoom=14"

url = f"https://api.telegram.org/bot{BOT_TOKEN}/sendMessage"
data = {"chat_id": CHAT_ID, "text": TEST_MESSAGE}
r = requests.post(url, data=data)

print(r.status_code, r.text)
