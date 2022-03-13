## Info

Coorg.ai is a simple solution based on the AWS content analysis service. 

## Config

Coorg.ai can easily be deployed to public cloud vendors, such as AWS, etc... We have created a set of IaC scripts for deployment, so you can quickly get started.

To deploy a new Coorg.ai build, please refer to INSTALLATION section in README file.

## Development

If you want to build a new release for CF, you will need to create a new CF build. This updated build will need to be uploaded to S3 so you can use it for future deployments.

To create new CF templates, please run the following script:
./deployment/build-s3-dist.sh --template-bucket coorg-templates --code-bucket coorg-code --version {version} --region {region}

If this runs successfully you should get output, including new CF template links, which you can use for future deployments.

## Questions

Please contact Coorg.ai team for any queries.