# Summer-Project
 
Finding wake angle and wavelengths from a top-down video of a water tank, using Hough transforms.
 
The analysis is in `Summer_Project_Analysis.ipynb`. For each frame it auto-crops to the region of interest, thresholds the image using its own mean and standard deviation to pull out the wave crests, runs a probabilistic Hough line transform (scikit-image) to find the crest lines, and uses those lines to get the wake angle and the wavelengths.
 
## Running it
 
Written for Google Colab with the frames in Google Drive, so the first cell mounts Drive. Frames are read from numbered image files.
 
Uses OpenCV, scikit-image, NumPy, SciPy, PIL and Matplotlib.
