# Automated Feature Segmentation from High-Resolution Satellite Imagery Using SAM: A Case Study Near Kandy Lake, Sri Lanka
## Overview
This analysis focuses on extracting and visualizing physical features in a small urban area near Kandy Lake, Sri Lanka, using high-resolution satellite imagery and the Segment Anything Model (SAM) from Meta AI. By leveraging the segment-geospatial (samgeo) Python library, we perform semantic segmentation of the landscape to identify and delineate visible features such as buildings, vegetation, roads, and water bodies.

The workflow begins by selecting a region near the lake, one of the most recognizable urban-natural landmarks in Sri Lanka. Using leafmap, we define and download satellite imagery tiles of this area. The SAM model is then applied to generate pixel-level segmentation masks, which are converted into vector format (GeoPackage and Shapefile) for further GIS-based analysis or visualization.

This approach provides a rapid and flexible method for automated land feature extraction from imagery, without the need for manual digitization or training a custom model, making it ideal for small-scale urban studies, rapid mapping, and remote sensing projects.

### Semantic segmentation of features near Kandy Lake, Sri Lanka, using the Segment Anything Model (SAM)
<img width="1920" height="747" alt="Screenshot (260)" src="https://github.com/user-attachments/assets/82ebe20e-4383-497e-ab56-f767c8ce0aea" />


## Tools & Libraries
- leafmap: For drawing AOI and visualizing maps interactively
- segment-geospatial (samgeo): For downloading basemap tiles, segmenting imagery, and exporting results
- os: File handling
- matplotlib: Optional for visualizing results

## Notes
1. The segmentation model used is the SAM ViT-H variant with pretrained weights (sam_vit_h_4b8939.pth). Make sure to upload or mount the checkpoint file.
2. You can experiment with different zoom levels, erosion parameters, and mask post-processing options.
3. SAM works well with clearly defined features such as buildings, roads, trees, and water bodies.






