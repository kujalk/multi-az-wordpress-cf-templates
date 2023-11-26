# Purpose

This CloudFormation (CF) template is for deploying a Wordpress site on Amazon Web Services (AWS). It creates an Elastic Load Balancer (ELB) with an attached target group, an Elastic File System (EFS) to store the Wordpress files, and an Aurora MySQL database cluster.

# To use this CF template, follow these steps:

1. Log in to your AWS account and navigate to the CloudFormation service.

2. Click the "Create stack" button.

3. Select "Upload a template file" and upload the template file or copy-paste the template content into the editor.

4. Fill out the parameters section according to your preferences, and click "Next".

5. On the "Options" page, you can configure additional settings for your stack, or you can leave them as default. Click "Next".

6. On the "Review" page, check that all the details are correct, and then click "Create stack".

# The resources that this CF template creates are:

- Elastic File System (EFS): A file system to store the Wordpress files.

- EFS mount targets: The mount points that allow EC2 instances to access the EFS file system.

- Aurora MySQL database cluster: The database instance that stores the Wordpress data.

- Public Application Load Balancer: The load balancer that routes traffic to the EC2 instances running Wordpress.

- ELB listener: The listener that listens to traffic on port 80 and forwards it to the target group.

- ELB target group: The target group that routes traffic to the EC2 instances running Wordpress.

# Final Step

After the resource is created, go to CF output and open the LB url

# Blog

https://scripting4ever.wordpress.com/2023/11/26/empowering-scalable-and-secure-wordpress-deployments-on-aws-a-deep-dive-into-infrastructure-templates/

# Developer

Janarthanan Kugathasan

