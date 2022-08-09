## CloudFront

Example: 2GB video they want to watch.

If the file is stored in London..
A global view, direct is not efficient.

* Edge Locations - location where content will be cached.
* Origin - S3 Bucket, EC2 Instance, Elastic Load Balancer, Or Route 53
* Distribution - Name given the Content Delivery Network which consists of Edge Locations.

Origin - S3 Bucket is in London.
If Cloud Front is used. Users will be directed to the EdgeLocation and cached, then streamed.

Cloud Front is a reverse proxy caching service.

TTL is usually 48 hours, using a global network of edge locations.

* Web Distribution - Typically used for Website.
* RTMP - Used for Media Streaming

```
https://d2mfr3qla69baf.cloudfront.net/
```

Exam Tips:

- Edge Location - The location where content will be cached. This is seperate to an AWS Region/AZ
- Origin - This is the origin of all the files that the Content Delivery Network will distribute. This can either be an S3 Bucket, an EC2 Instance, an Elastic Load Balancer, or Route53.
- Distribution - This is the name given the CDN which consists of a collection of Edge Locations -
	- Mine: https://d2mfr3qla69baf.cloudfront.net/
- Web Distribution - Typically used for Websites.
- RTMP - Used for Media Streaming

Edge Locations are not just READ only, you can write to them also.
Objects are cached for the life of the TTL
You can clear cached objects