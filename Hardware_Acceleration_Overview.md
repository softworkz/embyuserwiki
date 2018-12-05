Emby supports a broad range of hardware accelerated video transcoding methods on its supported platforms:

## Windows

Emby supports the following [hardware acceleration variants on Windows](Hardware_Acceleration_Windows)

- **Nvidia NVDEC & NVENC**  
API for video encoding and decoding acceleration using Nvidia GPUs

- **Intel QuickSync Video**  
 Intel's brand for its dedicated video encoding and decoding hardware 
 core

- **AMD AMF**  
 AMD Advanced Media Framework - multimedia API  AMD hardware for 
 real-time processing of multimedia

- **Microsoft DXVA**  
 Microsoft DirectX Video Acceleration API - hardware independent API 
 for hardware accelerated video decoding

## Linux

Emby supports the following [hardware acceleration variants on Linux](Hardware_Acceleration_Linux)

- **Nvidia NVDEC & NVENC**  
API for video encoding and decoding acceleration using Nvidia GPUs

- **VA API]**  
Video Acceleration API for Linux is supported by several device manufacturers

- **Intel QuickSync Video**  
 Intel's brand for its dedicated video encoding and decoding hardware 
 core


Important Background on CPU Usage in Hardware Acceleration Contexts

 

There's a common misconception about CPU load during a hardware accelerated transcoding session.

It's a subject that is more complicated than one would think in the first moment.

 

I'll give you one example that will make you think over it:

(apologies to the few that might have known)

 

Let's take a video file H.264 that is transcoded to H.264 but downscaled (for a mobile device).

There's also an audio track AC3 5.1 that needs to be transcoded to aac stereo (that mobile device can't do 5.1).

 

Let's also assume that you have some Intel onboard graphics which is pretty old but it supports QuickSync.

You also have one of the latest Nvidia boards offering high end computing power.

 

 

Then you compare the transcoding performance between both hardware accelerations:

With QuickSync, you see pretty low CPU load
.
then you try Nvidia
.
With Nvidia, you see the CPU load reaching 100% (calculated down to a single core at least)
 

So which hardware acceleration might be better here?

 

=> QuickSync? No - it's Nvidia!

 

The high CPU load is caused by the audio conversion. QSV might just not be quick enough while Nvidia would do video faster than the CPU can do Audio - which makes the CPU reach its maximum level.

 

Conclusion: CPU load is a rather bad indicator for assessing hw acceleration performance and can be very misleading!

 

Better look at the transcoding rates in the ffmpeg logs

(use only those where videos start from the beginning, there's a calculation error when resuming).