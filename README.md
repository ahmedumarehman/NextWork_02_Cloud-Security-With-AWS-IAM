<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Cloud Security with AWS IAM

**Project Link:** [View Project](http://nextwork.ai/projects/aws-security-iam)

**Author:** Ahmed Umar Rehman  
**Email:** ahmedumar475@gmail.com

---

![Image](http://nextwork.ai/calm_indigo_beautiful_lizard/uploads/aws-security-iam_1c864649)

---

## Introducing Today's Project!

### Project overview

### Tools and concepts

Services I used were
AWS Alias 
AWS IAM Users 
AWS IAM Group

Key concepts I learnt include...
- How to make policies in json for users 

### Project reflection

This project took me approximately 2 hours The most challenging part was Alias Sigin

---

## Tags

### What I did in this step

In this step, I will launch two EC2 instances to increase NextWork's computing power

### Understanding tags

Tags are to remember which instance is used for 

### My tag configuration

The tag I’ve used on my EC2 instances is called nextwork-dev-ahmedumar3313 & nextwork-prod-ahmedumar3313 The value I’ve assigned for my instances are also same

![Image](http://nextwork.ai/calm_indigo_beautiful_lizard/uploads/aws-security-iam_2e0e5a5d)

---

## IAM Policies

### What I did in this step

In this step, I will create IAM Policy because i want to give access to development instance which I made

### Understanding IAM policies

IAM Policies are rules about what to do about your resources who should you give and who should not

### The policy I set up

For this project, I’ve set up a policy using JSON format 

### Policy effect

I’ve created a policy that user will not delete or create usertags of instances 

### Understanding Effect, Action, and Resource

The Effect, Action, and Resource attributes of a JSON policy means 

Effect: what to allow or what to deny 
Action: what specific thing user can perform or not 
Resource: Which AWS resource the action applies to

---

## My JSON Policy

![Image](http://nextwork.ai/calm_indigo_beautiful_lizard/uploads/aws-security-iam_1c864649)

---

## Account Alias

### What I did in this step

In this step, I will simplify user login in AWS Account using Account Alias because it hives your account a custom, human-readable name used in the IAM sign-in URL,

### Understanding account aliases

An account alias is used to create easier user name login 

### Setting up my account alias

Creating an account alias took me exactly 10-12 minutes  Now, my new AWS console sign-in URL is 
https://nextwork-alias-ahmedumar3313.signin.aws.amazon.com/console

![Image](http://nextwork.ai/calm_indigo_beautiful_lizard/uploads/aws-security-iam_0eb4439b)

---

## IAM Users and User Groups

### What I did in this step

In this step, I will Set up a dedicated IAM group & User because I want to see how can I manage all intern candidate permissions from one place

### Understanding user groups

IAM user groups are those who get access to your resources and they also have limitations which resources to get and which to not

### Attaching policies to user groups

I attached the policy I created to this user group, which means the user cannot delete or create user tags in EC2 instance which they will recieve 

### Understanding IAM users

IAM users are those who represent one identity

---

## Logging in as an IAM User

### Sharing sign-in details

The first way is
download csv 

The second way is
give user signin credentials 

### Observations from the IAM user dashboard

Once I logged in as my IAM user, I noticed I am seeing many access denied This was because i setup the policy that user will not create or delete instances

![Image](http://nextwork.ai/calm_indigo_beautiful_lizard/uploads/aws-security-iam_6f2ab446)

---

## Testing IAM Policies

### What I did in this step

In this step, I will Log into AWS using the intern's IAM user. because it will test the intern's access to your production and development instance.

### Testing policy actions

I tested my JSON IAM policy by not stop instances and it was successful

### Stopping the production instance

When I tried to stop the production instance they tild me that i was not authorized.This was because the IAM User has not permission to delete instances 

![Image](http://nextwork.ai/calm_indigo_beautiful_lizard/uploads/aws-security-iam_0e7a9d6a)

### Stopping the development instance

Next, when I tried to stop the development instance it showed me an error This was because it was written in IAM Policies that i cannot stop instance 

![Image](http://nextwork.ai/calm_indigo_beautiful_lizard/uploads/aws-security-iam_1811801c)

---

## IAM Policy Simulator

### Understanding the IAM Policy Simulator

### How I used the simulator

---

---
