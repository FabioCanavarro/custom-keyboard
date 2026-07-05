# Custom Keyboard

My custom 65% mechanical keyboard designed from scratch for the Hack Club hardware grant.

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
