# 🌐 Project 1: Static Portfolio Website on AWS S3

## What This Project Does
Hosts a personal AWS portfolio website on Amazon S3.

## AWS Services Used
- **Amazon S3** — stores and serves website files
---

## Step-by-Step Deployment Guide

### Step 1: Prepare Your Files
- Edit `index.html` — replace [Your Name], email, LinkedIn, GitHub links
- Replace the bucket name in `bucket-policy.json`

### Step 2: Create S3 Bucket
1. Go to AWS Console → S3 → **Create bucket**
2. Bucket name: `myportfolio-yourname` (must be globally unique)
3. Region: choose closest to you (e.g., ap-south-1 for India)
4. **Uncheck** "Block all public access" → confirm
5. Click **Create bucket**

### Step 3: Upload Files
1. Open your bucket → click **Upload**
2. Upload `index.html`
3. Click **Upload**

### Step 4: Enable Static Website Hosting
1. Go to bucket → **Properties** tab
2. Scroll to **Static website hosting** → click Edit
3. Select **Enable**
4. Index document: `index.html`
5. Click **Save changes**

### Step 5: Set Bucket Policy
1. Go to bucket → **Permissions** tab
2. Scroll to **Bucket policy** → click Edit
3. Paste the contents of `bucket-policy.json`
4. Replace `YOUR-BUCKET-NAME` with your actual bucket name
5. Click **Save changes**

### Step 6: Access Your Website
1. Go to **Properties** → **Static website hosting**
2. Copy the **Bucket website endpoint** URL
3. Open in browser — your site is live! 🎉

---