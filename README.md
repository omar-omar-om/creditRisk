<h1>🛡️ Credit Risk Prediction with Machine Learning</h1>

<p>This project explores a robust and comparative machine learning approach to predict <strong>credit risk</strong>—whether a customer is likely to <strong>repay or default</strong> on a loan. Using tree-based algorithms, neural networks, and KNN, the project emphasises performance, interpretability, and data preprocessing strategies.</p>

<p>
  📍 <strong>Supervised by:</strong> Dr. Batoul<br>
  👨‍💻 <strong>Author:</strong> Omar I Elsayed<br>
  🏛️ <strong>Institution:</strong> Coventry University | KH6006CEM
</p>

<hr>

<h2>📂 Table of Contents</h2>
<ul>
  <li><a href="#problem-statement">Problem Statement</a></li>
  <li><a href="#dataset">Dataset</a></li>
  <li><a href="#preprocessing">Preprocessing & Feature Engineering</a></li>
  <li><a href="#models">Models Used</a></li>
  <li><a href="#results">Results & Evaluation</a></li>
  <li><a href="#tuning">Model Tuning</a></li>
  <li><a href="#challenges">Challenges</a></li>
</ul>

<h2 id="problem-statement">💡 Problem Statement</h2>
<p>In the evolving world of financial technology, assessing credit risk through automated machine learning systems provides faster and more accurate loan approval decisions. This project investigates methods to classify loan applicants based on whether they are likely to default or not.</p>

<h2 id="dataset">📊 Dataset</h2>
<p>The dataset is sourced from a <a href="https://www.kaggle.com/datasets/laotse/credit-risk-dataset">Kaggle Credit Risk Dataset</a>, consisting of 30,000 records with features such as income, loan amount, employment length, and credit history. The target variable is <code>loan_status</code>, where 1 indicates default.</p>

<h2 id="preprocessing">🛠️ Preprocessing & Feature Engineering</h2>
<ul>
  <li>Handled missing values via two methods: <strong>row removal</strong> and <strong>median imputation</strong>.</li>
  <li>Removed outliers, particularly in age and employment length.</li>
  <li>Engineered new features: <code>income_category</code> and <code>loan_percentage_of_income</code>.</li>
  <li>Applied both Label Encoding and One-Hot Encoding.</li>
</ul>

<h2 id="models">📈 Models Used</h2>
<ul>
  <li><strong>Tree-based:</strong> CatBoost, LightGBM, XGBoost, Random Forest, Decision Tree</li>
  <li><strong>Others:</strong> K-Nearest Neighbors (KNN), Neural Network</li>
</ul>

<h2 id="results">📊 Results & Evaluation</h2>
<p>Models were evaluated using metrics such as Accuracy, Precision, Recall, F1 Score, ROC AUC, Specificity, and Sensitivity.</p>
<ul>
  <li><strong>Best Performer:</strong> CatBoost (accuracy ~94.4%)</li>
  <li>Decision Trees showed high recall but lower precision.</li>
  <li>KNN performed worst; Neural Networks performed better but were slower than boosting models.</li>
</ul>

<h2 id="tuning">⚙️ Champion Model Tuning</h2>
<p>Manual tuning was applied to CatBoost due to limited computing resources. Key improvements included early stopping and learning rate adjustments. Post-tuning, the model showed stronger generalization and reduced test error.</p>

<h2 id="challenges">🚧 Challenges</h2>
<ul>
  <li>Training SVC took several days on Google Colab and eventually failed due to session limits.</li>
  <li>SMOTE-based balancing didn't significantly improve results, suggesting class imbalance wasn’t a major issue.</li>
</ul>


<h3>🔗 Project Links</h3>
<ul>
  <li><a href="https://github.com/omar-omar-om/creditRisk/blob/main/CreditRisk.ipynb">📄 GitHub Notebook</a></li>
  <li><a href="https://colab.research.google.com/drive/1RI0x9W9ENRiHLUHXAsgQD2WkZfSD_R85?usp=sharing">🔗 Google Colab Version</a></li>
</ul>

