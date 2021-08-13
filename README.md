# visual-object-tracking

### How to build & run

#### 1. install prerequisite
```bash
pip install numpy
pip install opencv-python
```

#### 2. run python implementation
```bash
cd gpu-object-tracking
python mosse.py   # has default ROI coordinates, no need select tracking object by user
python mosse2.py  # need to select tracking object ROI with mouse by user
```

#### 3. build and run c++ implementation 

a. dowload opencv Windows release package from this [link](https://sourceforge.net/projects/opencvlibrary/files/4.5.3/opencv-4.5.3-vc14_vc15.exe/download)
b. double click the package to extract it to: d:\library (or other location)
c. run cmake to generate VS project
```code
cd gpu-object-tracking
mkdir build
cd build
cmake -DOPENCV_DIR=D:\library\opencv ../src
```
d. open mosse.sln and build in VS

### Reference 
MOSSE paper: https://www.cs.colostate.edu/~draper/papers/bolme_cvpr10.pdf

