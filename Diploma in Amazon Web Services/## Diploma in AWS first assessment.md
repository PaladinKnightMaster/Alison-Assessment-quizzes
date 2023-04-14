## Diploma in AWS first assessment

#### Q1. Where can a customer find information about prohibited actions on AWS infrastructure?

- [ ] AWS Trusted Advisor
- [ ] AWS Identity and Access Management (IAM)
- [ ] AWS Billing Console
- [x] AWS Acceptable Use Policy

#### Q2. Which AWS offering enables customers to find, buy, and immediately start using software solutions in their AWS environment?

- [ ] AWS Marketplace
- [ ] AWS SDK
- [ ] AWS Config
- [x] AWS OpsWorks

#### Q3. Which EBS volume type is best for high performance NoSQL cluster deployments?

- [x] iol
- [ ] gpl
- [ ] standard
- [ ] gp2

#### Q4. Which service can identify what user made the API call when an Amazon Elastic Compute Cloud (Amazon EC2) instance is terminated?

- [ ] Amazon CloudWatch
- [x] AWS CloudTrail
- [ ] AWS X-Ray
- [ ] AWS Identity and Access Management (AWS IAM)

#### Q5. Which component of AWS global infrastructure does Amazon CloudFront use to ensure low-latency delivery?

- [ ] Amazon Virtual Private Cloud (Amazon VPC)
- [ ] AWS Regions
- [x] AWS edge locations
- [ ] AWS Availability Zones

#### Q6. Which AWS service would simplify migration of a database to AWS?

- [ ] AWS Storage Gateway
- [x] AWS Database Migration Service (AWS DMS)
- [ ] Amazon Elastic Compute Cloud (Amazon EC2)
- [ ] Amazon AppStream 2.0

#### Q7. What is the scope of an EBS volume?

- [ ] Placement Group
- [ ] Region
- [ ] VPC
- [x] Availability Zone

#### Q8. What is the scope of AWS IAM?

- [ ] Region
- [x] Global
- [ ] Availability Zone
- [ ] Placement Group

#### Q9. Which AWS networking service enables a company to create a virtual network within AWS?

- [ ] AWS Direct Connect
- [x] Virtual Private Cloud
- [ ] AWS Config
- [ ] Route53

#### Q10. A company is developing a highly available web application using stateless web servers. Which services are suitable for storing session state data? Choose two answers.

- [ ] Elastic Load Balancing
- [x] DynamoDB
- [ ] CloudWatch
- [x] Elasticache
- [ ] Storage Gateway

#### Q11. Company salespeople upload their sales figures daily. A Solutions Architect needs a durable storage solution for these documents that also protects against users accidentally deleting important documents. Which action will protect against unintended user actions?

- [ ] Store data on EC2 instance storage
- [x] Store data in an S3 bucket and enable versioning
- [ ] Store data in an EBS volume and create snapshots once a week
- [ ] Store data in two S3 buckets in different AWS regions

#### Q12. An application requires a highly available relational database with an initial storage capacity of 8 TB. The database will grow by 8 GB every day. To support expected traffic, at least eight read replicas will be required to handle database reads. Which option will meet these requirements?

- [ ] Redshift
- [ ] Aurora
- [x] S3
- [ ] DynamoDB

#### Q13. How would a system administrator add an additional layer of login security to a user's AWS Management Console?

- [ ] Audit AWS Identity and Access Management (IAM) roles
- [ ] Use AWS Cloud Directory
- [x] Enable Multi-Factor Authentication
- [ ] Enable AWS CloudTrail

#### Q14. What facilitates continuous delivery of Lambdas?

- [ ] CodeStack
- [ ] ElasticStack
- [ ] Mobile Hub
- [x] CodeDeploy

#### Q15. Which of the following is AWS's responsibility under the AWS shared responsibility model?

- [ ] Managing custom Amazon Machine Images (AMIs)
- [ ] Securing application access and data
- [ ] Configuring third-party applications
- [x] Maintaining physical hardware

#### Q16. Which major database needs a BYO license?

- [x] Oracle
- [ ] MySQL
- [ ] PostgreSQL
- [ ] MariaDB

#### Q17. Why is AWS more economical than traditional data centers for applications with varying compute workloads?

- [x] Amazon EC2 instances can be launched on-demand when needed.
- [ ] Customers retain full administrative access to their Amazon EC2 instances.
- [ ] Amazon Elastic Compute Cloud (Amazon EC2) costs are billed on a monthly basis.
- [ ] Customers can permanently run enough instances to handle peak workloads.

----------------------------------------------------------------------------------------------------------------------

#### Q18. What can AWS Amplify NOT do for a Lambda?

- [ ] create a Lambda
- [x] be an event source
- [ ] assign an IAM role
- [ ] delete a Lambda

#### Q19. How do you author a Lambda in a programming language that AWS does not support?

- [ ] Create a Lambda function with a custom runtime and reference the function in your Lambda
- [x] Create a Lambda layer with a custom runtime and reference the layer in your lambda
- [ ] You cannot use Lambda in this situation
- [ ] Create a Lambda function with a custom runtime

#### Q20. What are listed downstream resources based on?

- [ ] the execution policy
- [x] the Lambda configuration
- [ ] the Lambda nodes
- [ ] the IAM user

#### Q21. Which is an equivalent and valid tag for a pair of Lambdas?

- [ ] department:Sales,department:Sales
- [x] department:Sales,department:sales
- [ ] aws:demo;aws:demo
- [ ] aws:demo;aws:DEMO

#### Q22. Outbound connections from Lambdas must be `_`.

- [ ] neither of these answers
- [ ] UDP/IP
- [ ] TCP/IP
- [x] both of these answers

#### Q23. How are CloudWatch actions configured?

- [ ] automatically
- [ ] none of these answers
- [x] manually
- [ ] ad hoc

#### Q24. You are testing your stream-based application and the associated Lambda. AWS best practice advises you to test by varying what?

- [ ] stream and record sizes
- [ ] stream and shard sizes
- [x] batch and record sizes
- [ ] batch and shard sizes

#### Q25. You need to make your Lambda available to services in multiple VPCs. What do you do?

- [ ] Place each subnet in a VPC. Associate all subnets to your Lambda.
- [ ] Place all subnets in a VPC. Associate all subnets to your Lambda.
- [ ] Configure your Lambda to be available to multiple VPCs.
- [x] Configure all application VPCs to be peered.

#### Q26. How is the cost associated with Lambda function calculated?

- [ ] number of function calls
- [ ] amount of code run
- [x] compute time
- [ ] amount of infrastructure used

#### Q27. What is the fastest way to get started with Lambda?

- [ ] Author a Lambda from scratch.
- [x] Use a blueprint.
- [ ] Use a .zip deployment package.
- [ ] Use the serverless app repository.

#### Q28. Where is the disk space allocated for Lambda functions?

- [x] /tmp
- [ ] /default
- [ ] /temp
- [ ] /ds

#### Q29. How do you stop a running Lambda that is stuck in a recursive loop?

- [ ] Delete the function.
- [x] Set the function concurrent execution limit to 0 while you update the code.
- [ ] Reset the function.
- [ ] Set the function concurrent execution limit to 100 while you update the code.

#### Q30. What is AWS best practice for Lambda configuration?

- [x] Overprovision memory to run your functions faster and reduce your costs. Do not overprovision your function timeout settings.
- [ ] Overprovision memory and your function timeout settings to run your functions faster and reduce your costs.
- [ ] Do not overprovision memory. Overprovision your function timeout settings to run your functions faster and reduce costs.
- [ ] Do not overprovision memory. Do not overprovision your function timeout settings to run your functions faster and reduce costs.

#### Q31. Basic Lambda permissions include permissions for what?

- [ ] removing log groups
- [ ] none of these answers
- [ ] creating log groups
- [x] updating log groups

#### Q32. How are environment variables stored?

- [ ] DynamoDB tables
- [x] key-value pairs
- [ ] S3 buckets
- [ ] none of these answers

#### Q33. You need to use a Lambda to provide backend logic to your website. Which service do you use to make your Lambda available to your website?

- [ ] S3
- [x] API Gateway
- [ ] X-Ray
- [ ] DynamoDB

#### Q34. You are creating a Lambda to trigger on change to files in an S3 bucket. Where should you put the bucket name?

- [ ] in the Lambda function code
- [x] in a Lambda environment variable
- [ ] in the Lambda tags
- [ ] in another S3 bucket

#### Q35. What action is needed before you can test a Lambda?

- [ ] Deploy the Lambda
- [ ] Export the function
- [ ] none of these answers
- [x] Configure a test event

#### Q36. What kind of packages can you use with Node.js for Lambdas?

- [ ] Fleece
- [x] NPM
- [ ] none of these answers
- [ ] Pod

#### Q37. Lambdas are monitored by default using which service?

- [ ] CloudTrail
- [x] CloudWatch
- [ ] CloudFormation
- [ ] LogWatch

#### Q38. What can trigger a Lambda function execution?

- [ ] a table definition
- [ ] queue isolation
- [ ] STS Write
- [x] an SNS topic

#### Q39. You need to set an S3 event trigger on your Lambda to respond when data is added to your bucket from another S3 bucket. Which event type do you configure?

- [ ] POST
- [ ] "All object create events"
- [x] PUT
- [ ] COPY

#### Q40. To make Lambdas more testable, it is AWS best practice to separate which of these?

- [ ] Lambda configuration from logging code
- [ ] Lambda handler from logging code
- [x] Lambda handler from core logic
- [ ] Lambda configuration from core logic

#### Q41. What is included in an exported Lambda deployment package?

- [ ] YAML definition
- [ ] CloudFormation stack configuration
- [ ] SAML deployment stack
- [x] Zip file of all related files

#### Q42. When can you change the execution role of a Lambda?

- [ ] only at creation
- [ ] only before deployment
- [ ] never
- [x] anytime via configuration

#### Q43. What is the relationship between SAM template and CloudFormation template files?

- [ ] SAM templates are a superset of CloudFormation templates. SAM templates include additional resource types.
- [ ] SAM templates have some overlap with CloudFormation templates. Both SAM and CloudFormation templates include resource types that are not in the other type of template.
- [x] CloudFormation templates are a superset of SAM templates. CloudFormation templates include additional resource types.
- [ ] SAM templates are a different name for CloudFormation templates. Both template types include the same resource types.

#### Q44. What service deploys Lambdas regionally?

- [ ] EdgeCloud
- [ ] CloudEdge
- [x] CloudFront
- [ ] CloudStack

#### Q45. What programming language does AWS Lambda support?

- [ ] custom
- [x] all of these answers
- [ ] Java
- [ ] Ruby

#### Q46. You need to setup a mechanism to put controls in place to notify you when you have a spike in Lambda concurrency. What should you do?

- [ ] Deploy a CloudTrail alarm that notifies you when function metrics exceed your threshold. Create an AWS budget to monitor costs.
- [x] Deploy a CloudWatch alarm that notifies you when function metrics exceed your threshold. Create an AWS budget to monitor costs.
- [ ] Deploy a CloudWatch alarm that notifies you when function metrics exceed your threshold. Create an AWS CostMonitor to monitor costs.
- [ ] Deploy a CloudTrail alarm that notifies you when function metrics exceed your threshold. Create an AWS CostMonitor to monitor costs.

#### Q47. You want to minimize cold start time for your Lambda. What do you do?

- [x] Add extra code to check if the transient cache, or the /tmp directory, has the data that you stored.
- [ ] Add extra code to check if the permanent cache, or the /cache directory, has the data that you stored.
- [ ] Do nothing. AWS minimizes cols start time by default.
- [ ] Create a warm-up Lambda that calls your Lambda every minute

[Reference](https://aws.amazon.com/blogs/compute/new-for-aws-lambda-predictable-start-up-times-with-provisioned-concurrency/

#### Q48. When is Lambda code stored encrypted?

- [x] at rest
- [ ] at runtime
- [ ] at deployment
- [ ] non of these answers

[Reference](https://docs.aws.amazon.com/whitepapers/latest/security-overview-aws-lambda/lambda-functions-and-layers.html)

#### Q49. When you use a resource-based policy to give a service, resource, or account access to your function, how can you apply the scope of that permission??

- [ ] at the function level
- [ ] at the alias or function level
- [x] at the version, alias, or function level
- [ ] at the version or function level

[Reference](https://docs.aws.amazon.com/lambda/latest/dg/access-control-resource-based.html)

#### Q50. Lambda can read events from which other AWS services? (ref-https://docs.aws.amazon.com/lambda/latest/dg/lambda-services.html)

- [ ] Kinesis, S3, and SQS
- [ ] Kinesis, S3, and SNS
- [ ] Kinesis, DynamoDB, and SNS
- [x] Kinesis, DynamoDB, and SQS

**Explanation**

- `Lambda can used for all services mentioned on the question: Kinesis, S3, SNS, SQS, DynamoDB. But as you can see in the reference, Lambda's responsibility and method invocation can be categorized by Lambda polling and Event Driven (synchronous invocation). When you implement an event-driven architecture, you grant the event-generating service permission to invoke your function in the function's resource-based policy. Then you configure that service to generate events that invoke your function. When you implement a Lambda polling architecture, you grant Lambda permission to access the other service in the function's execution role. Lambda reads data from the other service, creates an event, and invokes your function. According to this analytics, Kinesis-DynamoDB-SQS use same method invocation, Lambda polling.`

#### Q51. Via what can a Lambda be called?

- [x] all of these answers
- [ ] a DynamoDB trigger
- [ ] an API Gateway
- [ ] an S3 bucket event

**Explanation** (source google)

- `With DynamoDB Streams, you can trigger a Lambda function to perform additional work each time a DynamoDB table is updated. Lambda reads records from the stream and invokes your function synchronously with an event that contains stream records.`
- `These events are considered synchronous events. Simply put, it means that when somebody is calling an API Gateway, it will trigger your Lambda function. It's a synchronous event because your Lambda function has to respond to the client directly at the end of its invocation.`
- `You can use Lambda to process event notifications from Amazon Simple Storage Service. Amazon S3 can send an event to a Lambda function when an object is created or deleted.`

#### 52. which is use case of lambda ?

- [ ] Image processing
- [ ] web application
- [x] both
- [ ] Neither 1st and 2nd

#### Q53. Events are AWS resources that trigger the Lambda function. What data type is the SAM file Events property?

- [ ] Integer
- [ ] Float
- [x] Array
- [ ] String

#### Q54. A company is using an API built using Amazon Lambda, Amazon API Gateway, and Amazon DynamoDB in production. The developer has observed high latency during peak periods. Which approach would best resolve the issue?

- [ ] Increase the Lambda function timeout
- [ ] Route traffic to API Gateway using a Route 53 alias
- [ ] Disable payload compression for the API
- [x] Enable API Gateway stage-level caching

#### Q55. The AWS Serverless Application Model (AWS SAM) is a model that \_\_\_\_ .

- [x] defines serverless applications
- [ ] associates permissions policies
- [ ] creates Lambda functions
- [ ] packages deployment artifacts

#### Q56. The code that you want AWS Lambda to invoke as per some defined triggers is known as **\_**.

- [ ] the event source
- [ ] the downstream resource
- [ ] the log stream
- [x] the Lambda function

#### Q57. A developer has created a Lambda function to scrub real-time data of extraneous information and then send the scrubbed data to Kinesis for further processing and storage. Some of the data showing up in Kinesis seems to be inaccurate. What's the best way for the developer to debug this?

- [ ] Look directly at the Lambda Logs in CloudWatch
- [ ] Send the Lambda failures to a Dead Letter Queue
- [x] Use AWS X-Ray to step through the function
- [ ] Use Kinesis to write their own custom logging tool

#### Q58. Lambdas can be created **\_**.

- [x] All of these answers
- [ ] From scratch
- [ ] From the app repository
- [ ] Using a blueprint

#### Q59. You need to quickly understand execution times for two different Lambda functions with different invocation types: asynchronous and synchronous. What do you do?

- [x] Enable tracing, rerun the lambdas, and view in the lambda console
- [ ] View the logs in CloudTrail
- [ ] View the logs in CloudWatch
- [ ] Enable tracing, rerun the Lambdas, and view in the X-Ray console

#### Q60. Which tool would you use to test a Lambda locally?

- [ ] AWS SAM
- [ ] AWS CLI
- [ ] AWS CloudFormation
- [x] AWS SAM CLI

#### Q61. Your function failed to execute due to a timeout. What type of error is this?

- [ ] Caller
- [x] Runtime
- [ ] Request
- [ ] Account

#### Q62. A company will be modernizing their application which is currently running on Amazon Elastic Cloud Compute (EC2) instances. They have experience with scaling this infrastructure using Amazon EC2 Autoscaling. They want to move to serverless infrastructure consisting of an Amazon API Gateway that triggers Lambda functions. They are consulting you about scaling this new infrastructure. What should the company consider in order to make sure the serverless infrastructure scales to their needs?

- [ ] Enable Auto Scaling Groups for AWS Lambda to ensure that enough Lambda functions are ready to handle the incoming requests
- [ ] Throttle Lambda functions by configuring reserved concurrency, sending the excess traffic to Dead Letter Queues (DLQ) that will be handled when the request volume reduces.
- [x] Look at service limits for Amazon API Gateway and Lambda functions used in order to identify potential bottlenecks and balance performance requirements, costs, and business impact
- [ ] Do nothing. API Gateway and AWS Lambda are managed services that have built-in horizontal scaling, security, and high availability to handle unlimited amount of requests

**Explanation**

In serverless it is important to understand the service limits of all the services used end to end to understand the level of requests that can be handled.