# OpenCV 4 Example

## Prerequisites

This example suppose that you have installed **`Ubuntu 18.04`** on your dev
machine. You need the SIFT implementation to run this code...

You need to install the missing non-free version of OpenCV4. To do that type the
following in the terminal:

```sh
# First cd into where you want to put the Opencv library, e.g ~/dev/libs/
mkdir -p ~/dev/libs && cd ~/dev/libs/
git clone https://github.com/opencv/opencv.git -b 4.3.0
git clone https://github.com/opencv/opencv_contrib.git -b 4.3.0
mkdir opencv/build && cd opencv/build
cmake -DOPENCV_EXTRA_MODULES_PATH=../../opencv_contrib/modules ..
make -j && sudo make install
```

## How to Build the examples on this repository

Build is straightforward:

```sh
mkdir build/
cd build/
cmake ..
make
```
