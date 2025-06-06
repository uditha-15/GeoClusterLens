# GeoClusterLens: Clustering & Visualizing Geotagged Images using DBSCAN

![Map Visualization](https://img.shields.io/badge/Map-Folium-green)
![Clustering](https://img.shields.io/badge/Clustering-DBSCAN-blue)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle--Geotagged--Images-orange)

**GeoClusterLens** is a Python-based tool for extracting GPS metadata from images, clustering them based on geographic coordinates using the DBSCAN algorithm, and visualizing the results interactively on a map using Folium.

---

## 📁 Dataset

This project uses the **[Geotagged Images Dataset](https://www.kaggle.com/datasets/deepzsenu/geotagged-images)** from Kaggle, which contains various images embedded with GPS EXIF metadata.

---

## ✨ Features

- Extracts latitude and longitude from EXIF metadata of `.jpg` or `.jpeg` images.
- Applies **DBSCAN clustering** on the geolocations to group images taken nearby.
- Generates an interactive **HTML map** with clustered markers and tooltips.
- Saves clustered image metadata to a CSV file for further analysis.

---

## 🧰 Dependencies

Make sure to install the following Python libraries:

```bash
pip install exifread pandas numpy scikit-learn folium
```

## 🗺️ Map Preview

Once the ipynb cells finish running, a geotagged_clusters_map.html is created. Open that in your browser to view a live interactive map of the clustered image locations.

Each cluster has its own color.
Outliers (noise points) are marked in red.
Hover over markers to view the image filename and cluster ID.

