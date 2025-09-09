# 🌳Random-Forest-Model-for-Breast-Cancer-Detection (Using-Text-Data)

## *📌 Project Overview*

This project implements a Random Forest Classifier to detect breast cancer (benign or malignant) using text-based CSV data.
It covers:

✨ Data Preprocessing → 🔎 Model Training → 📊 Evaluation → 🧾 Predictions (Single & Multiple Patients).

## *🛠 Technologies Used*

✅ Python

✅ NumPy

✅ Pandas

✅ Scikit-learn

✅ Google Colab / Jupyter Notebook


## *🔄 Workflow (Step-by-Step)*

🔹 Step 1: Load & Explore Dataset

    📂 Upload CSV file
    👀 Display first rows, check column types, handle missing values


🔹 Step 2: Data Preprocessing

    🧹 Fill missing values (mean imputation)
    🔖 Encode diagnosis → (Benign = 0, Malignant = 1)
    📏 Normalize features using StandardScaler

🔹 Step 3: Train-Test Split

    ✂️ Split into 80% Training and 20% Testing

🔹 Step 4: Train Model

    🌳 Train a Random Forest Classifier (100 trees)

🔹 Step 5: Model Evaluation

    📊 Compute accuracy on train & test sets
    📑 Generate classification report (Precision, Recall, F1-score)


🔹 Step 6: Predictions

    👤 Single Input Prediction → Upload .txt file with one patient’s features
    👥 Batch Prediction → Upload .txt file with multiple patients’ data
    📌 Save results into an output .txt file with probability of cancer

## *🚀 How to Run in Google Colab*

  1️⃣ Open notebook in Google Colab
  
  2️⃣ Upload the CSV dataset
  
  3️⃣ Run all cells to train the model
  
  4️⃣ Upload .txt file (single or multiple patients)
  
  5️⃣ 📥 Download the results file

## *📂 Example Input & Output*

🔹 Example1 : Single Patient Input (input_single.txt)

    13.54,14.36,87.46,566.3,0.09779,0.08129,0.06664,0.04781,0.1885,0.05766,
    0.2699,0.7886,2.058,23.56,0.008462,0.0146,0.02387,0.01315,0.0198,0.0023,
    15.11,19.26,99.7,711.2,0.144,0.1773,0.239,0.1288,0.2977,0.07259

  Output File (prediction_output.txt):
    
   🔍 Breast Cancer Prediction Result
  ========================================
  
    mean radius:              13.54
    mean texture:             14.36
    mean perimeter:           87.46
    mean area:                566.3
    mean smoothness:          0.09779
    mean compactness:         0.08129
    mean concavity:           0.06664
    mean concave points:      0.04781
    mean symmetry:            0.1885
    mean fractal dimension:   0.05766
    radius error:             0.4564
    texture error:            1.242
    perimeter error:          3.357
    area error:               45.5
    smoothness error:         0.0072
    compactness error:        0.0139
    concavity error:          0.0155
    concave points error:     0.006
    symmetry error:           0.0203
    fractal dimension error:  0.0028
    worst radius:             15.34
    worst texture:            18.25
    worst perimeter:          104.5
    worst area:               755.6
    worst smoothness:         0.134
    worst compactness:        0.175
    worst concavity:          0.198
    worst concave points:     0.089
    worst symmetry:           0.282
    worst fractal dimension:  0.07259



## *🔍 Prediction Result & Accuracy*

    Diagnosis: Malignant (Cancer Detected)
    
    🩸 Probability of Cancer: 82.45%


## *🔹 Example 2: Multiple Patients Input (input_multi.txt)*

    ✅ Input File Content (2 patients, 30 features each):
        
    13.54,14.36,87.46,566.3,0.09779,0.08129,0.06664,0.04781,0.1885,0.05766,
    0.2699,0.7886,2.058,23.56,0.008462,0.0146,0.02387,0.01315,0.0198,0.0023,
    15.11,19.26,99.7,711.2,0.144,0.1773,0.239,0.1288,0.2977,0.07259
    
    12.45,16.78,82.34,490.1,0.08912,0.07543,0.05423,0.04567,0.1821,0.05678,
    0.2456,0.6891,1.876,20.34,0.007891,0.01234,0.02012,0.01156,0.01876,0.0021,
    14.22,18.55,95.2,680.4,0.132,0.1554,0.2101,0.1123,0.2876,0.06954

    
## *Output File (prediction_output.txt):*

    🔍 Breast Cancer Prediction Results
    ==================================================
    Patient 1: Malignant (Cancer Detected)
    🩸 Probability of Cancer: 87.45%
    --------------------------------------------------
    Patient 2: Benign (No Cancer)
    🩸 Probability of Cancer: 23.15%
    --------------------------------------------------

## *📊 Results*

| Metric            | Value                          |
| ----------------- | ------------------------------ |
| Training Accuracy | \~98.6%                        |
| Testing Accuracy  | \~97.2%                        |
| Model Used        | Random Forest (100 Estimators) |


## *🚀 Future Enhancements*

✅Integrate Deep Learning (ANN/CNN) for higher accuracy.

✅Deploy the model as a Web App / API using Flask or FastAPI.

✅Add Explainable AI (XAI) techniques to understand predictions.

✅Extend support for image-based diagnosis (Mammograms, Ultrasound).










