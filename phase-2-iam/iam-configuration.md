
# Phase 2: AWS IAM Configuration

## Objective
Configure Identity and Access Management
(IAM) to provide secure access to AWS resources.

## IAM Role Details

- Role Name: Portfolio-EC2-S3-Role
- Trusted Entity: AWS Service
- Trusted Service: Amazon EC2
- Purpose: Allow EC2 instances to access
  selected AWS resources securely.

## Security Approach

The project uses IAM roles instead of
storing AWS access keys on EC2 instances.

A least-privilege custom policy will be
attached to allow read-only access to the
project's S3 bucket.

## Benefits

- Secure AWS resource access
- Role-based permissions
- No hardcoded AWS credentials
- Least-privilege access control

## Outcome

Successfully created an IAM role
trusted by the Amazon EC2 service.
