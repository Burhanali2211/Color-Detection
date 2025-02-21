# Colour Detection using Pandas and OpenCV

## Overview
This project is a simple color detection application using Python, Pandas, and OpenCV. The program allows users to click on an image and get the name of the color at that pixel automatically. The color names are derived from a dataset containing color values.

## Features
- Load and display an image.
- Click anywhere on the image to detect the color.
- Retrieve the name and RGB values of the selected color.
- Uses a CSV file with predefined color names and their RGB values.
- Efficient color matching by calculating the minimum distance.

## Technologies Used
- Python
- OpenCV (cv2)
- Pandas

## Steps to Run the Project

### 1. Install Required Packages
Ensure you have Python installed, then install the required libraries:
```bash
pip install opencv-python pandas
```

### 2. Load the Image
The program loads an image where the user can click to detect colors.

### 3. Read the CSV File
A CSV file containing color names and their RGB values is read using Pandas.

### 4. Set Up Mouse Callback Event
A window is created to display the image, and a callback function is triggered when a mouse event occurs.

### 5. Detect and Display Color
When the user double-clicks on a pixel, the program:
- Extracts the RGB values of the clicked pixel.
- Finds the closest matching color name from the CSV file.
- Displays the detected color name and RGB values on the image.

## Formula Used for Color Matching
The program calculates the closest color using the formula:
```python
d = abs(Red - ithRedColor) + abs(Green - ithGreenColor) + abs(Blue - ithBlueColor)
```
The color with the smallest distance is considered the best match.

## Running the Project
1. Save your image in the project folder.
2. Run the Python script:
```bash
python Color-Detection.py
```
3. Click on the image to detect colors.

## Example Screenshot
(Add a screenshot here if available)

## Project Structure
```
|-- Color-Detection.py
|-- colors.csv
|-- image.jpg
|-- README.md
```

## Future Improvements
- Support for multiple images.
- Enhanced color matching algorithm.
- GUI interface for a better user experience.

## License
This project is open-source and available for modification and distribution.

---
Happy Coding! 😊

