# Amazon S3 code examples for the SDK for Python

## Overview

Shows how to use the AWS SDK for Python (Boto3) to work with Amazon Simple Storage Service (Amazon S3).

<!--custom.overview.start-->
<!--custom.overview.end-->

_Amazon S3 is storage for the internet. You can use Amazon S3 to store and retrieve any amount of data at any time, from anywhere on the web._

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

### Get started

- [Hello Amazon S3](s3_basics/hello.py#L4) (`ListBuckets`)


### Single actions

Code excerpts that show you how to call individual service functions.

- [Add CORS rules to a bucket](s3_basics/bucket_wrapper.py#L171) (`PutBucketCors`)
- [Add a lifecycle configuration to a bucket](s3_basics/bucket_wrapper.py#L279) (`PutBucketLifecycleConfiguration`)
- [Add a policy to a bucket](s3_basics/bucket_wrapper.py#L226) (`PutBucketPolicy`)
- [Copy an object from one bucket to another](s3_basics/object_wrapper.py#L125) (`CopyObject`)
- [Create a bucket](s3_basics/bucket_wrapper.py#L35) (`CreateBucket`)
- [Delete CORS rules from a bucket](s3_basics/bucket_wrapper.py#L210) (`DeleteBucketCors`)
- [Delete a policy from a bucket](s3_basics/bucket_wrapper.py#L263) (`DeleteBucketPolicy`)
- [Delete an empty bucket](s3_basics/bucket_wrapper.py#L107) (`DeleteBucket`)
- [Delete an object](s3_basics/object_wrapper.py#L157) (`DeleteObject`)
- [Delete multiple objects](s3_basics/object_wrapper.py#L180) (`DeleteObjects`)
- [Delete the lifecycle configuration of a bucket](s3_basics/bucket_wrapper.py#L329) (`DeleteBucketLifecycle`)
- [Determine the existence of a bucket](s3_basics/bucket_wrapper.py#L64) (`HeadBucket`)
- [Get CORS rules for a bucket](s3_basics/bucket_wrapper.py#L190) (`GetBucketCors`)
- [Get an object from a bucket](s3_basics/object_wrapper.py#L73) (`GetObject`)
- [Get the ACL of a bucket](s3_basics/bucket_wrapper.py#L151) (`GetBucketAcl`)
- [Get the ACL of an object](s3_basics/object_wrapper.py#L264) (`GetObjectAcl`)
- [Get the lifecycle configuration of a bucket](s3_basics/bucket_wrapper.py#L305) (`GetBucketLifecycleConfiguration`)
- [Get the policy for a bucket](s3_basics/bucket_wrapper.py#L243) (`GetBucketPolicy`)
- [List buckets](s3_basics/bucket_wrapper.py#L85) (`ListBuckets`)
- [List objects in a bucket](s3_basics/object_wrapper.py#L21) (`ListObjectsV2`)
- [Set a new ACL for a bucket](s3_basics/bucket_wrapper.py#L122) (`PutBucketAcl`)
- [Set the ACL of an object](s3_basics/object_wrapper.py#L237) (`PutObjectAcl`)
- [Upload an object to a bucket](s3_basics/object_wrapper.py#L35) (`PutObject`)

### Scenarios

Code examples that show you how to accomplish a specific task by calling multiple
functions within the same service.

- [Create a presigned URL](s3_basics/presigned_url.py)
- [Get started with buckets and objects](s3_basics/scenario_getting_started.py)
- [Manage versioned objects in batches with a Lambda function](python/code_examples/s3_versioning)
- [Upload or download large files](file_transfer/file_transfer.py)
- [Work with versioned objects](s3_versioning/versioning.py)

### Cross-service examples

Sample applications that work across multiple AWS services.

- [Create an Amazon Textract explorer application](../../cross_service/textract_explorer)
- [Detect entities in text extracted from an image](../../cross_service/textract_comprehend_notebook)
- [Detect objects in images](../../cross_service/photo_analyzer)


<!--custom.examples.start-->
<!--custom.examples.end-->

## Run the examples

### Instructions


<!--custom.instructions.start-->
<!--custom.instructions.end-->

#### Hello Amazon S3

This example shows you how to get started using Amazon S3.

```
python hello.py
```


#### Create a presigned URL

This example shows you how to create a presigned URL for Amazon S3 and upload an object.


<!--custom.scenario_prereqs.s3_Scenario_PresignedUrl.start-->
<!--custom.scenario_prereqs.s3_Scenario_PresignedUrl.end-->

Start the example by running the following at a command prompt:

```
python s3_basics/presigned_url.py
```


<!--custom.scenarios.s3_Scenario_PresignedUrl.start-->
<!--custom.scenarios.s3_Scenario_PresignedUrl.end-->

#### Get started with buckets and objects

This example shows you how to do the following:

- Create a bucket and upload a file to it.
- Download an object from a bucket.
- Copy an object to a subfolder in a bucket.
- List the objects in a bucket.
- Delete the bucket objects and the bucket.

<!--custom.scenario_prereqs.s3_Scenario_GettingStarted.start-->
<!--custom.scenario_prereqs.s3_Scenario_GettingStarted.end-->

Start the example by running the following at a command prompt:

```
python s3_basics/scenario_getting_started.py
```


<!--custom.scenarios.s3_Scenario_GettingStarted.start-->
<!--custom.scenarios.s3_Scenario_GettingStarted.end-->

#### Manage versioned objects in batches with a Lambda function

This example shows you how to manage versioned S3 objects in batches with a Lambda function.


<!--custom.scenario_prereqs.s3_Scenario_BatchObjectVersioning.start-->
Start the example by running the following at a command prompt:

<!--custom.scenario_prereqs.s3_Scenario_BatchObjectVersioning.end-->


<!--custom.scenarios.s3_Scenario_BatchObjectVersioning.start-->
<!--custom.scenarios.s3_Scenario_BatchObjectVersioning.end-->

#### Upload or download large files

This example shows you how to upload or download large files to and from Amazon S3.


<!--custom.scenario_prereqs.s3_Scenario_UsingLargeFiles.start-->
<!--custom.scenario_prereqs.s3_Scenario_UsingLargeFiles.end-->

Start the example by running the following at a command prompt:

```
python file_transfer/file_transfer.py
```


<!--custom.scenarios.s3_Scenario_UsingLargeFiles.start-->
<!--custom.scenarios.s3_Scenario_UsingLargeFiles.end-->

#### Work with versioned objects

This example shows you how to do the following:

- Create a versioned S3 bucket.
- Get all versions of an object.
- Roll an object back to a previous version.
- Delete and restore a versioned object.
- Permanently delete all versions of an object.

<!--custom.scenario_prereqs.s3_Scenario_ObjectVersioningUsage.start-->
<!--custom.scenario_prereqs.s3_Scenario_ObjectVersioningUsage.end-->

Start the example by running the following at a command prompt:

```
python s3_versioning/versioning.py
```


<!--custom.scenarios.s3_Scenario_ObjectVersioningUsage.start-->
<!--custom.scenarios.s3_Scenario_ObjectVersioningUsage.end-->

### Tests

⚠ Running tests might result in charges to your AWS account.


To find instructions for running these tests, see the [README](../../README.md#Tests)
in the `python` folder.



<!--custom.tests.start-->
<!--custom.tests.end-->

## Additional resources

- [Amazon S3 User Guide](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)
- [Amazon S3 API Reference](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html)
- [SDK for Python Amazon S3 reference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html)

<!--custom.resources.start-->
<!--custom.resources.end-->

---

Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.

SPDX-License-Identifier: Apache-2.0