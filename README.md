# Parallel vs Sequential Image Processing

## Project Overview
This project evaluates the performance differences between **multiprocessing (parallel processing)** and **sequential processing** techniques in image processing. It specifically focuses on **background removal** using OpenCV’s GrabCut algorithm.

## Objective
The primary goal is to analyze whether parallelizing image processing tasks using Python’s `multiprocessing` module significantly improves execution speed and efficiency compared to sequential execution.

## Methodology

- **Dataset:** A directory containing multiple images that require background removal.
- **Approach:**
  - **Sequential Processing:** Each image is processed one by one in a loop.
  - **Parallel Processing:** Multiple images are processed simultaneously using Python's `multiprocessing.Pool()`, leveraging multiple CPU cores.
- **Background Removal Algorithm:**
  - Uses OpenCV's `GrabCut` algorithm to separate the foreground from the background.
  - A rectangular region is defined for initial segmentation.
  - OpenCV applies iterative segmentation to refine the mask.

## Performance Metrics
- Time taken per image in both methods.
- Total execution time for the entire dataset.
- CPU utilization comparison.

## Expected Outcome
Multiprocessing should reduce overall processing time, making it more scalable for larger datasets. Sequential processing, while simpler, may take significantly longer, especially for bulk image processing tasks.

## Use Cases
This project is useful for:
- Computer vision applications.
- Batch image processing workflows.
- Performance optimization in Python-based image processing.

## Installation & Usage
```sh
# Clone the repository
git clone https://github.com/your-username/Parallel-vs-Sequential-Image-Processing-OS.git

# Navigate to the project directory
cd Parallel-vs-Sequential-Image-Processing-OS

# Install dependencies
pip install -r requirements.txt

# Run the project
python main.py
```

## Contributing
Contributions are welcome! Feel free to fork this repository, create a new branch, and submit a pull request.

## License
This project is licensed under the MIT License.
