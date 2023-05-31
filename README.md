# Setup-S3-and-Macie-for-Data-Security

STEPS
1. Create an S3 bucket and upload your data file into your bucket
2. Go to Amazon Macie and click create job
3. Select your S3 bucket and click next
4. Select either a scheduled job or one time job and scroll to the bottom
5. In additional settings, select file extensions and in the big dialogue box below, enter your file extension (e.g .pdf, .csv, .docx,) and click next
6. Click on manage custom identifier tab and create a custom identifier and input a name for your custom identifier
7. In the regular expression section, enter the expression that suits your data set (e.g. [a-z]{2}-[0-9]{4}
8. Go back to your previous window tab and refresh to see the newly created custom identifier. Select it and click next
9. Name your job and click submit
10. Wait for about 10mins for the job to be completed
11. The job searches your data based on the custom identifier you set.
12. You can view the summary of all your buckets on the Macie dashboard
