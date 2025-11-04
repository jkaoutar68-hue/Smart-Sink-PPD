# Smart-Sink-PPD
A portable, programmable Power Delivery source 

# What it does
- Requests PPS voltages in 20 mV steps and current limits in 50 mA steps.
- Protects the output with a **TI TPS2595** eFuse (≤18 V, ~4 A path in this build).
- Measures :bus voltage, current, and power inline using **INA238**.
- Simple CLI over UART
- OLED display for V/I/P.

# Hardware 
- Source: 65 W USB-C PD charger with **PPS**.
- Sink controller: **AP33772** (MikroE USB-C Sink 2 Click) via **I²C**.
- Protection: **TPS2595EVM** (ILIM ≈ 3.5–4.0 A for bring-up).
- Meter: **INA238** breakout in series (VIN+→VIN−).
