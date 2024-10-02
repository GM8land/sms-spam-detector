# sms-spam-detector

## Build a Linear Suppor Vector Classification (SVC) model to predict whether a text message is spam or not spam (ham). Deploy to a Gradio app to test messages. 

### Define a function to perform SMS classiification
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

### Define a function to predict whether SMS is spam or not

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

### Create instance of Gradio app

Running on local URL:  http://127.0.0.1:7864
Running on public URL: https://656771abcf902861b9.gradio.live



### Test messages 

1. You are a lucky winner of $5000!
- Prediction: not spam
2. You won 2 free tickets to the Super Bowl.
- Prediction: not spam
3. You won 2 free tickets to the Super Bowl text us to claim your prize.
- Prediction: spam
4. Thanks for registering. Text 4343 to receive free updates on medicare.
- Prediction: spam