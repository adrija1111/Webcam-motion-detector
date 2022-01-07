# Webcam-Motion-Detector
A Python program that can detects moving objects with webcam and log their entry and exit time .

The script "main.py" utilizes the openCV library to capture video from the default webcam of the loacal machine. and we basically store the first frame, which ideally would capture the static background, and then check every coming frame captured from the camera to see if the difference (delta) in all pixels surpasses the set threshold. If it does, we draw rectangular contours on the frame to indicate where the detected objects are.

After we are able to successfully detect the moving objects, the next step is to record the entry and exit points in time and plot a time series with my second script- "plot.py".
The time series chart is plotted with the bokeh library and I have also enabled hovering effect to show the time stamps.

![Screenshot (170)](https://user-images.githubusercontent.com/70461834/125801817-276f7edb-7f9d-4ee1-b284-f7cff66ec488.png)
