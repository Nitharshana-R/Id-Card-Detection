Load the Image:
Reads the image from a specified file path using OpenCV (cv2.imread).
Displays the image using Matplotlib.

Convert to Grayscale:
Converts the image to grayscale using OpenCV (cv2.cvtColor).
Simplifies the image for edge and contour detection.

Edge Detection:
Detects edges in the grayscale image using the Canny algorithm (cv2.Canny).

Find Contours:
Extracts contours (boundaries of shapes) in the image using OpenCV (cv2.findContours).

Draw Detected Contours:
Draws all detected contours on the original image for visualization.

Extract the ID Card:
Sorts contours by area to find the largest one (assumed to be the ID card).
Extracts the region of interest (ROI) using bounding rectangle coordinates (cv2.boundingRect).

Save the Result:
Saves the cropped ID card to the specified file path (cv2.imwrite).

Output:
Visual Output:
The script will display:
The original image.
The image with detected contours.
The cropped ID card.
Saved Output:
The cropped ID card will be saved as a PNG file at the specified path.
