# IR-Search-Engine  

## Project Overview  
This repository contains two distinct search engines, each designed for different Information Retrieval (IR) methodologies:  
1. **Boolean & Proximity Search Engine**  
2. **Vector Space Model (VSM) Based Retrieval System**  

Both systems are implemented in **Python**, share a common preprocessing pipeline, and are evaluated using a **Gold Standard Query Set**. Each engine demonstrates a different retrieval strategy, showcasing core IR concepts with performance metrics.

---

## Search Engine 1: Boolean & Proximity Retrieval  
This system retrieves documents using:

- **Boolean Logic**: Supports `AND`, `OR`, `NOT` operators  
- **Proximity Search**: Retrieves documents where terms co-occur within a specific word window (e.g., `neural network /2`)  

#### Components
- Inverted Index for Boolean search  
- Positional Index for proximity queries  
- **Preprocessing**:  
  - Casefolding  
  - Tokenization  
  - Stopword Removal  
  - Stemming

#### Evaluation Metrics
- Precision  
- Recall  
- F1-Score  

---

## Search Engine 2: Vector Space Retrieval (VSM)  
This system ranks documents using the **Vector Space Model**:

- TF-IDF weighting  
- Cosine Similarity for ranking  
- Applies a similarity threshold (α = 0.05) to filter results  

#### Components
- Reuses inverted index and preprocessing steps from Boolean engine  
- The only change: uses **lemmatization** instead of stemming  

#### Evaluation Metrics
- Precision  
- Recall  
- F1-Score  
- Mean Average Precision (MAP) 
- Mean Average Recall (MAR)
---

## Notes & Considerations  
The **stopword list, gold standard queries, and abstracts** are **not included** in this repository.  
You **must manually add** these files before running the project.  

---

## Acknowledgments  
This project was developed as part of a **semester assignment** under the guidance of **Dr. Rafi**.  

---

## License  
This project is intended **for academic purposes only**. If you wish to **use or modify** this work, please ensure proper attribution.  

---
