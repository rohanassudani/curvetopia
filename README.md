2D Shape Processing and Visualization Project
Overview
This project is designed to process 2D geometric shapes extracted from CSV files, visualize them as PNG images, convert them into SVG files, and detect and classify shapes using OpenCV. The project utilizes Python libraries such as OpenCV, Matplotlib, NumPy, and svgwrite.

Features
CSV Parsing: Reads and organizes 2D path coordinates from CSV files.
PNG Visualization: Plots the extracted paths and saves them as PNG images.
SVG Conversion: Converts the 2D paths into SVG format for scalable vector graphics.
Shape Detection: Detects and classifies shapes (e.g., triangles, squares, circles) within the PNG images using OpenCV.
Boundary Marking: Draws contours and bounding boxes around detected shapes for clear visualization.
Dependencies
Python 3.x
OpenCV (cv2)
NumPy
Matplotlib
svgwrite
Install the required packages using pip:

bash
Copy code
pip install opencv-python numpy matplotlib svgwrite
Usage
Prepare the CSV File:

Ensure your CSV file contains 2D coordinates in the expected format.
Run the Script:

Update the csv_path, png_path, and svg_path variables with your file paths.
Execute the script to process and visualize the shapes.
python
Copy code
# Example usage:
csv_path = 'path/to/your.csv'
png_path = 'output_image.png'
svg_path = 'output_image.svg'

# Read CSV, plot, and save as PNG
paths_XYs = read_csv(csv_path)
plot_and_save(paths_XYs, png_path)

# Convert to SVG (optional)
polylines2svg(paths_XYs, svg_path)

# Detect shapes and display
detect_shapes(png_path)
Shape Detection and Visualization:
The detected shapes are displayed with contours and annotated labels indicating the shape type.
Functions
read_csv(csv_path): Reads and organizes 2D coordinates from a CSV file.
plot_and_save(paths_XYs, png_path): Plots paths and saves them as a PNG image.
polylines2svg(paths_XYs, svg_path): Converts paths into an SVG file.
detect_shapes(png_path): Detects shapes within the PNG image using OpenCV.
Contributing
Contributions are welcome! Feel free to fork this repository and submit pull requests.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For any questions or inquiries, please reach out to assudanirohan2103@gamil.com
