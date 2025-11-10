# Canny-Edge-Detection.
# workshop-3 - Canny Edge Detection
# Name :MANIKUMAR D.K
# reg no:212223230121
## AIM :
To implement the Canny Edge Detection algorithm on a digital image to accurately detect and highlight significant edges while minimizing noise and false detections.

## PROGRAM
```
import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('sakthivel.jpg',cv2.IMREAD_GRAYSCALE)
# Apply Gaussian blur to reduce noise
blurred =cv2.GaussianBlur(img, (5,5),0)
# Detect edges using Canny
edges = cv2.Canny(blurred, 50, 150) #Adjust threshold values as needed
# Plot the original image and the detected edges
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```
## OUTPUT
![WhatsApp Image 2025-11-10 at 11 11 16_3bbf93ce](https://github.com/user-attachments/assets/b5db6d95-49e2-4efd-874b-37ede957b68d)

## RESULT:
The Canny Edge Detection algorithm was successfully implemented.
