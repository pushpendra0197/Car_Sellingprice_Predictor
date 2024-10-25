I have made Car Price Prediction model after checking with all Regression is a supervised machine learning algorithm and chose best r2_score given algorithm.and deployed over modelbit 
Model is accessible from anywhere.
Kindly install modelbit in your IDE(jupyter,colab) by using (pip install modelbit) import modelbit module.



Command for Curl-


Curl -s -XPOST "https://pushpendradhamanya.us-east-2.aws.modelbit.com/v1/Car_SellingPrice_Predictor/latest" -d '{"data": [PricePresent, RunningKM, CarAge, DrivenFuel, TypeSeller, TypeTransmission]}' | json_pp

Python-

modelbit.get_inference(
  region="us-east-2.aws",
  workspace="pushpendradhamanya",
  deployment="Car_SellingPrice_Predictor",
  data=[PricePresent, RunningKM, CarAge, DrivenFuel, TypeSeller, TypeTransmission]
)
Enter the value according -- # "PricePresent":100000 written as 1.0,"Petrol":0,"Diesel":1,"CNG":2",Dealer":0,"Individual":1,"Manual":0,"Automatic":1"
Model will give you the Selling price of the car according to value you given.

