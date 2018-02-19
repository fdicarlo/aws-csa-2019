# Identity & Access Management

## IAM

  - Used to configure AWS users, groups and resources and their level of access to AWS.
  - IAM users and groups are universal or 'region-less' and available all over the world.
  - Can attach permissions to Groups AND individual Users directly
  - - Access key and Secret access key can only be used to programatically ('through console') login to AWS and username/password can only be used to login through the Web GUI console.
  - Always set up MultiFactor Auth on the root account.
  - Power Users allows access to all AWS services except for management of groups and users within IAM.
  - You can create and customize your own password rotation policies.
  - Billing Alert/Billing Alarm can be enabled via CloudWatch to set notifications when a bill exceeds a threshold
  - Identity Federation – Facebook, LinkedIn and Active Directory- You can login to AWS with your corporate credentials.
  - Temporary access to users and services
  - Integration with other AWS services.
  - Supports PCI-DSS compliance

### Critical Terms
  - MFA - 'Multi-Factor Authentication' (Helps secure the account if someone gets a hold of your username and password. Should ALWAYS be enabled for the root account. Ties the account to a verified device)
  - Root Account – The account tied to the email you created the AWS account with. This account has admin level access by default and should be logged into sparingly. 
  - Users – End users / people. No access by default. Assigned Access Key ID and Secret Access Keys when first created. Keys are only available on account creation and need to be regenerated in the future if not stored by the user initially. 
  - Groups – A way to group users and apply policies to them collectivly(HR, Sales, Developers, etc)
  - Roles – Created for AWS resources or users (i.e. enable read/write access for EC2 to S3)
  - Policy Documents – (JSON format) that defines one or more permissions. Can assign to users, groups or roles. (mosly auto generated from AWS)


### IAM Features

  - IAM is a global service. It is not region specific

  - Root account is the email address you use to sign up for AWS

  - AWS recommends very limited usage of root account

  - Setup MFA on root account.

  - You can attach permissions to individual users and groups.

  - Secret access key can be retrieved only once during user creation. In case you lose it then you can re-generate it.

  - IAM Password policy can be set to access the admin console.

  - New users have no permissions when first created. Everything has to be explicitly added.

  - Power User Access allows Access to all AWS services except the management of groups and users within IAM.

Manage AWS resources via

1. Management console – Using username and password

2. Rest APIs – Using Access Key ID and Secret Access Key

3. AWS CLI - Using Access Key ID and Secret Access Key

4. AWS SDK – various programming languages supported.

Using Access Key ID and Secret Access Key – can be used only via accessing programmatically. Akin to username and password used while accessing the console
