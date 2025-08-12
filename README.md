# 안녕하세요, 백엔드 & AI 인프라 엔지니어 김은선(리나)입니다 👋
### AWS 기반 서버·네트워크·스토리지 최적화와 운영 자동화를 합니다.
🧭 About
비용·가용성·대기시간 지표 중심으로 인프라를 설계/개선합니다.

리전 이전, VPC Peering, 라우팅/보안그룹 설계 및 자동화에 강점이 있습니다.

Stable Diffusion 모델 자산을 EFS/인스턴스 스토어로 공유·로컬화해 배포를 단순화합니다.

🔑 핵심 역량
- **AWS 인프라 설계·운영·최적화** (EC2/EBS/EFS/S3/Lambda/CloudWatch, VPC/Peering)
- **리전 이전 & 네트워킹** (서버 마이그레이션, 라우팅/보안그룹 설계)
- **운영 자동화** (Lambda, 태그·트래픽 기반 스케일링, CI/CD, 스크립트)
- **비용 절감 전략** (Savings Plans, Graviton 전환, GPU 크레딧 도입)

🛠 Tech Stack
- **Cloud/Infra**: AWS(EC2, EBS, EFS, S3, Lambda, CloudWatch, VPC, VPC Peering), GCP, Docker
- **OS/Server**: Ubuntu, Amazon Linux, Windows Server, Raspberry Pi OS
- **Network**: VPC, Subnet, Route Table, Security Group, NAT, IGW
- **DB/Cache**: MariaDB, MySQL, Redis, H2
- **Backend**: Java, Spring Boot, FastAPI, Python
- **Frontend**: HTML, JavaScript, CSS

📊 Impact
- **QR 처리 성능 개선**: 30s → 3s (−90%), 태그·트래픽 기반 스케일링으로 월 GPU 비용 ≤ 30만원
- **Graviton(Arm) 전환**으로 컴퓨팅 비용 ~20% 절감
- **스토리지 최적화**: EBS 125GiB → 20GiB(EFS 공유·인스턴스 스토어 활용)로 비용 절감
- **GPU 크레딧 제도 도입**으로 GPU 인프라 비용의 대부분 외부 지원 전환
- **Savings Plans 적용**으로 장기 비용 안정화

🚀 Projects
### 🎞 Chiki Rental — AI 네컷 렌탈/오프라인 서비스 (인스타그램: chiki_rental)

#### 스토리지/모델 자원 최적화 (2025.07 ~ 현재)
- **인스턴스 스토어 활용**: 임시 스토리지 마운트로 EBS 비용 절감
- **EFS 공유 구조**: 인스턴스·Docker 간 공통 모델 공유로 중복 제거, 배포 간소화
- **모델 로컬화**: Stable Diffusion 모델 구성 요소 추출 및 로컬 저장으로 외부 다운로드 없이 파이프라인 구성
- **Docker 표준화**: AI 서버 도커 이미지 패키징
- **GPU 크레딧 도입**: GPU 인프라 비용 대폭 절감

#### 리전 이전 및 VPC Peering 구축 (2025.04 ~ 2025.05)
- **서버 마이그레이션**: Seoul(G5.xlarge 부족) → Oregon, 다운타임 최소화
- **네트워킹 구성**: VPC Peering, 라우팅 테이블, 보안그룹 구성 및 점검

#### 컴퓨팅/비용 최적화 (2024.12 ~ 2025.03)
- **Graviton 전환**: 컴퓨팅 비용 약 20% 절감
- **AWS Savings Plans**: 장기 비용 안정화

### 🧠 Classendo — 교사용 학생 평가 자동화 (web: https://service.classendo.ai/)

#### 로드밸런서 구조 개선 작업
**문제**: 프론트/백 nginx + 이중 로드밸런서 경유로 경로 복잡 → 간헐적 오류 발생, 지연·관리 부담 증가

**해결**: ALB 레이어에서 라우팅을 단순화해 백엔드로 직접 연결, 중복 프록시와 불필요한 경유 지점 정리

```
(기존) ClassendoLB → FrontASG → Front Nginx → BackLB → BackASG → Back Nginx
→ 이중 ALB/프록시로 경로 복잡, 지연·설정 충돌 및 복구 지연

(개선) ClassendoLB → FrontASG 또는 ClassendoLB → BackASG 직결 
→ 홉 축소로 지연·장애요인 감소, 운영 단순화
```

- **운영 안정화**: 서버 리소스 최적화, 예외처리+자동배포로 장애 0건 유지

💼 Experience
### AI Research Engineer Intern, (주)프로젝트빌드업 (2025.07 ~ 현재)
- **스토리지 최적화**: 인스턴스 스토어 마운트로 무료 디스크 최대 활용 → EBS 의존도 감소, 스토리지 비용 절감
- **EFS 공유 구조**: EFS를 인스턴스와 Docker 컨테이너에 마운트해 Stable Diffusion 공통 모델 구성 요소 공유 → 자원 중복 최소화, 배포 간소화 → EBS 125GiB→20GiB 축소
- **모델 로컬화**: Stable Diffusion 모델 구성 요소를 로컬 저장하여 외부 다운로드 없이 자체 파이프라인 구성 가능하도록 개선
- **GPU 크레딧 도입**: 직접 조사·신청·도입으로 GPU 인프라 비용의 대부분 외부 지원으로 전환
- **오프라인 운영**: 2025 대구힙합페스티벌 Chiki Rental 부스 스태프

### Backend Developer Intern, (주)프로젝트빌드업 (2024.12 ~ 2025.06)
- **자동 스케일링**: AWS Lambda+태그/트래픽 기반 스케일링(15분 무요청 시 Scale-in, 피크 시 Scale-out) 및 CloudWatch 지표·알람 정비
- **리전 이전**: ap-northeast-2a(Seoul)에서 g5.xlarge GPU 부족 이슈 해결 → us-west-2(Oregon)로 이전
- **네트워킹**: 양 리전 간 VPC Peering 구성 및 라우팅 테이블/보안그룹 수정
- **비용 최적화**: Graviton(Arm) 전환으로 백엔드 컴퓨팅 비용 약 20% 절감, AWS Savings Plans 적용으로 장기 사용 리소스 비용 절감 구조 마련

🎓 Education
**경북대학교 전자공학부(주)/컴퓨터학부(부)** (2020.03 ~ 2024.08)
- **졸업프로젝트**: AI 및 IoT 시스템 개발 및 한국정보과학회 논문 게재 (2024.02~2024.06)

**카카오테크캠퍼스 2기 Backend** 수료 (2024.04 ~ 2024.11)

**멀티캠퍼스 Java 풀스택 개발 과정** 수료 (2023.09~2024.03)

**대구AI허브 AI 및 자율주행 로봇 개발 과정** 수료 (2023.07~2023.08)

**AI 및 IoT 분야 학술동아리** 활동 (2022.03~2023.11)

**AWS Summit 2025** 참가 (2025.05)

🏅 Awards & Certifications
#### 자격증
- **리눅스마스터 2급** (1차 합격, 2024.08)
- **정보처리기사** (필기 합격, 2025.02)  
- **SQLD** (취득, 2025.03)

#### 수상 내역
- **대학생논문경진대회 (은상)**, 한국정보기술학회  
  '차량 내 반려동물 안전을 위한 위험 요소 감지 복합 센서 시스템 제작'
  
- **대학생논문경진대회 (동상)**, 한국정보기술학회  
  '개 짖는 소리의 주파수 분석 및 인공신경회로망을 이용한 종 분류 시스템'
  
- **대학생논문경진대회 (동상)**, 한국정보과학회  
  'IoT 기반 다중센서를 이용한 낙상사고 예방 및 수면 환경 개선을 위한 영아용 침대'
  
- **세미프로젝트 (최우수상)**, 멀티캠퍼스  
  '반려동물을 위한 커뮤니티'
  
- **최종프로젝트 (최우수상)**, 멀티캠퍼스  
  'Kodi 한국 여행 안내 플랫폼'

✍️ Blog & Contact
- **Blog**: https://goingweb.tistory.com/
- **Email**: eunseon7325@gmail.com

---

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=eunsoni&show_icons=true&theme=radical" height="150"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=eunsoni&layout=compact&theme=radical" height="150"/>
</div>