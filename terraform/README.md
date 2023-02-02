## AWS EKS 클러스터 환경 아키텍처

### Infra Architecture
![infra](https://user-images.githubusercontent.com/59479926/209446219-9dcb1431-9f97-4e99-9b45-03094872e6da.jpg)
> - 관리자는 bastion을 통해 k8s mgnt로 접속하여 EKS를 관리, route53에 등록된 DNS를 통해 CI/CD와 monitoring 서버 관리
> - 고객은 route53에 등록된 도메인을 통해 웹 서비스 이용
> - AWS Infra를 Terraform으로 구축
> - RDS 이중화 구성

</br>

### 사용한 Stack
- AWS Serivce -> IAM, VPC, EC2, RDS, ALB, AS, S3, EKS, ECR, ACM, Route53
- IaC -> Terrafrom

</br>

---

### [👈 Go back](https://github.com/hyunjaebok/AWeSome_AWS_FinalProject)
