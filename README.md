# BB visual Demo

Runs tests on Best Buy Site.

Cross Browser

mvn dependency:resolve    
mvn test-compile

Run all tests with: mvn test

### Run via Saucectl in [Sauce Orchestrate](https://docs.saucelabs.com/orchestrate/)

```shell
docker login
docker build --no-cache -t leyfr01/so-demo-java:0.0.3 . --platform linux/amd64
docker push leyfr01/so-demo-java:0.0.3
export SAUCE_REGION="us-west-1"
saucectl run
```