This project uses OpenCV library in Python to identify a distinct color range in a video, which is then tracked frame-by-frame.
--
https://github.com/k4cper-g/object_tracking/assets/93160987/99d94617-b8fd-45fc-96f9-0ca6931a33a6

Steps to reproduce:
--

1) Tweak HSV lower and upper bound arrays for the mask to detect desired color correctly.
```python
# red color
lower = np.array([0,60,0])
upper = np.array([10,255,255])
```
2) Change input and output respectively.
```python
cap = cv2.VideoCapture('YOUR_INPUT_VIDEO')
out = cv2.VideoWriter('YOUR_OUTPUT_VIDEO', cv2.VideoWriter_fourcc(*'mp4v'), fps, (width, height)) 
```
3) Run code and enjoy tracked object.
