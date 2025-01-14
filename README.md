

## Module 21 Challenge: Build an SMS Spam Detector using Linear Suppor Vector Classification (SVC) model and deploy to Gradio App

### Instructions
- Create the SMS Classification Function
- Create the SMS Prediction Function
- Create a Gradio Interface application that takes a textbox for the inputs and has a textbox for the output. The textboxes should have labels that describe what each textbox contains.


### Requirements
- Create the SMS Classification Function (50 points)
    - The features variable is set equal to the text message column of the DataFrame. (8 points)
    - The target variable is set equal to the "label" column of the DataFrame. (8 points)
    - The data is split into training and testing sets, and the test_size is set to 33%. (8 points)
    - A Pipeline is built using the TfidfVectorizer and LinearSVC to transform the test set and compare it to the training set. (8 points)
    - The model is fitted to the transformed training data and the model is returned. (8 points)
    - The SMSSpamCollection.csv is read into a DataFrame. (5 points)
    - The DataFrame is passed to the sms_classification function and the result is set equal to the "text_clf" variable. (5 points)
- Create the SMS Prediction Function (30 points)
    - A variable that holds the prediction of a new text is created. (8 points)
    - A conditional statement that determines if the text message is "ham" or “spam” is created. (12 points)
    - The conditional returns a message if the text is “ham”. (5 points)
    - The conditional returns a message if the text is “spam”. (5 points)
- Create the Gradio Interface Application (20 points)
    - A Gradio Interface application is created with three parameters for the “function”, “outputs”, and “inputs”. (6 points)
    - The “outputs” parameter is a textbox that contains a label to let the user know what to type in the box. (4 points)
    - The “inputs” parameter is a textbox that contains a label to let the user know that the prediction will be displayed in the textbox. (4 points)
    - The Interface application can be shared with other users with a public URL. (2 points)
    - The Gradio Interface works as expected and there are no errors after a user submits a text message. (4 points)

### Summary:
"""
    Perform SMS classification using a pipeline with TF-IDF vectorization and Linear Support Vector Classification.

    Parameters:
    - sms_text_df (pd.DataFrame): DataFrame containing 'text_message' and 'label' columns for SMS classification.

    Returns:
    - text_clf (Pipeline): Fitted pipeline model for SMS classification.

    This function takes a DataFrame with 'text_message' and 'label' columns, splits the data into
    training and testing sets, builds a pipeline with TF-IDF vectorization and Linear Support Vector
    Classification, and fits the model to the training data. 
    The fitted pipeline is returned to make future predictions.
    """

Define a function to predict whether SMS is spam or not

 """
    Predict the spam/ham classification of a given text message using a pre-trained model.

    Parameters:
    - text (str): The text message to be classified.

    Returns:
    - str: A message indicating whether the text message is classified as spam or not.

    This function takes a text message and a pre-trained pipeline model, then predicts the
    spam/ham classification of the text. The result is a message stating whether the text is
    classified as spam or not.
    """

Create instance of Gradio app

Running on local URL:  http://127.0.0.1:7864
Running on public URL: https://656771abcf902861b9.gradio.live


Test messages 

1. You are a lucky winner of $5000!
- Prediction: not spam
2. You won 2 free tickets to the Super Bowl.
- Prediction: not spam
3. You won 2 free tickets to the Super Bowl text us to claim your prize.
- Prediction: spam
4. Thanks for registering. Text 4343 to receive free updates on medicare.
- Prediction: spam

### Grade: 100
### Grader Feedback:
Hi Geoff,



Thank you so much for the submission. I really appreciate all the hard work you’ve put into this assignment.



Your Gradio application looks clean, and I like how you added the title and description to it. Well done! Keep going the extra mile in your assignments. If you need any assistance, please don’t hesitate to reach out to AskBCS, tutoring services, or TAs during office hours. We’re here to support you!



AI Grader,

Nomsa Tsotetsi
