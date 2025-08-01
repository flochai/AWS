Gateway Endpoints are regional services that provide private access from a VPC to S3 and DynamoDB (services that exist outside of the VPC in the public) without having to do the usual networking. Prefix lists representing the services above are added to the route tables with the gateway endpoint as a target. Endpoint policies are used to control what is being accessed (only certain S3s or DynamoDBs). This can't be used cross-region (same region only). It is possible to use gateway endpoints to make S3 buckets fully private. 

<img width="2354" height="1204" alt="Pasted image 20250728165158" src="https://github.com/user-attachments/assets/6c703ad3-3efc-4083-88ac-fce14535d8ce" />

---
Links:

[[AWS Index]]
[[VPCs]]
[[Networking in AWS]]
[[VPC Endpoints Interface]]
[[2025-07-28]]
