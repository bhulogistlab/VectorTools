# GeoVec Studio 🌍

**A Cloud-Native WebGIS Platform for Advanced Spatial Data Processing**

GeoVec Studio is a high-performance, browser-based WebGIS application engineered for seamless spatial data processing. Developed by Cogniterra Labs, the platform brings desktop-grade GIS capabilities into the browser, featuring integrated raster and vector geoprocessing tools designed to handle heavy spatial datasets without compromising UI fluidity.

## 🚀 Key Features

* **Advanced Vector Operations:** In-browser geoprocessing (Buffer, Intersect, Dissolve, Voronoi, TIN) utilizing robust spatial algorithms via Turf.js.
* **Custom Binary Parsing:** Zero-dependency, client-side parsing of complex spatial files (Shapefile, DBF, GeoJSON, KML, GPX) directly via `ArrayBuffer` and `DataView`.
* **Cloud-Optimized Raster Workflows:** Integration of **SpatioTemporal Asset Catalog (STAC)** and **Cloud Optimized GeoTIFF (COG)** architectures to enable dynamic querying and rapid cloud-rendering of heavy imagery.
* **On-the-Fly Spectral Calculators:** Integrated spectral indices calculators (e.g., NDVI, NDWI) utilizing logarithmic stretch and S-curve contrast enhancements for real-time raster band math.
* **Lean Architecture:** State management and spatial operations are handled securely and efficiently in the client, drastically reducing server-side computational bottlenecks.

## 🛠️ Tech Stack

* **Frontend:** Vanilla JavaScript, HTML5, CSS3
* **Mapping Engine:** Leaflet.js
* **Vector Mathematics:** Turf.js
* **Raster Rendering:** GeoRaster, georaster-layer-for-leaflet, chroma.js
* **Coordinate Reprojection:** Proj4js

## 🧠 System Architecture

GeoVec is built on a "compute-where-it-makes-sense" philosophy. By leveraging modern browser APIs, heavy vector topology math is executed locally, while raster rendering leans on STAC/COG standards (HTTP Range Requests). This means only the pixels necessary for the current viewport are requested over the network, bypassing the need to download gigabytes of satellite imagery for spectral analysis.

## 👥 Development Team
* **Utkarsh Sharma** 
* **Sayandip Das** 
* **Organization:** Cogniterra Labs

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
