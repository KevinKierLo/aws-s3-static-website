<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://nextwork.ai/projects/aws-host-a-website-on-s3)

**Author:** Kevin Kier Lo  
**Email:** kevinkierlo29@gmail.com

---

![Image](http://nextwork.ai/joyful_lavender_trusty_freshwater_mussel/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate how to use Amazon S3 to host a static website. I'm doing this project to learn how to create and configure an S3 bucket, upload website files, manage access permissions, and make a website publicly accessible using AWS.

### Tools and concepts

Services I used were Amazon S3. Key concepts I learnt include S3 buckets, object storage, ACLs, public access, static website hosting, bucket policies, and access permissions.

### Time, challenges, and wins

This project took me approximately 1 hour. The most challenging part was configuring the S3 permissions and bucket policy. It was most rewarding to see my website successfully hosted online using Amazon S3.

---

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will create an Amazon S3 bucket to store my website files because S3 provides cloud storage for the files needed to host a static website.

### How long it took to create the bucket

Creating an S3 bucket took me 5 seconds because the setup process was quick and straightforward.

### Region selection

The Region I picked for my S3 bucket was Singapore because it is the closest AWS Region to my location, which can help reduce latency when accessing the website.

### Understanding bucket name uniqueness

S3 bucket names have to be globally unique, which means no two AWS accounts can have the same bucket name. This is because the bucket name is used as part of the bucket’s web address.

![Image](http://nextwork.ai/joyful_lavender_trusty_freshwater_mussel/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

In this step, I will upload the HTML file and image files to my S3 bucket because these files are needed to create and display the website.

### Files I uploaded

I uploaded two files to my S3 bucket - they were index (7).html and profile.jpg

### How the files work together

Both files are necessary for this project as index (7).html contains the portfolio website, while profile.jpg is used as the profile picture on the website.

![Image](http://nextwork.ai/joyful_lavender_trusty_freshwater_mussel/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

In this step, I will configure my S3 bucket for static website hosting because I want to make my HTML portfolio accessible through a public website link

### Understanding website hosting

Website hosting means storing your website files on a server so people can access your website through the internet.

### How I enabled website hosting

To enable website hosting with my S3 bucket, I enabled Static Website Hosting in the bucket’s Properties settings and set index (7).html as the index document. The HTML file name may vary depending on the name of the HTML file you uploaded.

### Access Control Lists (ACLs)

An Access Control List (ACL) is a set of permissions that controls who can access an S3 bucket or its objects. I enabled ACLs because this project uses them to make the website files publicly accessible.

![Image](http://nextwork.ai/joyful_lavender_trusty_freshwater_mussel/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website hosting is enabled, S3 produces a bucket endpoint URL, which is the web address I can use to access my website online.

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw an “Access Denied” error. The reason for this error was that the website files in my S3 bucket were private and did not have public access permissions.

![Image](http://nextwork.ai/joyful_lavender_trusty_freshwater_mussel/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

In this step, I will make my website files publicly accessible using S3 permissions because the files need to be viewable by anyone who visits my website.

### How I resolved the 403 error

To resolve this 403 Forbidden error, I made the website files publicly accessible by changing their ACL permissions in the actions of my S3 bucket.

![Image](http://nextwork.ai/joyful_lavender_trusty_freshwater_mussel/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

In this project extension, I'm about to set up a bucket policy to prevent my index (7).html file from being deleted. I'm doing this so that I can practice using S3 bucket policies to protect important website files and test how access permissions work.

### Understanding bucket policies

“An alternative to ACLs are bucket policies, which are rules that control access to the resources in an S3 bucket. The benefit of using bucket policies is that they can manage access for the entire bucket, while ACLs are useful for controlling access to individual objects.

![Image](http://nextwork.ai/joyful_lavender_trusty_freshwater_mussel/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy was used to prevent my index (7).html file from being deleted. I tested this by trying to delete the file from my S3 bucket and saw that the deletion was denied.

---

---
