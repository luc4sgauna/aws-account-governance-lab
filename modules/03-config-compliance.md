# Module 3: AWS Config and Compliance

📘 **Objective**  
Enable AWS Config for continuous compliance monitoring and deploy foundational compliance rules using CloudFormation.

✅ **Steps Completed**

**Step 3.1 – Enable AWS Config**  
• Resource Recording: All supported resources in region  
• Global Resources: Included ✅  
• Delivery Method: New S3 bucket created (`config-bucket-[account-id]`)  
• SNS Topic: Created and enabled (`ConfigAlerts`)  
📝 Confirmed Config is recording and notifications are active

**Step 3.2 – Deploy Config Rules via CloudFormation**  
• Stack Name: `config-security-rules`  
• Template File: `account-governance.yaml`  
• Stack Status: `CREATE_COMPLETE`  
📝 Confirmed the following AWS Config rules were deployed:
- IAM Password Policy check  
- Root account MFA check  
- IAM User MFA check  
- CloudTrail enabled check  
- S3 bucket public write protection check  

📸 **Screenshots**  


🧠 **Notes**  
• CloudFormation automates rule deployment, reducing manual error  
• Ensure SNS topic is subscribed to for alerts  
• Rules provide baseline security posture monitoring
