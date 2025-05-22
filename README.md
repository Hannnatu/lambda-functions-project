# AWS Cloud Cost Optimization - Identifying Stale Resources

## Identifying Stale EBS Snapshots

In this project, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs.

### Description:

Lambda Functions fetches all the EBS Snapshots owned by my account "self" and gathers the ec2 instances both running and stopped, checks if each snapshot is associated with a volume or not and then deletes the snapshots that are not. Doing this ensures cost-optimization.


