# InkTime

## Block Diagram
The system architecture centers on the nRF52840 SoC for wireless connectivity, with power stabilized at 3.3V via an RT6160 buck-boost regulator. It integrates a LiPo battery with USB-C charging alongside an e-paper display, IMU, fuel gauge, and haptic feedback.

<img width="1010" height="568" alt="Block_Diagram" src="https://github.com/user-attachments/assets/f175c803-042e-495b-b1c9-b85e4e8fdb73" />

## Bill of Materials (BOM)

|Component|JLC Part #|Package|Description|Datasheet|
| :--- | :--- | :--- | :--- | :--- |
|SJ1|N/A|Solder Jumper (Copper feature - leave open)|SMD solder JUMPER|N/A|
|R2, R3, R4|[C3920633](https://www.lcsc.com/product-detail/C3920633.html)|0201|7.68k 0201 Thin Film Surface Mount Fixed Resistor +/-0.5% 0.031W CPF0201D7K68C1|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2404081048_TE-Connectivity-CPF0201B511RE1_C3920633.pdf)|
|C23, C27, C34, C42|[C21012218](https://www.lcsc.com/product-detail/C21012218.html)|-|Check availability|[datasheet](https://jlc-prod-smt.oss-eu-central-1.aliyuncs.com/smtDataManualFile/8603520985945550848-C21012218.pdf?response-content-disposition=attachment%3B%20filename%3DC21012218.pdf%3B%20filename%2A%3DUTF-8%27%27C21012218.pdf&x-oss-date=20260407T205848Z&x-oss-expires=1800&x-oss-security-token=CAISgAN1q6Ft5B2yfSjIr5r9Dd2HhJt1xpCRZnzhgHQ0Psp9nrTKiTz2IHhMdHJsAOodtv0%2FmmhT6PkclqRLcbhpcmfjV%2BZHzLB8qYoRtS1%2F4J7b16cNrbH4M4H6aXeirtuwDsz9SNTCALjPD3nPii50x5bjaDymRCbLGJaViJlhHLN1Ow6jdmhpCctxLAlvo9NgFxm3D%2Fu2NQPwiWf9FVdhvhEG6Vly8qOi2MaRmFy8yFTx0b0SvJ%2BjYMrmPctoN9JnSdC5mfdzau3a1TJ84gRD0a5wkaVA1zbDs5bfISEIuUzebreLqY03dV4mOvdqIcMe8qigz88fk%2FfIioH6xyxKOexoSCnFTOiiupCcQLPyao9jLu6iayqViY7QaIOTqQohZmkAMwVOasAsI3Ngh4zF97Qt0cVNkXO9gWfLI8DtuMleWoolCMBMoNHD0eS19jklBdzSlusJRAJJUVBflCeKEaRNSAd3WGhEfM2%2BBt4QT30w5N2u00S8OSMIfXAg5qKWD5sagAGsz%2FZUSUxHdlmxVPmipF%2FTcZWs78wlHh10XRuVSQAFwkjbrT5Hik%2Bt6g43igoBe9p%2FcAdU6beRw%2F0OV8Ul08RsL45K5wTZwHFsbzFcwqB3eAqV0VruhFdx%2FHGC73AK3f%2BS3e6Qh1%2F1xoEQbmetO%2F%2BEcdyt%2BmwKiZrCa5Agq9keuCAA&x-oss-signature-version=OSS4-HMAC-SHA256&x-oss-credential=STS.NYHFg3iDTqRzdZPdta2EQqqak%2F20260407%2Feu-central-1%2Foss%2Faliyun_v4_request&x-oss-signature=20ddec61a1b664f2d44439cb342bbd932d8702b658f2816e0dfb7eb77563430a)|
|EPD_C5|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|R1_EP_DR|[C3920633](https://www.lcsc.com/product-detail/C3920633.html)|0201|7.68k 0201 Thin Film Surface Mount Fixed Resistor +/-0.5% 0.031W CPF0201D7K68C1|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2404081048_TE-Connectivity-CPF0201B511RE1_C3920633.pdf)|
|C15|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|C5, C7, C8, C12, C19|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|C11|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|R2_EP_DR, R9, R_PWR_EPD|[C3920633](https://www.lcsc.com/product-detail/C3920633.html)|0201|7.68k 0201 Thin Film Surface Mount Fixed Resistor +/-0.5% 0.031W CPF0201D7K68C1|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2404081048_TE-Connectivity-CPF0201B511RE1_C3920633.pdf)|
|R5, R7, R8|[C3920633](https://www.lcsc.com/product-detail/C3920633.html)|0201|7.68k 0201 Thin Film Surface Mount Fixed Resistor +/-0.5% 0.031W CPF0201D7K68C1|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2404081048_TE-Connectivity-CPF0201B511RE1_C3920633.pdf)|
|C1-EP-DR|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|C24, C39|[C9900179830](https://www.lcsc.com/product-detail/C9900179830.html)|402|0402 (1005 Metric)|N/A|
|L2|[C12669](https://www.lcsc.com/product-detail/C12669.html)|402|Generic chip inductor|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_Murata-Electronics-LQG15HS27NJ02D_C12669.pdf)|
|C1, C2, C17, C18|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|L3|[C12669](https://www.lcsc.com/product-detail/C12669.html)|402|Generic chip inductor|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_Murata-Electronics-LQG15HS27NJ02D_C12669.pdf)|
|C3, C4|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|C29, C30, C31, C32, C37, C38|[C3920633](https://www.lcsc.com/product-detail/C3920633.html)|0201|7.68k 0201 Thin Film Surface Mount Fixed Resistor +/-0.5% 0.031W CPF0201D7K68C1|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2404081048_TE-Connectivity-CPF0201B511RE1_C3920633.pdf)|
|EPD_C1, EPD_C2, EPD_C6, EPD_C7, EPD_C8, EPD_C9, EPD_C10, EPD_C11, EPD_C12|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|R_TYPE_SEL|[C3920633](https://www.lcsc.com/product-detail/C3920633.html)|0201|7.68k 0201 Thin Film Surface Mount Fixed Resistor +/-0.5% 0.031W CPF0201D7K68C1|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2404081048_TE-Connectivity-CPF0201B511RE1_C3920633.pdf)|
|SW_DN, SW_ENT, SW_UP|[C569760](https://www.lcsc.com/product-detail/C569760.html)|SMD,3.9x2.9mm|-40℃~+85℃ 1.6N 1.6mm 15V 2.9mm 20mA 3.9mm 500,000 Cycles IP67 J-Lead Rectangular Button SPST Surface Mount,Vertical White With Bracket SMD,3.9x2.9mm Tactile Switches ROHS|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2301111010_PANASONIC-EVPAKE31A_C569760.pdf)|
|Q1|[C2564](https://www.lcsc.com/product-detail/C2564.html)|TO-220AB|-55℃~+175℃ 1 P-Channel 180nC@10V 200W 20mΩ@10V 3.4nF 4V 55V 640pF 74A P-Channel TO-220AB MOSFETs ROHS|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_1809041724_Infineon-Technologies-IRF4905PBF_C2564.pdf)|
|C25, C33|[C9900179830](https://www.lcsc.com/product-detail/C9900179830.html)|402|0402 (1005 Metric)|N/A|
|ANT1|[C2917717](https://www.lcsc.com/product-detail/C2917717.html)|1206|-45℃~+125℃ 0.5dBi 1.3mm 1.6mm 100MHz 2.45GHz 2W 3.2mm 50Ω Patch Antenna 1206 Antennas ROHS|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2404021210_Johanson-Dielectrics-2450AT18B100E_C2917717.pdf)|
|L1|[C12669](https://www.lcsc.com/product-detail/C12669.html)|402|Generic chip inductor|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_Murata-Electronics-LQG15HS27NJ02D_C12669.pdf)|
|X2|[C32346](https://www.lcsc.com/product-detail/C32346.html)|SMD3215-2P|-40℃~+85℃ 12.5pF 32.768kHz 70kΩ Crystal Oscillator ±20ppm SMD3215-2P Crystals ROHS|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2404180925_Seiko-Epson-Q13FC13500004_C32346.pdf)|
|X1|[C9009](https://www.lcsc.com/product-detail/C9009.html)|SMD3225-4P|-40℃~+85℃ 12pF 32MHz Crystal Oscillator ±10ppm ±20ppm SMD3225-4P Crystals ROHS|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2403291504_YXC-Crystal-Oscillators-X322532MOB4SI_C9009.pdf)|
|R17, R18|[C3920633](https://www.lcsc.com/product-detail/C3920633.html)|0201|7.68k 0201 Thin Film Surface Mount Fixed Resistor +/-0.5% 0.031W CPF0201D7K68C1|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2404081048_TE-Connectivity-CPF0201B511RE1_C3920633.pdf)|
|C43|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|C2-EP-DR|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|C6, C14, C20, C21|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|C16|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|J1|[C122434](https://www.lcsc.com/product-detail/C122434.html)|SMD,P=0.5mm,Surface Mount，Right Angle|FFC & FPC Connectors 0.5mm FPC RA SMT Dual Contact 24Ckt|[datasheet](https://www.molex.com/content/dam/molex/molex-dot-com/products/automated/en-us/salesdrawingpdf/503/503480/5034802400_sd.pdf)|
|R1_USB, R2_USB|[C3920633](https://www.lcsc.com/product-detail/C3920633.html)|0201|7.68k 0201 Thin Film Surface Mount Fixed Resistor +/-0.5% 0.031W CPF0201D7K68C1|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2404081048_TE-Connectivity-CPF0201B511RE1_C3920633.pdf)|
|L5|[C1329646](https://www.lcsc.com/product-detail/C1329646.html)|SMD,4.8x4.8mm|1.6A 1.6A 4.7uH 41.4mΩ AEC-Q200 ±30% SMD,4.8x4.8mm Power Inductors ROHS|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2304140030_BOURNS-SRR4828A-4R7Y_C1329646.pdf)|
|C9|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|IC3|[C189517](https://www.lcsc.com/product-detail/C189517.html)|LGA-12(2x2)|Accelerometers Triaxial low-g 12bit Acceleration Sensor|[datasheet](https://www.lcsc.com/datasheet/C189517.pdf)|
|IC1|[C3682423](https://www.lcsc.com/product-detail/C3682423.html)|DSBGA-8(1.1x1.6)|Charger IC Lithium Ion/Polymer, Lithium Iron Phosphate 8-DSBGA (1.6x1.1)|[datasheet](https://www.ti.com/cn/lit/ds/symlink/bq25180.pdf?ts=1775594237116)|
|IC2|[C81079](https://www.lcsc.com/product-detail/C81079.html)|DSBGA-9|Haptic Driver for ERM/LRA with Built-In Library and Smart Loop Architecture|[datasheet](https://www.ti.com/cn/lit/gpn/drv2605)|
|L7|[C5832368](https://www.lcsc.com/product-detail/C5832368.html)|1008|13mΩ 470nH 6.5A 7.5A ±20% 1008 Power Inductors ROHS|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2306021632_cjiang--Changjiang-Microelectronics-Tech-FTC252012SR47MBCA_C5832368.pdf)|
|TP (Test Pads)|N/A|N/A|Test pad|N/A|
|J4|[C709357](https://www.lcsc.com/product-detail/C709357.html)|SMD|-40℃~+85℃ 1 10,000 cycles 16P 30V 3A 7.81mm Female Surface Mount, Right Angle Type-C SMD USB Connectors ROHS|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2404191039_Shenzhen-Kinghelm-Elec-KH-TYPE-C-16P_C709357.pdf)|
|U2|[C2682616](https://www.lcsc.com/product-detail/C2682616.html)|DFN-8-EP(2x2)|-40℃~+85℃ 1 2.5V~4.5V 3uA I2C Lithium Battery DFN-8-EP(2x2) Battery Management ROHS|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2410121738_Analog-Devices-Inc--Maxim-Integrated-MAX17048G-T10_C2682616.pdf)|
|D2, D4, D5|[C82046](https://www.lcsc.com/product-detail/C82046.html)|SOD-123|ON SEMICONDUCTOR - MBR0530 - DIODE, SCHOTTKY, 0.5A, 30V, SOD-123|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2304140030_onsemi-MBR0530T1G_C82046.pdf)|
|C10, C13, C22|[C9900156064](https://www.lcsc.com/product-detail/C9900156064.html)|201|Generic chip capacitor|[datasheet](https://ds.yuden.co.jp/TYCOMPAS/or/download?pn=MLAST063SCG681JFNA01&fileType=CA)|
|U1|[C3606653](https://www.lcsc.com/product-detail/C3606653.html)|QFN-48(6x6)|nRF52840|[datasheet](https://www.lcsc.com/datasheet/C3606653.pdf)|
|IC9|[C7065276](https://www.lcsc.com/product-detail/C7065276.html)|WLCSP-15B(2.3x1.4)|Buck-Boost Regulator Positive Output Step-Up/Step-Down I2C DC-DC Controller IC 15-WL-CSP (BSC) (1.4x2.3)|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2312271436_Richtek-Tech-RT6160AWSC_C7065276.pdf)|
|Q3|[C469327](https://www.lcsc.com/product-detail/C469327.html)|SOT-323|MOSFET N-Ch 30V 1.5A TrenchFET SC70 Vishay Si1308EDL-T1-GE3 N-channel MOSFET Transistor, 1.5 A, 30 V, 3-Pin SC-70|[datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_1912202016_Vishay-Intertech-SI1308EDL-T1-GE3_C469327.pdf)|
|J2|[C90533](https://www.lcsc.com/product-detail/C90533.html)|P=1mm|CABLE ADAPTER 6 POS|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/1810141506_LX-FFC6P1-0mm7CM_C90533.pdf)|
|D3|[C2969755](https://www.lcsc.com/product-detail/C2969755.html)|SOT-23-6L|Low Cap. ESD Protection Auto SOT-23-6 STMicroelectronics USBLC6-2SC6Y, Dual Uni-Directional TVS Diode Array, 6-Pin SOT-23|[datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2211080730_STMicroelectronics-USBLC6-2SC6Y_C2969755.pdf)|


## Hardware Functionality & Technical Architecture

The **InkTime** platform is an ultra-low-power wearable built around the **Nordic nRF52840 SoC**. The design focuses on maximizing battery autonomy through an E-Ink interface and advanced power management, ensuring the device remains functional for weeks on a single charge.

### 1. Core Processing Unit
The **nRF52840 (ARM Cortex-M4F @ 64 MHz)** serves as the system's brain. It was selected for its:
* **Connectivity:** Native Bluetooth 5.4 LE support for smartphone syncing.
* **I/O Versatility:** Integrated USB, SPI, and I2C peripherals to manage all sub-systems.
* **Efficiency:** Advanced "Deep Sleep" modes (sub-10 µA) and a dedicated 32.768 kHz crystal for accurate low-power timing.

### 2. Power & Energy Management
The power tree is designed to extract maximum energy from the **250 mAh Li-Po battery**:
* **Charging:** A **BQ25180 PMIC** manages the CC/CV charging cycle via **USB-C**, providing overvoltage and thermal protection.
* **Regulation:** The **RT6160 Buck-Boost converter** maintains a stable **3.3V** rail even as the battery voltage drops toward 3.0V, outperforming standard LDOs.
* **Fuel Gauge:** The **MAX17048G** monitor provides high-precision State of Charge (SoC) data via I2C, allowing for accurate battery percentage alerts.

### 3. Peripherals and User Interface
* **E-Paper Display (1.54"):** Connected via a 24-pin FPC (SPI). It draws power only during refreshes, making it ideal for static data. A dedicated driving circuit with MOSFETs and Schottky diodes manages the necessary bias voltages.
* **Motion Sensing:** The **BMA423 IMU (I2C)** enables "wrist-tilt" wake-up and step counting, allowing the MCU to stay in sleep mode until motion is detected.
* **Haptic Feedback:** The **DRV2605 driver** handles the vibration motor (shaker), offloading PWM waveform generation from the MCU for crisp, customizable alerts.
* **User Input:** Three physical buttons (`SW_UP`, `SW_ENT`, `SW_DN`) provide a reliable navigation interface.

### 4. Power Profile & Autonomy
With an average current draw ($I_{avg}$) of approximately **180 µA** (combining deep sleep, sensor polling, and periodic display updates), the theoretical autonomy is:

$$T = \frac{250\text{ mAh}}{0.18\text{ mA}} \approx 1389\text{ hours}$$

In real-world scenarios, this translates to an estimated **10–14 days** of continuous operation.

## nRF52840 Signal Assignment & Connectivity

| Pin(s) | Peripheral | Function | Justification |
| :--- | :--- | :--- | :--- |
| **P0.02** | SPI SCK | Clock | SPI clock for the E-Ink display interface. |
| **P0.03** | SPI MOSI | Data | Master Out Slave In; sends pixel data to display. |
| **P0.05** | EPD CS | Chip Select | Active-low signal to enable SPI display communication. |
| **P0.15** | EPD DC | Control | Toggles between Data and Command modes for E-Ink. |
| **P0.16** | EPD RST | Control | Provides a hardware reset path for the display. |
| **P0.17** | EPD BUSY | Status Input | Hardware flag indicating active display refresh cycles. |
| **P0.06** | I2C SDA | Data | Serial Data line shared by IMU, Fuel Gauge, and Haptics. |
| **P0.07** | I2C SCL | Clock | Serial Clock line for the high-speed I2C bus. |
| **P0.08** | IMU INT1 | Interrupt | Primary motion/event trigger from BMA421/BMA423. |
| **P1.08** | IMU INT2 | Interrupt | Secondary interrupt line for advanced motion features. |
| **P0.09** | Fuel Gauge ALERT | Interrupt | Real-time battery status alert from MAX17048. |
| **P0.11** | PMIC INT | Interrupt | Fault or charging status update from BQ25180. |
| **P0.12** | HAPTIC_EN | Control | Master enable signal for the DRV2605 haptic driver. |
| **P0.13** | Button UP | GPIO Input | Digital input for the 'Up' navigation switch. |
| **P0.14** | Button ENTER | GPIO Input | Digital input for the 'Enter/Select' switch. |
| **P1.02** | Button DOWN | GPIO Input | Digital input for the 'Down' navigation switch. |
| **P0.18** | nRESET | Reset | System hardware reset (Reset pin). |
| **D+ / D-** | USB Interface | USB Data | Dedicated lines for USB communication and charging. |
| **SWDIO** | Debug Port | Data | Serial Wire Debug bidirectional data line. |
| **SWDCLK** | Debug Port | Clock | Serial Wire Debug clock reference. |

## Design Log & Validation

### 1. Engineering Decisions
* **Density:** Used **0201 passives** and **1.0 mm PCB thickness** to fit all 49 components on the **TOP layer** within the compact enclosure.
* **RF Performance:** Maintained a strict **copper-free keep-out zone** under the 2.4 GHz antenna and used **via stitching** to stabilize the ground planes.
* **Routing:** Power lines are **0.3 mm** for stability, while data lines are **0.15 mm**. Decoupling caps are placed within **0.5 mm** of IC pins to minimize noise.

### 2. Approved Errors (DRC & ERC)
The following warnings were manually verified and intentionally accepted:

| Error Type | Reason for Approval |
| :--- | :--- |
| **DRC: Dimensions** | Button and USB-C placement is fixed by the **mechanical cutouts** of the 3D-printed case. |
| **DRC: Overlap** | Caused by **via-in-pad / escape routing** (0.15mm vias). Necessary for the dense fanout of the nRF52840. |
| **ERC: Input Pins Only** | Verified manually; all nets are functionally connected despite the CAD warning. |
| **ERC: Power Pins** | Confirmed that all supply rails (3V3, VBAT) are correctly routed to their regulators. |


