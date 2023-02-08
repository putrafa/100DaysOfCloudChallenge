# IAM MFA 

## IAM - Password Policy

To secure our users and groups from being compromised, we can have 2 defense mechanisms. The first is to define what is called a Password Policy.

- Strong password = Higher security for your account
- In AWS, you can set up a password policy :
      
    - Set a minimun password legth
    - Require specific character types :
      
        - Including uppercase letters
        - Lowercase letters
        - Numbers
        - Non-alphanumeric characters
    - Allow all IAM users to change their own password
    - Require users to change their password after some time(password expiration)
    - Prevent password re-use
    
Then for the second defense that must be known is Multi Factor Authenticaion or MFA. On AWS it is a must and highly recommended to use it.

- Users have access to your account and can possibly change configurations or delete resources in your AWS account
- You want to protect your Root Account and IAM Account
- MFA = Password you know + security device you own 

![image](https://user-images.githubusercontent.com/121589476/217415208-4ab39280-52e8-42c6-9a12-1b604507a0d7.png)

- Main benefit of MFA :
 
  If a password is stolen or hacked, the acoount is not compromised
  
## MFA Devices Option in AWS

So what are the MFA device options on AWS that we should know about? As follows :
1. Virtual MFA Device

This is what is used in the HandOn so that we can use Google Authenticator, which only works on one phone at a time. or using Aunthy which is multi device both work same except one is multi device. So for Aunthy we have support for multiple tokens on one device. So, it means that with Virtual MFA device we can have root account, IAM user and other accounts and other IAM users. We are free to have as many users and accounts as we want in Virtual kia. MFA tools, which makes for a very easy-to-use solution.

![image](https://user-images.githubusercontent.com/121589476/217417586-b84240c4-06e6-4618-847d-1a07406dbcb3.png)

2. Universal 2nd Factor(U2F) Security Key

It's a physical device, for example YubiKey by Yubico and Yubico is 3rd party for AWS, it's more than AWS provides, it's 3rd party and use physical device, because maybe it's so easy, we put it in our Key Fobs, and we are ready to do it. So this YubiKey supports multiple root users and IAM uses one security so we don't need to need as many keys as users.

![image](https://user-images.githubusercontent.com/121589476/217418539-e291474a-5ee1-4713-87d3-975bb7da31f5.png)

3. Hardware Key Fob MFA Device

This is provided by Gamalto who is also an AWS third party.

![image](https://user-images.githubusercontent.com/121589476/217419067-cadf72ab-44cb-4184-97d3-fca41a07d0ab.png)

If we use Government Cloud in US, WS GovCloud then we have a special Key Fob. provided by SurePassID which is also a 3rd party.

![image](https://user-images.githubusercontent.com/121589476/217419416-c3dd711d-5375-40ae-a4d9-4526a6aef654.png)
