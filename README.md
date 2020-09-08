 ## How to run?

### Setup

Create a staging profile with saml. With something like

 ```
saml2aws login --profile staging
 ```

Setup up ruby version and required gems:

```
rbenv install
bundle install

REGION=us-east-1 PROFILE=staging AWS_CA_ARN=arn:aws:acm-pca:us-east-1:589470546847:certificate-authority/c265f0ba-3378-421b-adff-93c3e51cd3fc ./bin/generate_cert

```

