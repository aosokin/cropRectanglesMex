This software implements the MATLAB function to crop patches of an image and resize them to the standard size (on a GPU):
a wrapper on top of NVIDIA Performance Primitives (https://developer.nvidia.com/NPP), function nppiResizeSqrPixel_32f_P3R
The NPP library is included in the standard CUDA package.

Anton Osokin, (firstname.lastname@gmail.com)
March, 2015
https://github.com/aosokin/cropRectanglesMex

PACKAGE
-----------------------------

./cropRectanglesMex.cu - the source code

./build_cropRectanglesMex.m - the build script

./cropRectanglesMex.m - the description of the implemented function

./example_cropRectanglesMex.m - the example of usage

USING THE CODE
-----------------------------

0) Install MATLAB, the supported compiler, and the appropriate version of CUDA

1) Run build_cropRectanglesMex.m

2) Run example_cropRectanglesMex.m to check if the code works

The code was tested under 
- ubuntu-12.04-x64 using MATLAB R2014b, gcc-4.6.3, cuda-6.5

This code was written to be used together with MatConvNet (http://www.vlfeat.org/matconvnet/) and in theory should work if MatConvNet works.
If you face compilation problems the MatConvNet compilation script (vl_compilenn.m) might be of some help.
