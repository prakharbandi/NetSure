# 🔗 NetSure MiniUPS Pro — Module Connections

## Overview

This document outlines the planned high-level module interconnections used in the NetSure MiniUPS Pro architecture.

The current system uses a modular embedded hardware approach to simplify:

* PCB development
* prototyping
* power routing
* telemetry integration

The listed connections represent concept-stage architecture planning and may evolve during future prototype iterations.

---

# ⚡ Primary Power Connections

## USB-C Input → Power Management Module

```text id="jlwmow"
USB-C VBUS  → Charging Module Input+
USB-C GND   → System Ground
```

Purpose:

* primary external power input
* battery charging
* system power routing

---

# 🔋 Battery Connections

## Battery Pack → Charging & Protection Module

```text id="jlwmkh"
Battery Positive → BAT+
Battery Negative → BAT-
```

Purpose:

* lithium-ion energy storage
* backup power source

---

# ⚙️ Power Output Connections

## Charging Module → Boost Conversion Modules

```text id="jlwmur"
OUT+ → Boost Module VIN+
OUT- → Boost Module GND
```

Purpose:

* provide regulated input power
* enable output voltage generation

---

# 🔌 12V Output Path

```text id="jlwm3w"
Boost Module #1 OUT+ → 12V Output Connector
Boost Module #1 GND  → System Ground
```

Purpose:

* router backup output

---

# 🔌 9V Output Path

```text id="jlwm9x"
Boost Module #2 OUT+ → 9V Output Connector
Boost Module #2 GND  → System Ground
```

Purpose:

* ONT/modem backup output

---

# 📡 ESP32 Telemetry Connections

## ESP32 → OLED Display

```text id="jlwms5"
ESP32 SDA → OLED SDA
ESP32 SCL → OLED SCL
ESP32 GND → OLED GND
ESP32 3.3V → OLED VCC
```

Purpose:

* runtime display
* battery monitoring
* telemetry visualization

---

# 🧠 Planned Monitoring Signals

Future telemetry planning may include:

* battery voltage sensing
* runtime estimation
* charging state monitoring
* output rail monitoring
* wireless diagnostics

---

# ⚠️ Important Note

This document represents:

* concept-stage architecture planning
* modular hardware interconnection strategy
* embedded systems layout planning

Final routing and electrical implementation may evolve during future prototype validation and PCB revisions.
