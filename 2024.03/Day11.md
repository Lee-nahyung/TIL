<h1>💻 AWS<2024.3.11></h1>
<h4>📖덤프 312p~361p <br></h4><br>

- 지연시간 없이 온프레미스 sys에서 모든 파일 형식에 즉시 엑세스 하려면, 저장된 볼륨 형식 필요<br>
- 멀티파트 업로드: 대형객체에 사용, 불완전한 멀티파트 업로드는 정리하지 않을수록 스토리지 소모.(따라서 정리하도록 S3 수명 주기 정책 구성 필요.)
- 빠른 스냅샷 복원 기능을 사용해  AMI 프로비저닝: AMI를 생산하는 가장 빠르고 효율적인 방법.
- AWS Aurora Global Database: Amazon Aurora 데이터베이스 클러스터의 다중 리전 배포를 지원하는 서비스. <br> ->여러 지역에 걸쳐 데이터베이스를 배포하고 글로벌 환경에서 응용 프로그램의 가용성과 성능 향상 o<br><br>
- 
    - Compute Saving Plans : 인스터스 패밀리, 크기, AZ, 리전, OS 또는 테넌시와 관계없이 EC2 인스턴스 사용량에 적용 
    - EC2 instance Savings Plans: AZ, 규모, OS 또는 테넌시에 관계없이 해당 리전에서 선택한 인스턴스 패밀리의 비용이 자동으로 절감<br><br>


- 🧷헤더 종류:

  - s3: x-amz-acl 헤더: 해당 객체에 대한 엑세스 권한을 제어하는데 사용.(private를 설정하면 객체에 대한 엑세스가 제한.)
  - asw:SecureTransport 헤더: 요청이 안전한 연결(HTTPS)을 통해 이루어져야 함을 나타냄.
  - x-amz-server-side-encryption 헤더: 객체 업로드 시 서버 측 암호화를 수행하도록 지시. 데이터를 자동으로 암호화하여 저장.<br><br>
  - 
- 🧷보안관련 사항:

  - GuardDuty: AWS 계정 내에서 악성 활동을 탐지하고 경보 생성. 이상 징후를 실시간으로 모니터링.(보안 전문가에게 알림 및 이벤트 기록 보냄)<br><br>
  - Security Hub: 민감한 데이터의 위치와 엑세스 패턴을 감지하고 분류하는 데이터보안 및 개인정보 보호 서비스 (기계학습 사용)<br><br>
  - WAF: 웹 애플리케이션에 대한 보안 강화, 특히 HTTP 및 HTTPS 트래픽 공격 차단. DDos 공격 대응 서비스 (애플리케이션 레벨, 나라에 대한 엑세스)<br><br>
  - Shield Advanced: DDos 공격 방어, (네트워크 계층)<br><br>
  - Macie: 데이터의 민감한 정보를 감지하고 보호하기 위한 서비스. 취약점 스캐닝 목적 x<br><br>
  - Inspector: 애플리케이션 및 인프라의 취약점을 검사하고 보고서를 생성하는 보안서비스<br><br>
  - Detective : 클라우드 환경에서 발생하는 보안 이벤트를 실시간으로 모니터링하고 감지(ex, 비정상적인 로그인 시도, 민감한 리소스 접근 시도 등의 이벤트 식별하고 경고 생성)
