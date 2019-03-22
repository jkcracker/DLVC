### Requirements:
nvidia-docker
nvidia driver >= 384.81

### 1. Get and run docker image from https://hub.docker.com/r/huzi96/dlvc-1.0
```nvidia-docker run -it huzi96/dlvc-1.0:gpu bash```

### 2. Navigate to working folder
```cd /opt/dlvc/tests```

### 3. Run the test [Example]
```../bin/TAppEncoderStatic -c ../cfg/encoder_lowdelay_jvet10.cfg -c ../cfg/per-sequence/RaceHorses.cfg -i RaceHorses_416x240_30.yuv -q 37 -wdt 416 -hgt 240 -f 30 -fr 30 -b str.bin -o rec.yuv -dl Caffe -mode GPU -gpuid 0```