
# FFmpeg for Homekit
</div>

This project provides static FFmpeg binaries for Raspberry Pi for use Homekit.

Specifically, we provide:

* Audio support using `libfdk-aac`
* Hardware-accelerated encoding support on Intel platforms using `h264_qsv` and hardware-accelerated encoding on Raspberry Pi 3+ using `h264_v4l2m2m`

## Build and Install

#### Raspbian or armv7/armv8-based Linux environments:

```
git clone https://github.com/0x000000000019b6/ffmpeg-for-homekit.git
```
```
cd ffmpeg-for-homekit/
```
```
./build-ffmpeg --build --enable-gpl-and-non-free --enable-alsa --latest --install
```

## Install from release

```
sudo apt-get update && \
sudo apt-get install -y wget libxcb1-dev libxcb-shm0-dev libxcb-xfixes0-dev libsndio7.0 libxv-dev libva-dev \
libopencore-amrnb-dev libopencore-amrwb-dev libmp3lame-dev libtheora0 libvorbis-dev libvdpau-dev
```
```
wget https://github.com/0x000000000019b6/ffmpeg-for-homekit/releases/download/ffmpeg-6.1/ffmpeg-6.1-homekit-ubuntu22.04-aarch64.tar.gz
```
```
sudo tar -xzf ffmpeg-6.1-homekit-ubuntu22.04-aarch64.tar.gz --strip-components=2 -C /bin workspace/bin/ffmpeg workspace/bin/ffplay workspace/bin/ffprobe
```
