# AWS Cloud Practitioner (CLF-C02) — Domain Checklist & Service Map

Two tools in one file: the exam's four domains as a study checklist, and the AWS service map organised the way the exam thinks — by category, with a one-line job description for each core service.

## Domain checklist

### Cloud Concepts
- [ ] What cloud computing is: on-demand delivery of IT resources over the internet, pay-as-you-go
- [ ] The six advantages: trade capital expense for variable expense, benefit from massive economies of scale, stop guessing capacity, increase speed and agility, stop spending money running data centres, go global in minutes
- [ ] Deployment models: all-in cloud, hybrid, on-premises (private cloud)
- [ ] The AWS Cloud Adoption Framework (CAF) and its perspectives in outline
- [ ] Migration strategies in outline (the "R" strategies: rehost, replatform, repurchase, refactor, retain, retire)

### Security & Compliance
- [ ] The shared responsibility model — what AWS secures ("of the cloud") vs what you secure ("in the cloud") — and how it shifts between EC2, RDS, and Lambda
- [ ] IAM: users, groups, roles, policies; root user protection and MFA; least privilege
- [ ] Compliance programs and where to find them: AWS Artifact (reports), AWS Config (resource compliance), AWS Audit Manager
- [ ] Security services by job: Amazon GuardDuty (threat detection), Amazon Inspector (vulnerability scanning), AWS Shield (DDoS), AWS WAF (web application firewall), Amazon Macie (sensitive data in S3), AWS KMS (encryption keys)

### Cloud Technology & Services
- [ ] Global infrastructure: Regions, Availability Zones, edge locations — and how to choose a Region (compliance, latency, price, services)
- [ ] Ways to interact: Management Console, CLI, SDKs, and infrastructure as code (CloudFormation)
- [ ] The service map below — recognising every core service and its one-line job on sight
- [ ] The Well-Architected Framework's six pillars: operational excellence, security, reliability, performance efficiency, cost optimisation, sustainability

### Billing, Pricing & Support
- [ ] Pricing models: On-Demand, Reserved Instances, Savings Plans, Spot Instances — and which workload each fits
- [ ] The billing toolkit: AWS Pricing Calculator (estimate), Cost Explorer (analyse), AWS Budgets (alert), Cost and Usage Report (detail), consolidated billing and cost allocation tags
- [ ] Free Tier: always free, 12-months free, and trials — and how bills happen anyway
- [ ] Support plans in order: Basic, Developer, Business, Enterprise On-Ramp, Enterprise — response times and Trusted Advisor access rise with the tier
- [ ] AWS Trusted Advisor: what it checks (cost, performance, security, fault tolerance, service limits) and that full checks need a paid plan

## The service map

### Compute
| Service | Its job in one line |
|---|---|
| Amazon EC2 | Virtual servers you configure and control |
| AWS Lambda | Run code on events, no server to manage |
| AWS Elastic Beanstalk | Deploy a web app without wiring the infrastructure yourself |
| Amazon Lightsail | Simple fixed-price virtual servers for small projects |
| AWS Outposts | AWS infrastructure run inside your own data centre |

### Storage
| Service | Its job in one line |
|---|---|
| Amazon S3 | Object storage — files as objects in buckets |
| Amazon EBS | Block storage volumes for a single EC2 instance |
| Amazon EFS | Shared file storage many instances can mount at once |
| Amazon S3 Glacier | Low-cost archive storage for rarely touched data |
| AWS Storage Gateway | Bridge between on-premises storage and AWS |
| AWS Backup | Central backup across AWS services |

### Databases
| Service | Its job in one line |
|---|---|
| Amazon RDS | Managed relational databases (MySQL, PostgreSQL, and others) |
| Amazon Aurora | AWS's own high-performance relational database |
| Amazon DynamoDB | Serverless key-value NoSQL database |
| Amazon Redshift | Data warehouse for large-scale analytics |
| Amazon ElastiCache | Managed in-memory caching (Redis / Memcached) |
| Amazon Neptune | Graph database |

### Networking & Content Delivery
| Service | Its job in one line |
|---|---|
| Amazon VPC | Your isolated private network inside AWS |
| Elastic Load Balancing | Spread traffic across targets (ALB for HTTP, NLB for raw TCP) |
| Amazon Route 53 | DNS service, plus domain registration |
| Amazon CloudFront | Content delivery network — edge locations cache your content |
| Amazon API Gateway | Front door for your APIs |
| AWS Direct Connect | A private dedicated line from your site into AWS |
| AWS VPN | Encrypted tunnel over the internet into your VPC |

### Management, Monitoring & Security
| Service | Its job in one line |
|---|---|
| AWS IAM | Who can do what: users, groups, roles, policies |
| AWS Organizations | Many accounts under one governance and one bill |
| Amazon CloudWatch | Metrics, logs, and alarms |
| AWS CloudTrail | The audit record of API activity in your account |
| AWS Config | Records resource configurations and checks them against rules |
| AWS Systems Manager | Operational management across fleets of resources |
| AWS KMS | Create and control encryption keys |
| Amazon GuardDuty | Intelligent threat detection for the account |
| AWS Trusted Advisor | Automated best-practice checks across five categories |

### Analytics, Integration & Machine Learning (recognise on sight)
| Service | Its job in one line |
|---|---|
| Amazon Athena | SQL queries directly on data in S3 |
| Amazon EMR | Managed big-data processing (Hadoop/Spark) |
| AWS Glue | Serverless data preparation and ETL |
| Amazon Kinesis | Real-time data streaming |
| Amazon QuickSight | Business-intelligence dashboards |
| Amazon SQS | Message queue — decouple components |
| Amazon SNS | Notifications and publish/subscribe messaging |
| Amazon EventBridge | Event bus connecting applications |
| AWS Step Functions | Coordinate multi-step workflows |
| Amazon SageMaker | Build, train, and deploy machine-learning models |
| Amazon Rekognition | Image and video analysis |
| Amazon Polly / Lex / Comprehend | Speech, chatbots, and language understanding |

---

*This service map is part of the free study resources from **Mastering Careers & Skills**, drawn from the structure of our complete book **AWS Cloud Certificate (Cloud Practitioner)** — the complete AWS cloud course for CLF-C02, taught from the ground up. **Read Chapter 1 free:** https://careersskillsbooks.com/book/aws-cloud-practitioner/*

*An independent study resource. It is not published by, affiliated with, endorsed by, or approved by Amazon Web Services.*
