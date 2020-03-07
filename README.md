# AWS Marketplace Stats

This stack creats all the resoruces necessary for the AWS Marketplace Collection setup found [here](https://docs.aws.amazon.com/marketplace/latest/userguide/commerce-analytics-service.html). Once the stack is deplyed in the Output tabe you'll have all the information needed for the Marketplace Portal.

# DISCLAIMER!

This stack is available to anyone at no cost, but on an as-is basis. 0x4447, LLC. is not responsible for damages or costs of any kind that may occur when you use the stack. You take full responsibility when you use it.

# How to deploy

<a target="_blank" href="https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=zer0x4447-aws-marketplace&templateURL=https://s3.amazonaws.com/0x4447-drive-cloudformation/aws_marketplace.json">
<img align="left" style="float: left; margin: 0 10px 0 0;" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png"></a>

All you need to do to deploy this stack is click the button to the left and follow the instructions that CloudFormation provides in your AWS Dashboard. Alternatively you can download the CF file from [here](https://s3.amazonaws.com/0x4447-drive-cloudformation/aws_marketplace.json).

# What will deploy?

- 1x S3 Bucket
- 1x SNS Topic

# Manual work

- Navigate to the [Commerce Analytics Service enrollment page](https://aws.amazon.com/marketplace/management/cas/enroll).
- Enter the Amazon S3 bucket name and Amazon SNS topic ARN, and choose Enroll.
- On the permissions page, choose Allow.
- On the AWS Marketplace Management Portal, record the Role Name ARN in the success message. You will need it to call the service.

# Pricing

Standard S3 and SNS pricing applyies.

# How to generate the CloudFormation file

This repo was build using the [Grapes Frameworks](https://www.npmjs.com/package/@0x4447/grapes). First you need to install the framework:

```
sudo npm install -g @0x4447/grapes
```

Then, go inside this repo and run this command:

```
grapes -s .
```

This will create a `CloudFormation.json` file in the root dir of the repo which you can upload to AWS.

# The End

If you enjoyed this project, please consider giving it a 🌟. And check out our [0x4447 GitHub account](https://github.com/0x4447), where you'll find additional resources you might find useful or interesting.

## Sponsor 🎊

This project is brought to you by 0x4447 LLC, a software company specializing in building custom solutions on top of AWS. Follow this link to learn more: https://0x4447.com. Alternatively, send an email to [hello@0x4447.email](mailto:hello@0x4447.email?Subject=Hello%20From%20Repo&Body=Hi%2C%0A%0AMy%20name%20is%20NAME%2C%20and%20I%27d%20like%20to%20get%20in%20touch%20with%20someone%20at%200x4447.%0A%0AI%27d%20like%20to%20discuss%20the%20following%20topics%3A%0A%0A-%20LIST_OF_TOPICS_TO_DISCUSS%0A%0ASome%20useful%20information%3A%0A%0A-%20My%20full%20name%20is%3A%20FIRST_NAME%20LAST_NAME%0A-%20My%20time%20zone%20is%3A%20TIME_ZONE%0A-%20My%20working%20hours%20are%20from%3A%20TIME%20till%20TIME%0A-%20My%20company%20name%20is%3A%20COMPANY%20NAME%0A-%20My%20company%20website%20is%3A%20https%3A%2F%2F%0A%0ABest%20regards.).