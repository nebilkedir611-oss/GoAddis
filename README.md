# GoAddis 🚕

> A lightweight urban transport coordination MVP for Addis Ababa that uses a Telegram bot and QR codes to connect passengers with minibuses, Dolphines, buses, and private cars.

---

## Overview

GoAddis solves the problem of long waiting times and uncertainty in Addis Ababa's informal transport system. Passengers scan QR codes at partner shops or use a Telegram bot to request a ride. A human dispatcher matches them with available drivers via Telegram groups. Drivers accept by replying "take," pick up passengers, and receive cash payment.

**No app install. No GPS required. No digital payments.**

---

## How It Works
# GoAddis

GoAddis is a lightweight transport coordination MVP for Addis Ababa that uses a Telegram bot and QR codes to connect passengers with minibuses and private cars; passengers scan QR codes at partner shops or use the Telegram bot to request a ride by entering their destination, after which a human dispatcher matches them with available drivers via Telegram groups; drivers accept trips by replying "take," pick up passengers, and receive cash payment, while local businesses host QR codes to increase foot traffic.

### Step-by-step

| Step | Action |
|------|--------|
| 1 | Passenger scans QR code at partner shop (or opens Telegram bot directly) |
| 2 | Bot asks: pickup location, vehicle type, destination |
| 3 | Request sent to human admin panel |
| 4 | Admin posts to driver Telegram group (minibus or car group) |
| 5 | Driver replies "take" |
| 6 | Admin confirms to passenger with driver ETA |
| 7 | Driver picks up → passenger pays cash |
| 8 | Driver replies "done" to admin |

---

## Vehicle Types Supported

- Code 2 Private Cars
- Code 3 Private Cars
- Minibuses (12-seat)
- Dolphines
- Large Buses

---

## Features

| Feature | Status |
|---------|--------|
| Telegram bot interface | ✅ MVP ready |
| QR code pickup hubs | ✅ Planned |
| Human admin dispatch | ✅ MVP ready |
| Driver Telegram groups | ✅ MVP ready |
| Voice note support | 🔜 Coming |
| USSD for non-smartphones | 🔜 Coming |
| Automated matching | 🔜 Coming |
| GPS tracking | 🔜 Coming |

---

## Tech Stack

- **Bot Framework:** python-telegram-bot v20.7
- **Language:** Python 3.11+
- **Deployment:** Render / Railway / Any cloud
- **Database:** None (MVP) / PostgreSQL (future)
- **QR Codes:** Static or dynamic (any generator)

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/goaddis-bot.git
cd goaddis-bot


python-telegram-bot==20.7
