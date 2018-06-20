---
swagger: "2.0"
x-collection-name: Datumbox
x-complete: 1
info:
  title: DatumBox
  description: datumbox-offers-a-machine-learning-platform-composed-of-14-classifiers-and-natural-language-processing-functions--functions-include-sentiment-analysis-topic-classification-readability-assessment-language-detection-and-much-more-
  version: 1.0.0
host: api.datumbox.com
basePath: 1.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /SentimentAnalysis.json:
    post:
      summary: Identifies the Sentiment of the Document
      description: The Sentiment Analysis function classifies documents as positive,
        negative or neutral (lack of sentiment) depending on whether they express
        a positive, negative or neutral opinion.
      operationId: SentimentAnalysis
      x-api-path-slug: sentimentanalysis-json-post
      parameters:
      - in: formData
        name: text
        description: The text that you want to analyze
      responses:
        200:
          description: OK
      tags:
      - Sentiment
      - Analysis
  /TwitterSentimentAnalysis.json:
    post:
      summary: Identifies the Sentiment of Twitter Messages
      description: The Twitter Sentiment Analysis function allows you to perform Sentiment
        Analysis on Twitter. It classifies the tweets as positive, negative or neutral
        depending on their context.
      operationId: TwitterSentimentAnalysis
      x-api-path-slug: twittersentimentanalysis-json-post
      parameters:
      - in: formData
        name: text
        description: The text of the tweet that we evaluate
      responses:
        200:
          description: OK
      tags:
      - Twitter
      - Sentiment
      - Analysis
---