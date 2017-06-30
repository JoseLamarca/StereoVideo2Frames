# StereoVideo2Frames

Auxiliar program for Hamlyn data treatment on ORBSlam2 that does the followin:
  
  0.Input: file dir +  "/" that contains:
    -"stereo.avi"
    -"camera_extrinsic.txt"
    -"Left_Camera_Calibration_Intrinsic.txt"
    -"Right_Camera_Calibration_Intrinsic.txt"

  1. Creates a dir ("data_ORBSLAM2") where the "stereo.avi" file is . Separates both parts of the stereo video "stereo.avi" 
    (left and right camera images) and saves them into cam0 and cam1 dir (inside "data_ORBSLAM2") respectively numerated from 
    0 to n (n=number of frames).
    
  2. Creates a "hamlyn.yaml" containing the following data:
  
    -Camera Parameters
    -ORB Parameters
    -Viewer Parameters
    
    The camera Parameters are calculated with the data obtained from the hamlyn center files:
      -"camera_extrinsic.txt"
      -"Left_Camera_Calibration_Intrinsic.txt"
      -"Right_Camera_Calibration_Intrinsic.txt"
