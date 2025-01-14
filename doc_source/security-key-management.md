# Key management<a name="security-key-management"></a>

You can protect your content from unauthorized use through encryption\. Store your encryption keys in AWS Secrets Manager, and then give the CodeBuild service role associated with the build project permission to obtain the encryption keys from your Secrets Manager account\. For more information, see [Create and configure a customer managed key for CodeBuild](setting-up.md#setting-up-kms), [Create a build project in AWS CodeBuild](create-project.md), [Run a build in AWS CodeBuild](run-build.md), and [Tutorial: Storing and retrieving a secret](https://docs.aws.amazon.com/secretsmanager/latest/userguide/tutorials_basic.html)\. 

Use the `CODEBUILD_KMS_KEY_ID` environment variable in a build command to obtain the AWS KMS key identifier\. For more information, see [Environment variables in build environments](build-env-ref-env-vars.md)\. 

You can use Secrets Manager to protect credentials to a private registry that stores a Docker image used for your runtime environment\. For more information, see [ Private registry with AWS Secrets Manager sample for CodeBuild](sample-private-registry.md)\. 