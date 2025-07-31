---
title: "Loop"
author: "Ayaan Grover"
description: "Loop is a compact MP3 player that's designed to be simple and portable."
created_at: "2025-07-12"
---

# Journal: Loop - 41 hrs

## July 12, 2025 - 3 hrs
Did a bit of plannning and research today. Here's what i ended up with:

### Parts:
- TF player
- TP4056/similar
- lipo
- audio jack
- maybe a speaker
- buttons
- case
- pcb to hold everything

most parts are cheap and can be sourced from aliexpress if needed. tf player is really good because no mcu is needed, just load the songs on (up to 32gb) and it can play them and skip and stuff.

## July 13, 2025 - 4 hrs
Did a lot of work today. It was very painful to get a lot of the symbols and footprints and i made a couple of my own. also did more research to see if i could make the tf player or tp4056 myself but the costs from PCBA would be too much. 

eventually got everything into kicad(it keeps crashing because i'm on the mac beta). did a basic layout(no wiring yet) and it looks good!

<img width="1059" height="429" alt="CleanShot 2025-07-13 at 18 38 11" src="https://github.com/user-attachments/assets/f88836a2-7640-4bfb-b6b8-5cab6ce41e36" />

Also made a PR to the highway repo with my project info.

## July 14, 2025 - 3 hrs
Spent a ton of time figuring out the wiring. i have everything except the TRRS jack because the datasheet is really useless...but i did the wiring in the schematic so it technically is working now(i think).

## July 15, 2025 - 2 hrs
spent some time figuring out the TRRS jack, got some help from friends, and i have what i think may be the correct way to do this. it looks right but i'll have to check again later. i also figured out that i'm not going to have an extender for the b+/b- because i dont know what size traces to put and i would rather not mess it up. Also decided to not add spdt a switch for speaker/headphones. i can leave the headphone jack on always and you can add speakers yourself. so i just added a spdt which im using as an spst for the power.

## July 15 - 5 hours
did the layout and wiring and redid it multiple times and now i feel good about it. took so long bc i kept moving stuff around...at least its done now

## July 16 - 4 hrs
made some of the case, used fusion and tinkercad(easier to move stuff and subtract stuff). going to make it look nice later, right now it's just an enclosure. also i didnt add any anchoring points yet.

## July 16 - 5 hrs
redid the case - made the case like a sleeve that you slide onto it for travel and a hook you can close it with, maybe using tpu?

## July 17 - 3 hrs
made a hybrid of the two prev case versions where the sleeve is for the holder for the pcb.

<img width="278" height="358" alt="CleanShot 2025-07-31 at 14 47 53@2x" src="https://github.com/user-attachments/assets/9de23922-42fd-4bba-8f12-17cc740ec7ad" />


## July 29 - 3 hours
edited the previous version of the case, uses tiny magnets now - its a desk mp3 player so no need for stability. cleaned it up in fusion and made a quick render.

## July 30 - 5 hours
redid the case bc it looked ugly before. now it uses screws instead of magnets and looks better. cleaned it up in fusion

also remade the renders. split the components and the pcb this time so it looks cool. 

also cleaned it up in figma for the readme. now it has a nice cover image.

also did some budget stuff:

## Parts List

| Component | Source | Price |
|-----------|--------|-------|
| DFPlayer | Amazon | $10 |
| TP4056 | AliExpress | $2 |
| M2 Screws | Aliexpress | $2 |
| M2 Heatset Inserts | Aliexpress | $2 |
| LiPo Battery | Amazon (900mAh) | $8 |
| Audio Jack | LCSC | $0.50 + $11 shipping |
| Buttons (x3) | LCSC | $0.60(same shipping as the audio jack) |
| Resistors | LCSC | $1.41(same shipping as the audio jack) |
| Speaker (x2) | Adafruit | $15 |
| PCB | JLCPCB | $31 |
| Case | Printed via Hack Club `#printing-legion` | Free |

**Total: $83.51**

## July 30 - 0.5 hr
made the readme!

## July 30 - 2 hrs
redid the pcb for an extra button using ADKEY1 and 3 resistors. now it has play/pause, next/volup, and prev/voldn.

## July 30 - 1 hr

polished the case and uploaded to github!

## July 30 - 0.5 hr

finished and submitted the project!