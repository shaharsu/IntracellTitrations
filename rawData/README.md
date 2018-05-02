This directory contains all raw data in .mat files readable by matlab. Each dataset is composed of a calibration jump under 
amber illumination (_calib.mat suffix) which is followed by a full jump under blue illumination (FRET data)

Each file contains the following fields:

coordleft   - coordinates of cropped and aligned acceptor channel on the original image
coordright  - coordinates of cropped and aligned donor channel on the original image
dataleft    - acceptor channel data. Not available in _calib files
dataright   - donor channel data. This will be mCherry in _calib files and AcGFP in datga files.
frame1      - original image size
imgstd      - cropped dimensions
numFrames   - number of frames in dataleft and dataright
videos      - a structure file containing camera data. Specifically, videos.TimeStamp includes the time from each frame.

