# **IR-Search-Engine**  

## Project Overview  
This project implements a **Boolean & Proximity Search Engine** that retrieves documents based on:  
- **Boolean queries** (AND, OR, NOT)  
- **Proximity-based word searches** (e.g., `word1 word2 /k`)  

The system is built using **Python** and leverages an **inverted index** for Boolean retrieval and a **positional index** for proximity-based search.  

It includes a **Gradio-based GUI** for easy interaction, along with evaluation metrics using a **Gold Standard Query Set** to verify the system’s accuracy.  

---

## Features  
-  Supports **Boolean Queries** (AND, OR, NOT)  
-  Implements **Proximity Queries** (e.g., `neural network /2`)  
-  Uses **Inverted Index** for Boolean retrieval  
-  Uses **Positional Index** for Proximity search  
-  **Preprocessing steps:** Casefolding, Tokenization, Stopword Removal, Stemming  
-  Includes a **Gold Standard Query Set** for evaluation  
-  **Gradio GUI** for an interactive search experience  

---

##  Installation & Setup  

### **1️⃣ Install Required Libraries**  
Before running the project, install the necessary Python libraries:  

```bash
pip install -r requirements.txt
```

---

### **2️⃣ Ensure All Required Files Are Present**  
Some files are **not included** in this repository, so you **must manually add** them before running the project.  

#### **Required Files**  

| File Name                         | Description |
|-----------------------------------|-------------|
| `Boolean_Proximity_Search_Engine.ipynb` | Jupyter Notebook containing the implementation |
| `Stopwords.txt` | List of stopwords used for preprocessing |
| `Gold Standard Queries.txt` | Predefined queries for evaluation |
| `abstracts/` | Folder containing `.txt` files representing documents |
| `inverted_index.json` | *(Automatically generated upon execution)* |
| `positional_index.json` | *(Automatically generated upon execution)* |

---

#### **📂 File Format Requirements**  

📌 **Abstracts Dataset**  
- Must be stored in a folder named `abstracts/`  
- Each document should be a `.txt` file with a **unique name** (e.g., `001.txt`, `002.txt`, etc.)  

📌 **Stopword List (`Stopwords.txt`)**  
- Each line should contain **one stopword**, like this:  
  ```
  a  
  an  
  the  
  ```

📌 **Gold Standard Queries (`Gold Standard Queries.txt`)**  
- The format should be as follows:  
  ```
  Example Query: information AND retrieval  
  Result-Set: 124, 100  

  Example Query: neural network /2  
  Result-Set: 175, 273, 333
  ```

---

### **3️⃣ Update File Paths**  
Since file paths **vary across systems**, update the **file paths** in the code to match your local directory.  

---

### **4️⃣ Run the Jupyter Notebook**  
Open `Boolean_Proximity_Search_Engine.ipynb` and **run all cells sequentially**.  

---

### **5️⃣ Use the Gradio GUI**  
Once executed, the **Gradio-based GUI** will launch automatically, allowing you to enter search queries interactively.  

---

## Evaluation (Gold Standard Queries)  
To verify the accuracy of the system, run the **Gold Standard Queries**. The system will compare the retrieved results with the expected results and display:

-  **Precision**  
-  **Recall**  
-  **F1-Score**  
-  **Match Status** 

---

## Notes & Considerations  
The **stopword list, gold standard queries, and abstracts** are **not included** in this repository.  
You **must manually add** these files before running the project.  

---

## Acknowledgments  
This project was developed as part of a **semester assignment** under the guidance of **Dr. Rafi**.  

- The **stopword list**, **gold standard queries**, and **abstracts** were provided by **Dr. Rafi** and are **not included** in this repository.  

---

## License  
This project is intended **for academic purposes only**. If you wish to **use or modify** this work, please ensure proper attribution.  

---
