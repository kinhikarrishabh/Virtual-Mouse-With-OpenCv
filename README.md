# VirtualMouse
This is a python project to create a virtual mouse control system using hand gestures. 
The projects captures video from the default camera, detects hand landmarks using the MediaPipe Library and moves the virtual mouse cursor based on the movement of the hand.

	1) Libraries Used :
		a. Cv2 : OpenCV for Computer Vision Tasks
		b. mediapipe : A library by Google for detecting hand landmarks
		c. pyautogui : Library for Controlling mouse and keyboard

	2) Hand LandMark Detection
		Step 1 : Creates a hands detector using MediaPipe
		Step 2 : Processes the captured frame to detect hands
		Step 3  : Retrieves the detected hand landmarks

	3) Mouse Control
		a. Landmark of index fingers (id=8) and thumb (id=4) for mouse control
		b. If the vertical distance is less than 20 pixels, call the pyautogui.click()
		c. If the distance between 20 and 100 pixels, call the pyautogui.moveTo(x,y) for smoother cursor movement

	

