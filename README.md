# C-Board
>AR application with drawing alphabet "C" on the chess board

I simply practiced AR application techniques on the chessboard with smartphone camera calibration.<br/>
This program renders the three-dimensional alphabet "C" on a chessboard for various camera perspectives.<br/>
You need to install following packages.
```
pip install opencv-python opencv-contrib-python
pip install numpy
```

- `camera_calibration.py` : Camera calibration for "chessboard.mp4".
- `pose_estimation_chessboard.py` : Perform camera pose estimation to draw the letter "C" on the chessboard.
- `chessboard.mp4` : Source video for program.
- `c-board.gif` : Showing the result.

## How to use
1. Run `camera_calibration.py`. <br/>
2. Press the `space bar` to pause the video, and select image by press the `enter key`. (Repeat several times.)<br/>
3. Apply the derived Camera matrix and Distortion coefficient values to the `pose_estimation_chessboard.py`. <br/>
```
[Values in my case]
* Camera matrix (K) =
[[1.17608879e+03 0.00000000e+00 6.49296415e+02]
 [0.00000000e+00 1.18162755e+03 3.83189680e+02]
 [0.00000000e+00 0.00000000e+00 1.00000000e+00]]
* Distortion coefficient (k1, k2, p1, p2, k3, ...) = [-5.70682357e-02 -8.71801912e-01  6.03146664e-03  9.29867696e-04
  4.79149816e+00]
```
4. Run the pose estimation code. <br/>
5. You can see how the program works as below. (c-board.gif)

<img src="https://github.com/NyaNyak/C-Board/blob/master/c-board.gif?raw=true" width="800" height="500"/>
<br/>

