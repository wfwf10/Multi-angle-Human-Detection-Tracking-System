# Multi-angle-Human-Detection-Tracking-System
fgm part:
1. Download files in https://www.dropbox.com/s/a1eq2l1wf8hxrz7/fgm.rar?dl=0 to your path.
2. Download and extract fgm.zip (which is a part in the dropbox file in 1), and run addPath.m to add the needed path to MATLAB, and run make.m to make up the C++ programs. 
3. Run RCNN_Tracker_Ver_4_0_ICIP2017.m for view 1, 5, and 7 in order(notice that you should modify the file paths for RCNN data and images). For each you need to modify which view you choose, and save location_time_info.mat and Representative_Lookup_Table in workspace to your path.
4. For multiview, we first do double trigger to view 1 aggaist view 7, then do double trigger to view 1 aggainst view 5 to get the final result. We take V1V7 for example (we always use demoCisco_V1V7.m and demoCisco_V7V1_fw180430_doubletrigger_advanced.m). First we run demoCisco_V1V7.m (notice that you should modify the path of the files you get from previous steps, the images, and which homography matrix you choose), and save VOB for both view, then run demoCisco_V7V1_fw180430_doubletrigger_advanced.m for selected view, then run demoCisco_V1V7.m again (always modify to the newest file path and save VOBs!).
5. The resulting images and videos are automatically saved to the fgm folder.
