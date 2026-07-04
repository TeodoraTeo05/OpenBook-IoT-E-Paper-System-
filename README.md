# OpenBook

## General Description

OpenBook is a portable e-book reader device based on the ESP32-C6. The device features an e-paper screen, control buttons, an environmental sensor, a real-time clock, and the ability to be powered by a Li-Po battery, designed as an energy-efficient and scalable system.
---

#### 1 Block Diagram

![Block Diagram](https://raw.githubusercontent.com/TeodoraTeo05/proiect-TSC/main/Images/diagrama.png)

---
## 2 BOM (Bill of Materials)

| Part | Device | Datasheet |
|------|--------|-----------|
| CHG_LED | ADAFRUIT_LEDCHIP-LED0603 | [ADAFRUIT_LEDCHIP-LED0603](https://www.snapeda.com/parts/KP-1608SURCK/Kingbright/view-part/?ref=search&t=LED%200603) |
| SJ1 | SJ | [SJ](https://grabcad.com/library/solder-jumpers-1) |
| EPD_C5 | EAGLE-LTSPICE_CC0402 | [EAGLE-LTSPICE_CC0402](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) |
| R3 | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | (https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) |
| R1_PWRUSB | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | (https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL) |
| C4_USB | EAGLE-LTSPICE_CC0402 | [EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| C1, C2, C6, C8, C9, C10, C_DELAY | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [ESP32_WROVER_EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| C3 | RCL_CPOL-EUCT3528 | [RCL_CPOL-EUCT3528](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| R1, R1_PINH, R1_PINH1, R2_PINH, R2_PINH1, R4, R5, R6, R7, R8, R9, R10, R_BOOT, R_CHANGE, R_CL1, R_RESET | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [ESP32_WROVER_EAGLE-LTSPICE_RR0402](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) |
| C7 | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [ESP32_WROVER_EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| J4 | 112A-TAAR-R03_ATTEND | [112A-TAAR-R03_ATTEND](https://store.comet.srl.ro/Catalogue/Product/43497/) |
| R_CAPACITOR | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [ESP32_WROVER_EAGLE-LTSPICE_RR0402](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) |
| C5 | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [ESP32_WROVER_EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| EPD_C6, EPD_C7, EPD_C8, EPD_C9, EPD_C10, EPD_C11, EPD_C12 | EAGLE-LTSPICE_CC0402 | [EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| EPD_C1, EPD_C2 | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [ESP32_WROVER_EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| R2 | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [ESP32_WROVER_EAGLE-LTSPICE_RR0402](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) |
| R1_BAT | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [ESP32_WROVER_EAGLE-LTSPICE_RR0402](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) |
| Q1, Q2 | ESP32_WROVER_SPARKFUN-DISCRETESEMI_MOSFET_PCH-DMG2305UX-7 | [ESP32_WROVER_SPARKFUN-DISCRETESEMI_MOSFET_PCH-DMG2305UX-7](https://componentsearchengine.com/part-view/DMG2305UX-7/Diodes%20Incorporated) |
| R2_BAT | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [ESP32_WROVER_EAGLE-LTSPICE_RR0402](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) |
| C5_USB | EAGLE-LTSPICE_CC0402 | [EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| C1_BAT, C1_BAT1, C1_BAT2, C2_BAT | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [ESP32_WROVER_EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| C4 | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [ESP32_WROVER_EAGLE-LTSPICE_CC0402](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) |
| R2-USB, R2-USB1 | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [ESP32_WROVER_EAGLE-LTSPICE_RR0402](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) |
| L1 | 744043680IND_4828-WE-TPC_WRE | [744043680IND_4828-WE-TPC_WRE](https://eu.mouser.com/ProductDetail/Wurth-Elektronik/744043680?qs=PGXP4M47uW6VkZq%252BkzjrHA%3D%3D) |
| IC1 | BD5229G-TR | [BD5229G-TR](https://componentsearchengine.com/part-view/BD5229G-TR/ROHM%20Semiconductor) |
| SENSOR2 | ESP32_WROVER_BME680_BME680 | [ESP32_WROVER_BME680_BME680](https://www.snapeda.com/parts/BME680/Bosch/view-part/?welcome=home) |
| BUTTON_CUSYOMV1 | BUTTON_CUSYOMV1 | [BUTTON_CUSYOMV1](https://industry.panasonic.com/global/en/products/control/switch/light-touch/number/evqpuj02k) |
| C10_SUPERCAP | CPH3225A | [CPH3225A](https://www.snapeda.com/parts/CPH3225A/Seiko+Instruments/view-part/?ref=snap) |
| U3 | DS3231SN# | [DS3231SN#](https://www.snapeda.com/parts/DS3231SN%23/Analog+Devices/view-part/?ref=snap) |
| U2 | ESP32-C6-WROOM-1-N8 | [ESP32-C6-WROOM-1-N8](https://www.snapeda.com/parts/ESP32-C6-WROOM-1-N8/Espressif+Systems/view-part/?ref=eda) |
| PFMF.050.1 | ESP32C6_VARISTORCN1812 | [ESP32C6_VARISTORCN1812](https://www.mouser.co.uk/ProductDetail/EPCOS-TDK/B72520T0350K062?qs=dEfas%2FXlABIszF52uu7vrg%3D%3D) |
| D2, D7 | ESP32_WROVER_AVX---SD0805S020S1R0_AVX_SD0805S020S1R0_0_0AVX_SD0805S020S1R0_0_0 | [ESP32_WROVER_AVX---SD0805S020S1R0_AVX_SD0805S020S1R0_0_0AVX_SD0805S020S1R0_0_0](https://eu.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0?qs=jCA%252BPfw4LHbpkAoSnwrdjw%3D%3D) |
| U5 | ESP32_WROVER_SPARKFUN-IC-POWER_MCP73831 | [ESP32-C6-WROOM-1-N8](https://componentsearchengine.com/part-view/MCP73831T-2ATI%2FOT/Microchip) |
| J1 | FH34SRJ-24S-0.5SH_99_ | [FH34SRJ-24S-0.5SH_99_](https://componentsearchengine.com/part-view/XC6220A331MR-G/Torex) |
| U4 | MAX17048G+T10 | [MAX17048G+T10](https://www.snapeda.com/parts/MAX17048G+T10/Analog+Devices/view-part/?ref=snap) |
| D3, D4, D5 | MBR0530 | [MBR0530](https://www.snapeda.com/parts/MBR0530/Onsemi/view-part/?ref=snap) |
| D6, D8, D9, D10, D11, D12 | PGB1010603MR | [PGB1010603MR](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=snap) |
| J3 | QWIIC_CONNECTORJS-1MM | [QWIIC_CONNECTORJS-1MM](https://www.snapeda.com/parts/PRT-14417/SparkFun%20Electronics/view-part/?ref=search&t=qwiic) |
| J2 | SAMACSYS_PARTS_USB4110-GF-A | (https://componentsearchengine.com/part-view/USB4110-GF-A/GCT%20(GLOBAL%20CONNECTOR%20TECHNOLOGY) |
| Q3 | SI1308EDL-T1-GE3 | [SI1308EDL-T1-GE3](https://componentsearchengine.com/part-view/SI1308EDL-T1-GE3/Vishay) |
| TP1, TP2, TP3, TP4, TP5, TP6, TP7, TP8, TP9, TP10, TP11, TP12, TP13, TP14, TP15, TP16, TP17 | TPTP20R | [made by me] |
| D1 | USBLC6-2SC6Y | [USBLC6-2SC6Y](https://www.snapeda.com/parts/USBLC6-2SC6Y/STMicroelectronics/view-part/?ref=snap) |
| U1 | W25Q512JVEIQ | [W25Q512JVEIQ](https://www.snapeda.com/parts/W25Q512JVEIQ/Winbond+Electronics/view-part/?ref=snap) |
| IC4 | XC6220A331MR-G | [XC6220A331MR-G](https://componentsearchengine.com/part-view/XC6220A331MR-G/Torex) |

## 3. Hardware Functionality

The OpenBook project is an e-paper reader, powered by a LiPo battery and built around the ESP32-C3-WROOM microcontroller. 
The device collects environmental data (temperature, humidity, CO2, particles), saves them to a microSD card, and can display them on the e-paper screen.

### ESP32-C3-WROOM
- Main module with Wi-Fi/BLE connectivity, capable of communicating via SPI, I2C, and UART.
- Supply voltage: 3.3V, provided by an LDO.

### Power System
- **USB-C** is used for charging and USB communication.
- **MCP73832** manages the LiPo battery charging.
- **3.3V LDO** powers the ESP32 and the rest of the components at 3.3V.
- **5V DC/DC** generates 5V for sensors that require a higher voltage (PM and CO2).

### Sensors
- **BME680** - temperature, humidity, and gas sensor, communicates via I2C.
- **MH-Z19B** - CO2 sensor powered at 5V, communicates via UART.
- **PMSA003** - fine particle sensor (PM2.5), communicates via UART, 5V.

### Display
- 1.5" monochrome e-paper display with 200x200 px resolution.
- Shared SPI interface with the SD Card.

### SD Card
- Module for storing collected data or text files.
- SPI interface.

### Buttons
- 3 tactile buttons connected to GPIO for interface control (e.g., menu navigation, screen refresh).

### Estimated power consumption calculations (average values)

| Module | Voltage | Current (mA) | Estimated Consumption |
|--------|---------|--------------|-----------------------|
| ESP32-C3 | 3.3V | 80-150 | 0.3-0.5W |
| E-Ink Display | 3.3V | 10 (refresh) | 0.03W |
| BME680 | 3.3V | 2-3 | 0.01W |
| MH-Z19B | 5V | 40-50 | 0.25W |
| PMSA003 | 5V | 60-100 | 0.5W |
| SD Card | 3.3V | 10 | 0.03W |
| MCP73832 (charger) | 5V | 1000 (max) | only when charging |

**Deep sleep mode:** Total consumption under 1 mA. Ideal for a portable device.

## 4. ESP32-C3 Pinout

| ESP32-C3 Pin | Component | Reason / Signal |
|--------------|-----------|-----------------|
| GPIO1 (I2C SDA) | BME680 | I2C Communication |
| GPIO2 (I2C SCL) | BME680 | I2C Communication |
| GPIO3 (UART RX) | PMSA003 | UART RX PM sensor |
| GPIO4 (SPI CS SD)| SD Card | SD Card Chip Select |
| GPIO5 | E-Ink DC | Data/Command E-Ink |
| GPIO6 (SPI CLK) | E-Ink & SD | SPI Clock |
| GPIO7 (SPI MOSI) | E-Ink & SD | SPI Data |
| GPIO8 (GPIO) | Button 1 | Menu control / page flip |
| GPIO9 (GPIO) | Button 2 | Menu control / page flip |
| GPIO10 (SPI CS) | E-Ink Display | e-paper Chip Select |
| GPIO11 (SPI CS) | External Flash (optional)| N/A |
| GPIO12 (USB D-) | USB | USB Communication |
| GPIO13 (USB D+) | USB | USB Communication |
| GPIO18 | MH-Z19B (UART TX) | UART for CO2 sensor |
| GPIO19 | Button 3 | Navigation / confirm |

## 5. Other relevant aspects

- The PCB design follows the recommendations for power traces (min 0.3mm) and signal traces (min 0.15mm).
- The ESP32-C3 antenna is placed towards the outside of the board, and the area underneath it is cut out.
- Decoupling capacitors are placed close to the VCC of the components.
- Solid ground plane on both layers and active via stitching.
- All passive components are SMD 0402.
- The layout is designed in Fusion360, aligned with the physical case dimensions.
- Rendered images of the device and case can be found in the `Images/` folder of this repository.
