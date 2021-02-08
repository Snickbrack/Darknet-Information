# Darknet-Information
This Repo contains information which I have found while working with the "darknet" Detection Software (https://github.com/pjreddie/darknet and/or https://github.com/alexeyab/darknet) created by PJReddie and AlexeyAB.

## Does Darknet load the images for training in the same order as I have defined it in my "train.txt"- or "train.list"-File?
No. Darknet grabs a collection of random chosen images. The Amount of used Images is calculated as follows:

`numberOfImages = batchSize * subdivisions * numberOfGPU`

Darknet will use a random Index to select an image out of the list of given train images. 



