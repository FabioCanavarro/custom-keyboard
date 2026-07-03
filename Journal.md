# Journal

## Brainstorming (July 2nd)

Spend around 1 hour brainstorming (with my brother and my friend lmao) about the features that my keyboard will have:

1. A macro column on the left side

Having a dedicated column of 5 macro keys on the far left side of the board would give me the ability to use shortcuts easily lmao.

> I havent actually seen many keyboards that have this kind of macro key, but i do remember the small device that is like a board?

2. A column isolated just for a display and a rotary encoder on the most right side

Where and why it is use?

- 0.91" SSD1306 OLED Display on the top of the column, displaying any one of these things (ex: Music visualizer, hardware data like temperature or usage, or timer) 

- EC11 Rotary Encoder, position either above or below the screen, it can be rotated infinitely and it has a built-in push-button (so I don't need to waste board space on a separate physical button). It will most likely be used for cycling menus in the OLED display.

> Honestly I am most excited for the music visualizer 

3. Physical Aesthetics & Switches

- Aesthetic: I am going for a sleeker catppuccin mocha kind of look on my keyboard

- Switches: High-quality Tactile/Linear switches (e.g., Boba U4T or similar).

> I love the sound of linear switches, but I still yearn for the distinct physical bump felt when pressing tactile switches.

- Keycaps: White blank DSA keycaps (?)

- Underglow: SK6812 MINI-E addressable RGB LEDs for a subtle ambient glow.

> Damn formatting all my thoughts into 1 clear information really took around 10 mins sheesh.

---

## The physical Layout design (July 2nd)

> Aint no way i just spent 1+ hour on something as simple as this bro 😭🥲

### 1st prototype 

<img width="1187" height="467" alt="image" src="https://github.com/user-attachments/assets/d7e419f2-c18e-44cb-bcd0-c2af9bd134be" />

> I think I nailed the catppuccin aesthetics, but idk how
> Btw I forgot to upload it here the 1st prototype, since I normally send it to my whatsapp for storage... 😅

### Final draft (?)

<img width="1188" height="463" alt="image" src="https://github.com/user-attachments/assets/bf3cc242-4457-4134-ad38-d62d5d8173f5" />

> OLED Screen is not to scale (Idk how to get the measurement of 0.91")

> I feel like the 1st prototype had too little colour variation, and also I forgot to add the Oled display, and I also edited the keys label (?) to be in various locations depending on the location of each individual key lmao

---

## Designing the PCB (July 2nd and 3rd)

<img width="2558" height="1598" alt="image" src="https://github.com/user-attachments/assets/8654a598-c914-4b94-8352-ddfbb7e4e727" />

> I just got the 4 basic thing placed and installed some plugins along the way heheheh

<img width="2558" height="1598" alt="image" src="https://github.com/user-attachments/assets/6c728a69-4faf-4a3b-934a-d4678aaa3ec5" />

Its been 32 Minutes

> I Finished it halfway then I realized, I was placing buses and not wires, that's why it wasn't connecting...

<img width="2558" height="1598" alt="image" src="https://github.com/user-attachments/assets/22f280f1-4e0f-4693-81a2-019550323794" />

> Its the day after, I added some things in 5 minute, I shall put it here to start the time recording of today lmao

<img width="2558" height="1598" alt="image" src="https://github.com/user-attachments/assets/d84fac1d-e2bc-49d2-bcb5-70f4affd049a" />

> Updated footprint and updated pcb from schematic

<img width="2558" height="1598" alt="image" src="https://github.com/user-attachments/assets/361e601b-7097-4a81-adac-cf4f0c7330b5" />

> Just realized I got 73 keys not 80...

<img width="2557" height="1598" alt="image" src="https://github.com/user-attachments/assets/624799bc-d01b-4e5f-86eb-147ad79fd53b" />

> Since kicad-kbplacer is allowed

<img width="273" height="198" alt="image" src="https://github.com/user-attachments/assets/b1c6c739-0e94-4094-9150-26ec9ff3d9f2" />

> I used kicad-kbplacer to speed up the placing of the keys with little to no error, then comes the hard part, I did not know how much gap to give anything. So I firstly tried to put it however I see fit, then after trying a lot of measurement, I realized all this time, I could've just used the ruler tool and alter the specific x,y coordinates instead of using my intuition...

<img width="2558" height="1598" alt="image" src="https://github.com/user-attachments/assets/164b28e4-5fcb-4d04-a7ee-4ce6067c0df3" />

> I finally routed everything, like my schematic was wrong from the very beginning, I didn't account for the fact that some keys took more space than others in the same row, leading to less keys in the row
