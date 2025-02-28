Features

Enhances image quality using deep learning (CNNs).

Supports multiple input images.

Ensures proper color and pixel enhancement.

API-based website integration (users can upload and download enhanced images).

Five filter options (Warm, Natural, Vivid, etc.).

Prerequisites

Ensure you have Python and necessary libraries installed:

python --version  # Check Python version (>=3.8 recommended)

2️⃣ Clone the Repository

git clone https://github.com/your-repo/AI_Image_Enhancer.git
cd AI_Image_Enhancer

3️⃣ Create & Activate Virtual Environment

python -m venv venv
# Windows:
venv\Scripts\activate
# Linux/Mac:
source venv/bin/activate

4️⃣ Install Dependencies

pip install -r requirements.txt

📸 Usage Instructions

🔹 1. Run the Enhancement Script

python main.py --input "C:\My project\AI_Image_Enhancer\dataset\input1.jpg"

🔹 2. Batch Processing Multiple Images

python main.py --input "dataset/input1.jpg" "dataset/input2.jpg" "dataset/input3.jpg"

🔹 3. API-based Image Upload & Enhancement

To use the website UI for image uploads, start the backend:

python app.py  # Runs the Flask/Django server

🔧 Troubleshooting

1️⃣ Image Not Found Error

❌ Error: cv::findDecoder imread_: can't open/read file

✅ Fix: Ensure the image path is correct. Use absolute paths if needed.

import os
print(os.path.abspath("dataset/input1.jpg"))  # Verify path

2️⃣ NumPy Compatibility Issue

❌ Error: A module that was compiled using NumPy 1.x cannot be run in NumPy 2.0.2

✅ Fix: Downgrade NumPy:

pip uninstall numpy -y
pip install numpy==1.26.4

3️⃣ CUDA Not Found (For GPU Users)

❌ Warning: Could not load dynamic library 'cudart64_110.dll'

✅ Fix: Install correct CUDA version or switch to CPU mode.

pip install tensorflow-cpu

📝 Future Improvements

Optimize CNN model for faster processing.

Add more enhancement filters.

Improve website UI/UX.

📩 Contact

For any issues or feature requests, feel free to reach out!
📧 Email: abishektjabishek@gmail.com
