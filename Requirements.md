 
### 1. requirements
```text
numpy
opencv-python
matplotlib
scikit-image

```

 

## 🛠️ Installation & Usage

To replicate this forensic analysis on your local machine, follow these steps:

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

```

### 2. Install Dependencies

Ensure you have Python installed, then run:

```bash
pip install -r requirements.txt

```

### 3. Execution Logic

The core analysis is contained within the Python script. You can run the frame extraction and the MSE/SSIM comparison by executing the cells in the provided Jupyter Notebook or running the script directly:

```python
# To extract frames from your own videos:
extract_multiple_videos(real_video_path, real_output_folder)
extract_multiple_videos(fake_video_path, fake_output_folder)

# To generate the Flicker Analysis graph:
analyze_video_folders(real_output_folder, fake_output_folder)

```

---

### Why these specific libraries?

* **OpenCV (`opencv-python`):** Essential for high-speed video decoding and frame manipulation.
* **Matplotlib:** Used to generate the "MSE Over Time" visualization which is the primary evidence of the temporal flicker.
* **Scikit-Image (`scikit-image`):** Provides the industry-standard implementation of the Structural Similarity Index (SSIM).
* **NumPy:** Handles the heavy mathematical calculations for the Mean Squared Error (MSE) across thousands of pixels.

