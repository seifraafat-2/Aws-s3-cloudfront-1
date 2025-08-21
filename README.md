# 🌐 Static Website Hosting using AWS S3 + CloudFront + CI/CD

This project demonstrates how to host a **static website** using **Amazon S3** along with **CloudFront** to accelerate and optimize content delivery.  
It also includes a **CI/CD pipeline** using **GitHub Actions** to automatically deploy any updates.

---

## Project Features
-  **Host files** on Amazon S3.
-  **Faster content delivery** using Amazon CloudFront.
-  **Automatic deployment** of any changes via CI/CD.
-  Option to add **SSL certificates** for better security.
-  Ability to link the website with a **custom domain** later.

---

## Implementation Steps

### **1. Create an S3 Bucket and Upload Website Files**
- Create a new **bucket** in **AWS S3**.
- Enable **Static Website Hosting**.
- Upload all your website files (HTML, CSS) into the bucket.
- Set proper permissions to make the files **publicly accessible**.

---

### **2. Configure CloudFront for Content Distribution**
- Create a new **CloudFront Distribution**.
- Link it to your **S3 Bucket** as the origin.
- Get your **CloudFront URL** (e.g.:  
  `https://d25i.cloudfront.net`)
- Optionally, you can add **SSL** and link a **custom domain**.

---

### **3. Set Up CI/CD with GitHub Actions**
A **workflow** is configured so that any code changes will be automatically deployed to **S3** and the **CloudFront cache** will be invalidated.


How to Update the Website
 After making any local changes:

   git add .
   git commit -m "Update: new changes"
   git push origin main


    https://seifraafat-2.github.io/Aws-s3-cloudfront-1/