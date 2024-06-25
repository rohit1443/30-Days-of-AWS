# Day 19/30: Dive into AWS Cloud - Static Website Hosting on S3

Hello AWS Enthusiasts!

Today marks Day 19 of our 30-day AWS challenge, and I’ve successfully hosted a static website on Amazon S3. Here’s a step-by-step guide on what I did for this project:

## 1. Created an S3 Bucket
- Went to the S3 console.
- Clicked “Create bucket” and named it `myStaticwebsite1443`.
- Chose a region and proceeded with the default settings.

## 2. Uploaded Website Files
- Cloned my GitHub repository using `git clone https://lnkd.in/gVJUFgHz`.
- Navigated to the S3 bucket `myStaticwebsite1443`.
- Clicked “Upload” and selected the files from the cloned repository to upload them.

## 3. Configured Bucket for Static Website Hosting
- Went to the “Properties” tab of my bucket.
- Scrolled down to the “Static website hosting” section.
- Enabled it and specified the index document (`index.html`) and error document (`error.html`).

## 4. Enabled ACLs for Object Ownership
- Went to “Permissions” and then “Object Ownership”.
- Edited the settings to enable ACLs and saved the changes.

## 5. Made Files Public Using ACL
- Returned to the bucket files.
- Selected the files and clicked on “Actions” -> “Make public using ACL”.

## 6. Accessed My Website
- My static website is now accessible via the S3 endpoint URL, which can be found in the “Static website hosting” section under “Properties”.

## Bonus Tip
For a custom domain, I plan to configure Amazon Route 53 and associate my domain with the S3 bucket.

Feel free to check out my repository for the files and any additional setup details: [https://lnkd.in/gVJUFgHz](https://lnkd.in/gVJUFgHz)

Let’s keep building and learning!
