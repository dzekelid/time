---
name: AWS Machine Learning
x-slug: aws-machine-learning
description: Amazon Machine Learning is a service that makes it easy for developers
  of all skill levels to use machine learning technology. Amazon Machine Learning
  provides visualization tools and wizards that guide you through the process of creating
  machine learning (ML) models without having to learn complex ML algorithms and technology.
  Once your models are ready, Amazon Machine Learning makes it easy to obtain predictions
  for your application using simple APIs, without having to implement custom prediction
  generation code, or manage any infrastructure.Amazon Machine Learning is based on
  the same proven, highly scalable, ML technology used for years by Amazon&rsquo;s
  internal data scientist community. The service uses powerful algorithms to create
  ML models by finding patterns in your existing data. Then, Amazon Machine Learning
  uses these models to process new data and generate predictions for your application.Amazon
  Machine Learning is highly scalable and can generate billions of predictions daily,
  and serve those predictions in real-time and at high throughput. With Amazon Machine
  Learning, there is no upfront hardware or software investment, and you pay as you
  go, so you can start small and scale as your application grows.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonMachineLearning.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Time
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/time/master/_listings/aws-machine-learning/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Machine Learning API Create Realtime Endpoint
  x-api-slug: aws-machine-learning-api
  description: Creates a real-time endpoint for the MLModel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonMachineLearning.png
  humanURL: https://aws.amazon.com/machine-learning/
  baseURL: ://///?Action=CreateRealtimeEndpoint
  tags: Machine Learning,Real Time
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/time/master/_listings/aws-machine-learning/actioncreaterealtimeendpoint-get-openapi.md
- name: AWS Machine Learning API Delete Realtime Endpoint
  x-api-slug: aws-machine-learning-api
  description: Deletes a real time endpoint of an MLModel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonMachineLearning.png
  humanURL: https://aws.amazon.com/machine-learning/
  baseURL: ://///?Action=DeleteRealtimeEndpoint
  tags: Machine Learning,Real Time
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/time/master/_listings/aws-machine-learning/actiondeleterealtimeendpoint-get-openapi.md
- name: AWS Machine Learning API Describe Tags
  x-api-slug: aws-machine-learning-api
  description: Describes one or more of the tags for your Amazon ML object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonMachineLearning.png
  humanURL: https://aws.amazon.com/machine-learning/
  baseURL: ://///?Action=DescribeTags
  tags: Machine Learning,Real Time
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/time/master/_listings/aws-machine-learning/actiondescribetags-get-openapi.md
- name: AWS Machine Learning API
  x-api-slug: aws-machine-learning-api
  description: Amazon Machine Learning is a service that makes it easy for developers
    of all skill levels to use machine learning technology. Amazon Machine Learning
    provides visualization tools and wizards that guide you through the process of
    creating machine learning (ML) models without having to learn complex ML algorithms
    and technology. Once your models are ready, Amazon Machine Learning makes it easy
    to obtain predictions for your application using simple APIs, without having to
    implement custom prediction generation code, or manage any infrastructure.Amazon
    Machine Learning is based on the same proven, highly scalable, ML technology used
    for years by Amazon&rsquo;s internal data scientist community. The service uses
    powerful algorithms to create ML models by finding patterns in your existing data.
    Then, Amazon Machine Learning uses these models to process new data and generate
    predictions for your application.Amazon Machine Learning is highly scalable and
    can generate billions of predictions daily, and serve those predictions in real-time
    and at high throughput. With Amazon Machine Learning, there is no upfront hardware
    or software investment, and you pay as you go, so you can start small and scale
    as your application grows.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonMachineLearning.png
  humanURL: https://aws.amazon.com/machine-learning/
  baseURL: :///
  tags: Time
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/time/master/_listings/aws-machine-learning/openapi.md
x-common:
- type: x-command-line-interface
  url: http://aws.amazon.com/cli/
- type: x-console
  url: https://console.aws.amazon.com/machinelearning
- type: x-documentation
  url: http://docs.aws.amazon.com/machine-learning/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/machine-learning/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/machine-learning/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/machine-learning/pricing/
- type: x-tools
  url: http://aws.amazon.com/developertools/
- type: x-website
  url: https://aws.amazon.com/machine-learning/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---