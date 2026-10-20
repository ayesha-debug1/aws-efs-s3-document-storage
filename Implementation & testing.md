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
| 1 | S3 upload | |
| 2 | S3 lifecycle setup | |
| 3 | EFS mount | |
| 4 | Establish connection b/w EC2 (server one) and EFS | |
| 5 | File sharing test result on server two | |
| 6 | S3 and EC2 (server one) connection via IAM role | |
| 7 | S3 and EC2 (server two) connection via IAM role | |
| 8 | File copied from server one to S3 | |
| 9 | File copied from server two to S3 | |
| 10 | Copied files successfully accessible in S3 | |



CONCLUSION
