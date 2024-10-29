# H - hue (цвет), S - saturation(насыщенность), V - value(яркость) от 0 до S
#преобразование в хсв
import cv2
cap=cv2.VideoCapture(1)

while True:

    ret, frame = cap.read()
    frame=cv2.cvtColor(frame, cv2.COLOR_BGR2HSV)
    cv2.imshow('camera', frame)
    key=cv2.waitKey(1)
    if key==ord(' '):
        break
    print(key)



# cvr_october_29_30
