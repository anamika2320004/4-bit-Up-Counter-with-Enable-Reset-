# 🔢 4-bit Up Counter with Enable & Reset (Verilog)

This project implements a **4-bit Up Counter** in Verilog with **Enable** and **Reset** functionality.  
The counter increments its value on each positive edge of the clock when `enable = 1`.  
If `reset = 1`, the counter resets to `0000`.

---

## 📌 Features
- 4-bit up counter (counts `0000` → `1111` → wraps back to `0000`)
- **Enable input** to control counting
- **Asynchronous Reset** to clear the counter
- Synchronous operation on positive clock edge
- Verified using **testbench** with console output and waveform (EPWave)

---

## 🛠 Files Included
- `txt file` → Verilog module for 4-bit up counter  and for testbench


---

## ▶️ Simulation Steps (EDA Playground)
1. Open [EDA Playground](https://www.edaplayground.com/).  
2. Create a new project and paste:
   - `txt file ` in **Design file**  
   - `txt file` in **Testbench file**  
3. Select a simulator (e.g., Icarus Verilog).  
4. Enable **EPWave** (waveform viewer).  
5. Click **Run**.  

---

## 📊 Console Output Example
| Time (ns) | Reset | Enable | Count (Binary) | Count (Decimal) |
| --------- | ----- | ------ | -------------- | --------------- |
| 0         | 1     | 0      | 0000           | 0               |
| 10        | 0     | 0      | 0000           | 0               |
| 20        | 0     | 1      | 0001           | 1               |
| 30        | 0     | 1      | 0010           | 2               |
| 40        | 0     | 1      | 0011           | 3               |
| 50        | 0     | 1      | 0100           | 4               |
| 60        | 0     | 1      | 0101           | 5               |
| 70        | 0     | 1      | 0110           | 6               |
| 80        | 0     | 1      | 0111           | 7               |
| 90        | 0     | 1      | 1000           | 8               |
| 100       | 0     | 1      | 1001           | 9               |
| 110       | 0     | 0      | 1001           | 9               |
| 140       | 0     | 1      | 1010           | 10              |
| 150       | 1     | 1      | 0000           | 0               |
| 160       | 0     | 1      | 0001           | 1               |
| 170       | 0     | 1      | 0010           | 2               |
| 180       | 0     | 1      | 0011           | 3               |

---

## 📉 Waveform (EPWave)
You should see:
- **Clock** toggling  
- **Reset** asserted and released  
- **Enable** controlling the counter  
- **Count** increasing from `0000` to `1111` and rolling over  

---

## ✅ Learning Outcomes
- Understand **Flip-Flops** and sequential circuits  
- Learn **Clock handling** in Verilog  
- Implement **Enable** and **Reset** in counters  
- Generate and analyze **waveforms** using EPWave  

---
