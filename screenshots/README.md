# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
![](./img/Screenshot-of-DockerHub-shows-the-images.png)
![](./img/DockerHub%20showing%20containers%20that%20you%20have%20pushed.png)
* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)

* Travis CI showing a successful build and deploy job
![](./img/Travis-CI-showing-a-successful-build%20job.png)

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![](./img/kubectl-get-pods.png)
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![](./img/kubectl-describe-services.png)
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![](./img/kubectl%20describe%20hpa.png)
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![](./img/kubectl-logs-frontend.png)
![](./img/kubectl-logs-reverseproxy.png)
