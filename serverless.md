serverless
EC2 컴퓨팅 자원을 사용해서 구축 - Elastic Beanstalk을 통해서 웹서버를 배포
zappa라는 python 기반의 serverless web hosting 프레임워크 
lambda에 django를 배포해서 이걸 API Gateway와 엮어서
serverless web hosting이 가능하도록 쉽게 배포해주는 서비스


EC2 - Elastic Beanstalk
Lambda - zappa
EB와 Zappa은 단지 이 전체적인 인프라를 DevOps로 관리 - 쉽게 말하자면 복잡하게 terraform을 쓰지 않아도 코드로 인프라 관리가 가능하다는 점

EB는 서버기반
Zappa는 Serverless기반
CloudFormation은 Amazon Web Services(AWS) 리소스를 자동으로 생성해 주는 서비스이다
Zappa는 이 CloudFormation을 매우 간단하게 json 형태로 사용할 수 있게 해주는 역할

profile를 지정하면 지정한 access key를 쓰는거고 아니면 환경 변수에서 해당 값을 찾는다는 것
Code Build에 배포 권한을 가진 IAM Role을 기본적으로 access key를 생성할 수 없다
