# Business-card
A PCB business card with a USB-C port and HID, so when you press the button it auto opens a link to the website encoded on it.
I feel like in tech you really need to stand out when it comes to how you spread your information, so I decided to create a twist on the standard business card design by creating a HID business card to make employers expend that little bit of effort to remember me by.

![image](https://github.com/user-attachments/assets/414face4-cf9b-498a-b71b-05192e1e3dca)


![image](https://github.com/user-attachments/assets/19d87a04-eea6-475d-85ef-8c7d656f9caa)

![image](https://github.com/user-attachments/assets/7bf4250c-620a-48d8-84b8-7a45ad1ab25a)

### Bill of Materials

| Reference         | Qty | Value              | DNP | Exclude from BOM | Exclude from Board | Footprint                                                              | Datasheet                                                                                     |
|------------------|-----|--------------------|-----|------------------|--------------------|------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| C1, C2, C3, C4    | 4   | 1uF                |     |                  |                    | Capacitor_SMD:C_0201_0603Metric                                        | ~                                                                                             |
| C5               | 1   | 10uF               |     |                  |                    | Capacitor_SMD:C_0201_0603Metric                                        | ~                                                                                             |
| C6, C7           | 2   | 22pF               |     |                  |                    | Capacitor_SMD:C_0201_0603Metric                                        | ~                                                                                             |
| J3               | 1   | USB_C_Receptacle   |     |                  |                    | Connector_USB:USB_C_Receptacle_Amphenol_12401548E4-2A                  | [USB Type-C Spec](https://www.usb.org/sites/default/files/documents/usb_type-c.zip)          |
| R1               | 1   | 10k                |     |                  |                    | Resistor_SMD:R_0402_1005Metric_Pad0.72x0.64mm_HandSolder               | ~                                                                                             |
| R2, R3           | 2   | 22                 |     |                  |                    | Resistor_SMD:R_0201_0603Metric                                         | ~                                                                                             |
| R4, R5, R6, R7   | 4   | 10k                |     |                  |                    | Resistor_SMD:R_0201_0603Metric                                         | ~                                                                                             |
| R11, R12         | 2   | 5.1k               |     |                  |                    | Resistor_SMD:R_0201_0603Metric                                         | ~                                                                                             |
| RST1             | 1   | SW_Push            |     |                  |                    | Button_Switch_SMD:SW_Push_1P1T_NO_CK_KMR2                              | ~                                                                                             |
| SW1, SW2, SW3    | 3   | SW_Omron_B3FS      |     |                  |                    | Button_Switch_SMD:SW_SPST_Omron_B3FS-100xP                             | [Omron B3FS Datasheet](https://omronfs.omron.com/en_US/ecb/products/pdf/en-b3fs.pdf)         |
| U1               | 1   | ATmega32U4-A       |     |                  |                    | Package_QFP:TQFP-44_10x10mm_P0.8mm                                     | [ATmega32U4 Datasheet](http://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-7766-8-bit-AVR-ATmega16U4-32U4_Datasheet.pdf) |
| Y1               | 1   | Crystal_GND24_Small|     |                  |                    | Crystal:Crystal_SMD_0603-4Pin_6.0x3.5mm                                | ~                                                                                             |
