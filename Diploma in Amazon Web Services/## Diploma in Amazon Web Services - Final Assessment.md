## Diploma in AWS second assessment

#### Q1. You need to replicate API calls across two systems in real time. What tool should you use as a buffer and transport mechanism for API call events?

- [ ] AWS SQS
- [ ] AWS SNS
- [x] AWS Kinesis
- [ ] AWS Lambda

#### Q2. Which of these is not a restriction on AWS EBS Snapshots?

- [x] Snapshots which are shared cannot be used as a basis for other snapshots.
- [ ] Snapshot restorations are restricted to the region in which the snapshots are create
- [ ] You cannot share unencrypted snapshots.
- [ ] You cannot share a snapshot containing an AWS Access Key ID or AWS Secret Access Key.

#### Q3. Which service can identify the user that made the API call when an Amazon Elastic Compute Cloud (Amazon EC2) instance is terminated?

- [ ] Amazon CloudWatch
- [x] AWS CloudTrail
- [ ] AWS Identity and Access Management (AWS IAM)
- [ ] AWS X-Ray

#### Q4. What is a circular dependency in AWS CIoudFormation?

- [ ] When Nested Stacks depend on each other
- [x] When Resources form a DependOn loop
- [ ] When a Template references a region, which references the original Template
- [ ] When a Template references an earlier version of itself

#### Q5. You are building a Ruby on Rails application for internal, non-production use which uses MySQL as a database.

You want developers without very much AWS experience to be able to deploy new code with a single command line push. You also want to set this up as simply as possible. 

Which tool is ideal for this setup?

- [ ] AWS CIoudFormation
- [ ] AWS ELB + EC2 with CLI Push
- [x] AWS Elastic Beanstalk
- [ ] AWS OpsWorks


#### Q6. You need the absolute highest possible network performance for a cluster computing application.

You already selected homogeneous instance types supporting 10 gigabit enhanced networking, made sure that your workload was network bound, and put the instances in a placement group.

What is the last optimization you can make?

- [ ] Bake an AMI for the instances and relaunch, so the instances are fresh in the placement group and don't have noisy neighbors.
- [ ] Segregate the instances into different peered VPCs while keeping them all in a placement group, so each one has its own Internet Gateway.
- [ ] Turn off SYN/ACK on your TCP stack or begin using UDP for higher throughput
- [x] Use 9001 MTU instead of 1500 for Jumbo Frames, to raise packet body to packet overhead ratios.