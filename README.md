# Product Recommendation System - Lazada Vietnam

## Overview
Implicit Collaborative Filtering system (ALS) trained on 57,395 products 
from Lazada Vietnam, achieving Recall@10 = 0.61 — outperforming User-based 
CF by 33% and Content-based Filtering by 116%.

## Tech Stack
Python | Implicit | Scikit-learn | Pandas | NumPy | SciPy | Matplotlib | Seaborn

## Results
| Model          | Recall@10 | NDCG@10 | MAP@10 |
|----------------|-----------|---------|--------|
| ALS (ours)     | 0.61      | 0.31    | 0.22   |
| User-CF        | 0.46      | 0.28    | —      |
| Content-based  | 0.28      | 0.17    | —      |

## How to Run
pip install -r requirements.txt

jupyter notebook CrawlData.ipynb       # Step 1: Crawl data
jupyter notebook EDA_improved.ipynb    # Step 2: EDA + Feature Engineering  
jupyter notebook final_model.ipynb     # Step 3: Train + Evaluate
