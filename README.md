# Autonomous Lane Detection and Mapping

Welcome to the **Autonomous Lane Detection and Mapping** project! This repository contains a series of Jupyter notebooks that implement key computer vision techniques for autonomous vehicle lane detection. The focus is on transforming real-world road images into actionable data that can guide an autonomous vehicle to follow the lanes accurately. The key components of the project are outlined below:

## Notebooks Overview:

### 1. **Canny_Edge.ipynb**
The `Canny_Edge` notebook implements the Canny Edge Detection algorithm, which processes the road image to highlight the edges. The Canny Edge algorithm transforms the entire road into a 2D form by identifying and marking sharp changes in intensity. This step is crucial for simplifying the image and isolating the significant edges that define the lane boundaries.

### 2. **Hough_Transform.ipynb**
The `Hough_Transform` notebook builds upon the Canny Edge detection by utilizing the Hough Transform algorithm to detect and connect the most likely edges from the detected edge map. It draws continuous lines along the identified edges, thus allowing the model to form straight-line representations of the road lanes. This technique is crucial for identifying the potential lane markers and road boundaries in a more structured way.

### 3. **Hough_Transform_Quadrilateral.ipynb**
The `Hough_Transform_Quadrilateral` notebook takes the Hough Transform results further by combining multiple edge lines into a more coherent lane structure. This algorithm identifies quadrilateral-like shapes formed by intersecting lines and merges them into a unified lane, accounting for curves and slight road irregularities. It ensures that the lane detection is not just based on simple straight lines but can adapt to varying road conditions.

### 4. **color_Region.ipynb**
The `color_Region` notebook applies color to the detected lanes, highlighting them with a given color that represents the lane recognized by an autonomous vehicle. This color-coding helps visualize the detected lane and is also useful for training the vehicle's software to recognize and follow specific lanes. The chosen color will make the lane stand out clearly, assisting the autonomous system in differentiating between various road features.

## Requirements:
- Python 3.x
- Jupyter Notebook
- OpenCV
- Numpy

## Installation

1. **Clone this repository** to your local machine:
   ```bash
   git clone https://github.com/imumarfarooq/Lane_Detection/
2. **jupyter notebook**:
Open the desired notebook (Canny_Edge.ipynb, Hough_Transform.ipynb, Hough_Transform_Quadrilateral.ipynb, or color_Region.ipynb) in your browser.

Follow the steps in each notebook to run the algorithms and visualize the lane detection process. Each notebook contains comments and explanations to guide you through the process.

**Contributing**
Feel free to fork the repository, contribute improvements, or report bugs. Pull requests are always welcome! If you have any questions or suggestions, please open an issue.

**License**
This project is licensed under the MIT License - see the LICENSE file for details.
