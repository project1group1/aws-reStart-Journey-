Hosting a Static Website on AWS S3
Project Overview

I wanted to host my own static website, so I used Amazon S3 (Simple Storage Service) to make it happen. A static website just means fixed content—HTML, CSS, maybe some JavaScript—nothing complicated on the backend. AWS S3 turned out to be perfect for this because it's simple, doesn't cost much, and scales automatically if people actually visit my site.
AWS CLI Automation
I am moving away from manual console clicks to master the AWS Command Line Interface (AWS CLI). Using an EC2 instance as my command center, I will programmatically build the Café & Bakery infrastructure.

My goal is to use the terminal to create a unique S3 bucket, configure a new IAM user with full access permissions, and deploy the website files directly from my instance. I will also develop a batch script to automate future updates, ensuring any local changes sync to the cloud instantly.

<img width="897" height="467" alt="Screenshot 2026-03-17 224257" src="https://github.com/user-attachments/assets/869c9dca-f8ae-40df-b929-89e4e4a3163d" />

Challenges
Everything seemed fine after I uploaded my files to the S3 bucket and enabled static website hosting. I was excited to see my site live. But when I opened the URL in my browser, this is what I got:

<img width="805" height="321" alt="Screenshot 2026-03-17 153234" src="https://github.com/user-attachments/assets/8d9c70e8-0972-47f8-bdfd-3992facbd852" />

A big fat 403 Forbidden error. Access denied. My files were in the bucket, the hosting was on, but nobody could see anything. The error told me exactly what was wrong—I hadn't made the bucket contents publicly readable. By default, everything in S3 is private. I needed to explicitly allow public access to the website files.

So that was my challenge: figuring out how to properly configure permissions so visitors could actually view my site without getting blocked.
How I Succeeded
After figuring out the permission issue, I fixed it by adding the right bucket policy to make my files public. Once that was done, I refreshed the browser and finally saw my website live:

<img width="842" height="478" alt="Screenshot 2026-03-17 153433" src="https://github.com/user-attachments/assets/15f01aed-b473-4b2f-8dcd-b265a7a7e3db" />

I successfully built and deployed my café website on AWS S3. The 403 error is gone and now anyone with the link can visit my site.
How I Made It Better with HTML and CSS
Once the basic site was live, I wanted to make it look more professional and inviting. I wrote custom HTML and CSS to create a proper layout with navigation, a hero section, and a clean design. Here's what the new version looks like:
<img width="937" height="481" alt="Screenshot 2026-03-17 154510" src="https://github.com/user-attachments/assets/8070a80c-29fb-426e-8488-166ae8dc16f2" />
I added a navigation bar so visitors can easily find their way around. The welcome message with the tagline gives the site personality, and the "Explore Our Menu" button invites interaction. I also styled the page with CSS to use warm colors, nice fonts, and a responsive layout that looks good on both desktop and mobile.

Now the site not only works—it actually looks like a real café website. I'm proud of how it turned out.
