# automa-jenkins
microk8s config for jenkins

see: [How to Setup Jenkins Build Agents on Kubernetes Pods](https://devopscube.com/jenkins-build-agents-kubernetes/)

```bash
:~/projects$ microk8s kubectl get pods --field-selector=status.phase=Running -n=devops-tools
NAME                                  READY   STATUS    RESTARTS   AGE
jenkins-deployment-86984d68b8-nfx4h   1/1     Running   0          107m
:~/projects$ microk8s kubectl logs jenkins-deployment-86984d68b8-nfx4h -n=devops-tools
Running from: /usr/share/jenkins/jenkins.war
```
