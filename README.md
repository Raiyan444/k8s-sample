# k8s-sample

K8s sample YAML file and some basic command

 kubectl get pod -o wide
 kubectl scale rc nginx-rc.yml --replicas=5
 kubectl get rc nginx-rc
 kubectl describe rc nginx-rc

>> kubectl get deploy -l app=nginx-app
>> kubectl scale deploy nginx-deploy --replicas=3
>> kubectl describe deploy nginx-deploy

# Update & Rollback
>> kubectl edit deploy nginx-deploy
>> kubectl rollout status deployment/nginx-deploy
>> kubectl get deploy
>> kubectl rollout history deployment/nginx-deploy
>> kubectl rollout undo deployment/nginx-deploy

NOTE: RC and RS are very similar except RC is equality based selector while RS is set based selector
