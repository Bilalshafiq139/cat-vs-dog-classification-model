Cat vs Dog Classifier Web App**

---

**Overview:**

This project is a Deep Learning-based **Cat vs Dog Classifier**, designed to run as a web application using **Streamlit** and a pre-trained **TensorFlow (.h5)** model. It allows users to upload multiple batches of images, manually assign the correct label to each batch (either cat or dog), and then evaluate the model’s predictions against those true labels.

The application generates a professional **accuracy report** and a clean, easy-to-read **dual pie chart** that compares predicted vs actual labels.

---

**Key Features:**

- Upload multiple sets of cat and dog images.
- Manually assign actual labels to each batch.
- Predict results using your own pre-trained model (`cat_dog_model.h5`).
- Get a visual and statistical breakdown of:
  - Accuracy (70% to 80% correct predictions)
  - Predicted and actual label distribution
  - Dual-layer pie chart for clean comparison.
- Clean, responsive web interface — no programming required to use!

---

**Technologies Used:**

- **Python 3.8+**
- **TensorFlow / Keras** – for model loading and prediction
- **Streamlit** – for web interface
- **Matplotlib** – for chart visualization
- **Pillow (PIL)** – for image loading and conversion
- **NumPy** – for numerical processing

---

**How to Use This App:**

**Step 1: Clone or Download the Repository**

Make sure you have Python installed on your computer.

**Step 2: Set Up Virtual Environment (Optional but Recommended)**  
- Open a terminal and run:

```bash
python -m venv venv
venv\Scripts\activate  (for Windows)
```

**Step 3: Install Required Packages**

```bash
pip install -r requirements.txt
```

**Step 4: Run the Streamlit Web App**

```bash
streamlit run app.py
```

---

**Using the App:**

1. You will be asked to upload a batch of images (e.g., only cats or only dogs).
2. Select the correct label (cat or dog) for that batch.
3. Optionally upload a second batch and label it too.
4. Click the **"Predict Now"** button to evaluate.
5. You will receive:
   - Total image count
   - Correct vs incorrect predictions
   - Accuracy percentage
   - A clean pie chart comparing predicted vs actual values.

---

**Folder Structure:**

```
cat-dog-classifier/
│
├── app.py                  ← Streamlit App File
├── cat_dog_model.h5        ← Your pre-trained model
├── requirements.txt        ← Dependencies
├── README.docx or README.md
└── sample_images/          ← (Optional) Example test images
```

---

**How to Reuse the Code with Your Own Model:**

- Replace the file `cat_dog_model.h5` with your own trained Keras model.
- Make sure your model accepts input images of size `(150, 150, 3)` or update `IMG_SIZE` in the code accordingly.
- Run `streamlit run app.py` and test with your own dataset.

---

**Best Practices:**

- Upload images in separate, clean batches.
- Use clear, real image data for best results.
- Adjust model thresholds or classes if you are working on a multi-class project.

---

**Author:**
Bilal Shafique  
GitHub: https://github.com/Bilalshafiq139  
Email: Bilalshafiq139@gmail.com

