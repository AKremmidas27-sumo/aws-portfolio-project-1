AWS S3 + CloudFront Static Website (Portfolio Project 1)

Overview
A fully deployed static website hosted on Amazon S3 and distributed globally via Amazon CloudFront, using an Origin Access Control (OAC) for security.

AWS Services Used 
- S3 – Static website storage
- CloudFront – Global CDN with HTTPS
- ACM – TLS certificate (if using custom domain)
- IAM – Bucket policy restricted to CloudFront
- AWS CLI – Deployment automation

Key Features
- Custom 404 error page
- AWS managed SecurityHeadersPolicy
- Versioned S3 bucket for rollback
- Cache-optimized deployment (no-cache HTML, long-cache assets)

Deployment Steps
1. Create S3 bucket with static hosting enabled
2. Uploaded 'index html' and '404 HTML' with correct 'ContentType'
3. Create CloudFront distribution with OAC and link to bucket
4. Abiltiy to Attach SecurityHeadersPolicy
5. Invalidate CloudFront cache after updates

Live Demo
[https://d24lku7z6siz5i.cloudfront.net](https://d24lku7z6siz5i.cloudfront.net)

Author
Andrew Kremmidas – AWS Solutions Architect Associate 

![IMG_1625](https://github.com/user-attachments/assets/7864035a-69ca-410e-a202-9ea188d69c78)
![IMG_1628](https://github.com/user-attachments/assets/c999f13c-9794-4c77-ab98-5851bfefc9ad)
![IMG_1629](https://github.com/user-attachments/assets/0a89f1be-140c-4cac-bb0f-c9c724f82f97)
![IMG_1631](https://github.com/user-attachments/assets/c9a8758d-c2b0-461f-97be-f84368a5bca0)
![IMG_1729](https://github.com/user-attachments/assets/4fa5b44c-62cb-4857-a7b1-2109094e9aca)
![IMG_1730 (1)](https://github.com/user-attachments/assets/54648620-24d3-4d00-9c4b-c27208961a1f)





