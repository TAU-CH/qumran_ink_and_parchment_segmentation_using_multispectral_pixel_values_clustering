# qumran_ink_and_parchment_segmentation_using_multipectral_pixel_values_clustering
This project focuses on segmenting ink on the Dead Sea Scroll fragments by clustering multispectral pixel values.

## Notebook Summary: multispectral_characterization_for_ink_parchment_hole_rice_background_pixels.ipynb

### Introduction
This notebook is structured to perform detailed multispectral analysis of different regions in a set of images. It focuses on ink, parchment, holes, rice, background, and other specified regions. The analyses are visualized through various plots to provide insights into the characteristics and variations of these regions across the multispectral images.

### Display and Histogram Equalization
Two primary functions are defined:
- `display_image(image, vmax)`: Displays images with a specified maximum value.
- `histogram_equalization(image)`: Performs histogram equalization on 16-bit images to enhance contrast.

### Reading Multispectral Images
- The folder containing multispectral images is [here](https://tauex-my.sharepoint.com/:u:/g/personal/berat_tauex_tau_ac_il/Ee9l3mTCIzNNteMEEKLhfsIBpCohdMuu3HYIVIFbIKjIGQ?e=PV4tO1).
- It constructs a multispectral image cube from this [folder](https://tauex-my.sharepoint.com/:u:/g/personal/berat_tauex_tau_ac_il/Ee9l3mTCIzNNteMEEKLhfsIBpCohdMuu3HYIVIFbIKjIGQ?e=PV4tO1). It reads the 12 `.tif` image files in the folder and stacks them along the first dimension to create the image cube.
- The images are cropped to focus on a specific fragment region.

### Image Processing and Analysis
Several image processing functions are defined and used:
- `plot_combined_trend`: Analyzes and plots trends for different categories (e.g., ink, background, hole, rice).
- `plot_pixel_trend`: Analyzes specific pixels and their trends over multispectral images.

### Visualization
The notebook includes several plots and visualizations to show the trends and characteristics of different regions' multispectral pixel values. Combined trends for different sets of these regions are plotted.

### Highlighting Regions
The `show_image_with_circle` function highlights specific regions corresponding to different regions in the images.


## Notebook Summary: segmenting_ink_using_multispectral_value_clustering_1.ipynb

### Introduction
The notebook titled "segmenting_ink_using_multispectral_value_clustering_1.ipynb" focuses on segmenting and analyzing various regions such as ink, parchment, holes, rice, and background using clustering techniques.

### Reading Multispectral Images
- The folder containing multispectral images is specified.
- Images are read into an array called `image_cube`.
- The images are cropped to focus on a specific fragment region.

## Clustering and Segmentation
- The notebook uses clustering techniques (KMeans and Gaussian Mixture) to segment the multispectral images into different regions based on pixel values.
- It assigns contrastive colors to different clusters for visualization.
- Functions like `get_pixel_info` and `plot_pixel_distribution` analyze and visualize the clustering results.

## Thresholding Techniques
- Various thresholding techniques such as Otsu, Niblack, and Sauvola are applied to segment specific regions in the images.
- The results of these techniques are visualized using matplotlib.





