# Week 0 — Billing and Architecture

## Homework Tasks:

### Cruddur Logical Diagram

Made a [Logical Diagram](https://lucid.app/lucidchart/fadae4ed-2e35-4a80-854c-97ea4bc53abb/edit?viewport_loc=441%2C276%2C1105%2C508%2C0_0&invitationId=inv_12d02464-918d-4eb8-a156-c69364f33ddf) using Lucid charts.

Added search service to it.

### Troubleshooted cloudshell

Here I faced a problem while using cloudshell on my IAM account and I was successfully able to troubleshoot it as it had to do something with permission boundaries which was preventing me access despite having admin access.

Gaining lots of insight regarding troubleshoot while along the way.

### Implimented AWS CLI

Successfully implemented AWS CLI in gitpod

![successful ran command using AWS CLI](./Assets/AWS%20CLI.png)

### Budget using CLI

Ran the following command to implement a budget using AWS CLI

```
aws budgets create-budget \
    --account-id $AWS_ACCOUNT_ID \
    --budget file://aws/json/budget.json \
    --notifications-with-subscribers file://aws/json/budget-notif-with-subscriber.json

```

Got it successfully deployed as seen in the AWS root account

![Budget details](./Assets/Budget%20using%20CLI.png)

### SNS service

Also successfully created a budget notification with subscribers feature (SNS) using aws cli using the following command

```
aws sns subscribe \
    --topic-arn="arn:aws:sns:us-east-1:$AWS_ACCOUNT_ID:billing-alarm" \
    --protocol=email \
    --notification-endpoint=wizard.reborn02@gmail.com

```

and the email used is not my main so no security risk there

![sns comfirmation](./Assets/sns%20confirmation.png)

## Homework Challenges

### Destroy root credentials

Deleted the root id and replaced it with an alias for login in AWS also applied MFA for both root as well as IAM account

### Reviewed the six pillars questions in the Well Architected Tool
