# Lane Detection System Using Image Processing

<p align="center">
  <a href="https://opencv.org/">
    <img src="https://img.shields.io/badge/OpenCV-4.x-blue?logo=opencv&logoColor=white" alt="OpenCV">
  </a>
  <a href="https://numpy.org/">
    <img src="https://img.shields.io/badge/NumPy-1.x-orange?logo=numpy&logoColor=white" alt="NumPy">
  </a>
  <a href="https://matplotlib.org/">
    <img src="https://img.shields.io/badge/Matplotlib-3.x-green?logo=matplotlib&logoColor=white" alt="Matplotlib">
  </a>
</p>
<p align="center">
  <a href="README.md">
    <img src="https://img.shields.io/badge/lang-English-blue.svg" alt="English">
  </a>
  <a href="README_TR.md">
    <img src="https://img.shields.io/badge/lang-Türkçe-red.svg" alt="Turkish">
  </a>
</p>

## About the Project

This project focuses on creating a system that accurately detects road lane lines using image processing techniques. By analyzing video frames or real-time feeds, the system identifies road lanes and visually marks them. It explores the applications of modern image processing techniques for lane detection.

• **Goal**: Accurately identify and track road lanes, which is crucial for autonomous vehicle systems.

• **Techniques**: Image processing steps have been implemented using popular libraries such as OpenCV and Matplotlib.

• **Model Status**: This project does not include model training; it is a basic implementation of image processing techniques.

<h2>📋 Project Steps</h2>

<h3>1. Extracting a Frame from Video</h3>
<p>A video frame is extracted for analysis. This ensures that the operations work effectively on real-time video streams.</p>
• This is the foundational step for processing video data.  
<img src="Images/test.png" alt="Frame Extraction">

<h3>2. Converting BGR to RGB</h3>
<p>Images read in BGR format with OpenCV are converted to RGB format to display correctly using Matplotlib.</p>
• Color format conversion ensures accurate visualization of images.  
<img src="Images/BGRtoRGB.png" alt="BGR Format">
<img src="Images/Matplotlib.png" alt="RGB Format">

<h3>3. Determining Image Dimensions</h3>
<p>The dimensions of the image are determined for further analysis.</p>
• The image's width, height, and channel count are calculated, which is essential for subsequent processing steps.  
<img src="Images/Shape.png" alt="Image Dimensions">

<h3>4. Cropping the Image (ROI)</h3>
<p>The image is cropped to focus only on the area containing the lane lines.</p>
• Region of Interest (ROI) cropping removes unnecessary parts of the image to focus on lane detection.  
<img src="Images/Cropped_Image.png" alt="Cropped Image">

<h3>5. Converting the Image to Grayscale</h3>
<p>The image is converted to grayscale to simplify analysis.</p>
• Grayscale conversion removes color information, focusing only on brightness levels. This simplifies tasks like edge detection.  
<img src="Images/Gray.png" alt="Grayscale Image">

<h3>6. Edge Detection Using Canny Filter</h3>
<p>The Canny algorithm is used to detect edges in the image.</p>
• The Canny edge detection filter highlights edges, allowing clear identification of lane boundaries.  
<img src="Images/Canny.png" alt="Canny Edge Detection">
<img src="Images/Cropped_Canny.png" alt="Cropped Canny Image">

<h3>7. Drawing Lane Lines</h3>
<p>Detected edges are used to draw lane lines on the image.</p>
• After detecting edges, lane lines are marked, making them clearly visible on the road.

<h2>🎥 Output</h2>
<p>The final output of the project is shown below.</p>
<img src="Videos/output_gif.gif" alt="Output GIF">

<h2>🛠️ Technologies Used</h2>
<ul>
  <li><strong>Python</strong> - The main programming language of the project.</li>
  <li><strong>OpenCV</strong> - Used for image processing operations.</li>
  <li><strong>Matplotlib</strong> - Used for visualizing and analyzing images.</li>
</ul>

<h2>📂 How to Run the Project</h2>
<p>Follow the steps below to run the project:</p>
<ol>
  <li>Clone the repository:  
    <code>git clone https://github.com/username/lane-detection.git</code>  
    <code>cd lane-detection</code>
  </li>
  <li>Install the required libraries:  
    <code>pip install opencv-python matplotlib</code>
  </li>
  <li>Run the project file:  
    <code>python main.py</code>
  </li>
</ol>

<h2>👨‍💻 Developers</h2>
<p><strong>Your Name</strong></p>
<p><strong>Email:</strong> your-email@example.com</p>
<p><strong>LinkedIn:</strong> <a href="https://linkedin.com/in/yourname" target="_blank">Visit My Profile</a></p>

<footer>
  <p>© 2024 Lane Detection Project | All Rights Reserved</p>
</footer>
