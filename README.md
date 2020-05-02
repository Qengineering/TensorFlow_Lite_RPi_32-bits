# TensorFlow_Lite_RPi_32-bits
TensorFlow Lite classification running at 33 FPS on bare Raspberry Pi 4

A fast C++ implementation of TensorFlow Lite classification on a bare Raspberry Pi 4.
Once overclocked to 2000 MHz, your app runs an amazing 33 FPS without any hardware accelerator.

https://arxiv.org/pdf/1712.05877.pdf <br/>
Training set: COCO with 1000 objects<br/>
Size: 224x224 <br/>
Frame rate Mobile_V1 Lite : 33 FPS (RPi 4 @ 2000 MHz - 32 bits OS) <br/>
Frame rate Inception_V2 Lite : 8.9 FPS (RPi 4 @ 2000 MHz - 32 bits OS) <br/>
Frame rate Inception_V4Lite : 1.6 FPS (RPi 4 @ 2000 MHz - 32 bits OS) <br/>
With a 64 bits OS you get higher frame rates see: https://github.com/Qengineering/TensorFlow_Lite_RPi_64-bits <br/>
<br/>
Special made for a bare Raspberry Pi see: https://qengineering.eu/install-tensorflow-2-lite-on-raspberry-pi-4.html <br/>
<br/>
To extract and run the network in Code::Blocks <br/>
$ mkdir *MyDir* <br/>
$ cd *MyDir* <br/>
$ wget https://github.com/Qengineering/TensorFlow_Lite_RPi_32-bits/archive/master.zip <br/>
$ unzip -j master.zip <br/>
Remove master.zip and README.md as they are no longer needed. <br/> 
$ rm master.zip <br/>
$ rm README.md <br/> <br/>
Your *MyDir* folder must now look like this: <br/> 
tabby.jpeg <br/>
schoolbus.jpg <br/>
grace_hopper.bmp <br/>
Labels.txt <br/>
TensorFlow_Lite_Mobile.cpb <br/>
TensorFlow_Lite_Class.cpp<br/>
 <br/>
Next, choose your model from TensorFlow: https://www.tensorflow.org/lite/guide/hosted_models <br/> 
Download a quantized model, extract the .tflite from the tarball and place it in your *MyDir* <br/>
Run TestTensorFlow_Lite.cpb with Code::Blocks. Remember, you also need a working OpenCV 4 on your Raspberry. <br/>
Preferably use our installation: https://qengineering.eu/install-opencv-4.3-on-raspberry-pi-4.html <br/>

![output image]( https://qengineering.eu/images/James_17.jpg )
