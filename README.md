# Loan_Officers
Our project's intent was to utilize two Kaggle datasets concerning loan applications. We intended to use the previous_application.csv file in order to train the model to make predictions on the application_data.csv file.

Our first steps in the project were to understand and clean both files in order to make the models work. We used missingno to display the created DataFrame in order to visualize missing data within the files. After that, we dropped NaNs and limited the number of columns in the previous_application DataFrame that were the same in the application_data, in order to train our models.

For our model, we chose to OneHotEncode 3 columns and scaled 5 columns, then saved the results to a DataFrame, which we used to then run a logistic regression.

Our model scores were incredibly impressive at 82.99% for the training score and 82.95% for a testing score. Our confusion matrix was scored on Approval and Denied loans, where our scores were excellent.

To optimize, we chose to use a Random Forest Classifier which then returned a potentially overfitted training score of 99.8% and an excellent testing score of 83.09%. With the minimal increase in testing score, we know that our model would be very good when deployed.

Our next steps would be to align the application_data in a similar format as the previous_application and then test on the entire application_data set.
