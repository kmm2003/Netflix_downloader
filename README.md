# Netflix_downloader

## requirement
+ Frida 15.2.2 (Android 9~13)
+ Frida 12.11.11 (Android 5,6)
+ python 3.9
+ pycurl
+ json, cbor2
+ humanize

## usage
### media download & L3 KeyBox Recovery
1. Install frida-server in Android device ("/data/local/tmp" in path with root)
```
adb push frida-server /data/local/tmp/frida-server
```
2. Set permissions for frida-server
```
adb shell

chmod 777 frida-server

chown root:root frida-server
```
3. Starting frida-server
```
./frida-server &
```
4. Turn on the Netflix app and wait
5. Starting python script
```
python netflix_media_download.py

python recover_l3keybox_mobile.py
```
6. Play video



![netflix_download](https://user-images.githubusercontent.com/69188747/205892336-b64058fc-c4a7-475c-8277-d0c064ea773a.png)<br>
7. The video is downloaded automatically


## Caution
+ The Frida version is different depending on the Android version.

