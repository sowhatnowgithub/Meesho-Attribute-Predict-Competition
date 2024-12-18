# Accessing the Dataset

The dataset used in this project is from the Kaggle competition [Visual Taxonomy](https://www.kaggle.com/competitions/visual-taxonomy/data). You can access the data using either of the following methods:

## Method 1: Kaggle Website
1. Visit the [Visual Taxonomy Competition Data Page](https://www.kaggle.com/competitions/visual-taxonomy/data).
2. Log in to your Kaggle account.
3. Click on the **Download All** button to download the dataset.

## Method 2: Kaggle API
1. Ensure you have the [Kaggle API](https://github.com/Kaggle/kaggle-api) installed and set up on your system.
2. Run the following command in your terminal to download the dataset:
   ```bash
   kaggle competitions download -c visual-taxonomy
3. Use zipfile to extract files to access:
   ```bash
   import zipfile
   zip_ref = zipfile.ZipFile('/content/visual-taxonomy.zip', 'r')
   zip_ref.extractall('/content')
   zip_ref.close()
