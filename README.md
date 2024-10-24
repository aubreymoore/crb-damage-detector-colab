# crb-damage-detector-colab

## Note on Image Size

The current model was trained on images having a maximum width or height of 960 pixels.
I recommend resizing your images before uploading.
This is not absolutely necessary.
But it will significantly speed up downloads and uploads.
It is important to use a method which preserves EXIF metadata, especially
if GPS coordinates are embedde within your images. 
```ImageMagick``` can be used. The following command resizes all images with the
current folder.
```
mogrify -resize "960>" *.JPG
```

# Quick Start - Using Example Data Stored in This Repository

## Scan images referred to by a list of URLS

This is the most efficient way of using crb-damage-detector.

1. Open the page for [data/urls.txt](data/urls.txt) and click on the ```Download raw file``` button [![](images/download_raw.png)](#)
2. Open crb-damage-detector in Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aubreymoore/crb-damage-detector-colab/blob/main/detect_and_annotate.ipynb)
3. Click on the ```Browse``` button and navigate to where you downloaded ```urls.txt``` (```Downloads/urls.txt``` for example)
4. After data from your scanned images will be saved in a temporary ```OUTPUT``` Colab folder. When all images have been scanned, the ```OUTPUT``` folder will be automatically downloaded to your computer as a ```ZIP``` file (```OUTPUT.zip```)

## (Optional) Scan images stored in a ZIP file

1. Open the page for [data/images.zip](data/images.zip) and click on the ```Download raw file``` button [![](images/download_raw.png)](#)
2. Open crb-damage-detector in Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aubreymoore/crb-damage-detector-colab/blob/main/detect_and_annotate.ipynb)
3. Click on the ```Browse``` button and navigate to where you downloaded ```images.zip``` (```Downloads/images.zip``` for example)
4. After data from your scanned images will be saved in a temporary ```OUTPUT``` Colab folder. When all images have been scanned, the ```OUTPUT``` folder will be automatically downloaded to your computer as a ```ZIP``` file (```OUTPUT.zip```)
