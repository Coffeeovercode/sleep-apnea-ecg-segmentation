# sleep-apnea-ecg-segmentation
ECG segmentation and labeling for sleep apnea classification — St. Vincent’s / UCD dataset.


This repository contains my code and workflow for **preprocessing and visualizing ECG data** from the **St. Vincent's University Hospital / University College Dublin Sleep Apnea Database**.  
I used Python, MNE, NumPy, Pandas, Matplotlib, and Seaborn to segment raw ECG recordings, label them into **six apnea classes** and **one non-apnea class**, and visualize the segments for further machine learning tasks.

---

## 📌 **What this project does**

- 📥 Loads raw ECG `.edf` files using **MNE-Python**
- ⏱️ Segments each ECG recording into **60-second windows**
- 🏷️ Labels each segment into multiple apnea and non-apnea classes
- 📊 Visualizes the ECG signals and class distribution using **Matplotlib** and **Seaborn**
- ⚙️ Prepares clean, labeled data ready for training deep learning models (in TensorFlow or any framework)

---

## 📂 **Project Structure**

📁 data/
├── raw/ # Place your raw .edf files here
└── processed/ # (Optional) Processed segments can be saved here

📄 Sleep_Apnea_Preprocessing_Visualization.ipynb # Main notebook: preprocessing + visualization
📄 requirements.txt # Python dependencies
📄 README.md # Project overview (this file)


---

## ⚙️ **Requirements**

Main Python libraries:
- Python 3.8+
- mne
- numpy
- pandas
- matplotlib
- seaborn
- tensorflow (optional, for later model training)

**To install all dependencies:**
```bash
pip install -r requirements.txt

🚀 How to run
1️⃣ Clone this repository:

bash
Copy
Edit
git clone https://github.com/Coffeeovercode/sleep-apnea-ecg-segmentation.git
cd sleep-apnea-ecg-segmentation
2️⃣ Put your .edf files in the data/raw/ folder.

3️⃣ Open the notebook:

bash
Copy
Edit
jupyter notebook Sleep_Apnea_Preprocessing_Visualization.ipynb
4️⃣ Run the cells step-by-step to:

Load ECG data

Segment and label it

Visualize the signals and classes

📈 Purpose
This preprocessing and visualization pipeline supports automated sleep apnea detection research by producing clean, labeled ECG segments that can be used to train and evaluate classification models.

⚠️ Data Licensing
Raw data is not included in this repository due to licensing.
Please download the St. Vincent's / UCD Sleep Apnea Database from PhysioNet and use it under the terms provided by the data owner.

🙌 Author
Supreet Sarita Das — https://github.com/Coffeeovercode
✅ Happy Coding!



git add README.md
git commit -m "Add project README"
git push

