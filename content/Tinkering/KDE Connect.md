Sunshine Status mobile command:
```bash
systemctl --user --quiet is-active sunshine && kdeconnect-cli -d 3e95308c0a594055a33fbc108f1aeb96 --ping-msg "Sunshine: Running ✅" || kdeconnect-cli -d 3e95308c0a594055a33fbc108f1aeb96 --ping-msg "Sunshine: Stopped ❌"
```

Webcam photo and send to mobile
```bash
ffmpeg -y -f v4l2 -video_size 1280x720 -i /dev/video0 -vframes 1 /tmp/snap.jpg && kdeconnect-cli -d 24f57aacb899486fa9ff9515625b81f2 --share /tmp/snap.jpg
```
