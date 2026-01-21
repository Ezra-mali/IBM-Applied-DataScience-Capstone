#  Falcon 9 Landing Outcome Predictor

##  Project Summary

This capstone project focuses on **building a machine learning system to predict whether SpaceX’s Falcon 9 rocket first stage will land successfully**.  
SpaceX has disrupted the space industry by significantly lowering launch costs—charging **roughly $62 million per launch** compared to competitors’ **$165 million**—largely due to **first-stage reusability**.  
Accurately predicting landing success helps estimate launch costs more precisely, offering **strategic insights for aerospace companies competing with SpaceX**.

---

##  Project Phases

The project follows a **structured, end-to-end data science workflow**:

### **Phase 1: Data Acquisition and Preparation**
- **API Data Collection**: Retrieved historical Falcon 9 launch records via the **SpaceX REST API**.
- **Web Scraping**: Gathered additional launch details from **Wikipedia using BeautifulSoup**, then converted HTML tables into structured DataFrames.
- **Data Cleaning**: Processed and standardized raw data to ensure **quality and consistency** for analysis.

### **Phase 2: Exploratory Analysis and Database Setup**
- **Exploratory Data Analysis (EDA)**: Used **Matplotlib and Seaborn** to visualize trends, correlations, and distributions within the launch data.
- **Database Integration**: Loaded the curated dataset into a **Db2 database** and performed **SQL-based queries** to extract meaningful insights.

### **Phase 3: Feature Engineering and Geospatial Visualization**
- **Feature Engineering**: Developed **new predictive variables** from existing data to improve model performance.
- **Interactive Maps**: Created **Folium-based maps** to display launch sites and visualize success/failure patterns geographically.

### **Phase 4: Interactive Dashboard Development**
- **Plotly Dash App**: Built an **interactive web application** with dynamic controls (dropdowns, sliders) to explore launch data through **live-updating charts and maps**.

### **Phase 5: Predictive Modeling**
- **Model Training & Selection**: Trained and compared multiple classifiers, including **SVM, Logistic Regression, K-Neighbors, and Decision Trees**.
- **Hyperparameter Optimization**: Applied **GridSearchCV** to fine-tune model parameters.
- **Model Evaluation**: Tested each model on held-out data; the **Decision Tree classifier achieved the highest accuracy (94.44%)**.

---

##  Key Outcome

The **Decision Tree model** performed best with **94.44% test accuracy**, successfully predicting Falcon 9 first-stage landing outcomes.  
This **predictive capability** can inform **cost models and competitive strategy** in the commercial launch industry.

---

##  Repository Organization

- **`data/`** – Datasets and supporting scripts
- **`notebooks/`** – Step-by-step Jupyter notebooks for each phase
- **`scripts/`** – Reusable Python modules for data processing, visualization, and modeling
- **`dash_app/`** – Source code for the interactive Dash application
- **`README.md`** – Project documentation (this file)

---

##  Credits

- **IBM** – for the learning curriculum and guidance
- **Coursera** – for hosting the Applied Data Science Capstone course

---

