
Explanation of the Infrastructure diagram:

All the static files would be present in s3 bucket

Cloudfront would act as CDN and serve the contents of the s3 bucket using https

Certificate Manager will provide the SSL certificates to Cloudfront and manages (renews in expiration) for us

Route53 manages all our DNS records and sets A record to point to Cloudfront distribution

Domain Registrars will point the domain name to AWS Nameservers
