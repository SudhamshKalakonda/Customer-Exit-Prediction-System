Business Impact:
Predicting customer churn is critical for financial institutions to maintain a competitive edge. This project provides an end-to-end Deep Learning solution that identifies at-risk customers with high precision, allowing for proactive retention strategies.

Technical Stack:
Language: Python 3.x 

Deep Learning: TensorFlow 2.15, Keras 

Data Science: Scikit-Learn, Pandas, NumPy 

Frontend/Deployment: Streamlit 

Model Optimization: SciKeras (for Hyperparameter Tuning)

Model Architecture & Methodology:
The core of this system is an Artificial Neural Network (ANN) designed to capture non-linear relationships in customer data.

1. Exploratory Data Analysis (EDA): Performed in experiments.ipynb to identify key churn drivers such as Age, Balance, and Geography.
2. Data Preprocessing: * Categorical variables encoded using LabelEncoder (Gender) and OneHotEncoder (Geography).
3. Feature scaling applied via StandardScaler to ensure stable gradient descent during training.
4. Optimization: Utilized GridSearchCV in the hyperparametertuningann.ipynb notebook to find the optimal combination of neurons, layers, and activation functions.
5. Deployment: A live web application built in app.py that loads the pre-trained .h5 model and .pkl encoders to provide real-time probability scores.

How to Run Locally:

Clone the Repository: 
git clone https://github.com/SudhamshKalakonda/Customer-Exit-Prediction-System.git
cd Customer-Exit-Prediction-System

Install Dependencies:
pip install -r requirements.txt

Launch the Dashboard:
streamlit run app.py

Key Features:
Real-Time Inference: Users can input customer details (Credit Score, Tenure, Balance, etc.) and receive an immediate churn probability.
Serialized Pipelines: The use of pickle files for encoders ensures that the data preprocessing during inference perfectly matches the training environment.
User-Centric UI: Built with Streamlit for a clean, intuitive experience.
