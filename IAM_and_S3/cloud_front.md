# Cloud Front

## Overview
- **Edge Location**: this is location where content is cache. This is separate to an Region/AZ  
- **Origin**: This is the origin of all the files that the CND will distribute. This can be S3,
EC2 Instance, Route53, Elastic Load Balancer  
- **Distribution**: The name given the CDN which consists of a collection of Edge Location    
- Edge Location are not just READ only - can write to them too  
- Object are cached for the life of the TTL (Time to life)  
- Can **invalidate cache objs**. But you will be charged

## Cloud Front Lab
We have 2 methods for my content
- Web Distribution: Typically used for website
- RTMP: Used for Media Streaming

## Cloud Front Signed URLs and Cookies
- Use signed URLs/cookies when want to secure content (like Netflix, FPT play...)
- A signed URL is for 1 file
- A signed cookie for multiple file, but limit time to access
- If your origin is EC2, then use CloudFront
