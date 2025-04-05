# AWS Config Conformance Pack for Well-Architected

This is an MVP for using AWS Config Rules (Managed and Custom) to automatically checks several areas of AWS Well-Architected Framework.

The MVP supports:
- AWS Managed Rules
- Custom, Lambda-backed Rules

## Deployment
- Deploy the aws-wa-rules.yaml to S3
- Update aws-wa-pack.yaml with S3 bucket where the rules are stored (you can do that through CFN Deployemnt using Parameter though)
- Deploy CloudFormation Stack with aws-pack-yaml
![Deployment](https://github.com/MartinGavanda/aws-wa-conformance-pack/blob/main/cfn_deplopyment.png)


## Usage
- Access AWS Config and select aws-wa Conformance Pack
- You will see the detail compliance of individual rules
![Rules](https://github.com/MartinGavanda/aws-wa-conformance-pack/blob/main/rules.png)


## Lambda-backed Rules
- Single Lambda Function si deployed
- Based on the InputParameters -> propertyName value given check is performed