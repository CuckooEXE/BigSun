# BigSun

## Prelude 
After my last blog post, I thought it would be cool to write up my new project regardless of whether or not it was successful. That way, anyone who stumbles on my blog can see the failures of a security researcher and see my thought process, etc. When I was first starting out in the industry, I was so intimidated by some people because their blog was CVE, after CVE, after CVE, after success. 

## Hardware
I went to eBay and bought the SKETCHIEST hardware I could find, in this case, I got a ["Spy Camera"](https://www.ebay.com/itm/284128949863) ([Wayback Archive Link](https://web.archive.org/web/20210524174343/https://www.ebay.com/itm/284128949863)). The premise is simple, you can connect directly to the device via the WiFi network it broadcast, and either just stream directly to your device, or you can tell it to connect to another WiFi network. It also has the ability to save video to a microSD onboard the device.

I had a pretty hard time getting this all set up, it looks like the Android app is totally broken, and refuses to connect to the camera correctly; I couldn't get video streamed to my phone, nor could I tell the camera to connect to another WiFi network. I ended up having to install the app on my iPad which worked. From there I could start getting to work.

## Inspecting the Network
So obviously this was generating regular WiFi traffic because multiple devices were able to connect to the device's hotspot/WiFi network, and my iPad could receive the video.