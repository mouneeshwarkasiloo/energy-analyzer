# Energy Analyzer

**Energy Analyzer** is a lightweight Python CLI tool that helps users estimate their daily and monthly electricity consumption. The program collects device-level inputs such as rated watts, hours of usage, and quantity, then computes per-device kWh, total consumption, and an estimated monthly bill based on the chosen tariff.

The output includes a clean terminal summary table and an auto-generated `energy_report.txt` file for offline reference. The script uses ANSI colors sparingly to keep the interface readable without looking automated or noisy.

---

## Features
- Interactive CLI prompts for device details  
- Calculates per-device and total daily consumption (kWh)  
- Estimates monthly kWh and electricity bill  
- Identifies the highest-consuming device  
- Generates a timestamped `energy_report.txt`  
- Pure Python 3 (no external libraries required)

---

## How to Run
1. Clone or download this repository  
2. Open a terminal inside the project folder  
3. Run the script:

```bash
python3 energy_analyzer.py



**Sample Input:**
Billing days (typical 30): 30
Tariff ₹/kWh (e.g., 8): 8
Number of devices: 3

1. Device name: Air Conditioner
   Watts (W): 1500
   Hours per day: 5
   Quantity: 1





**Sample Output:**
Per-Device Daily Usage
---------------------------------------------------------------
Device               | Watts  | Hours  | Qty  | kWh/day
---------------------------------------------------------------
Air Conditioner       | 1500   | 5.0    | 1    | 7.500
Refrigerator          | 200    | 24.0   | 1    | 4.800
Fan                   | 80     | 10.0   | 2    | 1.600
---------------------------------------------------------------

Summary
  Total daily consumption      : 13.900 kWh
  Billing cycle consumption    : 417.000 kWh
  Estimated bill               : ₹3336.00
  Highest daily consumer       : Air Conditioner
