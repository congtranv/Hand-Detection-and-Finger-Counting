# Hand-Gestures-and-Finger-Counting
A python program to recognize hand gestures and count fingers using OpenCV library. 

Here are some code parts followed by some images representing the code results.

```
if len(contours) > 0:
        # Find the maximum contour each time (on each frame)
        # --Max Contour--
        max_contour = max(contours, key=cv2.contourArea)
        # Draw maximum contour (blue color)
        cv2.drawContours(test_window, max_contour, -1, (255,0,0), 3)
```
<p align="center">
  <img width="300" height="250" src="Images/1.Contour/image1.jpg">
  <img width="300" height="250" src="Images/1.Contour/image2.jpg">
  <img width="300" height="250" src="Images/1.Contour/image3.jpg">
</p>

<p align="center">
  <img width="300" height="250" src="Images/1.Contour/image4.jpg">
  <img width="300" height="250" src="Images/1.Contour/image5.jpg">
</p>

```
        # Find the convex hull "around" the max_contour
        # --Convex Hull--
        convhull = cv2.convexHull(max_contour, returnPoints = True) 
        # Draw convex hull (red color)
        cv2.drawContours(test_window, [convhull], -1, (0,0,255), 3, 2)
```
<p align="center">
  <img width="300" height="250" src="Images/2.Convex_Hull/image1.jpg">
  <img width="300" height="250" src="Images/2.Convex_Hull/image2.jpg">
  <img width="300" height="250" src="Images/2.Convex_Hull/image3.jpg">
</p>

<p align="center">
  <img width="300" height="250" src="Images/2.Convex_Hull/image4.jpg">
  <img width="300" height="250" src="Images/2.Convex_Hull/image5.jpg">
  <img width="300" height="250" src="Images/2.Convex_Hull/image6.jpg">
</p>

## Author
* **Konstantinos Thanos**
