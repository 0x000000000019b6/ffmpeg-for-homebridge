
# FFmpeg for Homekit
</div>

This project provides static FFmpeg binaries for Raspberry Pi for use Homekit.

Specifically, we provide:

* Audio support using `libfdk-aac`
* Hardware-accelerated encoding support on Intel platforms using `h264_qsv` and hardware-accelerated encoding on Raspberry Pi 3+ using `h264_v4l2m2m`

## Install

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