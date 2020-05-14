### Cleanup

In order to delete the resources created during this workshop, run the commands below:   

```
kubectl delete --all deployments --namespace=default
kubectl delete --all deployments --namespace=nginx-ingress
kubectl delete --all svc --namespace=default
kubectl delete --all svc --namespace=nginx-ingress
cd terraform
terraform destroy --auto-approve
```
  
  
Finally, delete the `NGINX-EKS` stack in the [CloudFormation console](https://eu-central-1.console.aws.amazon.com/cloudformation/home?region=eu-central-1#/).

:warning: Please note: it will also delete the Cloud9 instance.


### Feedback