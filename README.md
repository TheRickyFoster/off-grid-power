# DIY Flywheel Pedal Generator (R600-Compatible)

**Goal:**  
Build a human-powered generator capable of charging a 299Wh power station (like the ALLPOWERS R600) or a 12V–24V battery bank, using **locally scavenged parts** such as a spin bike and scrap motors.  
This design is scalable, low-cost (~$200–$300 CAD), and smooth to pedal thanks to the built-in flywheel.

---

## Overview

This project converts a **spin bike** (or other exercise bike with a heavy flywheel) into a generator by:
1. Coupling the flywheel to a **permanent magnet DC motor** (PMDC) salvaged from a scooter, treadmill, or e-bike hub.
2. Running the motor output through a **DC-DC buck/boost converter** to stabilize voltage (18–24V) for the R600’s solar input or other devices.
3. Adding simple adapters so you can charge **USB devices, 12V batteries, or power stations** without overvoltage.

---

## Parts List (All Locally Salvageable)

### Core Components
- **Spin Bike with Flywheel**  
  Look for a free or cheap one on Facebook Marketplace, Kijiji, or scrap yards.  
  Any exercise bike with a heavy steel flywheel (10–20 lb) works.

- **Permanent Magnet DC Motor (250–500W, 12–48V)**  
  Salvaged from:
  - E-scooters (common 24V/36V motors)
  - Treadmills (often 90V but can still output usable DC at low RPM)
  - E-bike hub motors (can be used as a stationary generator)

- **Pulley or Belt Drive**  
  Use a timing belt, v-belt, or chain to connect the flywheel to the motor.  
  Many bikes already have a belt you can tap into.

### Electrical Parts
- **DC-DC Buck/Boost Converter (150–600W rated)**  
  Allows you to set a stable output (e.g., 18–24V at up to 10A) for the R600 or USB chargers.

- **Blocking Diode (Schottky, 10–20A)**  
  Prevents current from flowing back into the motor.

- **XT60 Connector Cable**  
  For plugging directly into the R600’s solar input port (or use Anderson connectors for a generic battery).

- **Optional Buffer Battery (12V 7–20Ah SLA or LiFePO₄)**  
  Smooths voltage spikes and stores power for a steady charge.

---

## Tools Needed
- Basic hand tools (wrenches, screwdrivers)
- Drill (for mounting motor brackets)
- Multimeter (to check output voltage)
- Soldering iron (for wiring connections, optional but recommended)

---

## Build Steps

### 1. Prepare the Spin Bike
- Secure the bike frame on a flat surface.
- Check the flywheel spins freely.
- Identify a spot to mount the motor near the flywheel (or tap into the bike’s drive belt).

### 2. Mount the Motor
- Use L-brackets, angle iron, or wood blocks to hold the motor securely.
- Align the motor shaft with the flywheel or belt to avoid slippage.
- Install a belt, chain, or friction roller between the flywheel and motor shaft.

### 3. Wire the Electrical System
1. Connect the **motor output** to the **blocking diode** (to prevent reverse current).
2. Run output from diode into the **DC-DC converter input**.
3. Set the converter to output **18–24V** (matches R600 solar input) or **5V USB** if using for phones.
4. Connect converter output to **XT60 cable** (for R600) or other connectors as needed.

### 4. Test and Tune
- Pedal the bike; check voltage with a multimeter.
- Adjust the converter so it outputs a safe voltage (start low, increase gradually).
- Confirm the R600 recognizes the input as a “solar panel” (green light or input reading).

---

## Performance Expectations

- **Average Pedaling Output**:  
  50–100W sustained (casual pace).  
  150W possible for short bursts.

- **R600 Charging Time**:  
  At 75W: ~4 hours to fully charge 299Wh.  
  At 100W: ~3 hours.

- **Phone Charging (Direct)**:  
  ~10 minutes of pedaling per phone charge at 50–75W.

---

## Tips for Efficiency
- Use the **flywheel’s natural momentum** to keep voltage steady (don’t stop pedaling abruptly).
- Gear the motor so the flywheel spins it at **optimal RPM** (usually 1,000–3,000 RPM for scooter motors).
- Consider adding a **capacitor bank or small battery** if powering sensitive devices (laptops).

---

## Safety Notes
- Always verify voltage with a multimeter before connecting to sensitive gear.
- Use a fuse (10–20A inline) to protect the circuit from shorts.
- Keep the motor cool (avoid continuous heavy loads without airflow).

---

## Cost Estimate (Scrapped Build)
- Spin bike: $0–$100 (used)
- DC motor: $50–$70 (salvaged or used online)
- Belt/chain + brackets: $40–$60
- DC-DC converter: $40
- Diode, wiring, connectors: $30
- (Optional buffer battery): $50–$100

**Total**: **~$200–$300 CAD** for a fully functional generator.

---

## Why This Build Works Well
- Heavy flywheel keeps power smooth and makes pedaling easier.
- Mostly salvaged parts reduce cost.
- Can charge **anything from USB devices to the R600** without wall power.
- Expandable — add a second motor or connect two bikes for double output.

---
