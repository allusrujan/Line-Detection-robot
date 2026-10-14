<div align="center">

# 🤖 Line Detection Robot
### Autonomous Path Tracking | Arduino Uno | IR Sensors
**Semester 1 · New Horizon College of Engineering · Sept – Dec 2024**


</div>

---



---

## What Is This?

An autonomous robot that follows a line on the ground — no human control, no remote. Just sensors, logic, and motor control working together in real time.

Built from scratch during Semester 1. Every component was individually wired, every threshold manually calibrated, every turn tested and tuned.

---

## Hardware

| Component | Details |
|---|---|
| 🧠 Microcontroller | Arduino Uno |
| 👁️ Sensors | IR Line-Following Sensor Array |
| ⚙️ Motors | DC Geared Motors |
| 🔌 Motor Driver | L298N |
| 🔋 Power | Dual 18650 Li-ion Cells |
| 💡 Indicators | Red LED (Uno) · Yellow LED (Chassis) |

---

## How It Works

```
IR Sensor (Left) ──┐
                   ├──► Arduino Uno ──► L298N Motor Driver ──► DC Motors
IR Sensor (Right) ─┘
```

- Both sensors detect **black line = LOW**, white surface = **HIGH**
- If **right sensor goes HIGH** → line is to the left → turn left
- If **left sensor goes HIGH** → line is to the right → turn right  
- Both LOW → straight ahead
- Both HIGH → stop

---

## What I Did

**Hardware**
- Assembled chassis, mounted motors and sensor array
- Wired L298N motor driver to Arduino and motors
- Set up dual 18650 power supply

**Software**
- Programmed motor control logic in Embedded C
- Calibrated IR sensor thresholds for accurate line detection
- Implemented intersection and course correction logic
- Added LED indicators for real-time status feedback

---

## Results

| Test | Outcome |
|---|---|
| Straight line tracking | ✅ Smooth and accurate |
| Left turns | ✅ Clean without overcorrection |
| Right turns | ✅ Clean without overcorrection |
| Intersection handling | ✅ Decision logic working |
| Full track completion | ✅ Completed |

---

## Demo

🎥 [Watch it run](Line-detection-robot.mp4)

---

## Key Learnings

- IR sensor threshold calibration is everything — small changes make a huge difference
- Motor response time directly affects turn accuracy
- Real-time decision logic needs to be lean and fast for smooth operation

---

<div align="center">

**Allu Srujan** · Aditya Anil · Devesh Sharma · Anurag Das  
📍 New Horizon College of Engineering, Bengaluru

</div>
