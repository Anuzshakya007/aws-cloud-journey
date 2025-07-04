# S3 Static Website Hosting Project

This project demonstrates how I used Amazon S3 to host a static website with public access and optional custom HTML.

## ✅ What I Did
- Created an S3 bucket (`anuj-cloud-static-site`)
- Disabled "Block all public access" to allow public hosting
- Uploaded a custom `index.html` page
- Enabled **static website hosting** via S3 bucket properties

## 🌐 Website URL
> https://anujshakyaportfolio.s3.us-east-1.amazonaws.com/index.html

## 🛠 Tools Used
- AWS S3
- HTML/CSS
- IAM (for access control)
- AWS Console

## 📂 Folder Contents
- `index.html`: Homepage for the static site

## 🚀 How to Reproduce
1. Create an S3 bucket (with a unique name)
2. Uncheck "Block all public access"
3. Enable static website hosting (set `index.html` and optional `error.html`)
4. Upload files and test your site using the generated endpoint

## 🧠 Lessons Learned
- How S3 can be used to serve static content publicly
- Difference between object URL and static site endpoint
- Bucket policy and permissions for public hosting

## 📸 Screenshots
