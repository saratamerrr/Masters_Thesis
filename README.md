# Master's Thesis: Definition Detection in Scientific Literature Using Large Language Models and Sentence Classification

---- abstract----


### Explanation of the Structure:
 - **`.gitignore`**: Describes directories to be ignored by Git.
  - **`README.md`**: Provides an overview of the project, instructions, and guidelines.

- **Notebooks**:
  - **`data_preprocessing.ipynb`**: Data preprocessing and preparation for extraction of the data needed.
  - **`data_split_augment.ipynb`**: Dataset splitting and independent augmentation (for training, validation, and test data).
  - **`Baseline_Experiment.ipynb`**: Notebook for training the baseline experiment using the MPNet embedding model and display its results and visualizations.
  - **`MiniLM-Mpnet-aug.ipynb`**: Notebook for training and evaluating the results of the MiniLM Model and the MPNet Model and comparing their results.
  - **`Class_1_5_Ratio_Aug.ipynb`**: Notebook for training and evaluating the model using 1:5 ratio of definitional to non-definitional sentences using augmented data.
  - **`Controlled_Class_Ratio_75_Augmented.ipynb`**: Notebook for augmenting 75% of the definitional sentences, and training and evaluating the model using 1:5 ratio of definitions to non-definitions.

- **Data**:
  - **`Data/`**: Contains CSV files used in the notebooks:
    - **`ArticlesContainingItems.csv`**: Article and item data used for data preparation and extraction.
    - **`ISItemsandVariables.csv`**: IS items and their variables used for data preparation and extraction.
    - **`extracted_definitions.csv`**: Extracted data.
    - **`train_split_*`**: Training data (original, fully augmented, and 75% augmented).
    - **`test_split_*`**: Test data (original, fully augmented, and 75% augmented).
    - **`val_split_*`**: Validation data (original, fully augmented, and 75% augmented).

- **`requirements.txt`**: Specifies all the libraries and their versions needed.

## How to use:
1. Clone this repository:
   ```bash
   git clone https://github.com/saratamerrr/Master_Thesis.git
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python3 -m venv myenv
   ```
3. Install the needed libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebooks:
   ```bash
   jupyter notebook
   ```
   
