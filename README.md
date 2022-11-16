# terraform-aws-hands-on

## introduce git-secrets

1. introduce git-secrets and settings for aws

```bash
git secrets --install
git secrets --register-aws
```

2. check for reject secrets commit

```bash
touch credentials
echo "aws_secret_access_key = ABcDe1F2hIjkl3nop45sTUv6XYz7aBcDEFghIJKL" > credentials
git add .
git commit -m "test for commit reject"
```

display of `[ERROR] Matched one or more prohibited patterns`
