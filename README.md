# facemask-detection
## Data
this open resource model published 7971 images to train the models. The dataset is composed of WIDER Face and MAFA, we verified some wrong annotations. You can download here from Google drive, if you can not visit Google, you can download it from BaiduDisk, click here to know how to download.

## Model structure
We used the structure of SSD. However, in order to make it run quickly in the browser, the backbone network is lite. The total model only has 1.01M parametes.

Input size of the model is 260x260, the backbone network only has 8 conv layers. The total model has only 24 layers with the location and classification layers counted.

SSD anchor configurtion is show bellow:

multibox layers	feature map size	anchor size	aspect ratio）

<img width="551" alt="image" src="https://user-images.githubusercontent.com/92298865/165650865-56e3f2c0-7387-4d5e-a3e2-9753d3cb27e3.png">

## Testset PR curve
![image](https://user-images.githubusercontent.com/92298865/165651021-5954663c-c870-4f2e-ac38-6f872a831c16.png)
<img width="253" alt="image" src="https://user-images.githubusercontent.com/92298865/165718756-8258cd0b-c606-4b2f-ac2d-0b3ca0bbcae9.png">
## The Webpage
https://demo.aizoo.com/face-mask-detection.html

![1021651140443_ pic](https://user-images.githubusercontent.com/92298865/165729773-4256ce9a-cd0b-471e-a552-3b016c11d3e0.jpg)

## The Challenge
* How to enable the system to play the voice of the mask being worn
* How to make this page connect to other camers for remote viewing
## the change 
* As this open source software is only able to detect if a mask is being worn, but as I mentioned earlier, we would prefer to build a software that can do the persuasion function, so I have modified some of the code so that it can give timely persuasion when someone is not wearing a mask.
<img width="449" alt="image" src="https://user-images.githubusercontent.com/92298865/165718598-d96c388a-e51b-4af7-b4bb-cd8d723b3292.png">

## Difficutly
* This material builds a website where you can more quickly log in with your mobile or computer device and authorise the current device's camera for recognition. But I would prefer that the site could link to other devices' cameras so that we could get the data even from a remote location (possibly elsewhere in the office, where we can also see the lobby)
* This need to connected with the api
* *（It is worth noting that there is no need to add the "please waring masks" voice to the web page, as we would prefer to view it remotely when using the web））
## In fruture
* Enables websites to connect directly to other devices
* Make data connections to mqtt and grafana so that managers can not only see lobby videos, but also have easier access to visual data
## video
https://user-images.githubusercontent.com/92298865/165721681-126e3968-d768-44ed-93f2-3c3d17599120.mp4


