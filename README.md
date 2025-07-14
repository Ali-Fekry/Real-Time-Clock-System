# ⏰ Real-Time Clock System (Embedded Project)

A complete real-time clock system implemented using an **AVR microcontroller** (e.g., ATmega32) and **RTC module** (DS1307).  
This embedded system displays the current time and date, and supports alarm setting, stopwatch, and countdown timer functionality.

---

## 🔧 Features

- ✅ Real-Time Clock & Date Display (with DS1307 RTC module)
- ⏰ Alarm Function — triggers buzzer at set time
- ⏱ Stopwatch — counts up in seconds and minutes
- ⏳ Countdown Timer — counts down and activates buzzer at 0
- 🧠 Push-button based user interface (no PC required)
- 🖥 Display output on **16x2 character LCD**

---

## 🛠 Technologies & Components Used

| Component        | Description                                  |
|------------------|----------------------------------------------|
| **AVR MCU**       | ATmega32 or similar                         |
| **RTC Module**    | DS1307 Real-Time Clock                      |
| **LCD Display**   | 16x2 Character LCD                          |
| **Push Buttons**  | For mode control, setting values, input     |
| **Buzzer**        | Alarm and timer alerts                      |
| **Power Supply**  | 5V regulated for microcontroller and modules |

---

## 🧩 System Modes

1. **Clock Mode:** Displays current time (HH:MM:SS) and date
2. **Alarm Mode:** Set alarm (HH:MM), triggers buzzer when time matches
3. **Stopwatch Mode:** Start/Stop/Reset counter (mm:ss)
4. **Countdown Mode:** Set countdown value, buzzer sounds when finished
5. **User Interface:** Switch between modes using push buttons

---

## 📁 Folder Structure
```Real-Time-Clock-System/
├── main.c # Core logic (mode switching, main loop)
├── rtc.c / rtc.h # RTC driver functions (read/write time/date)
├── lcd.c / lcd.h # LCD interfacing functions
├── utils.c / utils.h # Timer delays, button debouncing
├── README.md # This documentation file```

---

## 🚀 How to Run

1. Burn the compiled `.hex` file to your ATmega32 using any ISP programmer (e.g., USBasp)
2. Connect all hardware (RTC, LCD, buttons, buzzer) per your schematic
3. Power on the system — it starts in clock mode
4. Use buttons to switch modes and interact with each feature
