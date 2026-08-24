# IoT Device-to-Cloud & Dashboard APIs

## ThingSpeak

**What it is:** MathWorks-operated IoT platform for logging and visualizing sensor data
from devices like ESP32/ESP8266/Arduino, with a REST + MQTT API.

**Free tier:** Free for non-commercial use — commonly cited as up to ~8,000 API requests
per day (an update roughly every ~15 seconds), 8 fields per channel.

**Sign-up link:** https://thingspeak.com/users/sign_up (or via a MathWorks account:
https://www.mathworks.com/mwaccount/register)

**Steps to get a key:**
1. Create a free MathWorks/ThingSpeak account.
2. Click **New Channel**, name it, and enable the fields (sensors) you'll log.
3. Save the channel, then open its **API Keys** tab.
4. Copy the **Write API Key** (for devices sending data) and any **Read API Key** (for
   apps pulling data back out).

**Notes:** Rate limit on the free service is roughly one update per channel every 15
seconds — space out your device's `POST`/HTTP GET calls accordingly.

---

## Adafruit IO

**What it is:** IoT data logging and dashboard service, popular with Arduino/
CircuitPython/ESP projects; also supports MQTT.

**Free tier:** Free plan allows a limited number of data points per month and up to 10
active feeds — enough for hobby dashboards, not high-frequency logging.

**Sign-up link:** https://accounts.adafruit.com/users/sign_up

**Steps to get a key:**
1. Create a free Adafruit account.
2. Log into https://io.adafruit.com.
3. Click your profile icon → **My Key** to see your Username and AIO Key.
4. Use both in your device code's MQTT or HTTP calls.

**Notes:** Good pairing with Adafruit's own MicroPython/CircuitPython libraries if
you're already in that ecosystem.

---

## Blynk

**What it is:** Mobile-app-first IoT platform — build a phone dashboard for your
microcontroller with drag-and-drop widgets.

**Free tier:** Free plan includes a capped number of devices and data points/messages
per day, sufficient for one or two personal projects.

**Sign-up link:** https://blynk.io/getting-started

**Steps to get a key:**
1. Create a Blynk account (web or via the mobile app).
2. Create a new **Template**, then a **Device** from that template.
3. Open the device — the **Auth Token** is shown on its Device Info tab; that token is
   your API key for that device.

**Notes:** Auth tokens are per-device, not per-account — each new device you add gets
its own token.
