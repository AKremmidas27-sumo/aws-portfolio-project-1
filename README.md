# AWS Portfolio Project #1
## S3 + CloudFront Secure Static Website (OAC + HTTPS)

### 🎯 What Problem Does This Solve?
Static website hosting with secure global delivery and origin protection.

### 🏗 Architecture Overview
<architecture image>

### 🛠 AWS Services Used
- Amazon S3 — origin storage
- Amazon CloudFront — global CDN + HTTPS
- Origin Access Control (OAC) — blocks direct S3 access
- AWS CLI — deployment automation
- (Optional: ACM for custom domain)

### 🔐 Security Features
- CloudFront-only access to S3
- Managed SecurityHeadersPolicy
- Versioned S3 bucket

### 🚀 Deployment Steps (High-Level)
1. Create public-blocked S3 bucket
2. Upload index.html and 404.html
3. Create CloudFront distribution with OAC
4. Attach SecurityHeadersPolicy
5. Invalidate cache after update

### 📸 Deployment Proof
| Step | Screenshot |
|------|-----------|
| OAC enabled | ![](images/oac.png) |
| CloudFront Deployed | ![](images/cloudfront.png) |
| Bucket block public access | ![](images/s3.png) |
| Cache invalidation | ![](images/invalidation.png) |

### 🌍 Live Demo URL
➡️ https://d24lku7z6siz5i.cloudfront.net/

### 👤 Author
Andrew Kremmidas  
AWS Certified Solutions Architect – Associate


![IMG_1625](https://github.com/user-attachments/assets/7864035a-69ca-410e-a202-9ea188d69c78)
![IMG_1628](https://github.com/user-attachments/assets/c999f13c-9794-4c77-ab98-5851bfefc9ad)
![IMG_1629](https://github.com/user-attachments/assets/0a89f1be-140c-4cac-bb0f-c9c724f82f97)
![IMG_1631](https://github.com/user-attachments/assets/c9a8758d-c2b0-461f-97be-f84368a5bca0)
![IMG_1729](https://github.com/user-attachments/assets/4fa5b44c-62cb-4857-a7b1-2109094e9aca)
![IMG_1730 (1)](https://github.com/user-attachments/assets/54648620-24d3-4d00-9c4b-c27208961a1f)





