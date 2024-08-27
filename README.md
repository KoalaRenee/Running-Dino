# Setup From Fresh Jetpack 4.6.1 Installation
## Introduction
The Dinosaur Game is a built-in browser game in the Google Chrome Web Browser and was created by Sebstien Gabriel in 2014. This project is a program where you can use your own body as a controller to play this game. With the use of AI model - Yolov5, this program can detect the change of the length of your torso
## Aim
> Physical Activity and Fitness
- Interacting with the game through physical movements could turn it into a form of interactive exercise or gaming. This could make the experience more engaging and encourage physical activity, which can be beneficial for physical and mental health.
> Cognitive and Motor Skill Development
- Coordinating the physical movements with the game's actions can help players improve their hand-eye coordination, reaction time, and spatial awareness.
- The cognitive demands of recognizing and responding to the game's events through physical actions can also contribute to the development of cognitive skills, such as attention, decision-making, and problem-solving.
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
1. Download playground.py
2. Move playground.py to tensorrtx/yolov5/
3. Run playground.py
4. Test your camera by opening camera_test.ipynb
5. Run Chrome Dino in GOOGLE CHROME
   ```
   chrome://dino/
   ```
