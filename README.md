
# ⚡ **tmlshellkit**

![C++](https://img.shields.io/badge/lang-C%2B%2B17-blue)
![Realtime](https://img.shields.io/badge/realtime-1kHz-yellow)
![Platform](https://img.shields.io/badge/platform-linux--rt-informational)

> **industrial motion controller for robotic arms.**

---

### Overview

tmlshellkit provides deterministic control loops, path planning, and safety systems for multi-axis robotics.
Originally for research labs, now open for makers.

docs → [tml-shellkit.dev](https://tml-shellkit.dev)

---

### Build & Run

```bash
mkdir build && cd build
cmake ..
make
sudo ./tml_shellkit --config demo.yaml
```

---

### Key Features

* 1kHz control loop
* 5-axis interpolation
* CANopen + Modbus drivers
* Safety interlocks

---

### Config snippet

```yaml
safety:
  e_stop_gpio: 27
  torque_limit: 1.2
planner:
  mode: spline
  tick_ms: 1
```

---

### Visualization

Works with [rosbridge](https://rosbridge.dev) and [rviz](https://rviz.dev)

---

### License & Credits

GPLv3 • Maintained by you guys

> "Built after debugging for months."
