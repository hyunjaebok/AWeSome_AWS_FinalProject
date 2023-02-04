## K8s Cluster

### K8S Architecture
![k8s](https://user-images.githubusercontent.com/59479926/209427905-640e1df4-a3f1-4e8f-838d-1ec150d2ea43.png)
>- 각 서비스를 네개의 네임스페이스로 논리적으로 구분하여 그룹핑

</br>

#### CA 시연 영상
![CA](https://user-images.githubusercontent.com/110655823/216240173-76c821e5-6ad3-4797-8d26-b7a280226ece.gif)
> - Stress Test(사용자 접속 트래픽)을 실시했을 때 Node의 CPU 사용량 증가 확인
> - Grafana Dasbord에서 Node의 수가 증가 확인
> - Slack에서 Node CPU 사용량 경고 알림을 확인

#### HPA 시연 영상
![HPA](https://user-images.githubusercontent.com/110655823/216240217-1f1ada85-5c0f-488d-8359-2806268ab3e4.gif)
> - Stress Test(사용자 접속 트래픽)을 실시했을 때, Grafana Dasbord와 ArgoCD에서 Pod의 수가 증가하는 것을 확인

</br>

### 사용한 Stack
- AWS EKS

</br>

---

### [👈 Go back](https://github.com/hyunjaebok/AWeSome_AWS_FinalProject)
