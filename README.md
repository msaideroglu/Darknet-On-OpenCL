Darknet on OpenCL
==========

## Darknet
Darknet is an open source neural network framework written in C and CUDA.<br> 
It is fast, easy to install, and supports CPU and GPU computation.<br>
You can find the origin project [here](https://github.com/pjreddie/darknet).<br>
## Darknet on OpenCL
As the origin darknet project is written in CUDA, this project is to port<br>
the darknet to OpenCL. 
## Dependency
`OpenCL`<br>
Make sure you have OpenCL installed.<br>
You can check it with clinfo.<br>
`clBLAS`<br>
clBLAS is equivalent to cuBLAS, you can find the source code [here](https://github.com/clMathLibraries/clBLAS)<br>
and compile it yourself.<br>
or you can use binary library<br>
You can find clBLAS.lib and libclBLAS.so for Linux <br>
as well as header file [here](https://github.com/ganyc717/Darknet-On-OpenCL/tree/master/darknet_cl/clBLAS).<br>
## Build
`Linux`<br>
mkdir build && cd build<br>
cmake ../<br>
make<br>
## Usage
cp -r darknet ..<br> 
cd ..<br>
./darknet detect cfg/yolov3-tiny.cfg yolov3-tiny.weights data/drone.jpg<br>




