# evening_b
## 19july history
```
minikube start
  744  docker ps
  745  docker pull aakashgaur57/myssh
  746  docker history aakashgaur57/myssh:latest 
  747  docker run -itd -e ssh_user=ak1 -e ssh_pass=1234 aakashgaur57/myssh
  748  docker ps
  749  docker inspect stoic_carver 
  750  ssh ak1@172.17.0.3
  751  rm -rf .ssh/known_hosts 
  752  ssh ak1@172.17.0.3
  753  docker exec -it stoic_carver bash
  754  docker run -itd -e SSH_USER=akash -e SSH_PASSWORD=1234 aakashgaur57/myssh
  755  docker ps
  756  docker inspect focused_moser | grep IP
  757  ssh akash@172.17.0.4
  758  docker exec -it focused_moser bash
  759  ssh akash@172.17.0.4
  760  docker ps
  761  minikube status
  762  minikube node delete minikube-m02
  763  minikube status
  764  kubectl version
  765  kubectl version --output=yaml
  766  kubectl version --output=json
  767  kubectl get pod 
  768  kubectl delete deploy mydeploy 
  769  kubectl get pod 
  770  kubectl run akpod --image httpd --port 80 
  771  kubectl get pod
  772  kubectl get pod -o wide
  773  kubectl describe pod akpod
  774  kubectl get pod -o wide
  775  kubectl exec -it akpod bash
  776  kubectl exec -it akpod -- bash
  777  kubectl delete po akpod
  778  kubectl get po
  779  history 
```
```
akash@sky:~$ kubectl run akpod --image httpd --port 80 
pod/akpod created
akash@sky:~$ kubectl get pod
NAME    READY   STATUS    RESTARTS   AGE
akpod   1/1     Running   0          9s
akash@sky:~$ kubectl get pod -o wide
NAME    READY   STATUS    RESTARTS   AGE     IP               NODE       NOMINATED NODE   READINESS GATES
akpod   1/1     Running   0          2m33s   10.244.120.111   minikube   <none>           <none>
akash@sky:~$ kubectl describe pod akpod
Name:             akpod
Namespace:        default
Priority:         0
Service Account:  default
Node:             minikube/192.168.49.2
Start Time:       Wed, 19 Jul 2023 22:29:16 +0530
Labels:           run=akpod
Annotations:      cni.projectcalico.org/containerID: 86f0b8fa0479ee089e92ae8a4d602f4c4c326ded459e943ee4cffa924022d18e
                  cni.projectcalico.org/podIP: 10.244.120.111/32
                  cni.projectcalico.org/podIPs: 10.244.120.111/32
Status:           Running
```
