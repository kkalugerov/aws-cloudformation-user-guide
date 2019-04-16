# AWS CodeBuild Project RegistryCredential<a name="aws-properties-codebuild-project-registrycredential"></a>

`RegistryCredential` is a property of the [AWS::CodeBuild::Project](aws-resource-codebuild-project.md) resource that specifies information about credentials that provide access to a private Docker registry\. When this is set:
+  `imagePullCredentialsType` must be set to `SERVICE_ROLE`\. 
+  images cannot be curated or an Amazon ECR image\. 

## Syntax<a name="aws-properties-codebuild-project-registrycredential-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-codebuild-project-registrycredential-syntax.json"></a>

```
{
  "[Credential](#cfn-codebuild-project-registrycredential-credential)" : String,
  "[CredentialProvider](#cfn-codebuild-project-registrycredential-credentialprovider)" : String
}
```

### YAML<a name="aws-properties-codebuild-project-registrycredential-syntax.yaml"></a>

```
[Credential](#cfn-codebuild-project-registrycredential-credential): String
[CredentialProvider](#cfn-codebuild-project-registrycredential-credentialprovider): String
```

## Properties<a name="aws-properties-codebuild-project-registrycredential-properties"></a>

`Credential`  <a name="cfn-codebuild-project-registrycredential-credential"></a>
 The Amazon Resource Name \(ARN\) or name of credentials created using AWS Secrets Manager\.   
 The `credential` can use the name of the credentials only if they exist in your current region\. 
 *Required*: Yes  
 *Type*: *String*   
 *Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt) 

`CredentialProvider`  <a name="cfn-codebuild-project-registrycredential-credentialprovider"></a>
 The service that created the credentials to access a private Docker registry\. The one valid value, SECRETS\_MANAGER, is for AWS Secrets Manager\.   
 *Required*: Yes  
 *Type*: *String*   
 *Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt) 

## See Also<a name="aws-properties-codebuild-project-registrycredential-seealso"></a>
+ [ RegistryCredential](https://docs.aws.amazon.com/codebuild/latest/APIReference/API_RegistryCredential.html) in the *AWS CodeBuild API Reference*