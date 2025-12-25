# Data Mining Final Project  
## Inventory Receipt Price Variance Analysis for an EPC Company

### Project Overview
This project analyzes procurement transactions of an EPC company using *Inventory Receipt* data to identify price inconsistencies, abnormal procurement behavior, and potential overpayment.  
The main goal is to support data-driven procurement monitoring and cost optimization.

---

### Business Problem
In EPC companies, identical materials are often purchased at different prices by different managers or project teams.  
This leads to:
- overpayments,
- increased project costs,
- unreliable budgeting,
- gaps between planned and actual expenses.

The project aims to detect such inconsistencies and quantify their financial impact.

---

### Dataset Description
The dataset is based on *Inventory Receipt* documents and includes:
- receipt date,
- item (material),
- unit price,
- quantity,
- total amount,
- supplier,
- project,
- warehouse,
- currency,
- VAT indicator,
- responsible person and author.

---

### Methodology
The analysis follows a structured data mining approach:

1. Data cleaning and preprocessing (duplicates removal, quantity validation).
2. Feature engineering:
   - calculation of Net Unit Price with VAT and currency logic.
3. Exploratory data analysis (EDA) and visualization.
4. Missing value imputation using KNN.
5. Feature encoding and scaling for machine learning.
6. Clustering (KMeans, Agglomerative) to identify procurement behavior patterns.
7. Anomaly detection using Isolation Forest.
8. Expected price estimation using Random Forest regression.
9. Feature importance analysis to explain price drivers.
10. Financial impact assessment through potential overpayment calculation.
11. Development of procurement monitoring rules and alerts.

---

### Key Results
- Price variance is systematic and driven by procurement conditions rather than random noise.
- Overpayment is concentrated in specific projects and responsible persons.
- Supplier, project, warehouse, and currency are key drivers of procurement price differences.
- A baseline scenario shows that significant cost savings are possible through price standardization.

---

### Monitoring Logic
The project proposes a practical monitoring framework:
- price alerts based on IQR thresholds,
- anomaly flags for suspicious transactions,
- overpayment aggregation by project and responsible person.

---

### Technologies Used
- Python  
- pandas, numpy  
- matplotlib, seaborn  
- scikit-learn  

---

### Limitations
- The analysis is limited to available receipt-level data.
- Contract-level pricing and supplier quality indicators are not available.
- Results should be interpreted as decision-support insights rather than absolute benchmarks.

---

### Repository Structure
- `Data_mining_final.ipynb` — main analysis notebook  
- `README.md` — project description

---

### Author
Orazbai Dariga 22B030617
Kemelbay Merey 22B030375
Data Mining Final Project  
Kazakh-British Technical University
