# Detailed Sentiment Analysis of a Hotel Booking App User Reviews using Various Deep Learning Models

## Project Overview
This project involves analyzing and predicting the sentiment of user reviews from app using various deep learning (DL) approaches. The sentiment is classified as positive, negative, or neutral. The best accuracy was achieved using a GRU model at 95.42%, followed by an LSTM model at 95.23%, and a CNN model at 93.83%.

## Steps and Methodology

### Data Preprocessing
1. **Data Summary**:
   - The dataset consists of 84,696 rows and 3 columns, including `ID`, `rating`, and `CleanText`.

2. **Removing Duplicates**:
   - Identified and removed 22,950 duplicate rows.

3. **Text Cleaning**:
   - Removed stopwords using the NLTK library.
   - Removed emojis by converting them to text.
   - Applied lemmatization using the WordNet Lemmatizer to reduce words to their base form.

### Sentiment Analysis
1. **Sentiment Labeling with VADER**:
   - Used the VADER sentiment analyzer to label each review as positive, neutral, or negative based on the compound score.

2. **Class Distribution Visualization**:
   - Plotted the count of each sentiment class to visualize the distribution.

3. **Word Clouds**:
   - Generated word clouds for each sentiment category to visualize the most frequent words.

4. **Frequency Bar Graph**:
   - Created a frequency bar graph showing the top 15 words for each sentiment category.

5. **Words and Characters Plot**:
   - Plotted the distribution of the number of words and characters for each sentiment category.

### Model Training and Evaluation
1. **Tokenization and Padding**:
   - Tokenized the text data and padded sequences to ensure uniform input length.

2. **Data Splitting**:
   - Split the data into training and testing sets with an 80-20 ratio.

3. **Model Architectures**:
   - **GRU Model**:
     - Achieved the highest accuracy of 95.42%.
   - **LSTM Model**:
     - Achieved an accuracy of 95.23%.
   - **CNN Model**:
     - Achieved an accuracy of 93.83%.

4. **Class Weight Calculation**:
   - Calculated class weights to handle class imbalance during model training.

5. **Model Training**:
   - Utilized callbacks like early stopping and model checkpointing.
   - Plotted training and validation loss and accuracy.

6. **Model Evaluation**:
   - Evaluated the model using classification reports and ROC-AUC curves.

### Conclusion
This project demonstrates a comprehensive approach to sentiment analysis of app reviews using various ML and DL models. The GRU model outperformed other models in terms of accuracy, followed closely by the LSTM and CNN models. The results showcase the effectiveness of deep learning techniques in handling text data for sentiment classification tasks.

### Repository Contents
- **Data Preprocessing**: Code for cleaning and preparing the text data.
- **Sentiment Analysis**: Code for sentiment labeling and visualization.
- **Model Training**: Code for training and evaluating different models.
- **Visualization**: Code for generating word clouds, frequency bar graphs, and distribution plots.

This documentation provides a detailed step-by-step guide to replicating the sentiment analysis project, including the preprocessing steps, model training, and evaluation processes.
