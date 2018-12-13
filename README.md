# cube-solving-basic-algo
please read the read me first 

language: c

we are using the basic algorithm for solving the cube

this is a basic overview of the steps: https://rubiks-cube-solver.com/how-to-solve/

download this library for c : https://drive.google.com/open?id=1b1SzeZQT7itGW3T_t19YB4TKQdkxNb3P

to link this library to your code use the these steps: watch from 1:41 https://www.youtube.com/watch?v=-3BoOuSSCeI 

## basic overview of functioning of library
we see every step in form of rotation of one of six faces in either clockwise or anti-clockwise direction relative to the face and we have defined the functions for same 
![layout of cube](https://raw.githubusercontent.com/bhatakti-atama/cube-solving-basic-algo/master/Capture.JPG)
### here is the basic layout of the cube

we are imaganing cube as a 6x3x3 matrix which hold values according to the layout 

## using the library functions 

first we need to create a 6X3X3 matrix like this:

int cube[6][3][3]= {{{11,12,13},{14,15,16},{17,18,19}},{{21,22,23},{24,25,26},{27,28,29}},{{31,32,33},{34,35,36},{37,38,39}},{{41,42,43},{44,45,46},{47,48,49}},{{51,52,53},{54,55,56},{57,58,59}},{{61,62,63},{64,65,66},{67,68,69}}};

we can change the values depending on how we have scrambled the cube

to rotate one face clockwise we use the following statement:

face1(&cube[0][0][0],0)

this rotates the face1 clockwise ie. white

first parameter tells the address first element of the face 

second tells if rotation is colckwise or anti-clockwise 

0 for clockwise

1 for anti-clockwise

## list of functions

face1(int *a,int b) : rotates white face

face2(int *a,int b) : rotates red face

face3(int *a,int b) : rotates green face

face4(int *a,int b) : rotates orange face

face5(int *a,int b) : rotates blue face

face6(int *a,int b) : rotates yellow face
