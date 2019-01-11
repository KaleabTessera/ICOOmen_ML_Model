# ICOOmen_ML_Model
IcoOmen, a machine learning model which
predicts the value of an ICO token after 6 months. This uses historic
data that has been aggregated from various public websites and APIs, as well as data that has been manually collected and calculated.

Article can be found [here](https://towardsdatascience.com/icoomen-using-machine-learning-to-predict-ico-prices-29fa4cec6d86).

![](https://dashnews.org/wp-content/uploads/2018/07/bitcoin-ico.jpg)

## Getting Started: 
### Google Colab
1. Click on the link on the top of ICOData.ipynb or click [here](https://colab.research.google.com/github/KaleabTessera/ICOOmen_ML_Model/blob/master/ICOData.ipynb).

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

## Examples 
### Predict the Price of an ICO - NO TRAINING REQUIRED, USING PRE-TRAINED MODEL.
Run the following sections of Code: 
- Library Imports and creating useful functions.
- Create Folders if Necessary and download dateset.
- Loading ICO dataset into variables.
- Encoding and Splitting of Data.
- Linear Regression/Neural Network. 
    - Load Saved Linear Regression Models and Print out performance.
    - Use Model to make prediction - Value of ICO after 6 months.
     ```python
     # Load model with best rMse and make prediction
     fileName = "results/" + "bestRegressionModel_" + str(LineaReggressionMetrics.ROOT_MEAN_SQUARED_ERROR.name) + ".sav"
     bestRegression = joblib.load(fileName)

     #Example ICO
  #price_usd,price_btc,total_supply,market_cap_usd,available_supply,usd_raised,eth_price_launch,btc_price_launch,ico_duration,month,day,country
     example_x = np.array([1.71456,0.00019931,1000000000,905793616,528295082,24000000,297.63,3420.4,7,8,9,182])

     y_pred = makePrediction(bestRegression,example_x)

     print("Predicted value of example ICO after 6 months: ",y_pred )
     ```
  *Replace Example ICO with your ICO to predict. Use dataset/Country_Number_Mapping - Sheet1.csv to map a country to a number.*
