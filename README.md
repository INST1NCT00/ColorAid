# 🎨 ColorAid: AI-Powered Image Enhancement for Color Vision Deficiency (CVD)

🚀 **ColorAid** is an AI-powered tool that enhances images to make them more accessible for individuals with Color Vision Deficiency (CVD). Using computer vision and color science, the tool detects objects and intelligently adjusts colors to improve visual distinction.

---

## ✨ Features

- 🤖 **Object Detection**: Powered by Detectron2 (Mask R-CNN) for accurate object segmentation.
- 👁️ **CVD Support**: Simulates and enhances for major CVD types: Protanopia, Deuteranopia, Tritanopia, and more.
- 🎨 **Smart Color Enhancement**: Uses LAB color space and ΔE calculations to differentiate similar colors.
- 🌐 **Web Interface**: Gradio-powered, user-friendly web interface for easy image processing.
- 🔍 **CVD Simulation**: Visualize how images appear to users with different types of color blindness.

---

## 🔧 How It Works

1. 📤 Upload an image and select the CVD type.
2. 🤖 System detects objects using a pre-trained Mask R-CNN model.
3. 🔍 Compares color similarity between overlapping objects as perceived by the selected CVD type.
4. 🎨 Enhances colors of similar, overlapping objects for improved distinction.
5. 🔄 Iteratively refines until objects are clearly distinguishable.

---

## 🚀 Usage

1. Run the application:

   ```bash
   python cvd_enhancement_tool.py

2. 🌐 Open your browser at the provided URL (typically `http://127.0.0.1:7860`)
3. 📷 Upload an image and select the color vision deficiency type
4. ⚙️ Adjust settings (optional):
   - **Color Similarity Threshold:** How similar colors need to be considered problematic
   - **Object Overlap Threshold:** Minimum overlap to consider objects related
   - **Color Shift Amount:** Intensity of color adjustments
5. ✨ Click **Run Enhancement** to process the image.

---

## 🔬 Technical Details

- 👁️ **CVD Simulation:** Uses scientifically accurate transformation matrices
- 🤖 **Object Detection:** Mask R-CNN with ResNet-50 backbone, pre-trained on COCO
- 🎨 **Color Analysis:** LAB color space with ΔE distance measurement
- ⚡ **Enhancement:** Selective color adjustment of problematic object pairs

---

## 🎯 Use Cases

- 🌐 Web accessibility and inclusive design  
- 📚 Educational materials and data visualization  
- 🎨 UI/UX design testing  
- 🎮 Gaming and entertainment  
- 🏥 Medical imaging enhancement  
