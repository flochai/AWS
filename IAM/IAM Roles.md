#Amazon 

A role is a temporary type of identity that can be given to multiple users or services for a specific task. We can attach trust policies and permissions policies to IAM roles. 

1. Trust policies
	 - who can assume this role 
	 - includes temporary security credentials generated by the sts
2. Permissions policies 

Example Uses:
1. Lamba execution role     --->     gives lambda credentials to access AWS resources 
2. Out of the usual situations: 
	- a helpdesk gets a read-only access for usual activity
	- for exceptional actions to help a client, a break-glass emergency role can be used
3. To give external existing identities rights on AWS ([[Identity Federation]])
4. Apps that have millions of users
	 - the users need access to [[DynamoDB]] but there is a 5000 hard limit for IAM users
	 - they can assume a role to gain temporary access 
	 - this is more secure as well because no hardcoded ID
5. Cross account 

A [[Service-linked Role]] is an IAM role that is linked to a specific service. 


---
Links:

[[AWS Index]]
[[IAM]]
