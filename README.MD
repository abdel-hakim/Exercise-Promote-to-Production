1- CREATE S3 BUCKET NAME IT "buck-prod"AND MAKE IT PUBLIC
2- RUN THIS COMMAND MANUALLY :
`aws cloudformation deploy \
--template-file cloudfront.yml \
--stack-name production-distro \
--parameter-overrides PipelineID="${buck-prod}" \ # Name of the S3 bucket you created manually.
--tags project=udapeopl
`
