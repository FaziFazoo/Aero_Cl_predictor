
---

# Aero Cl Predictor

A machine learning project that employs a Multi-Layer Perceptron (MLP) to predict the lift coefficient (Cl) of airfoils based on their geometric coordinates, angle of attack, and Reynolds number.

## 📂 Dataset

The dataset used in this project is sourced from Kaggle and is named **DeepLearniWing**.

## 🧠 Model Overview

* **Input Features**:

  * Angle of attack
  * Reynolds number
  * X and Y coordinates of the airfoil shape (padded/truncated to 50 points each)

* **Target Variable**:

  * Lift coefficient (Cl)([Restack][1])

* **Model Architecture**:

  * Multi-Layer Perceptron Regressor with two hidden layers (128 and 64 neurons)
  * Trained using scikit-learn's `MLPRegressor`

* **Preprocessing**:

  * Standardization of input features and target variable using `StandardScaler`

## 📈 Results

The model demonstrates a reasonable ability to predict the lift coefficient, as evidenced by the Mean Squared Error (MSE) on the test set and the correlation between actual and predicted Cl values.

*Insert plot image here if available.*

## 🔧 Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/FaziFazoo/Aero_Cl_predictor.git
   ```



2. Navigate to the project directory:

   ```bash
   cd Aero_Cl_predictor
   ```



3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```



4. Run the Jupyter Notebook:

   ```bash
   jupyter notebook airfoil_cl_prediction.ipynb
   ```



## 📌 Notes

* The current model focuses solely on predicting the lift coefficient (Cl).
* Predictions for other aerodynamic coefficients like drag (Cd), moment (Cm), and lift-to-drag ratio (L/D) are not included and may require different modeling approaches.


## 🤝 Acknowledgments

Special thanks to the creators of the **DeepLearniWing** dataset on Kaggle for providing the data that made this project possible.

---

