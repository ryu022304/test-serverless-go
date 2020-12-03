# Test serverless with go
## Diagram
![test-serverless-diagram](https://user-images.githubusercontent.com/33801040/101046025-0fceb800-35c4-11eb-8245-bdcddb3a14fd.png)

## Usage
```bash
# Install Serverless Framework and plugin
$ npm install -g serverless
$ sls plugin install -n serverless-apigateway-service-proxy

# Build
$ GOOS=linux go build -o bin/sqs sqs/main.go

# Deploy
$ sls deploy -v

# Remove Resources
$ sls remove -v
```
