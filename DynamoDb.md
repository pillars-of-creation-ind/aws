# AWS Dynamo DB

- NoSQL database service
- DynamoDB has high performance and scalability
- It has on-demand backup and point-in-time recovery capabilities
  that allow users to easily roll back.

### Setup aws cli

```bash
# requires access key id, secret access key, region name
aws configure --profile aws-prod

# check all s3 buckets
aws s3 ls --profile aws-prod
```

### create a table in DynamoDB

Table Name: `mystore`
Partition Key: `clientId`
Sort Key: `created`

```
- Partition Key & Sort Key are a way to organizing items in our database.
- Settings: Customize
- Read/write capacity settings: Provisioned
- Read
Auto Scaling: on
Minimum Capacity: 1
Maximum Capacity: 4
Target Utilization: 70

- Write
Auto Scaling: on
Minimum Capacity: 1
Maximum Capacity: 4
Target Utilization: 70

```

### Operations on DynamoDB

```bash
# scan
aws dynamodb scan --table-name mystore --profile aws-prod
```
