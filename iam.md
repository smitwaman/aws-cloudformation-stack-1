
### IAM Role Template (IAMRole.yaml):
```yaml
AWSTemplateFormatVersion: '2010-09-09'
Description: "IAM Role with Full Access"

Resources:
  JenkinsIAMRole:
    Type: 'AWS::IAM::Role'
    Properties:
      RoleName: JenkinsIAMRole
      AssumeRolePolicyDocument:
        Version: '2012-10-17'
        Statement:
          - Effect: 'Allow'
            Principal:
              Service: 'ec2.amazonaws.com'
            Action: 'sts:AssumeRole'
      Policies:
        - PolicyName: FullAccessPolicy
          PolicyDocument:
            Version: '2012-10-17'
            Statement:
              - Effect: 'Allow'
                Action: '*'
                Resource: '*'
```

