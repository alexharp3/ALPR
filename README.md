# Automatic License Plate Recognition (ALPR) Project

**Author:** Alexandria Harp  
**Email:** aharp@txstate.edu  
**Institution:** Texas State University, Department of Computer Science  

---

## Project Overview

This project attempts to implement an end-to-end **Automatic License Plate Recognition (ALPR)** system. The pipeline includes:

- **License plate detection** using YOLOv8.
- **Image preprocessing** using OpenCV (grayscale conversion, CLAHE, filtering, thresholding).
- **Character recognition** using Tesseract, EasyOCR, and a custom CNN for segmented characters.

The goal was to detect license plates from multi-country images and read their text accurately. All code, preprocessing steps, and experimental outputs are provided in the accompanying Jupyter Notebook.

---

## Dataset

- The dataset is in TSV format with columns: `filename`, `country`, `plate_text`.
- Images are stored in country-specific subfolders under `data/`.
- Sample images and preprocessing steps are available in the Notebook.

---

## Installation

1. Clone this repository:

```bash
git clone <your-repo-url>
cd alpr-project
python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows
pip install -r requirements.txt
