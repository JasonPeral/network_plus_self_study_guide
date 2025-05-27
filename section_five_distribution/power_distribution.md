# Power Distribution Systems

### Core Summary

- Power Distribution Systems are crucial for consistent and reliable power delivery to networking equipment, infrastructure and environments
- There are several key topics about power distribution systems:
    - UPS
    - PDU
    - Generators
    - Power Load Management
    - Voltage Considerations

---

**Uninterruptible Power Supply (UPS)**

- An electrical apparatus/device that provides emergency power to a load when the main/primary input power source fails
- A lot of UPS that are within data centers are not just power backups but also provide surge protection, line conditioning and protection against power increases.
- UPS will typically last around 15 - 30 minutes depending on the electrical load needed and they are installed at the bottom of each rack in a data center

---

**Power Distribution Unit (PDU)**

- Specialized device for **distributing electric power** to various networking components and computing equipment
    - Advanced power strips with power, monitor and control features available to use
    - PDUs can be rack-mounted or in large cabinets for rows of servers
    - Provides surge protection but not full protection against complete power loss which is why its usually combined with a UPS and Backup Generator

---

**Generators**

- Installed outside data centers for longer-term power during outages that may have affected the region
- Generators can be powered by Diesel, Gasoline or Propane
- Generators take 60-90 seconds to spin up so being paired with a UPS or battery backup helps for seamless power transition
- Automatic transfer switch shifts power between UPS and generator

---

**Power Load Management**

- This topic is critical for preventing circuit overloads and ensuring efficient power usage across our data center
- Power load management includes careful calculation and monitoring of power loads on the circuits
- Whenever there is new equipment to be installed within the data center the installation requires assessing power impact and balancing loads across the data center

---

**Voltage Considerations**

- Voltage
    - Electric potential difference which is crucial when ordering equipment
    - US standards — 120 Volts
    - EU standards — 230 Volts
- Equipment that we have must match voltage standards within our country to operate properly
- Mismatched voltage can damage or destroy equipment such as US standard equipment being plugged in within EU which is overloading the voltage that the equipment can handle
- Modern equipment have dual voltage and can operate on both standards

**Some Key Considerations**

- We want to use UPS, PDU and backup generators together for comprehensive power management
- Having a good power distribution system ensures seamless power transition and protection against outages for data center reliability
- Consider power loads and voltage requirements before install equipment to ensure compatibility with US(120 Volts) or EU(230 Volts) standards