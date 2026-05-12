# ⚡ NetSure MiniUPS Pro - Power Management

## Overview

Power management is one of the core design areas of NetSure MiniUPS Pro.

The system is designed to provide uninterrupted backup power for WiFi routers and ONT/modem systems during power outages while maintaining compact embedded hardware architecture.

The current concept focuses on:

* modular power routing
* lithium-ion battery backup
* stable voltage conversion
* compact PCB integration
* simplified scalability

---

# 🔌 Primary Power Flow

```text id="jlwmw7"
USB-C Input
     ↓
Power Management & Charging Module
     ↓
Lithium-Ion Battery Pack
     ↓
DC Boost Conversion
     ↓
9V / 12V Router Outputs
```

---

# 🔋 Charging Architecture

The system uses a USB-C based charging input connected to a modular charging and protection subsystem.

Primary charging goals:

* safe battery charging
* compact implementation
* simplified integration
* portable product architecture
* improved usability

The charging subsystem is intended to manage:

* battery charging
* protection
* backup switching behavior
* power routing

---

# ⚙️ Battery Backup Logic

During normal operation:

* external power provides system input
* the battery subsystem remains charged
* output rails remain active

During a power outage:

* the battery subsystem becomes the primary power source
* boost conversion maintains router outputs
* uninterrupted networking operation is maintained

The architecture is intended to reduce interruption during power transitions.

---

# 🔌 Output Voltage Architecture

The current concept includes:

* 9V output support
* 12V output support

This allows compatibility with a wider range of:

* routers
* ONT systems
* networking hardware

Boost conversion modules are used for voltage regulation and output generation.

---

# 📊 Monitoring & Telemetry Roadmap

Future ESP32-based telemetry features may include:

* battery percentage estimation
* runtime monitoring
* charging status
* voltage monitoring
* wireless diagnostics
* dashboard integration

---

# 🧠 Design Priorities

The power management architecture prioritizes:

* stability
* modularity
* compactness
* practical implementation
* realistic product integration

The overall system is intentionally designed using modular embedded hardware concepts to accelerate development while maintaining startup-style product plausibility.

---

# 🚧 Current Development Stage

Current progress includes:

* architecture planning
* PCB layout development
* modular power path planning
* dashboard prototyping

Future stages may include:

* prototype validation
* thermal optimization
* firmware integration
* telemetry implementation
* real-world runtime testing
