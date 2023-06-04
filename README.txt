URL of this repo:
https://github.com/Lessstuck/ml.drumFeatures

This feature extractor is meant to help with classifying short sound samples. Each sample is played into an MFCC feature extractor once every 0.1s for a total of 1 sec. Times are added to the beginning of each MFCC list, so that multiple examples can be recorded without stopping. This means the patch can play a folder full of samples automatically.

Group similar samples into folders with their class names. Do as many as you like. Then set aside other samples into a test folder where the classes are mixed together. Choosing a folder will automatically play each sample in the folder, and send time-stamped MFCC data to Wekinator. After recording and training, choose the test folder to see how well your classifier is working.

_____INSTALL

It will work only an a Mac computer.

Install Max
https://cycling74.com/downloads

Launch Max & install Zsa package
File > Show Package Manager
Install
zsa descriptors

_____SETUP & RECORD

Double-click
featureTester.maxpat
You may need to toggle audio on/off/on

Run Wekinator classifier
25 inputs
1 output 
Number of classes equals number of sample folders you'll be analyzing

_____RUN

Wekinator: Choose class, Record
Max: Choose Folder
After all samples are played,
Wekinator: Stop
Repeat with next folder

Wekinator: Train

_____TEST

Wekinator: Run
Max: choose test folder to see how well your classifier is working!