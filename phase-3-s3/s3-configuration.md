
# Phase 3: Amazon S3 Configuration

## Objective
Configure Amazon S3 for secure object storage
in the AWS portfolio project.

## Bucket Details

- Bucket Name: YOUR-ACTUAL-BUCKET-NAME
- Region: Same as Portfolio-VPC
- Bucket Type: General Purpose
- Object Ownership: ACLs Disabled
- Versioning: Enabled
- Encryption: SSE-S3
- Public Access: Blocked

## Folder Structure

- website-assets/
- project-documents/

## IAM Integration

Created a custom IAM policy named
Portfolio-S3-Read-Policy.

Permissions granted:
- s3:ListBucket
- s3:GetObject

Attached the policy to:
Portfolio-EC2-S3-Role

## Security Features

- Private bucket
- Public access blocked
- Server-side encryption
- Object versioning
- Least-privilege IAM permissions

## Outcome

Successfully created and configured an
Amazon S3 bucket for secure object storage
and prepared IAM-based access for EC2.
