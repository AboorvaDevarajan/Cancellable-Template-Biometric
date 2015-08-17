# Cancellable-Template

Understanding and Implementing Cancellable Templates in Biometrics for privacy protection

<b>Implemented minutiae extraction from the finger print image. </b>

Steps involved
  1. Image thinning.
  2. Detection of the ridges and bifurcations.
  3. Plotting the (x,y)  coordinates which contains the minutiae points.

<b> Transform input image to black and white image. </b>

![input](https://cloud.githubusercontent.com/assets/3117217/9293507/32d008b0-444b-11e5-9853-82b97d6af00d.png)

<b> Image thinning -  Convert input image to thin image. </b>

![thin_finger_print](https://cloud.githubusercontent.com/assets/3117217/9293509/32d9e484-444b-11e5-87d7-a2a30194cd44.png)

<b> Detecting the bifurcations and ridges. </b>

<b> Bifurcation Points </b>

![bifurcation](https://cloud.githubusercontent.com/assets/3117217/9293506/32ce1230-444b-11e5-9e28-640422762576.png)

<b> Minutiae Points </b>

![minutiae](https://cloud.githubusercontent.com/assets/3117217/9293508/32d3e728-444b-11e5-8ba4-9bdfa23dcbc9.png)

<b> Converting coordinates to csv for processing </b>

Get the respective (x,y) coordinates for the corresponding ridges and bifurcation points (minutiae) and store it in a csv / array.

Coordinates of  minutiae points are stored in an 1-D array and the corresponding line graph is plotted to visualize the points.

![screenshot from 2015-08-17 10 27 42](https://cloud.githubusercontent.com/assets/3117217/9298375/85c0ec6c-44cb-11e5-99de-733e6bdcfe01.png)


<b> Cancellable Template implementation (POC) : Method 1 </b>

Proposed Method : 1 
 1. Distance calculation between the minutiae coordinates using neo4j graph database.
 2. Implementing reverse tranformation logic.


Implemented:

1. Choose a reference point in the list of minutiae.
2. Find the distance from the reference minutiae to all other minutiae points.

![screenshot from 2015-08-17 10 24 31](https://cloud.githubusercontent.com/assets/3117217/9298390/e42232d4-44cb-11e5-9d1f-c95d274fcfe4.png)
