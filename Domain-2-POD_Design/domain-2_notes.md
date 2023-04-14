#### To delete Replicaset, you can run the following command:
```sh
kubectl delete -f replicaset.yaml
```

#### Create Deployment using command line
```sh
kubectl create deployment hk-deployment --image=nginx --dry-run=client -o yaml > .\deployment_cli.yaml
```

#### Set Image with record option
```sh
kubectl set image deployment demo-deployment nginx=nginx --record
```

#### Scale Deployment command
```sh
kubectl scale deployment demo-deployment --replicas 10
```

#### Rollout undo
```sh
kubectl rollout undo deployment demo-deployment
```

