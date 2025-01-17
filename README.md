# Master's Thesis: Definition Detection in Scientific Literature Using Large Language Models and Sentence Classification

There has been an increasing demand over the years for the advancement of information retrieval methods such as definition detection, given the excessive amount of data existing in our world today regardless of what field. In this thesis, we aim to explore the intricate process of definition detection through NLP tasks for scientific literature using both large language models (LLMs) and sentence classification. As there is a gap in research and experiment regarding the benefits of definition detection in such domains. This is done by taking advantage of models such as MPNet and MiniLM. Different approaches are used to test the selected model to determine which is the most effective and yields the best evaluation metrics. After analysis and considering the metrics, it is determined that MPNet is a better fit for this task as the F2-score (among other metrics) is the best performing when employing approach 2. The results indicate that ensuring the dataset is augmented and balanced is crucial to attaining useful results. The significance of the findings drawn from this thesis can contribute to fields like information retrieval and knowledge management systems. If models such as MPNet were to be trained further and perform even better, the real world applications of tasks such as definition detection could be groundbreaking in many fields.


### Explanation of the Structure:
 - **`.gitignore`**: Describes directories to be ignored by Git.
  - **`README.md`**: Provides an overview of the thesis, instructions, and guidelines.

- **Notebooks**:
  - **`data_preprocessing.ipynb`**: Data preprocessing and preparation for extraction of the data needed.
  - **`data_split_augment.ipynb`**: Dataset splitting and independent augmentation (for training, validation, and test data).
  - **`Baseline_Experiment.ipynb`**: Notebook for training the baseline experiment using the MPNet embedding model and display its results and visualizations.
  - **`MiniLM-Mpnet-aug.ipynb`**: Notebook for training and evaluating the results of the MiniLM Model and the MPNet Model and comparing their results.
  - **`Class_1_5_Ratio_Aug.ipynb`**: Notebook for training and evaluating the model using 1:5 ratio of definitional to non-definitional sentences using augmented data.
  - **`Controlled_Class_Ratio_75_Augmented.ipynb`**: Notebook for augmenting 75% of the definitional sentences, and training and evaluating the model using 1:5 ratio of definitions to non-definitions.

- **Data**:
  - **`Data/`**: Contains CSV files used in the notebooks:
    - **`extracted_definitions.csv`**: Extracted data used.
    - **`train_split_*`**: Training data (original, augmented, and 75% augmented).
    - **`test_split_*`**: Test data (original, augmented, and 75% augmented).
    - **`val_split_*`**: Validation data (original, augmented, and 75% augmented).

- **`requirements.txt`**: Specifies all the libraries and their versions needed.

## How to use:
1. Clone this repository:
   ```bash
   git clone https://github.com/saratamerrr/Masters_Thesis.git
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
   
