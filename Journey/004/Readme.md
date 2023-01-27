# IAM 
# Introduction Users, Group, and Pollicies
## IAM : Users and Group
IAM : Identity and Access Management

IAM stands for Identity and Access Management, it is a global service because in IAM it is made to define users in groups. When we create an account, we create a root account, and it has been created by default. In this root we use to manage our account. But then we don't have to use the account anymore, or even share it. 
![image](https://user-images.githubusercontent.com/121589476/214769044-3f5f4c81-f659-4deb-a737-84a688727732.png)
Like the example above, we have two groups in IAM. And the group contains only users, no other groups. The group contains only users. And in the picture above, there is 1 user who is not in the group. It's not a best practice, but it's something we can do on AWS. And also a user can belong to multiple groups.

## IAM : Permissions

Users and groups can be provided with what's called a JSON document. As shown below, this is what is called a policy, IAM policy. 
![image](https://user-images.githubusercontent.com/121589476/214770551-e9b0ddf1-5e37-4aea-a376-ea8e27f56c2d.png)

That's how it looks. 


# IAM USers and Groups Hands On
## AWS Management Console

The AWS service console is called IAM. IAM is a Global service, whereas many other AWS services will be regional services and there will be regional divisions. But for IAM, users and groups are created globally.

# IAM Policies
## IAM Policies Inheritance

![image](https://user-images.githubusercontent.com/121589476/214983644-8c0e64fb-4642-4100-9cb1-79d4405af71e.png)

For example we have a group like the image above. And there is a policy attachment at the group level. The policy will be applied to each member, so they will all get access and inherit this policy.
![image](https://user-images.githubusercontent.com/121589476/214984544-87a74d36-2717-4cce-931b-161b5f1fcc32.png)

Now if there is a second group with different operations and policies then its members will have different policies than the developer group.
![image](https://user-images.githubusercontent.com/121589476/214984805-347cf184-ef66-4dad-a509-5ef8be422711.png)

Then there is another user. he has the possibility of not being part of the group.
![image](https://user-images.githubusercontent.com/121589476/214985983-1ce0d482-024f-4e7d-a309-805edd474c16.png)

And it has the possibility to create what are called inline policies which have policies only attached to the user. So that a user can or can't be a member of a group, we can have an inline policy for any user we want.
![image](https://user-images.githubusercontent.com/121589476/214987558-32cd6664-719d-4d7d-a735-30ff586f11d0.png)

Then if there is 1 more team, namely Audit. And we also attach a policy to it, then the user added there will inherit the policy. So that means CHARLES has policies from the Developer and policies from the Audit team and DAVID has policies from Operations and policies from the Audit team. It should go in when we get into hands-on.

## IAM Policies Structure

In terms of policy structure, we just need to know at a high level how it works, and what it's called.
![image](https://user-images.githubusercontent.com/121589476/214990752-4fa28e1a-e923-4809-a162-8dbb81621ce5.png)

- Consisits Of
        
    - Version : policy language version, always include "2010-10-17"
    - ID : an identifier for the policy (optional)
    - Statement : one or more individual statements (required)
    
- Statements Consist Of 
    
    - Sid : an identifier for the statement (optional)
    - Effect : whether the statement allows or denies access (allow, deny)
    - Principal : account/ user/role to which this policy applied to
    - Action : list of action this policy allows or denies
    - Resource : list of resources to wich the actions applied to
    - Condition : conditions fir when this policy is in effect (optional)
