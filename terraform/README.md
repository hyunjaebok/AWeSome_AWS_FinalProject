## AWS EKS 클러스터 환경 아키텍처

### Infra Architecture
![infra](https://user-images.githubusercontent.com/59479926/209446219-9dcb1431-9f97-4e99-9b45-03094872e6da.jpg)
> - 관리자는 bastion을 통해 k8s mgnt로 접속하여 EKS를 관리, route53에 등록된 DNS를 통해 CI/CD와 monitoring 서버 관리
> - 고객은 route53에 등록된 도메인을 통해 웹 서비스 이용
> - AWS Infra를 Terraform으로 구축

</br>

#### CA 시연 영상
![CA](https://user-images.githubusercontent.com/110655823/216240173-76c821e5-6ad3-4797-8d26-b7a280226ece.gif)

#### HPA 시연 영상
![HPA](https://user-images.githubusercontent.com/110655823/216240217-1f1ada85-5c0f-488d-8359-2806268ab3e4.gif)


### 사용한 Stack
- AWS Serivce -> IAM, VPC, EC2, RDS, ALB, AS, S3, EKS, ECR, ACM, Route53
- IaC -> Terrafrom

</br>

---

### [👈 Go back](https://github.com/hyunjaebok/AWeSome_AWS_FinalProject)
