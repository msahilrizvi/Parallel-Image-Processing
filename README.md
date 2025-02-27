#Parallel-vs-Sequential-Image-Processing-OS

This project evaluates the performance differences between multiprocessing (parallel processing) and normal (sequential processing) techniques in image processing, specifically focusing on background removal using OpenCV’s GrabCut algorithm.

Objective:
The primary goal is to analyze whether parallelizing image processing tasks using Python’s multiprocessing module significantly improves execution speed and efficiency compared to sequential execution.

Methodology:
Dataset: A directory containing multiple images that need background removal.
Approach:
Sequential Processing: Each image is processed one by one in a loop.
Parallel Processing: Multiple images are processed simultaneously using Python's multiprocessing.Pool(), utilizing multiple CPU cores.
Background Removal Algorithm:
The GrabCut algorithm is used to separate the foreground from the background.
A rectangular region is defined for initial segmentation.
OpenCV applies iterative segmentation to refine the mask.
Performance Metrics:
Time taken per image in both methods.
Total execution time for the entire dataset.
CPU utilization comparison.
Expected Outcome:
Multiprocessing should reduce overall processing time, making it more scalable for larger datasets.
Sequential processing, while simpler, may take significantly longer, especially for bulk image processing tasks.
The results will help determine whether parallelization is worth implementing in image-heavy applications.
This project is useful for computer vision applications, batch image processing, and performance optimization in Python-based image processing workflows.
