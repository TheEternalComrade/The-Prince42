---
title: "The Prince42"
author: "@ayo"
description: "A wireless low profile, split keyboard"
created_at: "2024-06-27"
---
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


