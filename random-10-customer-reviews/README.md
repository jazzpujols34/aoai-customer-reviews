# AOAI Top 10 Customer Review Analysis

This repository contains a Jupyter notebook that uses the Azure OpenAI service to analyze a random sample of 10 customer reviews. 

The script reads a CSV file containing customer reviews, uses the OpenAI GPT-3 model to analyze the sentiment, summarize the content, generate keywords, and draft a reply message for each review. The results are then saved into a new CSV file and visualized as a pie chart.

## Prerequisites

- Python 3.6 or higher

- pandas library

- openai library

## Setup

1. Clone this repository.

2. Install the required Python libraries using pip and the provided `requirements.txt` file:

```
pip install -r requirements.txt
```
The `requirements.txt` file should contain the following libraries:

```
matplotlib
pandas
openai
python-dotenv
```

3. Replace <YOUR_AOAI_ENDPOINT>, <YOUR_AOAI_KEY>, and <YOUR_MODEL_DEPLOYMENT_NAME> in the script with your Azure OpenAI endpoint, key, and model deployment name respectively.



## Usage

Run the script using Jupyternotebook or Python:

The script will read the customer reviews from ./data/asos_transform.csv, analyze the reviews using the Azure OpenAI service, and save the results into ./data/analyzed_review_content.csv.

## Output

The output CSV file will contain the following columns for each review:

- `review_content`: The original review content.

- `classified_sentiment`: The sentiment of the review classified by the OpenAI GPT-3 model.

- `summarized_sentence`: A one-sentence summary of the review generated by the OpenAI GPT-3 model.

- `summarized_keywords`: Three keywords summarizing the review generated by the OpenAI GPT-3 model.

- `reply_message`: A draft reply message to the review generated by the OpenAI GPT-3 model.

The script will also print a summary of all the reviews and display a pie chart visualizing the distribution of the classified sentiments.

Please replace the commands and file paths as necessary to match your actual environment and requirements.




