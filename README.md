# insurance_payment_predictor
Predicts Customer's monthly premium
This script utilizes scikit-learn (sklearn) to predict life insurance rates based on age, gender, and smoking status using a linear regression model.

Prerequisites:
Python 3.x
scikit-learn
numpy
Installation:

You can install the required dependencies using pip:
##pip install scikit-learn numpy

Here is an example to use the code:
'''
  from insurance_rate_predictor import InsuranceRatePredictor
  
  predictor = InsuranceRatePredictor()

  # Example training data
  train_X = np.array([[30, 1, 0], [40, 0, 1], [50, 1, 1], [60, 0, 0]])  # Age, Gender, Smoker
  train_y = np.array([150, 200, 300, 250]).reshape(-1, 1)  # Example insurance rates

  predictor.train(train_X, train_y)

  # Predict for user input
  user_X = predictor.preprocess_data(35, 'male', 'no')
  predicted_rate = predictor.predict(user_X)
  print(f"Your estimated insurance rate is: ${predicted_rate[0]:.2f}")
'''
Contributors:

Your Name (https://github.com/aditsinsinwal)
