# HTML5-Live-Playback-for-NVR-DVR
The purpose of the SDK is to show you how to embed HTML5 live & playback video into HTLM page for NVR/DVR.
<BR>
![image](/images/picture.jpg)
# Prerequisite
Product supported: DVR/NVR 5 & 6 series
Firmware supported: 5.0.28.7551 SVN 7551 and later

# System architecture
![image](/images/picture1.jpg)

1. Visit the Network->Other page via NVR/DVR’s browser.  
2. Enable HTTP CROS to On setting.  
<BR>

![image](/images/step1.png)

<BR>
3. Copy the access key of the HTTP CROS setting.
<BR>
![image](/images/step2.png)
<BR>
4. Software developer uses the Access key for authenticating simpleLive.html and simplePlayback.html.
5. Live video page in HTLM embedded by a third-party web system:
  
CGI: http://192.168.0.111/newlang1/simpleLive&ch=0x0001&res=hd&accesskey=ABC123

Parameters:
ch (Channel): It can be a single screen (must support) or any 4-way combination.

Full screen: Alow customers to embed into web pages, log in (authentication), fill the entire screen, and let customers adjust the resolution of IFrame by themselves

Res=HD: HD, SD small stream
Access key: Include username and password of the NVR/DVR.


