# Soil Moisture Sensor PCB Using KiCad

## 📌 Project Overview

This project is a **Soil Moisture Sensor PCB** designed using KiCad 9. It detects the moisture level in soil using two conductive probes and an electronic sensing circuit.

The circuit uses an LM358 operational amplifier, a 10 kΩ potentiometer, resistors, capacitors, and indicator LEDs to detect changes in soil conductivity. The PCB includes two long sensing prongs that can be inserted into the soil.

The main objective of this project is to understand soil moisture detection, analog sensing circuits, and PCB design.

## 🎯 Objectives

- Design a soil moisture sensing circuit.
- Understand how soil conductivity changes with moisture.
- Use the LM358 for signal conditioning or threshold detection.
- Adjust the detection threshold using a potentiometer.
- Indicate the sensor status using LEDs.
- Design the schematic in KiCad.
- Assign component footprints.
- Create and route the PCB.
- Perform ERC and DRC checks.
- Visualize the completed PCB using KiCad's 3D Viewer.

## ⚙️ Working Principle

The sensor works by detecting changes in the electrical conductivity of soil.

The two sensing prongs act as electrodes. When inserted into soil, the electrical resistance between the electrodes changes depending on the soil's moisture content.

- **Wet soil:** Generally provides a lower resistance between the probes because it contains more conductive moisture.
- **Dry soil:** Generally provides a higher resistance between the probes.

The sensing circuit detects this change and provides a corresponding electrical signal.

The LM358 processes the sensing signal. The 10 kΩ potentiometer can be used to adjust the detection threshold, depending on the circuit configuration. The LEDs indicate the detected condition according to the actual circuit connections.

**Note:** The exact LED behavior depends on the schematic. Confirm which LED indicates wet or dry soil before using the sensor.

## 🔌 Block Diagram

```text
       Soil Moisture
             |
             v
      Two Sensing Probes
             |
             v
      Sensing Circuit
             |
             v
        LM358 Circuit
             |
             v
       Indicator LEDs
```

## 🧩 Components Used

| Reference | Component | Value / Type |
|---|---|---|
| U1 | Operational amplifier | LM358 |
| RV1 | Potentiometer | 10 kΩ |
| R1 | Resistor | 1 kΩ |
| R2 | Resistor | 10 kΩ |
| R3 | Resistor | 1 kΩ |
| D1 | Indicator LED | As selected |
| D2 | Indicator LED | As selected |
| C1 | Capacitor | As per schematic |
| C2 | Capacitor | As per schematic |
| J1, J2 | Connectors | As per schematic |
| Sensor probes | Conductive electrodes | PCB prongs |

*Verify the component values and reference designators against the final KiCad schematic before manufacturing.*

## 🖥️ PCB Design Using KiCad

The PCB was designed using KiCad 9.

### Design Process

1. Create the soil moisture sensor schematic.
2. Add the LM358, resistors, capacitors, potentiometer, LEDs, and connectors.
3. Connect the components according to the circuit diagram.
4. Assign suitable footprints.
5. Update the PCB from the schematic.
6. Arrange the components in the upper section of the board.
7. Design the fork-shaped sensing prongs.
8. Route the copper tracks.
9. Configure the board outline using the `Edge.Cuts` layer.
10. Run ERC in the schematic editor.
11. Run DRC in the PCB editor.
12. Inspect the completed board using the 3D Viewer.

## 📐 PCB Design Features

- Compact circuit layout.
- Two extended sensing prongs.
- LM358-based sensing circuit.
- Adjustable detection threshold.
- LED status indication.
- Dedicated component and connector placement.
- PCB layout designed in KiCad.

## 📁 Project Structure

```text
Soil-Moisture-Sensor/
├── Soil-Moisture-Sensor.kicad_pro
├── Soil-Moisture-Sensor.kicad_sch
├── Soil-Moisture-Sensor.kicad_pcb
├── README.md
└── Images/
    ├── schematic.png
    ├── pcb_layout.png
    └── 3d_view.png
```

## 🧪 Testing Procedure

1. Inspect the PCB for solder bridges and incorrect connections.
2. Verify the LM358 pinout and component orientation.
3. Check the potentiometer connections.
4. Verify LED polarity and resistor values.
5. Run ERC and DRC in KiCad.
6. Power the circuit using the specified supply voltage.
7. Insert the sensing prongs into soil with different moisture levels.
8. Adjust the potentiometer to set the detection threshold.
9. Observe the LED response.
10. Repeat the test with dry and moist soil.

## ⚠️ Design Considerations

- Use the correct supply voltage for the LM358 circuit.
- Ensure the two sensing electrodes remain electrically separate.
- Keep the sensing area free of solder mask if direct soil contact is required.
- Prevent the circuit section from contacting wet soil.
- Protect the electronics from water and corrosion.
- Use suitable PCB clearances and track widths.
- Avoid applying excessive voltage directly to the sensing probes.
- Verify the actual detection threshold experimentally.

## ✅ Advantages

- Simple and compact design.
- Adjustable moisture detection threshold.
- Visual status indication using LEDs.
- Easy to study and modify.
- Suitable for learning analog electronics and PCB design.
- Can be adapted for basic gardening and soil-monitoring experiments.

## 🚀 Future Improvements

- Add an Arduino or ESP32 interface.
- Display the moisture level on an LCD or OLED.
- Add an analog output connector.
- Implement digital soil moisture monitoring.
- Add wireless monitoring using Wi-Fi.
- Improve electrode corrosion resistance.
- Develop an automatic plant-watering system.

## 📚 Learning Outcomes

Through this project, I learned:

- Soil conductivity and moisture sensing.
- Basic analog sensing circuits.
- LM358 operational amplifier applications.
- Potentiometer-based threshold adjustment.
- LED indicator circuits.
- KiCad schematic design.
- Footprint assignment and PCB routing.
- PCB outline design.
- ERC and DRC verification.
- PCB 3D visualization.

## 🛠️ Software Used

**KiCad 9.0**

## 📄 License

This project is intended for educational and learning purposes. The circuit can be modified and improved for personal electronics projects.
