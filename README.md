# FuzzyShrink



    Fuzzy Wavelet-based Shrinkage Method 


    Schulte Stefan, Huysmans Bruno, Pizurica Aleksandra, Kerre Etienne E. and Philips Wilfried. A new fuzzy-based wavelet shrinkage image denoising technique . Advanced Concepts for Intelligent Vision Systems, Lecture Notes in Computer Science 4179 (2006) 12-23 

    Download the zip file here.


    Unzip the file into a certain directory.


    You have to add the folder to the current MATLAB search path by using the commando: addpath('path'), with ‘path’ the directory followed by the new map '/FuzzyShrink' which should be created.


    The FuzzyShrink filter is executed by using the Matlab commando:

    Out = FuzzyShrink(A,W);
    where A is the input image of any size and W the window-size (for example 3).


    In order to overcome some problems of Matlab we have implemented most files in C-code. The switching between Matlab and C in realized by the mex (see Matlab help for more information). If you never have used mex files before you probably have to do the following thinks:

    cd 'C:\Directory\'
    the current directory has to be changed to that map that was created in the first step

    mex –setup
    => Choose a compiler

    mex shrink.c

