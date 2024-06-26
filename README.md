# aws-cloudformation-stack-1
We are building this project using cfn yaml templates.
Here we are building AWS resources using AWS cloudformation service.

Process we will follow is that

1. We will clone repository in local system.
2. Login to AWS console. Search and navigate to Cloudformation service.
3. Here we will create stack for S3 bucket using S3.yaml template or we can create it manually also.
   To create an S3 bucket manually using CloudFormation, follow these steps:

### Step 1: Navigate to CloudFormation
1. Sign in to the AWS Management Console.
2. Open the CloudFormation service.

### Step 2: Create Stack
1. Click on "Create stack" to start creating a new stack.
2. Choose "Template is ready" and "Upload a template file".
3. Select the CloudFormation template (S3Bucket.yaml) that defines the S3 bucket configuration.

### Step 3: Configure Stack Parameters
1. Provide a stack name for your S3 bucket.
2. Fill in any required parameters defined in the template, such as bucket name, access control settings, etc.
3. You can leave the parameters with default values if they are optional.

### Step 4: Review and Create Stack
1. Review the configuration settings for your CloudFormation stack.
2. Click "Create stack" to initiate the creation process.

### Step 5: Wait for Stack Creation
1. CloudFormation will start creating the S3 bucket based on the provided template.
2. Wait for the stack creation to complete. You can monitor the progress in the CloudFormation console.

### Step 6: Verify S3 Bucket
1. Once the stack creation is complete, verify that the S3 bucket was created as expected.
2. You can check the details of the bucket in the AWS Management Console under the S3 service.

By following these steps, you can manually create an S3 bucket using CloudFormation. This approach allows you to define and manage your infrastructure as code, enabling automated deployment and consistent resource provisioning.
5. After creation of bucket we will upload all templates to bucket or we can use them from local system also.

6. To create a VPC and an EC2 instance using CloudFormation templates stored in an S3 bucket, follow these steps:

### Step 1: Upload Templates to S3 Bucket
1. Store your CloudFormation templates (VPC.yaml and EC2Instance.yaml) in an S3 bucket. Make sure the templates are accessible and have the necessary permissions.

### Step 2: Create CloudFormation Stack
1. Go to the AWS Management Console and navigate to the CloudFormation service.
2. Click on "Create stack" to start creating a new stack.
3. Choose "Template is ready" and "Upload a template file".
4. Select the VPC.yaml template stored in your S3 bucket and click "Next".

### Step 3: Configure Stack Parameters
1. Provide a stack name and fill in any required parameters for the VPC template.
2. Click "Next" to proceed.

### Step 4: Review and Create Stack
1. Review the configuration settings for your CloudFormation stack.
2. Click "Create stack" to initiate the creation process.

### Step 5: Wait for VPC Creation
1. CloudFormation will start creating the VPC based on the provided template.
2. Wait for the stack creation to complete. You can monitor the progress in the CloudFormation console.

### Step 6: Create EC2 Instance Stack
1. Once the VPC stack creation is complete, repeat steps 2-4 to create another stack for the EC2 instance.
2. Choose the EC2Instance.yaml template stored in your S3 bucket.
3. Fill in any required parameters for the EC2 instance, including the VPC ID and subnet ID created in the previous stack.
4. Review and create the stack.

### Step 7: Wait for EC2 Instance Creation
1. CloudFormation will start creating the EC2 instance based on the provided template.
2. Wait for the stack creation to complete. You can monitor the progress in the CloudFormation console.

### Step 8: Verify Resources
1. Once both stacks are created successfully, verify that the VPC and EC2 instance were created as expected.
2. You can check the details of the resources in the AWS Management Console under the respective services (VPC and EC2).

By following these steps, you can create a VPC and an EC2 instance using CloudFormation templates stored in an S3 bucket. This approach helps in automating the infrastructure provisioning process and ensures consistency across environments.

