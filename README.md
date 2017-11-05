# serverless-aws-python3-intro

This is an introductory project for creating a basic Python 3 serverless system in AWS managed by Serverless Framework.  The project demonstrates triggering a Lambda via a CloudWatch event and storing the event data in S3.

To read how it was created see: http://...

It is a fork of [aws-console-auditor](https://github.com/tmclaugh/aws-console-auditor) for education purposes.
![Architecture Diagram](serverless-aws-console-auditor.png)

This service records AWS console login events.  When a user logs in a CloudTrail event is created.  This will trigger a lambda function that will record the event to S3.  This provides a record of console logins that can be referenced later.
