### Bounded Context : DDD
* DDD와 클린 아키텍처에서는 UseCase와 Entity 레이어를 작성할 때, Entity 레이어의 “비즈니스 객체”에 최대한 많은 비즈니스 룰을 담아, 응집성을 높이고 중복을 줄이는 코드를 작성을 권고
* Bounded Context는 “같은 도메인이어도, 사용되는 맥락이 다르면 엔티티를 별도로 매핑하라”라는 원칙
* CQRS는 Command and Query Responsibility Segregation, 즉 “명령과 조회의 책임 분리”
* CQRS는 정보를 업데이트 할때와 조회할 때 다른 모델을 사용

* DDD 도메인에 대해서 "탐험의 시간" 이벤트 스토밍 - https://miro.com/ko/
