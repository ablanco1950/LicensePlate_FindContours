# LicensePlate_FindContours
A recognition of car plates that instead of using photos with labels that mark the plates,
performs a license plate detection using cv2.FindContours. Labeling effort is saved, in exchange for lower performance
below 50% (50 hits in 117 images) compared to more than 70% that is achieved with a treatment from images with labels
 in the https://github.com/ablanco1950/LicensePlate_CLAHE project, starting in both cases from the same photo file to be processed.
Processing time is also much longer.

Requirements:

pytesseract

numpy

cv2

you

re

imutils

skimage (is scikit-image)

In the download directory you should find the downloaded test6Training.zip and must unzip folder: test6Training with all its subfolders,
containing the images for the test. This directory must be in the same directory where you program LicensePlateFindContours.py
 ( unziping may create two directories with you name test6Training and the images may not be founded when executing it, it would be necessary
copy of inner directory test6Training in the same directory where is LicensePlateFindContours.py)

from the download directory, run:

LicensePlateFindContours.py

The crops created to detect the license plates and the filters that have allowed their detection are indicated on the screen.
as well as the filters that have allowed the complete and exact recognition of the license plate by pytesseract.
For reasons of pricing time not all created crops are processed and processing is terminated earlier.

In the treatment, the accuracy of the result is checked because the license plate of the car of each photo  is known as
 the name of the photograph.
