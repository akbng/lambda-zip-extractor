# Lambda Zip Extractor
![The Cover Image explaining the process](https://i.imgur.com/6qTmDWX.png)
This is a lambda function to extract zip files from and back to s3 bucket.

## How to use the function
- Clone this repository, then compress the files into a zip file.
- Go to **AWS console** visit the lambda functions section and then create a new lambda function.
- Give a name to the Lambda Function and make sure the correct permissions are set to access the **S3 and CloudWatch services**. CloudWatch services are required to monitor the lambda function.
- Create the Function.
- In the *Code Source*, Select the **upload from .zip file** and upload the zip file containing the files from this repository.
- Add a trigger for the S3 and select the Bucket name from the dropdown
- Select **PUT** in the event type and enter **.zip** in the suffix field so that only zip files trigger the lambda function.
- Now test the function by uploading a **.zip** file in the specific S3 bucket.


The detailed guide is available in a [medium article](https://aws.plainenglish.io/extract-zip-files-from-and-back-to-the-s3-bucket-using-node-js-f19f009ace22).

Don't forget to configure the lambda function as per your need.
