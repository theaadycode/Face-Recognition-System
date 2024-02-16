Face-Recognition-System

1. cam.py:
Imports the OpenCV library (cv2).
Loads a pre-trained Haar Cascade face detection model from a specified XML file path (haarcascade_frontalface_default.xml).
Opens the webcam using cv2.VideoCapture(0).
Captures frames from the webcam in a loop, converts each frame to grayscale, and detects faces using the Haar Cascade classifier.
Draws rectangles around detected faces in the frame.
Displays the resulting frame in a window titled 'Webcam Face Detection.'
Breaks the loop if the 'q' key is pressed.
Releases the webcam and closes OpenCV windows.

2. data_collection.py:
Imports the OpenCV library (cv2), operating system module (os), tkinter for GUI (tkinter), and PIL for image processing (PIL).
Defines a class DataCollectionApp for a data collection application with a GUI.
GUI includes entry widgets for name, buttons for using the webcam, choosing from the gallery, and saving images.
Provides methods to capture images from the webcam, save the images, and choose images from the gallery.
Uses the Haar Cascade face detection similar to cam.py for webcam image capture.
The class is instantiated, and the GUI event loop is started (tk.Tk() and root.mainloop()).

3. face_recognition.pt (presumed typo in the file name, should be frs.py):
Similar to data_collection.py, this script defines the same DataCollectionApp class for a data collection application with a GUI.
Provides methods for capturing images from the webcam, saving images, and choosing images from the gallery, just like data_collection.py.
However, it lacks the final instantiation and main loop (if __name__ == "__main__":) found in data_collection.py.
Note:
The face_recognition.pt script seems to be identical to data_collection.py, and the class and methods are defined twice, which might be an error or oversight.
The scripts related to data collection use Tkinter for the graphical user interface and OpenCV for webcam interaction and image processing. They provide options to capture images from the webcam, save them, and choose images from the gallery. The captured images are stored in a 'database' folder.
