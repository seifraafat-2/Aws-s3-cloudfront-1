# Hosting a Static Website using AWS S3 and CloudFront

Hello,  
I uploaded my static website files to Amazon S3 and used CloudFront to distribute the content faster and with better security.

---

## Steps I followed

1. **Uploading files to S3**  
I created a new bucket on AWS S3 and enabled Static Website Hosting.  
Then, I uploaded all my site files (HTML, CSS, JavaScript, images) to the bucket.  
I set the proper permissions to make the files publicly accessible.

2. **Creating a CloudFront Distribution**  
I created a new CloudFront distribution linked to my S3 bucket.  
I used the URL provided by CloudFront as the website address.  
CloudFront helped speed up loading times and improve security.

3. **Updating the site**  
Whenever I make changes locally, I upload the updated files again to S3 using this command:

Notes:

I didn’t use a custom domain, so the website is accessible only through the CloudFront URL.
I can easily connect a custom domain to CloudFront later if needed.

I can easily connect a custom domain to CloudFront later if needed.

