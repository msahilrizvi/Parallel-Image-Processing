<!DOCTYPE html>
<html>
<head>
    <title>Parallel vs Sequential Image Processing</title>
</head>
<body>
    <h1>Parallel vs Sequential Image Processing</h1>
    <p><strong>Project Overview:</strong></p>
    <p>This project evaluates the performance differences between <strong>multiprocessing (parallel processing)</strong> and <strong>sequential processing</strong> techniques in image processing. It specifically focuses on <strong>background removal</strong> using OpenCV’s GrabCut algorithm.</p>
    
    <h2>Objective</h2>
    <p>The primary goal is to analyze whether parallelizing image processing tasks using Python’s <code>multiprocessing</code> module significantly improves execution speed and efficiency compared to sequential execution.</p>
    
    <h2>Methodology</h2>
    <ul>
        <li><strong>Dataset:</strong> A directory containing multiple images that require background removal.</li>
        <li><strong>Approach:</strong>
            <ul>
                <li><strong>Sequential Processing:</strong> Each image is processed one by one in a loop.</li>
                <li><strong>Parallel Processing:</strong> Multiple images are processed simultaneously using Python's <code>multiprocessing.Pool()</code>, leveraging multiple CPU cores.</li>
            </ul>
        </li>
        <li><strong>Background Removal Algorithm:</strong>
            <ul>
                <li>Uses OpenCV's <code>GrabCut</code> algorithm to separate the foreground from the background.</li>
                <li>A rectangular region is defined for initial segmentation.</li>
                <li>OpenCV applies iterative segmentation to refine the mask.</li>
            </ul>
        </li>
    </ul>
    
    <h2>Performance Metrics</h2>
    <ul>
        <li>Time taken per image in both methods.</li>
        <li>Total execution time for the entire dataset.</li>
        <li>CPU utilization comparison.</li>
    </ul>
    
    <h2>Expected Outcome</h2>
    <p>Multiprocessing should reduce overall processing time, making it more scalable for larger datasets. Sequential processing, while simpler, may take significantly longer, especially for bulk image processing tasks.</p>
    
    <h2>Use Cases</h2>
    <p>This project is useful for:</p>
    <ul>
        <li>Computer vision applications.</li>
        <li>Batch image processing workflows.</li>
        <li>Performance optimization in Python-based image processing.</li>
    </ul>
    
    <h2>Installation & Usage</h2>
    <pre><code>
    git clone https://github.com/your-username/Parallel-vs-Sequential-Image-Processing-OS.git
    cd Parallel-vs-Sequential-Image-Processing-OS
    pip install -r requirements.txt
    python main.py
    </code></pre>
    
    <h2>Contributing</h2>
    <p>Contributions are welcome! Feel free to fork this repository, create a new branch, and submit a pull request.</p>
    
    <h2>License</h2>
    <p>This project is licensed under the MIT License.</p>
</body>
</html>
