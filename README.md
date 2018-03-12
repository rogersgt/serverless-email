# Serverless SES
### Tests
Use `yarn test` to invoke mochai/chai tests. Create a `.env` for tests with the following:
* FROM_EMAIL='some email address'
* TO_EMAIL='some email address'
* AWS_REGION='some region like us-east-1'
* AWS_ACCESS_KEY_ID='your access key'
* AWS_SECRET_ACCESS_KEY='your secret key'

### Configure
Replace `profile` in `serverless.yml` with the appropriate aws-cli profile located in `~/.aws/credentials`.
Also replace the `vpc` section with the appropriate values for your AWS VPC.

### Deploy
Create a `env.json` file with at least the following:
* FROM_EMAIL: 'some email address'
* TO_EMAIL: 'some email address'
* NODE_ENV: 'node environment'

Use `yarn deploy:dev` or `yarn deploy:prod`.
