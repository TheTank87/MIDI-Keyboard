# MIDI-Keyboard
A board to create my own beats, to make it mine, I will add my own doodles.
<img width="776" height="468" alt="Screenshot 2026-10-24 at 4 33 40 PM" src="https://github.com/user-attachments/assets/a2bff2dc-7f56-494e-81e2-a0f46e2be30e" />

This is the MIDI Keyboard. It is a small hand-held device that creates musical sounds in the right hands. It uses capacitative touch keys, buttons, switches, and a rotary knob. It also includes SK6812 MINI-E Neopixels that light up whenever I press those keyboard buttons. It also includes that USB plugin brain thing from the Starbie, but this time it's a little bit more powerful, featuring the waveshare.

# Features
* EC11 Rotary Encoders
* SK6812 MINI-E Neopixels
* Bourns Slide Potentiometers
* Kailh Choc Low-Profile Switches

# BOM
|Designator|Footprint|Quantity|Value|Total Cost|Links|
|----------|---------|--------|-----|----------|-----|
|D1, D2, D3|LED_SK6812MINI-E_3.2x2.8mm_P1.5mm_ReverseMount|3|SK6812MINI-E|$3.36|[Link](https://www.aliexpress.us/item/3256807677321116.html?spm=a2g0o.productlist.main.7.607a1c3clvX5x9&algo_pvid=bee2faba-4c6b-4fa4-89c4-5ca66e556568&algo_exp_id=bee2faba-4c6b-4fa4-89c4-5ca66e556568-6&pdp_ext_f=%7B%22order%22%3A%22643%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21CAD%215.30%214.88%21%21%213.65%213.36%21%402101e81117919481938394582e0f6e%2112000042594617264%21sea%21US%213725344934%21X%211%210%21n_tag%3A-29919%3Bd%3Ae2161723%3Bm03_new_user%3A-29895%3BpisId%3A5000000219770668&curPageLogUid=ehnx03TU7wEm&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007863635868%7C_p_origin_prod%3A)|
|J1|Capacitative Keys|1|Capacitative Touch Buttons|||
|RV1, RV2|Potentiometer_Bourns_PTA1543_Single_Slide|2|Slider|$3.16|[Link](https://www.digikey.com/en/products/detail/bourns-inc/PTA1543-2010CIB103/3781161)|
|SW1, SW2, SW3|Kailh Choc Low-Profile Switches|3|SW_Push|$6.04|[Link](https://www.aliexpress.com/item/1005008883418065.html?spm=a2g0o.productlist.main.1.13d14a7e068OmL&algo_pvid=4e5fe6cd-3562-4ef4-ac3e-085a2d4634fe&algo_exp_id=4e5fe6cd-3562-4ef4-ac3e-085a2d4634fe-0&pdp_ext_f=%7B%22order%22%3A%221475%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21CAD%2111.40%212.38%21%21%217.81%211.63%21%402103128917919263557114360e0ebd%2112000047082945007%21sea%21CA%210%21ABX%211%210%21n_tag%3A-29910%3Bd%3A778dde27%3Bm03_new_user%3A-29895%3BpisId%3A5000000218640848&curPageLogUid=CXjsh9TOCyFt&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008883418065%7C_p_origin_prod%3A)|
|SW4|RotaryEncoder_Alps_EC11E-Switch_Vertical_H20mm|1|RotaryEncoder_Switch_MP|$1.44|[Link](https://www.aliexpress.us/item/3256807457768762.html?spm=a2g0o.productlist.main.1.52d22c6as0ZCnv&algo_pvid=9965a6c7-9d4c-44f9-a2d4-a43aa1b0ae45&algo_exp_id=9965a6c7-9d4c-44f9-a2d4-a43aa1b0ae45-0&pdp_ext_f=%7B%22order%22%3A%224739%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21USD%211.52%211.40%21%21%211.52%211.40%21%402101e7a317919489056767943e0e88%2112000041630839409%21sea%21US%213725344934%21X%211%210%21n_tag%3A-29919%3Bd%3A1bb91aa6%3Bm03_new_user%3A-29895%3BpisId%3A5000000219770668&curPageLogUid=AOe3dpbqRVrY&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007644083514%7C_p_origin_prod%3A)|
|U1|Waveshare ESP32-S3-Zero|1|Waveshare ESP32-S3-ZERO|$6.62|[Link](https://www.aliexpress.com/item/1005007004089798.html?src=google&gatewayAdapt=4itemAdapt)|
|||Total Parts Cost|$17.46||
|||Total Digikey Cost-Not using fast shipping|$8.67||
|||Total JLCPCB|$12.20||
|||Total Cost|$38.33||

# Process:
<img width="1012" height="534" alt="Screenshot 2026-10-23 at 12 02 36 PM" src="https://github.com/user-attachments/assets/1480e497-b76f-419c-af2f-a73459ccf5cd" />

I started with the schematic design of my PCB and wired up everything using the guide as reference. However, I did make a mistake of accidentally swapping the TX and RX ports so I fixed that asap.
<img width="740" height="171" alt="Screenshot 2026-10-23 at 4 56 44 PM" src="https://github.com/user-attachments/assets/7ab3ac1f-b125-4471-924f-8586148ff675" />

After that as fixed, I then went into the PCB editor and created my first design.
<img width="1012" height="534" alt="Screenshot 2026-10-23 at 11 55 53 AM" src="https://github.com/user-attachments/assets/1343e66f-20fc-4bfe-ada4-2fb643c81be1" />

However, there was a major flaw in this design, that is, the wiring of the waveshare was not efficient and the entire layout was doomed to be messy. So I had to go back the schematic editor and redo the wiring so that it fits with a better layout.
<img width="776" height="468" alt="Screenshot 2026-10-24 at 4 33 40 PM" src="https://github.com/user-attachments/assets/8d7a2599-b783-4eb5-866f-6d2a85521d26" />

As one can see, everything now wires up more cleanly. Insert crying emoji...
