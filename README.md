# English-to-Swahili-translation-Using-multi-head-attention-Transformer

This repository contains notebooks and datasets for building an English-Swahili machine translation model. It includes steps for data collection, cleaning, and model training.

## Repository Contents

### Data Collection
- `data_collection.ipynb`: Notebook for collecting raw data.
- `english_swahili_sentence_pairs.csv`: Raw dataset containing English-Swahili sentence pairs.
- `english_swahili_sentence_pairs_cleaned.csv`: Cleaned version of the sentence pairs.

### Data Cleaning
- `data_cleaning.ipynb`: Notebook for cleaning and preprocessing the raw dataset.
- Additional test files: These include test CSV files for both the original and cleaned English-Swahili sentence pairs.

### Model Training
- `eng_swahili_mt_5.9.ipynb`: Notebook that contains the code for training the translation model.
  - This notebook imports the cleaned dataset as a DataFrame:
    ```python
    import pandas as pd
    df = pd.read_csv("english_swahili_sentence_pairs_cleaned.csv")
    ```
    
## How to Run the Model

### 1. Environment Setup
- Ensure you have Python 3.x and Jupyter Notebook installed.
- Install the necessary Python libraries:
  ```bash
  pip install pandas numpy tensorflow torch
  ```

### 2. Data Cleaning
- Open `data_cleaning.ipynb` in Jupyter Notebook.
- Run the cells sequentially to preprocess and clean the raw dataset.
- Once the cleaning process is complete, ensure that the `english_swahili_sentence_pairs_cleaned.csv` file is available in your working directory.

### 3. Model Training
- Open `eng_swahili_mt_5.9.ipynb` in Jupyter Notebook.
- The notebook is pre-configured to import and use the cleaned dataset:
  ```python
  import pandas as pd
  df = pd.read_csv("english_swahili_sentence_pairs_cleaned.csv")
  ```
- Execute the notebook cells to train and evaluate the machine translation model.
- For model training, the process was run using Kaggle’s GPU (P100). It is recommended to use a similar GPU environment for optimal performance.

## Dependencies

Make sure your environment includes:
- Python 3.x
- Pandas
- NumPy
- TensorFlow
- PyTorch
- NLTK


## Additional Notes

- The notebooks are designed to work directly with the cleaned dataset, so no further data manipulation is needed after running the cleaning notebook.
- If you encounter any issues, please check that all dependencies are installed and that the cleaned dataset file is in the correct directory.

