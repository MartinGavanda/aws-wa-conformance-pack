# AWS Config Conformance Pack for Well-Architected

This is an MVP for using AWS Config Rules (Managed and Custom) to automatically checks several areas of AWS Well-Architected Framework.

The MVP supports:
- AWS Managed Rules
- Custom, Lambda-backed Rules

![Overview](https://github.com/MartinGavanda/aws-wa-conformance-pack/blob/main/overview.png)

## Lambda-backed Rules
- Single Lambda Function si deployed
- Based on the InputParameters -> propertyName value given check is performed