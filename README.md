**libyuv** is an open source project that includes YUV scaling and conversion functionality.

* Scale YUV to prepare content for compression, with point, bilinear or box filter.
* Convert to YUV from webcam formats for compression.
* Convert to RGB formats for rendering/effects.
* Rotate by 90/180/270 degrees to adjust for mobile devices in portrait mode.
* Optimized for SSSE3/AVX2 on x86/x64.
* Optimized for Neon on Arm.
* Optimized for MSA on Mips.

### Development

See [Getting started][1] for instructions on how to get started developing.

You can also browse the [docs directory][2] for more documentation.

[1]: ./docs/getting_started.md
[2]: ./docs/

### note

填坑之一：上面的方法下载的sdk在有些gcc交叉编译环境下不能编译通过　需要通过gclient下载   
方法见libyuv/doc下的deprecated_builds.md     
要先下载gclient　方法见     
https://www.chromium.org/developers/how-tos/install-depot-tools     
然后在执行       
gclient config https://chromium.googlesource.com/libyuv/libyuv

### CLion make libyuv.so for linux at h616 
cmake && make 
