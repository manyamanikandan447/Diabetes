#  Diabetes Progression Modeling (ANN)
##  Objective
Build an Artificial Neural Network (ANN) to model diabetes progression using the **sklearn Diabetes dataset**.  
The project explores how patient features influence progression and evaluates model performance.

---

##  Workflow

1. **Data Loading & Preprocessing**
   - Loaded dataset from `sklearn.datasets`.
   - Checked for missing values (none found).
   - Normalized features using `StandardScaler`.

2. **Exploratory Data Analysis (EDA)**
   - Visualized target distribution.
   - Correlation heatmap of features.
   - Scatterplots of features vs target.

3. **ANN Model**
   - Baseline model: 1 hidden layer, ReLU activation.
   - Output layer: Linear activation for regression.

4. **Training**
   - Train/test split (80/20).
   - Optimizer: Adam, Loss: MSE.
   - Trained for 100 epochs.

5. **Evaluation**
   - Metrics: Mean Squared Error (MSE), R² Score.
   - Plotted training vs validation loss.

6. **Improvements**
   - Added more layers/neurons.
   - Tried `tanh` + `relu` activations.
   - Used Dropout + L2 regularization.
   - Adjusted learning rate, applied EarlyStopping.
   

---

## 📊 Results

| Model        | MSE   | R² Score |
|--------------|-------|----------|
| Baseline ANN | ~3037 | ~0.42   |
| Improved ANN | ~3830 | ~0.27   |


