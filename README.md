# Deploy Stack on AWS CloudFormation

## Overview
This guide provides steps to deploy a stack on AWS CloudFormation. AWS CloudFormation is a service that allows you to manage, configure, and provision AWS resources in a predictable and repeatable way. By following these steps, you can model your entire infrastructure in a text file, enabling you to version control your AWS infrastructure the same way as you version control your software. The application is built using technologies such as Linux, Apache, MySQL, and PHP (LAMP Stack).

## AWS CloudFormation Set Up
1. Open AWS CloudFormation on a separate tab.
2. Click on "Create Stack".
3. Under "Prerequisite - prepare template", choose "Use a sample template".
4. Under "Select a sample template", choose anything under the "SIMPLE" category (e.g. LAMP Stack), optionally click on "View in designer" to see preview of template, then click "Next".
5. Enter the following information: Stack name="Any name or My-LAMP-Stack-123456", DBName="any name", Password="any password", DBUser="any name or admin", Instance Type="any or t2.small", Key Name="an  existing one", then click "Next".
6. Under "Configure stack options", configure as needed, then click "Next".
7. Review the configurations, then click "Create stack".
8. Wait until the creation process is complete.
9. Under "Outputs" tab, open the Website URL value on a new tab.

## Clean Up
1. Open CloudFormation on a separate tab.
2. Choose CloudFormation stack you just created, click on "Delete". Note: By deleting the CloudFormation stack, you will also be getting rid of all underlying services, such as EC2, S3, RDS, which makes it easier than removing them manually. You can always verify this step.

## Conclusion
In this project, we demonstrated how to deploy a stack on AWS CloudFormation. By leveraging the power of AWS CloudFormation, we have automated the process of creating and managing our AWS resources, saving us time and effort. This project has shown the potential of AWS CloudFormation in managing complex infrastructures. Feel free to message me with code improvement suggestions or any questions you may have.

## Acknowledgment
This tutorial is adapted from the [Creating a stack on the AWS CloudFormation console](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-console-create-stack.html) provided by Amazon Web Services. We extend our gratitude to AWS for providing this valuable resource, which served as the foundation for the "Deploy LAMP Stack on AWS CloudFormation" tutorial.
