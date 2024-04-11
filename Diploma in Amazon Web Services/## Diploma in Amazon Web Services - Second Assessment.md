## Diploma in AWS second assessment

#### Q1. What is web identity federation?

- [ ] Use of AWS IAM User tokens to log in as a Google or Facebook user.
- [ ] Use of an identity provider like Google or Facebook to become an AWS IAM User.
- [x] Use of an identity provider like Google or Facebook to exchange for temporary AWS security credentials.
- [ ] Use of AWS STS Tokens to log in as a Google or Facebook use.

#### Q2. Your API requires the ability to stay online during AWS regional failures. Your API does not store any state, it only aggregates data from other sources - you do not have a database.
What is a simple but effective way to achieve this uptime goal?


- [x] Even if a region fails, the other AZ will stay online.
- [ ] Use an ELB and a cross-zone ELB deployment to create redundancy across datacenter.
- [ ] Even if the region your API is in goes down, the edge locations CIoudFront uses will be fine.
- [ ] Use a CloudFront distribution to serve up your AP.

#### Q3. There is a very serious outage at AWS. EC2 is not affected, but your EC2 instance deployment scripts stopped working in the region with the outage.
What might be the issue?


- [ ] AWS turns off the ˂code˃DepIoyCode˂/code˃ API call when there are major outages, to protect from system floods
- [ ] The AWS Console is down, so your CLI commands do not work
- [x] S3 is unavailable, so you can't create EBS volumes from a snapshot you use to deploy new volumes
- [ ] None of these are accurate

#### Q4. From a compliance and security perspective, which of these statements is true?

- [x] You do not ever need to rotate access keys for AWS IAM Role
- [ ] You do not ever need to rotate access keys for AWS IAM Roles, nor AWS IAM Users.
- [ ] You do not ever need to rotate access keys for AWS IAM Users.
- [ ] None of these statements are true.

#### Q5. Why are more frequent snapshots or EBS Volumes faster?

- [ ] The snapshots are incremental so that only the blocks on the device that have changed after your last snapshot are saved in the new snapshot.
- [ ] Snapshotting the first time forces full block range allocation, so the second snapshot doesn't need to perform the allocation phase and is faster
- [x] Blocks in EBS Volumes are allocated lazily, since while logically separated from other EBS Volumes, Volumes often share the same physical hardware
- [ ] AWS provisions more disk throughput for burst capacity during snapshots if the drive has been pre-warmed by snapshotting and reading all blocks.
- [ ] The drive is pre-warmed, so block access is more rapid for volumes when every block on the device has already been read at least one time.

#### Q6. What is the order of most-to-least rapidly-scaling (fastest to scale first)?
(A) EC2 + ELB + Auto Scaling (B) Lambda (C) RDS.

- [ ] C, B, A
- [x] B, A, C
- [ ] C, A, B
- [ ] A, C, B

#### Q7. You are creating a new API for video game scores. Reads are 100 times more common than writes, and the top 1% of scores are read 100 times more frequently than the rest of the scores.

What's the best design for this system, using DynamoDB?

- [x] DynamoDB table with roughly equal read and write throughput, with EIastiCache caching.
- [ ] DynamoDB table with 100x higher read than write throughput, with CloudFront caching.
- [ ] DynamoDB table with roughly equal read and write throughput, with CloudFront caching.
- [ ] DynamoDB table with 100x higher read than write throughput, with E|astiCache caching.

#### Q8. For AWS CIoudFormation, which stack state refuses UpdateStack calls?

- [ ] ˂code˃CREATE_COMPLETE˂/code˃
- [ ] ˂code˃UPDATE_CONIPLETE˂/code˃
- [ ] ˂code˃UPDATE_ROLLBACK_COMPLETE˂/code˃
- [x] ˂code˃UPDATE_ROLLBACK_FAILED˂/code˃

#### Q9. When thinking of DynamoDB, what are true of Local Secondary Key properties?

- [ ] Only the partition key can be different from the table
- [x] Only the sort key can be different from the table
- [ ] Either the partition key or the sort key can be different from the table, but not both
- [ ] The partition key and sort key can be different from the table

#### Q10. If you want CIoudFormation stack status updates to show up in a continuous delivery system in as close to real-time as possible, how would you achieve this?

- [ ] Subscribe your continuous delivery system to an SQS queue that you also tell your CIoudFormation stack to publish events into
- [x] Subscribe your continuous delivery system to an SNS topic that you also tell your CIoudFormation stack to publish events into
- [ ] Use a long-poll on the Resources object in your CIoudFormation stack and display those state changes in the UI for the system
- [ ] Use a long-poll on the ˂code˃ListStacks˂/code˃API call for your CIoudFormation stack and display those state changes in the UI for the system

#### Q11. What is the scope of an EBS snapshot?

- [ ] Region
- [ ] Placement Group
- [x] Availability Zone
- [ ] VPC

#### Q12. Which of the following is not a restriction on AWS EBS Snapshots?

- [ ] You cannot share a snapshot containing an AWS Access Key ID or AWS Secret Access Key
- [x] Snapshots which are shared cannot be used as a basis for other snapshots
- [ ] You cannot share unencrypted snapshots
- [ ] Snapshot restorations are restricted to the region in which the snapshots are create

#### Q13. You have an asynchronous processing application using an Auto Scaling Group and an SQS Queue. The Auto Scaling Group scales according to the depth of the job queue.

The completion velocity of the jobs has gone down, and the Auto Scaling Group size has maxed out, but the inbound job velocity did not increase. 

What is a possible issue?

- [ ] Someone changed the IAM Role Policy on the instances in the worker group and broke permissions to access the queue
- [ ] The routing tables changed and none of the workers can process events anymore
- [x] Some of the newjobs coming in are malformed and unprocessable
- [ ] The scaling metric is not functioning correctly

#### Q14. You run a 2000-engineer organization. You are about to begin using AWS on a large scale for the first time.

You want to integrate with your existing identity management system running on Microsoft Active Directory because your organization is a power-user of Active Directory.

How should you manage your AWS identities in the most simple manner?

- [ ] Use an Sync Domain running on AWS Directory Service
- [ ] Use a large AWS Directory Service Simple AD
- [x] Use a large AWS Directory Service AD Connector
- [ ] Use an AWS Directory Sync Domain running on AWS Lambda

#### Q15. Your CTO has asked you to make sure that you know what all users of your AWS account are doing to change resources at all times.

She wants a report of who is doing what over time, reported to her once per week, for as broad a resource type group as possible.

How should you do this?

- [ ] Subscribe the CTO to an email type delivery on this SNS Topic.
- [ ] Use CIoudWatch Events Rules with an SNS topic subscribed to all AWS API call.
- [ ] Configure a script to aggregate the log data delivered to S3 once per week and deliver this to the CTO.
- [x] Create a global AWS CIoudTraiI Trail.

#### Q16. When thinking of AWS OpsWorks, which of the following is true?

- [ ] Instances have many stacks, stacks have many layers
- [x] Stacks have many layers, layers have many instances
- [ ] Layers have many stacks, stacks have many instances
- [ ] Layers have many instances, instances have many stack

#### Q17. Which service would you use to send alerts based on Amazon CloudWatch alarms?

- [ ] Amazon Route 53
- [x] Amazon Simple Notification Service (Amazon SNS)
- [ ] AWS CloudTrail
- [ ] AWS Trusted Advisor

#### Q18. You need to migrate 10 million records in one hour into DynamoDB. All records are 1.5KB in size. The data is evenly distributed across the partition key.

How many write capacity units should you provision during this batch load?

- [ ] 2778
- [ ] 5556
- [x] 6667
- [ ] 4166

#### Q19. You are experiencing performance issues writing to a DynamoDB table. Your system tracks high scores for video games on a marketplace. Your most popular game experiences all of the performance issues.

What is the most likely problem?

- [ ] You did not provision enough read or write throughput to the table
- [ ] DynamoDB's vector clock is out of sync, because of the rapid growth in request for the most popular game.
- [x] You selected the Game ID or equivalent identifier as the primary partition key for the table.
- [ ] Users of the most popular video game each perform more read and write requests than average.

#### Q20. Which of these techniques enables the fastest possible rollback times in the event of a failed deployment?

- [ ] Rolling; Immutable
- [ ] Rolling; Mutable
- [ ] Canary or A/B
- [x] Blue-Green

#### Q21. Your company needs to automate 3 layers of a large cloud deployment. You want to be able to track this deployment's evolution as it changes over time, and carefully control any alterations.

What is a good way to automate a stack to meet these requirements?

- [x] Use CloudFormation Nested Stack Templates, with three child stacks to represent the three logical layers of your cloud.
- [ ] Use OpsWorks Stacks with three layers to model the layering in your stack.
- [ ] Use AWS Config to declare a configuration set that AWS should roll out to your cloud.
- [ ] Use Elastic Beanstalk Linked Applications, passing the important DNS entries between layers using the metadata interface.

#### Q22. Which of the following tools does not directly support AWS OpsWorks, for monitoring your stacks?

- [ ] AWS CloudTraiI
- [ ] Amazon CIoudWatch Metrics
- [x] AWS Config
- [ ] Amazon CIoudWatch Logs

#### Q23. When thinking of AWS Elastic Beanstalk, which statement is true?

- [ ] Worker tiers pull jobs from JSON
- [ ] Worker tiers pull jobs from HTTP
- [ ] Worker tiers pull jobs from SNS
- [x] Worker tiers pull jobs from SQ