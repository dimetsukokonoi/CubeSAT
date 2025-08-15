# 🔋 Battery Management

This section describes how we powered the **ESP32** using a 3-cell battery, UPS booster module, and buck converter to ensure a stable 5V supply.

---

## 🛠 Components Used

- **One Cell Battery** (Used **three cells** in [circuit design](circuit.image.png) due to model limitations) 🔋  
- **UPS Booster Module** ⚡  
- **Mini Buck Converter** ⬇️  
- **ESP32 Microcontroller** 🖥️  

---

## ⚡ Power Flow

1. **Battery Output:**  
   - Each cell provides **3.7V–4.2V**   

2. **Voltage Boost:**  
   - Connected to **UPS Booster Module**  
   - Boosts voltage to **9V–12V**  

3. **Voltage Regulation:**  
   - Output from UPS → **Mini Buck Converter**  
   - Buck converter steps voltage down to **constant 5V**  

4. **ESP32 Power:**  
   - Buck converter output → **ESP32 5V pin**  
   - Ground connected → **ESP32 GND**  

---

### 🔹 Notes

- The **UPS booster** ensures voltage stability even if the battery level drops.  
- The **buck converter** provides a clean, regulated 5V for the ESP32.  
- A proper **GND connection** is essential to avoid damage.  

---

A flowchart to easily understand
> **Battery → UPS Booster → Buck Converter → ESP32**
