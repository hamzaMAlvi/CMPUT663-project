# CMPUT663-project

## Data
The datasets used in this project can be found in the Data folder. Raw data is also present along with processed data. To process data yourself, you can use processdata notebook present in the repository. The processed data is also present in the folder.

## How to RUN
I used the TPU's provided by kaggle to train the models. For using kaggle, follow these steps:
- Create a dataset using the files provided in the Data folder.
- Upload notebooks in this repo on kaggle.
- Add the dataset created in the first step in these notebooks using the data tab on right side of notebook.
- Change the accelator to TPU in the settings tab on right side of the notebook.
- Run all cells of the notebook. The required output/results will be present in the output of last cell.

To run on your local machine. Follow these steps:
- Download and install anaconda from this website: https://www.anaconda.com/products/individual.
- After installation, you will need to install dependencies. For this run following commands:
  - conda install -c anaconda jupyter 
  - conda install -c anaconda tensorflow-gpu
  - conda install -c conda-forge tqdm
  - conda install -c conda-forge numpy
  - conda install -c conda-forge pandas
  - conda install -c jmcmurray json
  - conda install -c anaconda scikit-learn 
  - conda install -c conda-forge transformers 
 - Now open notebook by running following command in the repository where this repo is cloned: jupyter notebook
 - You can train models on CPU or GPU but it will take hours, and you need to adjust the batch size of model.fit call w.r.t. to the RAM of your system and/or memory of GPU.
