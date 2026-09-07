# drug_release_data_analysis

This is a series of Jupyter notebooks (Python) for analyzing real-time drug release data measured via fluorescence. Built to work with the data format exported by PTI FelixGX software (Version 4.2.0, Photon Technology International, Edison, NJ, USA).

This README is currently a work-in-progress, and will be updated as I keep adding the notebooks.

## Function of each notebook — Summary

| Notebook | Function |
| :--- | :--- |
| Step 1 | - Processes raw fluorescence readings <br> - Normalizes into cumulative fractional release (CFR) <br> - Exports summary of release data (time, CFR, raw fluorescence readings) into an Excel file |

## Function of each notebook — Detailed

| Notebook | Function |
| :--- | :--- |
| Step 1 | This notebook loads the raw txt files containing the fluorescence readings, normalizes the data to get the cumulative fractional release (CFR) at each datapoint, and exports the summary of the release data into an Excel file. The file is exported into the same directory as the notebook. <br><br> The notebook is structured to process all the `.txt` files of a given directory, which corresponds to a given batch of liposomes, for example. Each `.txt` file, on the other hand, corresponds to a given sample prepared from this batch. So the Excel file published at the end contains the time, CFR, and raw intensity of each sample, with each sample in its own worksheet. <br><br> This makes it easy for one to proceed with the data analysis in Excel if they so wish, after having offloaded the burden of processing each .txt file individually. |
