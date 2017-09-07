# Kinect Related Codes and Docs

## config kinect v2 on ubuntu and warp it using python 2.7
git clone libfreenect2 and follow the readme.
### Note1. jpeg version is not in consistence.  
Anaconda using jpeg 90. the libfreenect2 using jpeg 80. Needs to uninstall anaconda jpeg and install jpeg 80. After that, delete all build files and re-cmake the build files.
### Note2. Somehow the environment is not set. Even I use sudo. so the ./Protonect is not runable after restart.
Need to manual add the environment path. I chagne the ~/.profile using gedit.
    add below two lines:
    export LIBFREENECT2_INSTALL_PREFIX="/home/richard/freenect2"
    export LD_LIBRARY_PATH="/home/richard/freenect2/lib"
### Note3. using python
using python needs to clone pylibfreenect2. You can find more info from 'http://r9y9.github.io/pylibfreenect2/stable/installation.html#build-requirements'. really helpful.
Note that using anaconda opencv3 verison may not have gtk2.0 intergrated. I tried using opencv3 but failed. Even I installed gtk2.0. For opencv2.0 it works. 
### Note4 . Tobe solved: not showing rgb depth data.
  [Debug] [RgbPacketStreamParser] skipping rgb packet!
  [Debug] [RgbPacketStreamParser] skipping rgb packet!
  [Debug] [RgbPacketStreamParser] skipping rgb packet!
  
## Tensorflow
  CPU: just follow the official website.
  GPU: not tried.
 
## TODO install cuda and using gpu to run this and tensorflow.
