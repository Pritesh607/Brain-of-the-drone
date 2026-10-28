# Brain-of-the-drone
A cool flight controller for drone with brushed motors with inbuilt motor driver made using esp32 and can be controlled using wifi or your transmitter with the betafpv firmware.
If we come to the esp32 model i used in this project is an esp32 S3 by Xiao Speed studio, i could have also used esp32 C3 or even an esp8266 which are comparatively cheaper than the esp32 S3 i used but they lake the performance that esp32 S3 gives because I also want to fly the drone with Betafpv firmware as an FPV drone which need a lot faster processing time which an esp32 S3 can deliver and there are many sensors to read but for now i didn't added ant extra sensor except mpu6050 because it will make this project more complex and costlier and here is a comparison between an esp32 C3 and esp32 S3 to show the clear difference: 

-CPU Architecture
Esp32 C3:32-bit RISC-V (Open-source)	CPU Architecture
Esp32 S3:32-bit Xtensa LX7
-CPU Cores
Esp32 C3:Single-core	CPU Cores
Esp32 S3:Dual-core
-Max Clock Speed
Esp32 C3:160 MHz	Max Clock Speed
Esp32 S3:240 MHz
-SRAM (Internal)
Esp32 C3:400 KB	SRAM (Internal)
Esp32 S3:512 KB
-Available GPIOs
Esp32 C3:22	Available GPIOs
Esp32 S3:45

Now if we come to the hardware part, we will use 816 coreless motor or any comparable coreless motor for more thrust and we will not require any external motor driver as it is inbuild into the flight controller and for the frame we can use any small drone frame that can fit all the components and will be stable and for the battery we will use an 1s lipo battery.  

For the Wi-Fi controlled drone firmware you can see the video "ESP32 WI-FI CONTROLLED DRONE from scratch tutorial" by Dr Electronics on YouTube because it is a long process. Now for the Betafpv firmware you just have to flash the Betafpv compatable firmware onto the Esp32 S3 which i have given and install the betafpv v10.10.   

NOTE: To give power to the Esp32 you have to directly solder a wire to the back of the esp32 s3 because there is a external battery connector and you can charge the battery directly from the esp32 Type-C connector.
## PCB Design

![image alt](https://github.com/Pritesh607/Brain-of-the-drone/blob/c1979ad6ae038782cff72d6b6be79a0cc504ad1e/Images/Screenshot%202026-10-06%20153152.png)
![image alt](https://github.com/Pritesh607/Brain-of-the-drone/blob/main/Images/Screenshot%202026-10-08%20193431.png)
