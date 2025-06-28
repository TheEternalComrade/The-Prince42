---
title: "The Prince42"
author: "@ayo"
description: "A wireless low profile, split keyboard"
created_at: "2024-06-27"
---
## June 27, 2025
This keyboard is based upon my er.. endeavors to make the Prince54. Imma be real, it kinda sucks. I made so many mistake and oversights. But, what does't kill us makes us stronger? Lets hope nothing goes wrong this time.

I'm going to handwire this board. Why? Because it makes replacing a broken microcontroller(4 broke with the Prince54) much easier. Also, I ain't tryna bankrupt Hack Club with the pcb cost. I'm trying to make this board as affordable as I can.

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

## June 28, 2025
I spent a lot of timing figuring out a compact tenting solution. After some research, I think I'll settle on something like these.
![image](https://github.com/user-attachments/assets/31606ef8-f5a2-4467-9985-42b1f31a15c8)
![image](https://github.com/user-attachments/assets/b457f1f2-e7be-41ab-86f5-9cdb678deb1d)


So, I'm going to be using 2 Nice!Nano clones as microcontrollers for this keyboard
