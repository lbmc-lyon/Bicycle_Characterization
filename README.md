# Characterization of a bicycle
The codes that are presented here are used to :
 1. Determine the position of the center of gravity for one part of a bicycle in the world reference
 2. Determine the distance between the center of gravity and an axis given by two points of contact
 3. Compute the inertia along given axis from multiple measurements

## How to use this protocol ? 
1. First, you can read the *protocol.pdf* file to observe the experimental setup needed and understand the method used. 
2. Then, you can create an environment by using the *environment.yml* file. In your anaconda prompt, change directory to this one and type :
	conda env create -f environment.yml
3. When you will execute the codes, you will have an error saying that some dll files are missing, I managed to solve this issue by following this link : https://github.com/NaturalHistoryMuseum/pyzbar/issues/161
4. Finally, you can run the 4 *ipynb* files and complete the steps of the characterization. 

## Specifications
General :
In the notebooks, the things you need to do with the images are written below the current cell. When an image is displayed, check the notebook to see what you have to do.

For the center of gravity : 
Sometimes, the recognition of the QR code does not work. I am not able to explain all the reasons but I always managed to use at least 3 of the 4 images that I took during the experiment for the center of gravity. By modifying the $origin$ and $scalepercentage$ of the display, sometimes the QR code recognition works better. Plus, you have to make sure that your images have the highest quality available. Our images were taken with an Iphone 8 or a samsung Galaxy A71. 

For the inertia measurement :
If you have uncertainties that are way too high, you can verify your signals by checking the plots displayed to see if the optimized signals matched correctly with the original signals. You can also check the plots where Gyroscopic signals are displayed to verify if the signal used is in the same range as the measured signals. 

## Dictionnary :
- Method 1 : calibration with a QR code
- Method 2 : calibration with the frame of the bicycle
- Wheelbase : distance between the 2 contact points of the wheels

