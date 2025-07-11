# Total time spent: 5 hours
---
title: "Smart Business Card"
author: "Veracles"
description: "A business card for my personal site, and info, with a HID setup so they can access my website with a button push"
created_at: "2025-07-08"
---
# July 8th
I created the schematic for the business card, and the MCU. I struggled a lot with the chip itself, because crystals (XTAL) have to be routed equally, which sucks. My initial plan was a XOR gate, but I think it would be noot complicated enough, so I'm swapping to a HID device on arduino atmega32u4, with buttons, because it honestly seems more fun.

![image](https://github.com/user-attachments/assets/79441aac-049e-4ca9-a3aa-d8622e377478)

Initial schematic, I fiddled a bit with a rasperry pi pico and Arduino Nano, but ultimately went with a normal MCU due to space requirements and my own ego. The initial plan was to make a bare MCU, but it ended up frustrating me because of the previously mentioned crystal issue, so I tried to go with a devboard, but they were either too expensive or not complex enough technically for what I needed. I tried the Arduino Nano, SMD edition, but it was too big for what I needed. I also did the Pico, but it didn't like me using the GPIO for data transfer for the USB-C, because, say with with me: **USB-C is evil, and my hatred for it is biblical**.
![image](https://github.com/user-attachments/assets/7fda69c2-bc3a-44b3-951f-6836dd878260)

Couldn't find a good USB c footprint so I had to use a different library, good lord USB-C is an evil format, for evil people. Honestly 

**Total time spent: 2 Hours**
# July 9th
I made the PCB, and got it wired up, I struggled with implementing ground planes, and you ccan see that the USB c pins are difficult because of the size of the traces I'm doing for the GND and +5v nets (to avoid a funny mistake) I'll add the silkscreen after I eat lunch. 

![image](https://github.com/user-attachments/assets/cc31b22b-bb01-434d-a8d9-a1fd6464dfc3)

Done! Lunch was very tasty, I spent a like 30 minutes on a silkscreen in inkscape, but lost all my footage, so I have the final result below, but I added the buttons and the details (my phone number is on there too, but I redacted for obvious reasons). It's easy enough to code, as each of the buttons is wired to a GPIO pin with a pull down resistor to the ground plane.

![image](https://github.com/user-attachments/assets/a4e2fa40-42b4-4a2f-9e81-9030aff01d96)

** Total Time spent: 5 Hours**
