
#  Customer Segmentation

## Problem Statement
Segment customers based on purchasing behavior to identify 
distinct customer groups for targeted marketing.

## Dataset
- Source: Online Retail UCI (Kaggle)
- Raw Rows: 541,909 | After Cleaning: 392,692

## Data Cleaning
- Removed 135,080 rows with missing CustomerID
- Removed 5,225 duplicate rows
- Removed 8,900 cancelled/returned orders
- Fixed DateTime and datatype conversions

## Feature Engineering (RFM)
| Feature | Description |
|---|---|
| Recency | Days since last purchase |
| Frequency | Number of transactions |
| Monetary | Total amount spent |

## Steps Performed
- RFM Feature Engineering from scratch
- StandardScaler
- PCA (2 components, 81% variance retained)
- Elbow Method to find optimal K
- KMeans Clustering (K=3)

## Results
| Cluster | Type | Avg Spend | Avg Frequency | Avg Recency |
|---|---|---|---|---|
| 0 | Regular Customers | £2,003 | 100 | 41 days |
| 1 | Churned Customers | £634 | 27 | 247 days |
| 2 | VIP Customers | £113,424 | 2485 | 5 days |

- Silhouette Score: 0.63

## Libraries Used
pandas, numpy, scikit-learn, matplotlib, seaborn, joblib
