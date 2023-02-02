# CI/CD

### CI/CD Architecture
![cicd](https://user-images.githubusercontent.com/59479926/209446164-5d67698c-6fe6-4c94-8f7f-011d25a8c715.jpg)
> - 관리자가 소스 코드를 작성 후 Git 저장소에 commit →  CI tool인 Jenkins를 통해 빌드 작업 실행.
> - 빌드된 컨테이너 이미지를 ECR에 업로드 → Git에 저장된 매니페스트의 이미지 태그 부분을 업데이트하고, Git 저장소에 commit 후 작업이 종료
> - Jenkins Pipeline의 스테이지마다 성공, 실패 여부는 slack을 통해 알림
> - Argocd가 ECR에 업로드된 컨테이너 이미지와 매니페스트에 저장되어 있는 Git 저장소를 참조하여 EKS에 서비스 배포

</br>


</br>

#### Blue-Green 시연 영상
![Blue-Green](https://user-images.githubusercontent.com/110655823/216240624-8f7593a0-d127-460f-89b0-d2a7369935c9.gif)

</br>

### 사용한 Stack
- CI -> Jenkins
- CD -> ArgoCD
- Alert -> Slack
- Container Repo -> Amazon ECR

---

### [👈 Go back](https://github.com/hyunjaebok/AWeSome_AWS_FinalProject)
