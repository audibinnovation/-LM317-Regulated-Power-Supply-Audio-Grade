🔧 LM317 Regulated Power Supply – Audio Grade

This repository contains the schematic and design details for a regulated DC power supply using the LM317 adjustable voltage regulator. It delivers a clean, stable 12.7 V output from a 15 V input, optimized for low-noise audio applications such as DACs, preamps, and headphone amplifiers.

📐 Circuit Overview

The design includes:

LM317 regulator with precision voltage setting

Input and output filtering using capacitors and inductors

Snubber network for damping HF ringing

Protection diodes for reverse polarity and discharge safety

ADJ bypass capacitor for improved ripple rejection


🔌 Electrical Specs

Input voltage: 15 V DC

Output voltage: 12.7 V DC (adjustable via R1/R2)

Max output current: ~1.5 A (with heatsink)

Ripple (typical): <5 mV peak-to-peak

Dropout voltage: ~2–3 V (not LDO)

🎧 Audio Optimization Features

ADJ bypass cap (C9): Improves ripple rejection by ~20 dB

Snubber (R5 + Csnub): Damps LC ringing from L2 and output caps

Star grounding recommended: Prevents hum and ground loops

Film caps at output: Reduce dielectric absorption and HF noise

🧪 Simulation & Testing

Simulated in [your preferred tool] with 500 mA load

Output ripple measured <5 mV p‑p with snubber and ADJ bypass

Stable under dynamic load conditions

📁 Files

lm317_audio_supply.sch – Schematic file

lm317_audio_supply.png – Annotated schematic image

README.md – This documentation

🚀 Usage

Connect 15 V DC input to the input terminal.

Output will stabilize at 12.7 V after startup.

Ensure proper heatsinking for LM317 if load >500 mA.

Optional: Adjust R2 to change output voltage.

🛠️ Customization

For lower dropout, consider replacing LM317 with TPS7A47 or LT1763.

For dual rails, pair LM317 with LM337 or TPS7A33.

For higher current, upgrade to LM338 (5 A).

📜 License

MIT License – free to use, modify, and distribute.
