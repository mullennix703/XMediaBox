Introduction
------------
**XMediaBox** is a customized android rom based on LineageOS.  
It enable users to capture system's playing audio/video of this device. So the quality is better than screenshot/speaker. It also provides video/audio push and relay service by rtmp/rtsp protocal.  
XMediaBox's mic/camera data is highly customizable ,which means users can  specify any video/audio source(file/stream video) as inut of mic/camera.In this way users can broadcast any live streaming video/audio to any friend or group by video chat app.  
XMediaBox could be a local media server.It shares system's playing video/audio with other devices.  
The target of XMediaBox is to build a data bridge over different apps and devices. Nowdays people knows that data is valuable, but limitation is data is only binded to a single app.XMediaBox hopes to help users reuse, porcess and send data easily.   



Download
------------
***~~[drive link]~~***(https://drive.google.com/drive/folders/13N474eoRZy6ForTilsq1gpN-NWi70AV-?usp=sharing)
Outdated.Contact me for valid one.



Typical Usage scenario
-----------
1. For youtuber. Broadcast personal live streaming to all streaming video platforms around the world and group chat channels such as zoom.  
The solution is like below graph. The user chooses a main platform and boardcasts live streaming as usual. The background system works like this. A XMediaBox device captures live streaming video and forwards it to the a media server. The media server supports relay server to forward video to other rtsp/rtmp based live steraming platforms and supports other XMediaBox devices to forward video to group chat apps.Synchronization robots(under development)  monitor all related channels and send all comments back to main platform, which makes two way communication for every live streaming channel.This solution doesn't interrupt user's normal operation and is easy to deploy.It is suitable both for single youtuber and third part service provider.  
![](https://github.com/mullennix703/XMediaBox/raw/master/images/XMediaBox.png)

2. For sport fans. XMediaBox makes it easy to be a match commenator and share live streaming and ideas to friends in a chat group. 



Configuration 
-------
The functionality is triggered by a configuration app (MediaCenter). The user needs to specify a working mode there.All configuration items are divided into two catagory push mode and tunnel mode.  
Push mode supports rtsp/rtmp push server.Tunnel mode supports camera/mic hacking.The solution performance depends on hardware capacity(1080p require Qcom835).  
### Push Stream Configuration
1. **Push Server Address.** rtmp/rtsp push server.
2. **Rtsp Server.** Make the device become a rtsp server, share system video/audio with other rtsp client.
3. **Third part apps source.** Aim to capture third part running apps' video/audio data, which is forwarded to other endpoints according to above two configurations. Currently this function is compatible for some major video apps. Feel free to contact me for compatibility issue.
4. **Select a video file.** Choose a local video file to be source of internal video player. Click start button in the menu button, video file is pushed to other endpoints acorrding to first two configurations.
5. **Set source video network address.** Set a streaming video address as source of internal video player. Click start button in the menu button, streaming video is relayed to other endpoints according to above first configurations.
6. **Audio only.** Only processing audio data.

### Tunnel Stream Configuration
1. **Select a video file.** Choose a local video file to be source of camera&mic. Currently zoom, WeChat work, Dingtalk are supported.Compatibility will be improved according to uses' requirement.
5. **Set source video network address.** Set a streaming video address as source of camera&mic. 
6. **Audio only.** Only hacking mic.

### Howto install
[guidance](https://wiki.lineageos.org/install_guides.html)

### Enable Stay Awake in Setting->Developer Options to prevent disturbance

### Contact
mullennix703@gmail.com


