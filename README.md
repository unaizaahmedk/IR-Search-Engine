# IR-Search-Engine

## Project Overview
This project implements a Boolean & Proximity Search Engine that retrieves documents based on Boolean queries (AND, OR, NOT) and proximity-based word searches (word1 word2 /k). The system is built using Python and supports query evaluation through an inverted index and a positional index for efficient document retrieval.

It includes a Gradio-based GUI for easy interaction, along with evaluation metrics using a Gold Standard Query Set to verify the system's accuracy.

## Features
- Supports Boolean Queries (AND, OR, NOT)
- Implements Proximity Queries (e.g., neural network /2)
- Uses Inverted Index for Boolean retrieval
- Uses Positional Index for Proximity search
- Preprocessing steps: Casefolding, Tokenization, Stopword Removal, Stemming
- Includes a Gold Standard Query Set for evaluation
- Gradio GUI for an interactive search experience

## Installation & Setup 
### 1. Install Required Libraries
Before running the project, install the necessary Python libraries using:

```bash
pip install -r requirements.txt
```

### 2. Ensure All Files Are in Place
Check that the following files and folders exist in your directory:

- `Boolean_Proximity_Search_Engine.ipynb` → Notebook containing the implementation
- `Stopword-List.txt` → List of stopwords used for preprocessing
- `Gold Query-Set Boolean Queries.txt` → Predefined queries for evaluation
- `abstracts/` → Folder containing text files for document retrieval
- `inverted_index.json` → *(Will be generated automatically)*
- `positional_index.json` → *(Will be generated automatically)*
  
### 3. Update File Paths
Since file paths differ across systems, update the paths in the code wherever necessary to match your local directory.

### 4. Run the Jupyter Notebook
Open `Boolean_Proximity_Search_Engine.ipynb` and run all cells sequentially.

### 5. Use the Gradio GUI
The Gradio GUI will launch automatically, allowing you to enter search queries interactively.


## Acknowledgments
This project was developed as part of a semester assignment under the guidance of Dr. Rafi.

