AWS Portfolio Project #1 - Andrew Kremmidas - AWS Solutions Architect Associate - 2026

S3 + CloudFront Secure Static Website (OAC + HTTPS)
What Problem Does This Solve?
Securely serve static website content with global low-latency delivery without exposing S3 directly to the public internet.

# Architecture Overview
Global content delivery via CloudFront with restricted access to an S3 origin.

User → CloudFront (HTTPS + CDN) → S3 (private origin via OAC)
S3 bucket is not publicly accessible — only CloudFront can read objects.

AWS Services Used
Service	Purpose
Amazon S3	Private origin for static assets
Amazon CloudFront	Global CDN + HTTPS
Origin Access Control (OAC)	Restrict S3 access to CloudFront only
AWS CLI	Deployment automation
(Optional) AWS ACM	Custom HTTPS domain support
Security Features
* OAC enforced — S3 bucket blocks all public access
* HTTPS required
* CloudFront managed SecurityHeadersPolicy
* Versioning enabled for rollback protection (optional but recommended)

Deployment Steps (ADVANCED)
1. Create private S3 bucket (block all public access)
2. Upload index.html & 404.html
3. Create CloudFront distribution using OAC
4. Apply SecurityHeadersPolicy
5. Invalidate CloudFront cache after updates

Deployment Proof
Step	Screenshot
OAC enabled	
CloudFront deployed	
Bucket blocks public access	
Cache invalidation	
(Screenshots will be added later — placeholders included.)

Live Demo
https://d24lku7z6siz5i.cloudfront.net/
(Available via CloudFront domain — custom domain optional)

## Author  
Andrew Kremmidas |
 AWS Certified Solutions Architect – Associate


![IMG_1625](https://github.com/user-attachments/assets/7864035a-69ca-410e-a202-9ea188d69c78)
![IMG_1628](https://github.com/user-attachments/assets/c999f13c-9794-4c77-ab98-5851bfefc9ad)
![IMG_1629](https://github.com/user-attachments/assets/0a89f1be-140c-4cac-bb0f-c9c724f82f97)
![IMG_1631](https://github.com/user-attachments/assets/c9a8758d-c2b0-461f-97be-f84368a5bca0)
![IMG_1729](https://github.com/user-attachments/assets/4fa5b44c-62cb-4857-a7b1-2109094e9aca)
![IMG_1730 (1)](https://github.com/user-attachments/assets/54648620-24d3-4d00-9c4b-c27208961a1f)





