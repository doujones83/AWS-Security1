# Creating and Assuming an IAM Role for Developer Access
## Clean up 
### Detach the PowerUserAccess policy from the role:
```
aws iam detach-role-policy --role-name AWSBoswell \
--policy-arn arn:aws:iam::aws:policy/PowerUserAccess
```

### Delete the IAM role:

`aws iam delete-role --role-name AWSBoswell`

### Unset your local variables:
```
unset ROLE_ARN
unset PRINCIPAL_ARN
```
