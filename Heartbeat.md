### Heartbeat
> Heartbeat는 한 시스템이 다른 시스템에게 "나는 살아있다"는 것을 알리는 신호
* Heartbeat는 시스템이 온라인 상태이고 메시지를 받을 수 있는지 확인하는 데 사용
* 만약 Heartbeat 메시지가 도달하지 않는다면, 해당 시스템이 다운되었거나 네트워크에 문제가 발생했을 가능성이 있다고 눈치챌 수 있다
* Heartbeat 사용 예시
	1. 웹 서비스 모니터링 도구
	2. 분산 데이터베이스 시스템에서는 종종 마스터 노드가 여러 개의 슬레이브 노드와 통신하며, 이들 간의 동기화를 유지. 슬레이브 노드가 heartbeat에 응답하지 않는다면, 마스터 노드는 해당 노드에 문제가 있을 수 있음을 감지하고, 필요한 조치를 필요.

* Beats + ELK
* Beats 로그 에이전트에서 최초로 로그를 생성합니다. 직접 Elasticsearch로 전달 할 수도 있고 Logstash(실시간으로 수집된 데이터를 확인할 수 있게 해주는 파이프 라인 도구)로 전달 할 수도 있습니다. 그 외에도 Kafka, Redis, File, Console, Cloud 등으로 전달 할 수 있습니다.
* Beats는 명확한 목적에 따라 나누어져 나누어져 있습니다. Filebeat, Metricbeat, Packetbeat, Winlogbeat, Auditbeat, Heartbeat 등이 있습니다. 
* Heartbeat 활용하여 모니터링 하기
	* Heartbeat는 네트워크 health 체크를 위한 모듈입니다.
	* Heartbeat 설정을 통해 다음 openbase 홈페이지, secuwave 홈페이지, support.redmine을 모니터링할 수 있습니다. Heartbeat는 url 을 모니터링하고 모니터링 데이터는 elasticsearch로 전달합니다. Elasticsearch에 저장된 데이터는 Kibana를 통해 모니터링할 수 있습니다.
