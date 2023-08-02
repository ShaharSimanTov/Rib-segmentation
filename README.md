# Image segmentation project

## Data backround
The data set we worked on is based on data from patients with pulmonary embolism. It is taken from the KAGGLE website (https://www.kaggle.com/datasets/andrewmvd/pulmonary-embolism-in-ct-images) and contains CT scans in DICOM format which is a standard for saving medical images. The data set consists of angiography scans of 35 different patients, where each patient has ~200 scans.

## Method
The final goal of the project was to present a clean three-dimensional scan of the rib cage. We tried to work with several different methods to reach the desired result and among them: performing a simple segmentation and using the Canny algorithm. After realizing that segmentation on a single image is not the way to reach the desired result, we switched to working with a segmentation method on volume scans. We chose the Connected Components algorithm that divides the largest areas that are connected to each other into separate components. After reaching a better result, we also made corrections to the scans using morphology.

### links
Before segmentation: https://youtu.be/iw8pmTdwdjo
After segmentation: https://youtu.be/v9CzQdcz_TY

## Project conclusions
An experiment and questioning must be carried out separately for each patient in order to find the optimal number of Connected Components for him.
Our model will not work optimally on every patient and every scan due to the wide variety of scans.

*This project is my final project in the Biomedical Image Processing course as part of my Bachelor's degree in Digital Medical Technologies.
