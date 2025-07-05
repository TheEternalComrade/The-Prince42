---
title: "The Prince42"
author: "@ayo"
description: "A wireless low profile, split keyboard"
created_at: "2024-06-27"
---
### Total time spent: 16 hours
## June 27, 2025
This keyboard is based upon my er.. endeavors to make the Prince54. Imma be real, it kinda sucks. I made so many mistake and oversights. But, what does't kill us makes us stronger? Lets hope nothing goes wrong this time.

I'm going to handwire this board. Why? Because it makes replacing a broken microcontroller(4 broke with the Prince54) much easier. In fact, it makes replacing everything easier(except maybe keycaps). Also, I ain't tryna bankrupt Hack Club with the pcb cost. I'm trying to make this board as affordable as I can.

In addition, this keyboard will be wireless cause it's just more convenient.

Now, this is the part where I justify some of my more "basic" design choices.

### Why no led?
They draw more power. Plus, I don't particularly care for the effect.

### Why no oled?
Also draws more power. Having one gives more reason to look at the boards when typing, which is a big no-no when it comes to touch typings.

(Also, both of the previous cost more money.)

While an oled could be useful for indicating layer and the like, I think it would be more useful to create firmware that creates a popup at the change, like so:
![image](https://github.com/user-attachments/assets/5b52fa8e-0bbf-4b7a-8015-38912b0aa48b)

On to the designing!
Here's a photo of my layout
![image](https://github.com/user-attachments/assets/6f637538-ed53-4dda-878b-5488ec5c6f96)

I did take some inspiration from the Corne on this layout.

Tommorrow, I'll work one the case and wiring.

Time spent: 1 hour

## June 28, 2025
I spent a lot of timing figuring out a compact tenting solution. After some research, I think I'll settle on something like these:
![image](https://github.com/user-attachments/assets/31606ef8-f5a2-4467-9985-42b1f31a15c8)
<i>https://imkulio.com/build-guide.html</i>

![image](https://github.com/user-attachments/assets/b457f1f2-e7be-41ab-86f5-9cdb678deb1d)
<i>https://kriscables.com/product/corne-cherry-tenting-case-kit/</i>

I'm going to be using 2 Nice!Nano clones as microcontrollers for this keyboard. I'm also adding a slide switch so I can cut off power and preserve battery when not in use. Here are the wiring diagrams:
![image](https://github.com/user-attachments/assets/9181c307-5418-44a2-a3bd-ab242bf50409)
![image](https://github.com/user-attachments/assets/6ce1fec0-73e3-40c5-8b7c-b2074254437c)

I experimented a bit with the thumb cluster on the Prince54, and decided that it would be a good idea to shift the thumb cluster a little bit closer to the other keys.
![image](https://github.com/user-attachments/assets/6de886cd-e504-48b3-9bb9-7544d7c5de3e)

Next, i'll make the plate.

Time spent: 1 hour

## June 29, 2025
I imported a dxf of my plate in to fusion 360. This is what I've got so far:
![image](https://github.com/user-attachments/assets/84dd3b3e-7bf6-4797-a502-7fcd25a5a3ea)

Designing the case will be a little harder than I thought, as there is no pcb to design it around. But, this also means less limitations!

Time spent: 1 hour

## June 30, 2025
At work, I drew some sketches of how the microntroller would be mounted![20250630_141002](https://github.com/user-attachments/assets/3050a7af-cbdd-451e-86b7-cec8de6645a3)

I was originally going to use header pins on the microntrollers, then I saw a design with none and realized I could essential use the matrix wires as header pins.

I designed the barebones for the bottom part and plate of my pcb.
![Screenshot 2025-06-30 220742](https://github.com/user-attachments/assets/c3a44c24-824e-4ef8-ad50-db289ed3fd34)
![image](https://github.com/user-attachments/assets/e28b316c-e569-4c10-b700-fefd680e210b)

I'll mostly remove parts from the plate to make room for the microcontroller and microcontroller cover. 

Time Spent: 2 hours

## July 2, 2025
I added keycaps and switches!
![Screenshot 2025-07-01 232804](https://github.com/user-attachments/assets/d0d6bd6b-92e2-4618-af66-a0a15f38ba19)

In addition, on the underside of my switch plate I made a 1mm offset around each switch and made those areas 1.2 mm thick, the thickness needed for the Gateron ks-33 switches to snap in.
![image](https://github.com/user-attachments/assets/12d3dd97-ef87-46c3-b2c2-8c6861905a21)

I think having a cover for the microcontroller on this case would be really cool, so this is what I have so far:
![image](https://github.com/user-attachments/assets/65bab1f7-eddd-4183-82ae-b1706822b0c4)
I wanna use the m2 x 10 screws I have on hand, instead of getting a different length, so I might need to raise the screw hole. 

Time Spent: 2 hours

## July 3, 2025
Today I worked on the microcontroller cover, the tenting solution, and the slide switch placement.

Generally speaking, laying your hands flat while typing isn't the most optimal position. In fact, our hands naturally tend to want to be on their sides. So, with tenting, your hands can lay in a more natural and ergonomic position. I considered many different tenting options, but ultimately, I decided that using screws would be the best option, it's very compact, and it's pretty cheap.
![image](https://github.com/user-attachments/assets/aa8ca6ca-e3fd-44c8-a8c9-5890c9168122)

I'm using a ss12f15 slide switch. This will allow me to turn off the keyboard halves when I'm not using them and conserve energy.
![image](https://github.com/user-attachments/assets/ca8d2747-9b30-490a-8fa7-7598589fbfc7)

Time spent: 3 hours

## July 4, 2025
We're almost there! I've more or less finished the cad part of this project and added some branding.
![image](https://github.com/user-attachments/assets/c4145c90-716c-4d77-834b-ae748b4c9a62)

I also spent some time considering whether or not I wanted to add a [cirque trackpad](https://bastardkb.com/wp-content/uploads/2023/09/IMG_1087-2-scaled.jpg) to my keyboard. Unfortunately, ZMK doesn't have native support for it and a mini trackpad would be kinda finicky to use.

Time Spent: 2 hours

## July 5, 2025
Now, we make the firmware:
![image](https://github.com/user-attachments/assets/56a8cc50-a569-4b36-afa5-e540da7f466b)

Contrary to seemingly common sentiment, the ZMK docs were extremely useful for making my firmware, along with Joe Scotto's firmware guide.

Of course, while compiling my firmware I ran into quite a few errors:
![image](https://github.com/user-attachments/assets/ba63e64f-07af-4243-929b-10392d401811)

But it was really easy to figure out with ZMK's troubleshooting guide.

So, my firmware is done!!! Which means the Prince42 is done! For now...
![image](https://github.com/user-attachments/assets/d3c4d604-b6b8-4212-ad8c-6bd2fda50d6a)


Time Spent: 4 hours

