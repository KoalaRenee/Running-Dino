# Setup From Fresh Jetpack 4.6.1 Installation RUNNING DINO
## Introduction
The Dinosaur Game is a built-in browser game in the Google Chrome Web Browser and was created by Sebstien Gabriel in 2014. This project is a program where you can use your own body as a controller to play this game.
![6f68e50c-9a58-4826-b158-1eabf84d12d2 (1)](https://github.com/user-attachments/assets/b78bc92c-4025-4b03-abb2-fe045ad43f0f)
## About
This programme involves the use of yolov5 to detect your motion. We determine whether you are jumping or squatting (Dino: jump or bend over to avoid obstacles) by comparing the size of the square surrounding your whole body generated by yolov5. If the square is higher than a point, you will be considered as jumping. If the height of the square decrease but still stick with the floor, you will be considered as squatting. If you didn't do either action mentioned, you will be considered as "none" but your dino will still be jumping. It then uses the result to control the dino to play the game.

![4c8a5180-8bfd-468f-86eb-32bf5a847167](https://github.com/user-attachments/assets/9160d6a8-f3be-4587-bbe0-e58c3052b36b)
## Aim
> Physical Activity and Fitness
- Interacting with the game through physical movements could turn it into a form of interactive exercise or gaming. This could make the experience more engaging and encourage physical activity, which can be beneficial for physical and mental health.
> Cognitive and Motor Skill Development
- Coordinating the physical movements with the game's actions can help players improve their body coordination, reaction time, and spatial awareness.
- The cognitive demands of recognizing and responding to the game's events through physical actions can also contribute to the development of cognitive skills, such as attention and decision-making.
> Educational and Therapeutic Application
- The setup can be used in educational or therapeutic settings to teach topics like computer vision, machine learning, and human-computer interaction.
- The game can also be adapted for use in physical therapy or occupational therapy, helping patients improve their physical abilities and mobility.
## Install necessary package
- Install tensortx for yolov5 (2.0)
```
git clone -b yolov5-v2.0 https://github.com/wang-xinyu/tensorrtx.git
```
- Install yolov5 (2.0)
```
git clone https://github.com/ultralytics/yolov5.git
```
- Install pycuda for jetson nano
```
pip3 install pycuda --user
```
## Run the code
1. Connect jetson nano to your device
2. Download and run playground.py
3. Test your camera
   - Download the file camera_test.ipynb
   - Run the file in Jupyterlab by the following instruction
   ![2f59e540-6085-4b04-8d45-27f5b32cccee](https://github.com/user-attachments/assets/a6595bc4-4bcc-43bd-90bf-2ea03c369e32)
   Run from here
   ![270766ab-6201-4502-a578-6ce725e10da5](https://github.com/user-attachments/assets/b7de940f-6845-4285-96ae-c6eef0dddbdf)
   To here
   ![3fea16e2-89ea-49df-a3ce-8c2ba18e3c77](https://github.com/user-attachments/assets/81bd21b3-b6e1-402e-af26-24d3e0daf0b3)
   Then, you may see this window displaying.
   - After that, you may adjust your camera so that it can see your full body and the bottom edge of the window is lined with your feet. (This program ONLY allows ONE person to play, DON’T have more than ONE person standing in front of the camera)
   ![95037026-23a3-44bd-9c31-fa0065a38cfa](https://github.com/user-attachments/assets/aa8bc3a1-79b7-4fb4-9767-39c763daecb1)
   - Next, try jumping and squatting to test whether the camera can detect your motion. The text at the upper right corner will show your state (none is jumping, jump is jumping and knee is squatting)
   - If the camera can detect your motion correctly, your camera is ready for the game.
4. Run Chrome Dino in GOOGLE CHROME
   ```
   chrome://dino/
   ```
   
Enjoy the game!
