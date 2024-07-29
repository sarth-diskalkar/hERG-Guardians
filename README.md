# hERG_Guardians

**Unveiling the HERG Guardians: Ligand Discovery and Molecular Insights for Cardio-Safe Drug Design**

This repository contains Jupyter notebooks showcasing models for predicting ligands that protect the HERG channel from potential blockers. The models were developed using XGBoost and deep learning approaches.

## Dataset and Preprocessing

The dataset used for model training was obtained from the research paper titled "Primary cell-based high-throughput screening assay for identification of compounds that protect hERG from block by proarrhythmic agents."

**Source**:
- National Center for Biotechnology Information (2024). PubChem Bioassay Record for AID 1511, Source: Johns Hopkins Ion Channel Center. Retrieved April 29, 2024, from [PubChem Bioassay](https://pubchem.ncbi.nlm.nih.gov/bioassay/1511).

The molecular structures (SMILES) from this dataset were processed using Mordred:
- Moriwaki, H., Tian, YS., Kawashita, N. et al. Mordred: a molecular descriptor calculator. J Cheminform 10, 4 (2018). [Mordred DOI](https://doi.org/10.1186/s13321-018-0258-y).

Preprocessing steps included data cleaning and scaling of biologically relevant descriptors generated from the data.

All the notebooks were run on Google Colab:
- Bisong, E. (2019). Google Colaboratory. In: Building Machine Learning and Deep Learning Models on Google Cloud Platform. Apress, Berkeley, CA. [Google Colab DOI](https://doi.org/10.1007/978-1-4842-4470-8_7).

## Models

The models were implemented using Python, with the deep learning model built using TensorFlow/Keras. 

**Deep Learning Model Architecture**:
- Dense layers with ReLU activation.
- Dropout layers to prevent overfitting.
- Model training involved splitting the dataset into train-validation and test sets.
- Best model weights saved using early stopping and model checkpoint callbacks.

**Evaluation Metrics**:
- Accuracy
- Precision
- Recall
- F1-score
- ROC AUC

## Code

The code for both models (XGBoost and deep learning) is provided in the notebooks. Libraries such as NumPy, Pandas, scikit-learn, SMOTE, and TensorFlow were utilized for data manipulation, model development, and evaluation.

## Files

- **Notebooks**: Containing the code for model development and evaluation.
- **Models**: Trained models saved in the `models` folder.
- **Data**: Cleaned and scaled data for active and inactive molecules.
  - **Active molecules**: Protect the HERG channel.
  - **Inactive molecules**: Do not protect the HERG channel.

## Next Steps

- Further optimize or fine-tune the trained models for better performance.
- Explore additional features or descriptors to enhance model predictive power.
- Apply the models to predict HERG channel blocker activity for new compounds, aiding in drug discovery and safety assessment.

## Contributing

Feel free to explore the provided code and models to understand the process and results in detail. If you have any questions or suggestions, please don't hesitate to reach out.


## Contributing

Feel free to explore the provided code and models to understand the process and results in detail. If you have any questions or suggestions, please don't hesitate to reach out.

