**Goal**
  Migrate an on permise application to multicloud for a luxery hotel to keep track of the customers and their covid reports
  PDFs contains -- Covid reports
**Goal**

---------- Mission 1 ---------------
1. Create a GCP and AWS Accounts
2. Create IAM User in AWS Account and accessKey.csv for CLI operations for S3Full Access, for creating S3 instance
3. Attach it with deploy it along with scripts into GCP
4. Modify the shell scripts to make them excecutable 
5. Run the AWS shell script with the accessKeys
6. Run the GCP set project Shell script
7. Enable the Container Registry API, Kubernetes Engine API and the Cloud SQL API

8. Run the terraform Commands
   i.Terraform init
   ii. Terraform Plan
   iii. Terraform Apply

This will initialize the Clouds with required instances


---------- Mission 2 ---------------
1. Create an other user for GCP in AWS for S3 bucket, so it can access PDF reports of covid and download the csv file
2. Create a database in google cloud sql instance
3. import the mission 2 files, which contains docker image with yaml script
4. build the docker image and push it into GCR
5. run the yaml script(pipeline which creates applicaition and its connection to database)
6. initiaize the database with tables and its records


---------- Mission 3 ---------------
1. Load all the pdfs into the s3 bucket
2. Now you can see the data and corrosponding reports in application


---------- to delete the instances ------
1. Delete all the data in s3 bucket
2. Delete the database in Cloud SQL, ensure you have disabled the deletion protection for kubernates, S3 and MySQL instances
3. Navigate to terraform folder then enter
     i. Terraform Destroy




