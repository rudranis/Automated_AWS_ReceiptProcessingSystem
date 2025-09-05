## **Automated AWS Receipt Processing System**

## **Overview**
This project automates the process of extracting, storing, and notifying users about receipt data using AWS services. It leverages Amazon Textract, AWS Lambda, Amazon S3, DynamoDB, and SES to build a fully serverless solution for receipt processing.

## **Tech Stack**
Amazon S3 → Storage for uploaded receipts

AWS Lambda → Orchestration & automation

Amazon Textract → Extract text and structured data from receipts

Amazon DynamoDB → Store extracted structured data

Amazon SES (Simple Email Service) → Send email notifications


**Architecture Diagram**
![alt text](<Blank diagram (1).png>)

## **Workflow Steps**
1.The user uploads the receipt to Amazon S3.

2.The S3 upload triggers a Lambda function.

3.Lambda invokes Amazon Textract to extract text/data from the receipt.

4.Textract returns structured data to Lambda.

5.Lambda stores the processed data into a DynamoDB table.

6.Lambda also uses Amazon SES to send an email notification to the user.

## **Example Use Cases**
Automated expense tracking

Bookkeeping & accounting

Invoice/receipt digitization

Business audits & compliance
