# Neural_Network_Charity_Analysis

## Analysis Overview 
The goal of this project was to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. Our analysis was completed on a dataset was received containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. 

## Results 

### Data Preprocessing 

The target variable for the model: 
- IS_SUCCESSFUL

The feature variables for the model:
- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT

We removed the following variables from the input data due to the fact that they were just identification columns: 
- EIN
- NAME

### Compiling, Training, and Evaluating the Model 
I first found the input number which was the length of X_train. This came out to 43. I chose a 80 nodes for the first hidden layer due to the fact that 80 nodes is almost 2x the amount of our input. For our second hidden layer 30 nodes were used. The activation function was relu due to the types of input data we had. 

The output layer was set to a unit of 1 since this is a binary classifier. We are trying to determine if a company will be successful or not so we know what companies to fund. The activation to use was sigmoid due to the binary classifier as well. 

![image](https://user-images.githubusercontent.com/117782103/230746284-f1772799-bd28-4495-a9fa-0229304f7836.png)

We were not able to achieve the target model performance of 75%. Our model accuracy was 70%

![image](https://user-images.githubusercontent.com/117782103/230746535-a78ddaaa-342c-46ce-91ea-6e359ecc06fc.png)

The first thing I did to try and increase the accuracy was to add additional hidden layers. Two more hidden layers were added for a total of 4. 

![image](https://user-images.githubusercontent.com/117782103/230746572-700eba7d-9677-48fe-b192-09fa19a7a23f.png)

Our accuracy decreased to 53%. 
![image](https://user-images.githubusercontent.com/117782103/230746584-5b43c645-2f4e-4382-ba30-3af2e102552e.png)

The second thing tried was to go back to 2 hidden layers, adjust the neurons and adjust the epochs to 50 as we were not seeing much change after 50 epochs. 

![image](https://user-images.githubusercontent.com/117782103/230746608-2a50ec1e-b941-46a7-90a8-6f9e579f343f.png)

The accuracy was basically the same at 53.6%.

![image](https://user-images.githubusercontent.com/117782103/230746629-311eb512-48ef-4cc3-82e2-bdc0872575fc.png)

The last attempt made was to use different activation functions. Sigmoid activation was used for all layers. 




