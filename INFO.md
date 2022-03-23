## Info

Coorg.ai is a simple solution based on the AWS content analysis service. 

It includes a basic frontend where users can login and analyze media assets.

## Technologies

Coorg.ai uses a SPA architecture, and its frontend includes a VueJS app. The backend mostly uses AWS ML services.

For deployment, Coorg.ai, uses AWS Amplify. It is currently setup for simple a deployment, consisting of one environment (production).


## Deployment

If you would like to develop or configure Coorg.ai stack please follow sections below.

## Requirements

Please ensure you have the following tools installed:

```
Node>=14
AWS CLI v2
```

### Config

Coorg.ai can easily be deployed to public cloud vendors, such as AWS, etc... We have created a set of IaC scripts for deployment, so you can quickly get started.

To deploy a new Coorg.ai build, please refer to INSTALLATION section in README file.

### IaC code -- deploy CF templates

If you want to build a new release for CF, you will need to create a new CF build. This updated build will need to be uploaded to S3 so you can use it for future deployments.

To create new CF templates, please run the following script:
./deployment/build-s3-dist.sh --template-bucket coorg-templates --code-bucket coorg-code --version {version} --region {region}

If this runs successfully you should get output, including new CF template links, which you can use for future deployments.

## Making changes -- updating app code

If you would like to deploy changes, please refer to the following steps:

To redeploy the app:

1. Navigate to website directory. For example:
```
cd /path/to/project/website
```
2. Run deploy command
```
npm run deploy
```

## Questions

Please contact Coorg.ai team for any queries.