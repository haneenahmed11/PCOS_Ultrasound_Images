# PCOS Ultrasound Images Classification

##  Objective
This project aims to **classify ovarian ultrasound images to detect Polycystic Ovary Syndrome (PCOS)** using a **Convolutional Neural Network (CNN)**.  
The goal is to assist doctors in faster and more accurate diagnosis.

##  Dataset
- Source: Kaggle – **PCOS 2023 Ultrasound Dataset**  
- Dataset structure:  
  - `train/infected` – images labeled as infected  
  - `train/notinfected` – images labeled as not infected  
  - `test/infected` and `test/notinfected` for testing  
- Images are resized to **128x128 pixels** to fit the model input.

##  Tools & Libraries
- Python 3.x  
- Image processing & analysis: `numpy`, `pandas`, `matplotlib`, `opencv`, `PIL`  
- Deep learning: `tensorflow`, `keras`  
- Optional interface/server: `Gradio`, `FastAPI`, `ngrok`  
- Model saving & conversion: `TFLite`  

##  Project Steps
1. **Copy data to working directory** and remove corrupted images.  
2. **Visualize sample images** to verify the dataset.  
3. **Prepare data** using `ImageDataGenerator` for training and testing.  
4. **Build CNN model** with multiple Conv2D, MaxPooling2D, and Dense layers.  
5. **Train the model** for 20 epochs while tracking `accuracy` and `loss`.  
6. **Visualize results** with plots for training and validation metrics.  
7. **Save the trained model** as `.h5` and convert it to `.tflite`.  
8. **Test the model on a new image** using TFLite Interpreter and display the prediction.  

##  Results
- Best Training Accuracy: 🔹 e.g., 0.98  
- Best Validation Accuracy: 🔹 e.g., 0.95  
- Lowest Training Loss: 🔸 e.g., 0.05  
- Lowest Validation Loss: 🔸 e.g., 0.12  

## Project Files
- `PCOS_Ultrasound_Images.ipynb` – Main notebook  
- `pcos_model.h5` – Trained model  
- `pcos_model.tflite` – Converted model for lightweight applications  
- `README.md` – This file  

##  How to Use
1. Open the notebook or run the `.py` script.  
2. Make sure all images and data are in the correct directories.  
3. Run the code sequentially to train the model or use the pre-trained model.  
4. Use the trained model to classify new images and visualize predictions.

##  Contributions
- Contributions are welcome for **model improvements or interface enhancements**.  
- Please open an Issue or Pull Request on GitHub to share your updates.
