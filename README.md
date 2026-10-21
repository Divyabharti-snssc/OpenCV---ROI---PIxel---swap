# ## Nalanda IT Zone.
* ** Project report under Nalanda it zone internship program.
  # Name : **Divya Bharti
  # Course : **BSC (5th Semester)
  # Session : **(2024-2028)
  # University Roll Number : **(24281200454)
  # University Registration NUMBER :**(24120023228)
  # College Name : S.N. Singh College
   
  # Institute Name : **(Nalanda It Zone)
  # Application ID : **(2PFWM0BB)
  
  # Project Topic  : **(OpenCV - ROI - Pixel - swap.

# ## Image Processing Basic ROI and Pixel Manipulation.
* ** This project explain two funda mental concepts of image processing using **Python** and **OpenCV**: **Region of Interest (ROI)** and **Exchanging pixel values**.

## 1. What is (ROI) ?
**Region of Interest(ROI)** is a specific portion or sub-part of on image that your want to isolate to apply filters, operations, or processing. 

# ## Why is it important 
* **Efficiency:** Processing only a small relevant section in a instead of the entire image significantly saves computational time and speeds up execution.
* **Accuracy:** For example, in face detection system the algorithm define area as the ROI and ignores the rest of the background.

# ## How to use ROI in OpenCV:
* ** open CV represents image and **NumPy arrays**. Therefore, we can easily extract and ROI using array slicing.

'''python 
# Syntax
# ROI = image[ymin:ymax, xmin:xmax]

import cv2

# 1. Load the input image
image = cv2.imread('input.jpg')

# 2. Crop the ROI(e.g., y from 100 to 300, x from 200 to 400)
roi = image[100:300, 200:400]

# 3. Display the isolated region in a split window 
cv2.imshow('ROI Window' , roi)
cv2.waitkey(0)
cv2.destroyAllWindows()
'''

---

# ## How to Exchange Pixel Value ?
* ** Exchanging or manipulation pixel values modifying the color/intensity data of specific pixel or replacing one region of an image with another region.

### Method 1: Modifying a Specific  values (Direct Manipulation) 
you can directly change the colour of a specific co-ordinate using its array index:python
'''python 
# Change the pixel at(y = 50, X = 50)
to pure Blue (OpenCV uses BGR formate)
image[50, 50] = [255, 0, 0,]
'''

### Method 2. Swapping/Exchanging Two Regions (Image Patches)
If you have tow areas of the exact same size, you can swap their pixel values like this:

'''python 
import cv2

# Load the input image
image = cv2.imread('input.jpg')

# 1. Copy the first region(Region 1)
region 1 = imag[100:200, 100,200].Copy()

# 2. Copy the second region(Region 2)
region 2 = imag[300:400, 300:400].Copy()

# 3. Exchange/Swap the value between both region
image[100:200, 100:200] = region_1
image[300:400, 300:400] = region_2

# Display the final swapped result
cv2.imshow('Swapped Image',image)
cv2.waitkey(0)
cv2.destroyAllWindowd()
'''

> **Important Note:** When exchanging or replacing pixel blocks, both rgions must have the **exact same dimensions (height and weight) if the size do not match, Numpy will throw a 'Value Error'.

---

## Requirements 
* Python 3.x
* OpenCV ('pip install opencv-python')
* NumPy ('pip install numpy')


    # Thank You 🌿

       * Respectful thanks to the teacher for guidance checking my project file.



  
