## 6. Implementation Plan

1. Create a private S3 bucket with encryption enabled.
2. Upload and download sample documents.
3. Configure an EFS file system and mount targets.
4. Launch Linux EC2 instances in the same VPC.
5. Mount EFS on both instances.
6. Verify that files created on one instance are accessible from the other.
7. Configure an EC2 IAM role for restricted S3 access.
8. Copy a sample file from EFS to S3.
9. Test security settings and document the results.
10. Clean up resources when testing is complete.



| Test | Description | Result |
|------|-------------|--------|
| 1 | S3 object creation and file upload | [s3-object-creation.png](screenshots/s3-object-creation.png) |
| 2 | S3 lifecycle setup | [s3-Lifecycle.png](screenshots/s3-Lifecycle.png) |
| 3 | EFS mount target setup | [efs-mount-target.png](screenshots/efs-mount-target.png) |
| 4 | Establish connection b/w EC2 (server one) and EFS and create files for sharing | [EFS-testing-EC2-1.png](screenshots/EFS-testing-EC2-1.png) |
| 5 | Establish connection b/w EC2 (server two) and EFS and retrieve files from server one | [EFS-testing-EC2-2.png](screenshots/EFS-testing-EC2-2.png) |
| 6 | S3 and EC2 (server one) connection via IAM role | [IAM-role-ec2-1.png](screenshots/IAM-role-ec2-1.png) |
| 7 | S3 and EC2 (server two) connection via IAM role | [IAM-role-ec2-2.png](screenshots/IAM-role-ec2-2.png) |
| 8 | File copied from server one to S3 | [EC2-1-to-s3-copy.png](screenshots/EC2-1-to-s3-copy.png) |
| 9 | File copied from server two to S3 | [EC2-2-to-s3-copy.png](screenshots/EC2-2-to-s3-copy.png) |
| 10 | Copied files successfully accessible in S3 | [ec2-s3-copyresult.png](screenshots/ec2-s3-copyresult.png) |



CONCLUSION
