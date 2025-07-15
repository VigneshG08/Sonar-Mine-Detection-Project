# Sonar-Mine-Detection-Project
# 🔍 Mine vs Rock Classification

This project aims to classify sonar signals as either **Mine** or **Rock** using various machine learning models. The dataset consists of sonar returns bounced off metal cylinders (mines) and rocks, each sample having 60 numeric features corresponding to frequency-based signal strengths.

---

## 📁 Project Structure

- **`Mine_or_Rock.ipynb`**: Jupyter notebook containing EDA, visualizations, model training, and evaluation.
- **`mine_or_rock.py`**: Standalone Python script version of the notebook for direct execution.
- **Dataset**: Loaded from Google Drive in the notebook (`mine_vs_rock.csv`).

---

## 🧠 Models Used

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree (Entropy criterion)
- Support Vector Machine (RBF kernel)

Each model's performance is evaluated using:
- Accuracy score
- Confusion matrix
- Classification report

---

## 📊 Visualizations

- Class distribution before and after resampling
- Feature histograms
- Signal pattern plots of Rock vs Mine
- Model-wise accuracy comparison (bar chart)

---

## 📈 Performance Snapshot

| Model             | Accuracy (Approx.) |
|------------------|--------------------|
| LogisticRegression | ~83%              |
| KNN                | ~96%              |
| Decision Tree      | ~91%              |
| SVM                | ~88%              |


---

## ✅ Requirements

You can install required packages using:

```bash
pip install numpy pandas scikit-learn matplotlib
```

Additional requirement (for notebook):
- Google Colab (or manual dataset download if running locally)

---

## 🚀 How to Run

**Notebook:**
1. Open `Mine_or_Rock.ipynb` in Google Colab.
2. Mount Google Drive and ensure dataset path is correct.
3. Run cells sequentially to train and evaluate models.

**Script:**
1. Make sure the dataset path in `mine_or_rock.py` is updated to your local file system.
2. Run with Python:

```bash
python mine_or_rock.py
```

---

## 🔮 Prediction Example

The script includes a sample input:

```python
input_data = (0.0201, 0.0376, ..., 0.0032)
```

It reshapes the data and uses KNN to predict:

```
The object is a Rock
```

---

## 📌 Notes

- Dataset is resampled to balance the class distribution.
- Final evaluation includes a side-by-side comparison of models.
- Code emphasizes clarity and interpretability over deep tuning.

---

## 📧 Author

**Vignesh**  
CSE Graduate | Passionate about ML, DSA, and cloud technologies
