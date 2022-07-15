## Prereq: we have lambda + api gateway
- run terraform
- show lambda
- show api gateway
- show route53 hosted zone
- invoke it with default url




## issue a certificate using console (without Route53)

- request cert for api.devopsbyexample.io
- create CNAME record to validate cert
- check if the cert is valid

## Create custom domain using console (Route53)

- create custom domain in api gateway for api.devopsbyexample.io
- create CNAME for api gateway
- create api mapping for root and v1
- curl https://api.devopsbyexample.io/hello
- curl https://api.devopsbyexample.io/v1/hello

- delete all of the above



## issue a certificate using console (Route53)
- request cert for api.antonputra.com
- create route53 records
- check if the record was created in route53
- check if the cert is valid


## Create custom domain using console (Route53)
- create custom domain in api gateway for api.antonputra.com
- create alias for api gateway
- create api mapping for root and v1
- curl https://api.antonputra.com/hello
- curl https://api.antonputra.com/v1/hello





## issue a certificate using terraform (Route53)

- create 5-certificate.tf


## Create custom doamin using terraform (Route53)
- create 6-custom-domain-name.tf
- create 7-api-mapping.tf
- terraform apply
- curl https://api.antonputra.com/hello
- curl https://api.antonputra.com/v1/hello