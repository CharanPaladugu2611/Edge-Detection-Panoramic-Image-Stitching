# 🧠 Edge Detection & Panoramic Image Stitching

This project showcases two key areas of classical computer vision:

* Edge and line detection using Canny and Hough Transform, applied frame-by-frame on a video to produce corner-tracked and line-annotated output.

* Panoramic image stitching using SIFT, Brute-Force feature matching, manual RANSAC-based homography, and warping — resulting in a smoothly blended panorama from overlapping photos.

It uses OpenCV, NumPy, and matplotlib to simulate and visualize these vision algorithms.

## 🎯 Part 1: Edge Detection & Frame-Based Line Tracking
Features:
* Laplacian Variance Filter: Detects sharp frames for further processing

* Canny Edge Detection: Identifies strong edges

* Hough Line Transform: Finds dominant lines

* Intersection Computation: Calculates line intersections

* Corner Filtering: Removes invalid points outside frame boundaries

* Line Overlay + Corner Marking: Draws annotated frames

📹 Output is saved as output.mp4, skipping blurry frames and showing corner-tracked lines.

## 📈 Part 2: Panoramic Image Stitching
Steps:
* Uses SIFT for feature detection

* Performs Brute-Force matching with ratio test

* Computes manual RANSAC-based homography using DLT

* Applies perspective warping to align images

## 🧠 Key Concepts
* Image gradient filtering using Laplacian variance

* Edge maps and binary thresholding

* Line detection via probabilistic Hough transform

* Homography estimation from feature matches

* Panoramic warping with forward compositing

* Robust estimation with RANSAC

* Sequentially stitches multiple images into a panorama

📸 Tested on 4 overlapping landscape images.
![image](https://github.com/user-attachments/assets/399290fd-1d4d-4713-bc68-fe8ae9283f69)
