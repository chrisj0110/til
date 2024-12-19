# ffmpeg

to convert a file from m4a to wav, and with volume 5x louder than the original:

```bash
ffmpeg -i filename.m4a -filter:a "volume=5" filename.wav
```

