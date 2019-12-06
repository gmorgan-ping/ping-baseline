# Kubernetes - Full Stack

## Deploy All Services

To deploy all included services, deploy from the root of this repo
```kubectl apply -R -f kubernetes```

## Product Login

### PingFederate Admin Console

* Go to: [https://<service_external_ip>:9999/pingfederate/app](https://<service_external_ip>:9999/pingfederate/app)
* Credentials
  * Username: administrator
  * Password: 2FederateMore

### PingFederate OAuth Playground

* Go to [https://<service_external_ip>:9031/OAuthPlayground](https://l<service_external_ip>:9031/OAuthPlayground)
* Click on `implicit` link
* Click on `Submit` button
* Log in with `user.0 / 2FederateM0re`

### PingAccess Admin Console

* [https://<service_external_ip>:9000](https://<service_external_ip>:9000)
* Credentials
  * Username: administrator
  * Password: 2FederateMore

### PingDirectory Management Console

* Go to [https://<service_external_ip>:8443/console](https://<service_external_ip>:8443/console)
* Credentials
  * server: pingdirectory
  * user: Administrator
  * password: 2FederateM0re

## Clean Up Deployments

```kubectl delete -R -f kubernetes```
