# DocScanner

A Python notebook-based document scanning and processing tool (Jupyter Notebook: `DocScanner.ipynb`).  
Provides features like image capture, edge detection, perspective correction, and export to PDF/image.

## 🚀 Features
- Load or capture document images  
- Automatic edge detection & document cropping  
- Perspective transform to flatten the document  
- Image enhancements (contrast/brightness/denoise)  
- Export output as PDF or high-quality image  
- Optional: Batch process multiple pages into one PDF  

## 🧰 Prerequisites
- Python 3.7+  
- Jupyter Notebook or JupyterLab  
- Required libraries (example):  
  ```bash
  pip install opencv-python numpy matplotlib scikit-image pillow
## 📂 Usage
  1. Clone the repository
       git clone https://github.com/h5rsh/DocScanner.git
       cd DocScanner
  2. Open Jupyter Notebook: 
       jupyter notebook DocScanner.ipynb
  3. Follow the notebook cells:
      - Load image(s)
      - Run edge-detection and transform steps
      - Apply image enhancements
      - Export scanned document
  4. To export as PDF, use the provided export cell or add:
      from PIL import Image
      imgs = [...]  # list of PIL Image objects
      imgs[0].save('output.pdf', save_all=True, append_images=imgs[1:])
## 🎯 Customisation
  - Adjust parameters for edge detection (Canny thresholds, Hough lines)
  - Modify perspective transform based on document size/shape
  - Add custom filters for image enhancement (denoise, sharpen, binarize)
  - Extend notebook to include OCR (e.g., using Tesseract) or mobile image capture support
## 📋 File Structure

  DocScanner/
   ├── DocScanner.ipynb       ← Main notebook
   ├── images/                ← Sample document images (optional)
   └── output/                ← Output folder for scanned PDFs/images
## ✅ Licence

  Specify the licence here (e.g., MIT License).

## 📞 Contact

  For issues, please open an issue in the GitHub repository or contact the author.  

