## 비용 절감

### Open Source IDE Tool과 Cloud 9 비교
![image](https://user-images.githubusercontent.com/110655823/215355622-a418fde3-5d12-4efd-a355-98547d0a90d9.png)
> - Terraform 개발 환경을 VSCode 사용하여 추가 비용 발생하지 않음
> - Cloud9는 컴퓨팅 리소스 추가 비용 발생

</br>

###  Open Source CI/CD Tool과 Code series 비교
![image](https://user-images.githubusercontent.com/110655823/215355543-dad8b940-c2a8-46d1-9492-51c56b06ca4a.png)
> - Jenkins는 공식 권장 스펙에 따라 t3.medium을, argocd는 worker Node에 올라가므로, worker node의 스펙인 t3.medium을 사용
> - AWS Code Series는 Build 200번과 Pipeline 6개의 기준으로 비용 산정

</br>

### Open Source Monitoring Tool과 Cloud Watch & SNS 비교
![image](https://user-images.githubusercontent.com/110655823/215355564-14a5d1f9-81c5-4961-a6e5-32040d435528.png)
> - 모니터링 오픈소스도 worker node에 올라가므로 worker node의 스펙인 t3.medium을 사용
> - AWS CloudWatch와 SNS는 3일간 쌓인 매트릭과 로그의 기준으로 비용 산정

</br>

### 결과
![웹 캡처_30-1-2023_6139_s3 us-west-2 amazonaws com](https://user-images.githubusercontent.com/110655823/215355476-7a18775c-93e2-48cf-951c-1a153535ff69.jpeg)
> - AWS Service보다 Open Source를 사용하여, 최소 48.1%의 비용 절감

</br>

---

### [👈 Go back](https://github.com/hyunjaebok/AWeSome_AWS_FinalProject)
