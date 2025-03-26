# Region Splitting and Merging (Color Image Processing)

This project implements **Region Splitting and Merging** for color images using **OpenCV** and **NumPy**. The algorithm recursively divides an image into smaller regions based on color variance and then merges similar regions to produce a simplified image representation.

## 📂 Project Structure
```
├── Region_Splitting.ipynb             # Jupyter Notebook with main code
└── regionn.jpeg                       # Input image (sample)
```

## 📜 Features

- **Region Splitting**: Recursively divides the image based on a color variance threshold.
- **Region Merging**: Combines similar regions to reduce image complexity.
- **Optimized Performance**: Uses deque for faster operations and dynamic merging for better accuracy.
- **Visualization**: Displays the original and processed images side-by-side.
- **Region Count Output**: Prints the total number of regions after splitting.

## 📊 Requirements

Ensure the following packages are installed:

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- Matplotlib

To install dependencies, run:

```bash
pip install opencv-python numpy matplotlib
```

## 🚀 Usage

1. Ensure you have the **regionn.jpeg** image in the same directory.

2. Open the Jupyter Notebook:

```bash
jupyter notebook Region_Splitting.ipynb
```

3. Execute the notebook cells to:
   - Load and display the **original image**.
   - Perform **region splitting and merging**.
   - Display the **processed image** and **total region count**.

## 🔧 Parameters

You can adjust the following parameters in the notebook:

- **threshold** (for splitting): Controls the sensitivity to color variance during region splitting.
- **merge_threshold** (for merging): Determines how similar regions must be to merge.

Example:
```python
regions = split_region_color(image, threshold=15)
merged_image = merge_regions_color(image, regions, merge_threshold=10)
```

## 📷 Example Output

1. **Original Image**: Displays the original color image.
2. **Region Merged Image**: Shows the image after splitting and merging with regions labeled.

## 📌 Notes

- Ensure the input image is in the **same directory** as the notebook.
- Adjust **thresholds** for different image complexities.

## 📖 References
- Image Processing with OpenCV
- Region Splitting and Merging Algorithms

## 📝 License

This project is open-source and available under the **MIT License**.

