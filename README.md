A repo containing binaries built from src, optimized for my machine.

Tensorflow built with these optimizatons:
`--copt=-mavx --copt=-mavx2 --copt=-mfma --copt=-mfpmath=both --copt=-msse4.2`
based on [this guide](https://gist.github.com/Brainiarc7/6d6c3f23ea057775b72c52817759b25c).
Install the provided .whl with pip3.

OpenCV 4.0.1, with opencv_contrib and nonfree modules, python3 support only. Should automatically include native optimizations.
based on [this guide](https://www.pyimagesearch.com/2018/08/15/how-to-install-opencv-4-on-ubuntu/).
To successfully build, I also did `sudo apt-get install opencl-headers` and provided explict paths for `cmake`.
Install the provided .so into your python's `site-packages/` directory, and rename it to `cv2.so`.

Machine:
 - i5-9600k (Intel coffee lake refresh) 
 - nvidia RTX 2080
 - Ubuntu 18.04
 - 32GB RAM
