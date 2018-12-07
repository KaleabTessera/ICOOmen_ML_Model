# ICOOmen_ML_Model
![ICO - When Moon](https://dashnews.org/wp-content/uploads/2018/07/bitcoin-ico.jpg)

## Introduction
In this project, we propose IcoOmen, a machine learning model which will
predict the value of an ICO token after 6 months. This will use historic
data that has been aggregated from various public websites and APIs, as well as data that has been manually collected and calculated.

## Ways to Run:
### Google Colab
1. Click on the link on the top of ICOData.ipynb.

### Docker
1. Install Docker and Docker-Compose 
https://docs.docker.com/compose/install/#install-compose
 
2. Build and Run Docker-compose
```
docker-compose up
```
3. Head to url specified from terminal.

### Jupyter-Notebooks
1. Run locally via Jupyter Notebooks.

## Predict the Price of an ICO - NO TRAINING REQUIRED, USING PRE-TRAINED MODEL.
Run the following sections of Code: 
- Library Imports and creating useful functions.
- Create Folders if Necessary and download dateset.
- Loading ICO dataset into variables.
- Encoding and Splitting of Data.
- Linear Regression.
    - Load Saved Linear Regression Models and Print out performance.
    - Use Model to make prediction - Value of ICO after 6 months.
- Neural Network.
    - Load Saved Neural Network Models and Print out performance.
    - Use Model to make prediction - Value of ICO after 6 months.
