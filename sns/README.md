# Amazon SNS code examples for the SDK for Python

## Overview

Shows how to use the AWS SDK for Python (Boto3) to work with Amazon Simple Notification Service (Amazon SNS).

<!--custom.overview.start-->
<!--custom.overview.end-->

_Amazon SNS is a web service that enables applications, end-users, and devices to instantly send and receive notifications from the cloud._

## ⚠ Important

* Running this code might result in charges to your AWS account. For more details, see [AWS Pricing](https://aws.amazon.com/pricing/) and [Free Tier](https://aws.amazon.com/free/).
* Running the tests might result in charges to your AWS account.
* We recommend that you grant your code least privilege. At most, grant only the minimum permissions required to perform the task. For more information, see [Grant least privilege](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege).
* This code is not tested in every AWS Region. For more information, see [AWS Regional Services](https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services).

<!--custom.important.start-->
<!--custom.important.end-->

## Code examples

### Prerequisites

For prerequisites, see the [README](../../README.md#Prerequisites) in the `python` folder.

Install the packages required by these examples by running the following in a virtual environment:

```
python -m pip install -r requirements.txt
```

<!--custom.prerequisites.start-->
<!--custom.prerequisites.end-->

### Single actions

Code excerpts that show you how to call individual service functions.

- [Create a topic](sns_basics.py#L33) (`CreateTopic`)
- [Delete a subscription](sns_basics.py#L164) (`Unsubscribe`)
- [Delete a topic](sns_basics.py#L70) (`DeleteTopic`)
- [List the subscribers of a topic](sns_basics.py#L116) (`ListSubscriptions`)
- [List topics](sns_basics.py#L52) (`ListTopics`)
- [Publish an SMS text message](sns_basics.py#L179) (`Publish`)
- [Publish to a topic](sns_basics.py#L205) (`Publish`)
- [Set a filter policy](sns_basics.py#L139) (`SetSubscriptionAttributes`)
- [Subscribe an email address to a topic](sns_basics.py#L85) (`Subscribe`)

### Scenarios

Code examples that show you how to accomplish a specific task by calling multiple
functions within the same service.

- [Create and publish to a FIFO topic](sns_fifo_topic.py)

### Cross-service examples

Sample applications that work across multiple AWS services.

- [Create an Amazon Textract explorer application](../../cross_service/textract_explorer)


<!--custom.examples.start-->
<!--custom.examples.end-->

## Run the examples

### Instructions


<!--custom.instructions.start-->
Run this example at a command prompt with the following command.

```
python sns_basics.py
``` 
<!--custom.instructions.end-->



#### Create and publish to a FIFO topic

This example shows you how to create and publish to a FIFO Amazon SNS topic.


<!--custom.scenario_prereqs.sns_PublishFifoTopic.start-->
<!--custom.scenario_prereqs.sns_PublishFifoTopic.end-->

Start the example by running the following at a command prompt:

```
python sns_fifo_topic.py
```


<!--custom.scenarios.sns_PublishFifoTopic.start-->
<!--custom.scenarios.sns_PublishFifoTopic.end-->

### Tests

⚠ Running tests might result in charges to your AWS account.


To find instructions for running these tests, see the [README](../../README.md#Tests)
in the `python` folder.



<!--custom.tests.start-->
<!--custom.tests.end-->

## Additional resources

- [Amazon SNS Developer Guide](https://docs.aws.amazon.com/sns/latest/dg/welcome.html)
- [Amazon SNS API Reference](https://docs.aws.amazon.com/sns/latest/api/welcome.html)
- [SDK for Python Amazon SNS reference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html)

<!--custom.resources.start-->
<!--custom.resources.end-->

---

Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.

SPDX-License-Identifier: Apache-2.0