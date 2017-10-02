# CustomerFeedbackSentimentAnalysis

Python code to be inserted into an AWS Lambda function as part of an system to analyze and prioritize customer feedback.

Uses NLTK and Textblob libraries for the sentiment analysis. In fact uses the Textblob.sentiment property which is based upon PatternAnalyzer (based on the pattern library).

The system basically supossed that if customer feedback is formatted as a text file and sent to S3 bucket, a lambda function can trigger to start a sentiment analysis on that particular feedback. If the results from the sentiment analysis is that it is a negative feedback, the file is copied to a high priority S3 bucket, a bucket that is set up to be monitored and acted on it quickly.

