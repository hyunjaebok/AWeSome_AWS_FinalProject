## Mornitoring
### Monitoring Architecture
![mornitoring](https://user-images.githubusercontent.com/59479926/209446258-ddf8b294-4219-429e-b59f-fed45788d4c4.jpg)
>- 리소스 모니터링은 Node-Exporter로 메트릭 정보를 수집 → Prometheus TSDB로 전달 → Grafana를 통해 수집된 매트릭을 시각화
>- Grafana에서 node의 CPU와 메모리 사용률이 일정 수치가 넘으면 slack을 통해 알림
>- 애플리케이션 모니터링은 fluentd로 로그를 수집 → elasticsearch로 데이터를 보관하고 실시간으로 저장 → kibana를 통해 수집된 로그를 시각화

</br>

### Grafana Dasbord
![grafana](https://user-images.githubusercontent.com/59479926/209428192-f7a6ba1b-2b99-4fb5-a2f8-6cecd68c5f23.png)
> - Node의 수, CPU, Memory Monitoring
> - Pod의 수, CPU, Memory Monitoring

### Kibana Dashboard
![Kibana](https://user-images.githubusercontent.com/59479926/209428055-8ede0586-3f9d-45d2-8e6a-75202447b8b5.png)
> - Frontend의 총 Log 수, HTTP 상태 코드 종류별 수 시각화
> - Backend의 총 Log 수, HTTP 상태 코드 종류별 수 시각화
> - HTTP 프로토콜의 Method별 수
> - api 종류별 수

</br>

### 사용한 Stack
- Resources Monitoring -> nodeExporter, Prometheus, Grafana
- Applications Monitoring -> ElasticSearch, Fluentd, Kibana
- Alert -> Slack

</br>

---

### [👈 Go back](https://github.com/hyunjaebok/AWeSome_AWS_FinalProject)
