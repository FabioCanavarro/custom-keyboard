# Custom Keyboard

My custom 65% mechanical keyboard designed from scratch for the Hack Club hardware grant.

| Phase | Date(s) | Time Spent |
| :--- | :---: | ---: |
| Brainstorming & Ideation | July 2 | 1 hr 0 mins |
| Physical Layout (KLE) | July 2 | 1 hr 10 mins |
| PCB Design (KiCad) | July 2 – July 4 | 5 hrs 59 mins |
| 3D Modeling (Onshape) | July 4 – July 5 | 4 hrs 25 mins |
| Total Build Time |  | 12 hrs 34 mins (15 hrs 34 mins, check notes below) |

> Note: Post submit, I realized I sent the wrong bom file so I made the bom file and updated the pcb art, I spent around 3 hours in total? (but I forgot to add photos, so Idk if it can be considered)

> Hours spent is based calculated based on the time difference of each screenshots, as normally I take one when starting and when ending.
> For more specific hours/day tracking, head over to the [Journal dump](journaldump.md) file

## Keyboard Layout

<img width="1188" height="463" alt="image" src="https://github.com/user-attachments/assets/bf3cc242-4457-4134-ad38-d62d5d8173f5" />

## Keyboard Case

### Top View

<img width="1832" height="991" alt="image" src="https://github.com/user-attachments/assets/8ed7ca7e-d78b-4324-8eff-a46c798eaff9" />

### Isometric View

<img width="1997" height="1285" alt="image" src="https://github.com/user-attachments/assets/cdccaf15-314e-4635-9ff7-f4d14c5ca76e" />

## PCB View

### With PCB Art

<img width="1695" height="1197" alt="image" src="https://github.com/user-attachments/assets/8cd16b0a-f5a0-403a-818e-45b9ab07b808" />

### Without PCB Art

<img width="1781" height="1216" alt="image" src="https://github.com/user-attachments/assets/8b9bb740-4016-429f-b014-bc645c83254e" />

## Schematic View

<img width="1935" height="1372" alt="image" src="https://github.com/user-attachments/assets/f3e76e18-473b-4cdf-a1f3-43f0efa12aa0" />

## Specs

- Brain: Raspberry Pi Pico (RP2040)

- Switches: Boba U4T

- Keycaps: Blank White DSA

- Forehead: 0.91" OLED screen + EC11 Rotary Encoder (knob)

- Colors: Catppuccin Mocha aesthetic

## What I built

I made a custom 65% layout with a 5-key macro column on the left (for dev shortcuts) and a "forehead" on the top right for an OLED screen and a knob.

For the case, I went with a 3D-printed tray mount design. It has a bottom tub with 6mm pillars for the PCB to sit on, and a 1.5mm top switch plate that drops right in. I also cut a window in the top plate to expose the Pico and leave room to wire up the OLED.

## Why I built it

I type a lot and wanted a board that actually fits my workflow. But mostly, I just wanted to figure out how hardware actually works. I know how to code, but I had no clue how physical switches turn into keypresses or how to use CAD without the physics engine yelling at me. I wanted to build the whole stack from the circuit board up to the plastic case.

## What I learned

This was a massive learning curve.

- I learned that MX switches need exactly 5mm of gap between the PCB and the switch plate to clip in properly. I almost crushed my Pico because I didn't account for the height of the header pins, which is why I ended up cutting a display window for it in the top plate so it could fit.

- When making the switch plate, I kept accidentally extruding 70 floating cubes instead of a solid plate. I learned how to use projection tools to draw a proper boundary wall around the keys so the software knows what's solid plastic and what's empty space.

- This project has also taught me a lot about Computer Aided Design, specifically in OnShape. 

## Next up

While the PCB and parts are shipping, I'm going to write the firmware in Rust using the RMK framework so I can get the OLED visualizer and knob working.
