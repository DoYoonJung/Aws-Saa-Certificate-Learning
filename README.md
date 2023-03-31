# Aws-Saa-Certificate-Learning


## AWS Step Functions 

분산 애플리케이션과 마이크로 서비스의 구성요소를 손쉽게 조정, 애플리케이션을 빠르고 쉽게 확장 및 변경 가능

기능 및 이점

1.	애플리케이션 구성요소 배열 및 시각화 할 수 있는 그래프 콘솔 제공
2.	자동으로 각 단계 추적하여 오류 발생시 재도전을 통해 애플리케이션 정상화
3.	단계의 상태 기록으로 빠르게 문제 디버깅
4.	코드 작성 없이 단계를 변경 및 추가 가능, 간편하게 애플리케이션 개선
 
 
 
## AWS X-Ray

개발자가 프로덕션 분산 애플리케이션(예: 마이크로 서비스 아키텍처를 사용해 구축된 애플리케이션)을 분석하고 디버깅하는 데 도움을 주는 서비스

요청이 애플리케이션을 통과함에 따라 요청에 대한 엔드 투 엔드 뷰를 제공하고 애플리케이션의 기본 구성 요소를 맵으로 보여준다. 



## Amazon S3 Transfer Acceleration

클라이언트와 S3 버킷 간의 장거리에서 파일을 빠르고 쉽고 안전하게 전송할 수 있는 버킷 수준 기능이다.

Amazon CloudFront의 전 세계적으로 분산되어 있는 엣지 로케이션을 활용한다. 데이터가 엣지 로케이션에 도착하면 데이터는 최적화 네트워크 경로를 통해 Amazon S3으로 라우팅 된다.



## Amazon S3 조건 키

 
## Amazon Kinesis Data Streams

특수 요구에 맞춰 스트리밍 데이터를 처리 또는 분석, 다양한 유형의 데이터를 kinesis 데이터 스트림에 추가하고 몇초안에 해당 데이터를 읽고 처리 가능

***자동으로 수행하는 관리작업***

배포 혹은 지속적인 유지 관리 작업, 높은 가용성과 데이터 내구성 제공, 용량을 자동으로 조정

***Amazon Kinesis Data Streams의 성능향상***

→ 샤드를 늘린다.

## Amazon Kinesis Data Firehose

kinesis data streams가 데이터를 실시간으로 캡쳐 및 수집한다면 firehose는 해당 데이터를 분석 서비스롤 이동 및 모니터링 한다. 
 
## Amazon SQS keyword  -> 분리 , 분산 (decoupling)

메시지 대기열 기능, 유지 관리 자동화, 메시지 비 동기적 전송 및 검색 가능
 
## FIFO 대기열 keyword  -> 특정 순서


## Amazon SQS 지연 대기열

몇 초 동안 소비자에게 새 메시지 전달을 연기할 수 있다. 지연 대기열은 가시성 제한 시간 과 유사하다 . 두 기능 모두 특정 기간 동안 소비자가 메시지를 사용할 수 없도록 하기 때문이다. 

차이점으로는 지연 대기열의 경우에 메시지가 대기열에 처음 추가될 때 메시지가 숨겨지는 반면 가시성 제한 시간의 경우 메시지가 대기열에서 소비된 후에만 숨겨진다는 것이다 .

## Amazon SQS 가시성 제한 시간  - > Keyword  메세지 중복 방지 , 메세지 한번만 처리

## Amazon Redshift Spectrum

데이터 로딩이나 ETL 없이도 Amazon S3의 데이터 레이크에 대해 쿼리를 실행할 수 있게 해주는 Amazon Redshift의 기능.

SQL 쿼리를 발행하면, 쿼리가 Amazon Redshift 엔드포인트로 전달되고 여기에서 쿼리 플랜을 생성하고 최적화한다. Amazon Redshift는 로컬에 있는 데이터와 Amazon S3에 있는 데이터가 무엇인지 파악하고, 읽어와야 하는 S3 데이터 양을 최소화하기 위한 플랜을 생성하고, 공유 리소스 풀의 Amazon Redshift Spectrum 작업자에게 S3에서 데이터를 읽고 처리하도록 요청한다.

## Amazon EventBridge(Amazon CloudWatch Events)

다양한 소스의 데이터와 애플리케이션을 쉽게 연결할 수 있는 서버리스 이벤트 버스 서비스이다. 

EventBridge 는 자체 애플리케이션, SaaS(Software-as-a-Service) 애플리케이션 및 AWS 서비스의 실시간 데이터 스트림을 제공한 다음, 
해당 데이터를 AWS Lambda 등의 대상으로 라우팅한다. 데이터를 전송할 대상을 결정하는 라우팅 규칙을 설정하여 모든 데이터 원본에 실시간으로 대응하는 애플리케이션 아키텍처를 구축할 수 있다. EventBridge를 사용하면 느슨하게 결합되고 분산된 이벤트 중심 아키텍처를 구축할 수 있다.

## AWS CloudTrail - > keyword API호출 

사용자 활동 및 API 사용을 추적하여 감사, 보안 모니터링 및 운영 문제 해결을 지원한다.

## AWS Batch

배치 관리,작업 도움 기능 세트이다. 제출된 배치 작업의 볼륨 및 특정 리소스 요구 사항에 따라 최적의 수량 및 컴퓨팅 리소스의 유형(예: CPU 또는 메모리 최적화 컴퓨터 리소스)을 동적으로 프로비저닝한다. 

작업 실행을 위한 배치 컴퓨팅 소프트웨어나 서버 클러스터를 설치하여 관리할 필요가 없으므로 결과 분석과 문제 해결에 집중할 수 있다. -> 배치 작업 볼륨, 오구사항에 따라 자원을 최적의 상태로 프로비저닝 한다. 따로 관리할 필요는 없다.

## Amazon QuickSight

신속한 데이터 시각화 도구이다. 사용량에 대해서만 요금을 지불하면 된다.
개별 Amazon QuickSight 사용자 및 그룹에게 Amazon QuickSight의 대시보드에 대한 액세스 권한 부여 방법

## Amazon SWF

분산 애플리케이션 구성 요소에서 작업을 쉽게 조정할 수 있도록 해주는 웹 서비스. 
Amazon SWF를 사용하면 진행 상황 추적 및 상태 유지와 같은 근본적인 복잡성에 대한 걱정 없이 작업 구현 및 조정을 완벽하게 제어할 수 있다. 

## S3 Select

SQL을 통해 애플리케이션이 객체에서 일부 데이터만 가져올 수 있도록 하는 서비스. 
상당한 비용절감과 성능향상 

## Amazon EKS (Amazon Elastic Kubernetes Service)

자체 Kubernetes 컨트롤 플레인 또는 노드를 설치, 운영 및 유지 관리할 필요 없이 AWS의 Kubernetes 실행에 사용할 수 있는 관리형 서비스. Kubernetes는 컨테이너화된 애플리케이션의 배포, 확장, 관리를 자동화하기 위한 오픈 소스 시스템.

•	고가용성을 보장하기 위해 여러 AWS 가용 영역에서 Kubernetes 제어 플레인을 실행하고 확장한다.

•	로드를 기반으로 컨트롤 플레인 인스턴스를 자동으로 확장하고 비정상 컨트롤 플레인 인스턴스를 감지 및 교체하며 자동화된 버전 업데이트 및 패치를 제공한다.

## Elastic Fabric Adapter(EFA)

Amazon EC2 인스턴스에 연결하여 고성능 컴퓨팅(HPC) 및 기계 학습 애플리케이션의 속도를 높일 수 있는 네트워크 디바이스입니다. EFA를 사용하면 AWS 클라우드가 제공하는 확장성, 유연성 및 탄력성으로 온프레미스 HPC 클러스터의 애플리케이션 성능을 달성할 수 있습니다. 

## EC2 배치그룹

조건키에는 클러스터, 파티션, 분산이 있다.
 
클러스터의 경우, 네트워크 지연 속도가 짧고 네트워크 처리량이 높은 경우와 대부분의 네트워크 트래픽이 그룹내 인스턴스간 전송될 때 사용한다.
 
파티션은 하드웨어의 장애를 줄일 수 있다.
 
분산은 소규모 인스턴스 그룹을 다른 하드웨어에 분산하여 상호 관련 오류를 줄일 수 있다.

## 인스턴스 메타데이터

호스트 이름, 이벤트 및 보안 그룹과 같은 범주로 분류, 인스턴스를 시작할 때 지정한 사용자 데이터에도 액세스할 수 있다. 

## AWS 네트워크 방화벽(AWS Network Firewall)

모든 Amazon Virtual Private Cloud(VPC)에 대한 필수 네트워크 보호 기능을 쉽게 배포할 수 있게 해주는 관리형 서비스.

네트워크 트래픽에 따라 자동으로 확장되므로 인프라 배포 및 관리 가능. 네트워크 방화벽의 유연한 규칙 엔진을 사용하면 아웃바운드 서버 메시지 블록(SMB) 요청을 차단하여 악의적인 활동의 확산을 방지하는 등 네트워크 트래픽을 세밀하게 제어할 수 있는 방화벽 규칙을 정의할 수 있다. AWS Network Firewall은 AWS Firewall Manager와 함께 작동하므로 중앙에서 보안 정책을 관리하고 기존 및 새로 생성된 계정과 VPC에 필수 보안 정책을 자동으로 적용할 수 있다. 


## AWS Firewall Manager

AWS Organization의 여러 계정과 애플리케이션에서 방화벽 규칙을 중앙에서 구성 및 관리할 수 있는 보안 관리 서비스. Firewall Manager를 사용하는 경우, 새로운 애플리케이션이 생성될 때 새로운 애플리케이션 및 리소스가 공통 보안 규칙 세트를 손쉽게 준수하도록 할 수 있다. 

Firewall Manager를 활용하여 중앙에서 조직의 여러 VPC에 AWS Network Firewall에 대한 규칙을 배포함으로써 네트워크의 들어오고 나가는 트래픽을 제어할 수 있다. 동시에 방화벽 관리자를 사용하여 계정 전체의 VPC를 Route 53 Resolver DNS Firewall 규칙과 연결하여 알려진 악의적인 도메인에 대해 만들어진 DNS 쿼리를 차단하고 신뢰할 수 있는 도메인에 대한 쿼리를 허용할 수도 있다.

## Amazon GuardDuty

GuardDuty는 보안 소프트웨어 또는 에이전트를 사용하지 않고 데이터에서 악의적 활동을 지속적으로 모니터링하는 지능형 위협 탐지 서비스이다. 워크로드의 성능이나 가용성에 영향을 주지 않는다. 

## AWS Budgets

예산 비용 또는 사용량을 초과(또는 초과할 것으로 예상)될 때 알려주는 예산, 알림을 설정할 수 있다. 

## Amazon DynamoDProvision a DynamoDB Accelerator(DAX)

DAX는 Amazon DynamoDB를 위한 가용성이 뛰어난 완전관리형 인 메모리 캐쉬이다.
개발자가 캐시 무효화, 클러스터 관리 또는 데이터 집단을 관리할 필요 없이 DAX가 DynamoDB 인 메모리 가속화를 위해 필요한 모든 작업을 수행한다. 애플리케이션 로직을 변경할 필요가 없다.

## AWS Config - > keyword - 감사 , 검토 , 변경이 없는지 확인

AWS 리소스 인벤토리, 구성 기록, 구성 변경 알림을 제공하여 보안 및 거버넌스를 실현하는 완벽한 관리형 서비스. 
Config 규칙 : 특정 조건을 충족하는 이벤트가 발생하면 알림이나 Lambda 함수를 실행한다.

## Amazon S3 server access logging
Amazon S3 버킷에 수행된 요청에 대한 상세 레코드를 제공한다. 서버 액세스 로그는 많은 애플리케이션에 있어 유용하다. 

보안 및 액세스 감사에 유용할 수 있다. 또한 고객 기반을 이해하고 Amazon S3 청구 비용을 파악할 수 있다.

## AWS Single Sign-On (AWS SSO) = AWS IAM Identity Center

직원 사용자를 한 번 생성하거나 연결하고 여러 AWS 계정 및 애플리케이션에 대한 직원 사용자 액세스를 중앙에서 관리한다.

## identity provider (IdP) 자격 증명 공급자

자격 증명 공급자(IdP)를 사용하면 AWS 외부의 사용자 자격 증명을 관리와 AWS 리소스에 대한 사용 권한을 부여할 수 있다. 

## Amazon AppFlow  - > keyword  SaaS

서비스형 소프트웨어(SaaS) 애플리케이션과 AWS 서비스 간에 데이터를 안전하게 전송할 수 있게 해 주는 완전관리형 통합 서비스이다.

## Amazon AppFlow 기능

•	원하는 빈도로 즉 일정에 따라, 비즈니스 이벤트에 대한 응답으로 또는 온디맨드로 데이터 플로우를 실행할 수 있다.

•	필터링 및 검증과 같은 데이터 변환 기능을 구성하여 추가 단계 없이 플로우 자체의 일부로 바로 사용 가능한 풍부한 데이터를 생성할 수 있다.

•	AppFlow는 이동 중의 데이터를 자동으로 암호화하며 사용자가 AWS PrivateLink와 통합된 SaaS 애플리케이션을 위해 퍼블릭 인터넷상의 데이터 플로우를 제한할 수 있게 해 주므로 보안 위협에 대한 노출이 감소시킬 수 있다.

## AWS Systems Manager  -> keyword 데이터베이스 암호 자동 교체

대규모 인프라 관리 작업을 단순화할 수 있는 플랫폼 서비스.

## AWS Systems Manager Run Command

관리형 노드의 구성을 원격으로 안전하게 관리할 수 있다. 

관리 태스크를 자동화하고 대규모로 일회성 구성 변경을 수행할 수 있다. AWS Management Console, AWS Command Line Interface(AWS CLI), AWS Tools for Windows PowerShell 또는 AWS SDK에서 Run Command를 사용할 수 있다.

## AWS Certificate Manager(ACM)  - >keyword SSL/TLS인증서 자동 교체 (외부 SSL/TLS인증서는 수동 교체)

SSL/TLS(Secure Sockets Layer/Transport Layer Security) 인증서를 쉽게 프로비저닝, 관리 및 배포할 수 있는 서비스. 

: SSL/TLS 인증서를 사용하면 웹 브라우저가 SSL/TLS프로토콜을 사용하여 웹 사이트에 대한 암호화된 네트워크 연결을 식별하고 설정할 수 있다. 


## 네트워크 ACL (네트워크 액세스 제어 목록)

서브넷 수준에서 특정 인바운드 또는 아웃바운드 트래픽을 허용하거나 거부한다. VPC에 보안 계층을 추가할 수 있다.

## Amazon Textract 

스캔한 문서에서 텍스트, 필기 및 데이터를 자동으로 추출하는 기계 학습(ML) 서비스. 

## Amazon Comprehend Medical  - > keyword - 병원 의료 보고서 건강정보 (PHI)

기계 학습을 사용하여 구조화되지 않은 텍스트에서 관련 의료 정보를 쉽게 추출할 수 있게 해주는 자연어 처리 서비스.

## CostExplorer  - > keyword ~개월간의 비용 비교 그래프 생성 및 분석

비용 및 사용량을 보고 분석할 수 있는 도구입니다. 기본 그래프, 비용 탐색기 비용 및 사용 보고서 또는 비용 탐색기 RI 보고서를 사용하여 사용량 및 비용을 탐색할 수 있다. 

## Amazon FSx 파일 게이트웨이  - > keyword - Windows

온프레미스 시설에서 Windows 파일 서버용 클라우드 인 FSx 파일 공유에 대해 짧은 지연시간, 효율적인 액세스를 제공한다
 완전히 관리되고 안정적이며 사실상 무제한의 Windows 파일 공유에 원활하게 액세스할 수 있다

## AWS Shield Advanced  - >keyword 대규모 DDos 공격

DDoS 공격 보호 기능을 제공한다.

## Amazon CloudFront keyword - 정적, 동적 웹사이트 , 대기시간 성능 개선, 데이터 캐싱

.html, .css, .js 및 이미지 파일과 같은 정적 및 동적 웹 콘텐츠를 사용자에게 더 빨리 배포하도록 지원하는 웹 서비스. CloudFront는 엣지 로케이션이라고 하는 데이터 센터의 전 세계 네트워크를 통해 콘텐츠를 제공한다. CloudFront를 통해 서비스하는 콘텐츠를 사용자가 요청하면 지연 시간이 가장 낮은 엣지 로케이션으로 요청이 라우팅되므로 가능한 최고의 성능으로 콘텐츠가 제공된다.

CloudFront의 캐시 관련 문제

· Cache-Control의 max-age 디렉티브 설정

· 배포할 때의 캐시 설정

최종 사용자와 CloudFront간의 통신에 HTTPS 요구

: CloudFront 배포에 하나 이상의 캐시 동작을 구성하여 최종 사용자와 CloudFront 간의 통신에 HTTPS를 요구할 수 있다. 클라이언트에서 HTTPS를 요구하도록 CloudFront를 구성함으로 보안을 강화시킬 수 있다.

## Amazon FSx 

keyword - Windows , Lustre

## Amazon ECS + AWS Fargate

keyword - 컨테이너화 , 운영 오버헤드 , 관리에 대한 책임X

## Amazon Rekognition

keyword - 부적절한 콘텐츠 감지

## Amazon Macie

keyword - 개인 식별 정보(PII), 민감한 데이터

## S3 버킷 버전관리 / MFA 삭제

keyword - S3 버킷 삭제 방지, 안전한 보안 솔루션

## Amazon S3

keyword - 정적 웹사이트, 고가용성 스토리지

## S3 + CloudFront / DynamoDB / Lambda

keyword - 확장성

## S3수명주기 + S3 Glacier Deep Archive

keyword - ~동안은 자주 액세스. 단 ~이후에는 거의 액세스 안함/무기한 보관

## Amazon S3 Intelligent Tiering

keyword - 액세스 패턴을 알 수 없거나 예측할 수 없는.

## NLB

keyword - TCP , UDP, 4계층, 전송계층

## ALB

keyword - HTTP, HTTPS, 7계층

