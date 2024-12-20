# 🚴‍♂️ London Bike Rental Predictor 📊

Hi there! 👋 I'm excited to share my project, **London Bike Rental Predictor**, with you. This repository combines Python, data science, and machine learning to analyze and predict bike rental patterns in London.

For this project, I made use of the **London Bike Data dataset** from the **Transport for London (TfL)** and **freemeteo.co.uk** collaboration to create prediction models for **Santander Cycles** (formerly Barclays Cycle Hires). 🏙️

---

## 📂 Repository Structure

- **`Cycles_ML.ipynb`**: The Jupyter Notebook file containing all the Python code for data analysis, visualization, and model training.
- **`London_bike_data.csv`**: The dataset used for training and testing the machine learning models. It includes features like temperature, humidity, weather, and more.

---

## 📜 Project Objective

The goal of this project is to predict the number of bike rentals for various time periods based on environmental and temporal features. By doing this, we can assist decision-makers in better managing bike availability across different stations in London.

---

## 🛠️ Key Features and Workflow

### 1. **Dataset Overview**
   - The dataset includes details like:
     - Hour of the day 🕒
     - Temperature 🌡️
     - Humidity 💧
     - Weather conditions 🌤️
     


---

### 2. **Data Preprocessing**
   - The `bike_rented` column is transformed into numeric categories (`0` for "very low", `1` for "low", etc.).
   - Checked for missing values and overall data structure.
  ![image](https://github.com/user-attachments/assets/19e2088b-045d-442b-9cfc-46f342573c94)
     


---

### 3. **Model Building**
   - **Logistic Regression**:
     - Trained to predict rental categories but achieved limited accuracy (~42%).
    ![image](https://github.com/user-attachments/assets/d61a7b71-6961-41b3-9d05-4223a53b7548)

   - **Decision Trees**:
     - Performed significantly better, achieving an average R² score of **~97.7%**.
    ![image](https://github.com/user-attachments/assets/fab34578-a1ee-4f05-8f4e-cbd9d2cd61a9)

  ![image](https://github.com/user-attachments/assets/5953f627-a0fd-4301-8c02-a6ea0ddd721a)


---

### 4. **Evaluation**
   - Used metrics like accuracy, precision, recall, and F1-score to evaluate the models.
   - Implemented **K-Fold Cross-Validation** to ensure model robustness.
   

---

## 📈 Results

- Logistic Regression struggled with an overall accuracy of **~42%**, showcasing its limitations for this task.
- Decision Trees emerged as the clear winner with an accuracy of **~76%** and an average R² score of **~97.7%** during cross-validation.

---

## 🚀 How to Run the Code

1. Clone the repository:
   ```bash
   git clone https://github.com/Amay-W/London-Bike-Rental-Predictor-ML.git
   cd London-Bike-Rental-Predictor-ML
2. Install the necessary Python libraries:
   ```bash
   pip install pandas numpy sklearn matplotlib seaborn
3. Open the Jupyter Notebook:
   ```bash
   python -m notebook Cycles_ML.ipynb
4. Run the notebook cells step by step to view data preprocessing, analysis, and model performance.

---

## 🤔 What I Learned

- The importance of data preprocessing in achieving high model accuracy.
- Decision Trees are highly effective for classification tasks with clear decision boundaries and performed exceptionally well in this project.
- Logistic Regression, while simpler and computationally efficient, may not always be suitable for datasets with complex patterns or non-linear relationships.

---

## 🖼️ Future Scope

- **Exploring Advanced Models**: Experimenting with ensemble methods like Random Forests and Gradient Boosting to further improve prediction accuracy.
- **Hyperparameter Tuning**: Adding feature scaling and tuning parameters to optimize model performance, especially for Logistic Regression.
- **Visualization**: Creating visual representations of the Decision Tree structure to improve interpretability.
- **Real-World Applications**: Expanding the project to predict bike demand at specific stations or during peak hours to provide actionable insights.

---

Feel free to explore the project, and if you have any suggestions or feedback, let me know! 😊







