# Baja-SAE-RF-Video-Transmitter-Integration

RF integration and troubleshooting project for a 2.5 W analog FPV video transmitter installed on a Baja SAE competition vehicle.

---

## Overview

This project investigated the integration of a high-power analog FPV video transmission system onto a collegiate Baja SAE vehicle. The objective was to provide real-time video transmission during testing and vehicle operation while evaluating RF system performance in a challenging off-road environment.

The project involved hardware selection, antenna selection, system packaging, RF troubleshooting, and future antenna validation using impedance and VSWR measurements.

---

## System Configuration

### Transmitter Side

- 2.5 W Analog Video Transmitter (VTX)
- Omnidirectional Antenna
- Flight Controller Interface
- Vehicle Electrical Integration
- Custom Housing

### Receiver Side

- Diversity Video Receiver
- Omnidirectional Antenna
- Directional Patch Antenna
- Ground Station Display

---

## Engineering Challenges

Several factors limited RF link performance during testing:

### Frequency Compatibility

The transmitter could not reliably change operating frequency, limiting flexibility during system configuration and troubleshooting.

### Antenna Matching

The installed antenna may not have been optimally tuned for the transmitter operating frequency, potentially increasing mismatch losses and reducing transmitted power.

### Vehicle Integration

The transmitter was mounted near the aluminum firewall of the Baja SAE vehicle. The large metal structure likely influenced the antenna radiation pattern and introduced RF shadowing effects.

### Non-Line-of-Sight Operation

Unlike drone applications, the transmitter often operated without direct line of sight to the receiver due to vehicle body structure, terrain, and testing conditions.

### Multipath and Blockage

Vehicle components, chassis members, and surrounding terrain introduced opportunities for reflection, diffraction, and signal blockage.

---

## RF Design Decisions

To improve reception under dynamic vehicle conditions:

- A higher-gain omnidirectional antenna was selected for the transmitter
- A diversity receiver was used on the receive side
- A directional patch antenna was paired with an omnidirectional antenna to improve reception under varying orientations

---

## Planned RF Characterization

Future testing will include:

- VSWR Measurements
- Return Loss Measurements
- Impedance Measurements
- Smith Chart Analysis
- Mounted vs. Unmounted Antenna Comparisons
- Frequency Sweep Testing

---

## Expected Results

### VSWR vs Frequency

<img src="images/vswr_plot.png" width="700">

### Return Loss

<img src="images/return_loss.png" width="700">

### Smith Chart

<img src="images/smith_chart.png" width="700">

### Vehicle Test Setup

<img src="images/baja_vtx_setup.jpg" width="600">

---

## Lessons Learned

This project demonstrated that transmitter output power alone does not guarantee RF link performance. Antenna tuning, mounting location, line-of-sight conditions, and nearby conductive structures can significantly affect overall system reliability.

The work provided practical experience with:

- RF System Integration
- Antenna Selection
- Diversity Reception
- Link Reliability Analysis
- VSWR and Impedance Matching
- Vehicle Electronics Integration
- Real-World Wireless Troubleshooting

---

## Future Improvements

- Verify antenna resonance frequencies using a VNA
- Match antenna selection to transmitter operating frequency
- Relocate antenna away from conductive structures
- Evaluate alternative antenna placements
- Quantify link quality under varying terrain conditions
- Compare omnidirectional and directional antenna performance

---

## Skills Demonstrated

- RF Engineering
- Wireless Communications
- Antenna Systems
- Video Transmission Systems
- Signal Propagation
- Hardware Integration
- Root Cause Analysis
- Vehicle Electronics
- Test & Validation

---

## Author

Anthony Garcia

Electrical Engineering • RF Systems • Embedded Systems • Wireless Communications
