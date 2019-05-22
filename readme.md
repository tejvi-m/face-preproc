# Using dlib and image processing to align images of human faces #

Uses dlib and OpenCV.

Works by calculating the angle the line that the reference points on the nose make with the horizontal, and the image is rotated by the appropriate angle.

Based on the reference points of the newly rotated image, the image is cropped to only focus on the face. This can be done using either OpenCv's Haarcascades or dlib. Haarcascades have been used here.

Was tested extensively on the [ColorFeret dataset](https://www.nist.gov/itl/iad/image-group/color-feret-database).

Doesn't work as well (about 5 or 6 images for which the output was worse out of 3000 frontal face images in the dataset) when the nose is naturally slant.
Can be corrected by using the line along the eyes instead.


![referenceimage](https://github.com/tejvi-m/face-preproc/blob/master/dlibLandmarks.png "references")

an image of all the numbered landmark points

still a work in progress.
code to be added : scaling and full alignment.
