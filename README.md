# 안녕하세요, 백엔드 & AI 인프라 엔지니어 김은선(리나)입니다 👋

<div align="center">
  
  ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white&labelColor=232F3E)
  ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white&labelColor=2496ED)
  ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54&labelColor=3776AB)
  ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white&labelColor=007396)
  ![Spring Boot](https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white&labelColor=6DB33F)
  
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=%F0%9F%9A%80%20Infrastructure%20Engineer&fontSize=40&fontAlign=50&fontAlignY=40&desc=Cost%20Optimization%20%7C%20Performance%20Tuning%20%7C%20Automation&descAlign=50&descAlignY=60" />
</div>

---

## 🧭 About

> 비용·가용성·대기시간 지표 중심으로 인프라를 설계/개선합니다.

- 🌐 **리전 이전, VPC Peering, 라우팅/보안그룹 설계 및 자동화**에 강점
- 🤖 **Stable Diffusion 모델 자산을 EFS/인스턴스 스토어로 공유·로컬화**해 배포 단순화

## 🔑 핵심 역량

- **AWS 인프라**: EC2, EBS, EFS, S3, Lambda, CloudWatch, VPC, VPC Peering
- **네트워킹**: 서버 마이그레이션, 라우팅/보안그룹 설계, 리전 이전
- **운영 자동화**: Lambda 스케일링, CloudWatch 모니터링, CI/CD
- **비용 최적화**: Savings Plans, Graviton 전환, GPU 크레딧 도입

## 🛠 Tech Stack

- **Cloud/Infra**: AWS (EC2, EBS, EFS, S3, Lambda, CloudWatch, VPC), GCP, Docker
- **OS/Server**: Ubuntu, Amazon Linux, Windows Server, Raspberry Pi OS
- **Network**: VPC, Subnet, Route Table, Security Group, NAT, IGW
- **Database**: MariaDB, MySQL, Redis, H2
- **Backend**: Java, Spring Boot, FastAPI, Python
- **Frontend**: HTML, JavaScript, CSS

## 📊 주요 성과

- **QR 처리 성능**: 30s → 3s (90% 개선)
- **컴퓨팅 비용**: Graviton 전환으로 20% 절감
- **스토리지 비용**: EBS 125GiB → 20GiB (83% 절감)
- **GPU 비용**: 크레딧 도입으로 대부분 외부 지원
- **월 GPU 운영비**: 태그 기반 스케일링으로 ≤ 30만원

## 🚀 주요 프로젝트

### Chiki Rental — AI 네컷 렌탈 서비스
> **Instagram**: [@chiki_rental](https://instagram.com/chiki_rental)

#### 스토리지/모델 최적화 (2025.07 ~ 현재)
- **인스턴스 스토어 활용**: 임시 스토리지 마운트로 EBS 비용 절감
- **EFS 공유 구조**: 인스턴스·Docker 간 공통 모델 공유로 중복 제거
- **모델 로컬화**: SD 모델 구성 요소 추출로 외부 다운로드 없이 파이프라인 구성
- **Docker 표준화**: AI 서버 이미지 패키징
- **GPU 크레딧 도입**: 인프라 비용 대폭 절감

#### 리전 이전 & VPC Peering (2025.04 ~ 2025.05)
- **서버 마이그레이션**: Seoul → Oregon (G5.xlarge 부족 해결)
- **네트워킹 구성**: VPC Peering, 라우팅 테이블, 보안그룹 설계

#### 컴퓨팅/비용 최적화 (2024.12 ~ 2025.03)
- **Graviton 전환**: 컴퓨팅 비용 20% 절감
- **Savings Plans**: 장기 비용 안정화

---

### Classendo — 교사용 학생 평가 자동화
> **Website**: [service.classendo.ai](https://service.classendo.ai/)
#### 로드밸런서 구조 개선
**문제점**
```
ClassendoLB → FrontASG → Front Nginx → BackLB → BackASG → Back Nginx
```
- 이중 ALB/프록시로 경로 복잡
- 간헐적 오류 발생, 지연·관리 부담 증가

**해결책**
```
ClassendoLB → FrontASG 또는 ClassendoLB → BackASG 직결
```
- 홉 축소로 지연·장애요인 감소
- 운영 단순화

**결과**: 서버 리소스 최적화, 예외처리+자동배포로 **장애 0건 유지**

## 💼 Experience

### AI Research Engineer Intern
**프로젝트빌드업** | `2025.07 ~ 현재`

### Backend Developer Intern  
**프로젝트빌드업** | `2024.12 ~ 2025.06`

## 🎓 Education & Certifications

### Education
- **AWS Summit 2025** 참가 `2025.05`
- **카카오테크캠퍼스** 2기 Backend `2024.04~2024.11` 
- **경북대학교** 전자공학부(주)/컴퓨터학부(부) `2020.03~2024.08`
- **멀티캠퍼스** Java 풀스택 개발 `2023.09~2024.03`
- **대구AI허브** AI/자율주행 로봇 개발 `2023.07~2023.08`
- **학술동아리** AI & IoT 분야 `2022.03~2023.11`

### Certifications
- **리눅스마스터 2급(1차)** (2024.08)
- **정보처리기사(필기)** (2025.02)  
- **SQLD** (2025.03)

### 주요 수상 내역
- 🥈 **은상** | 한국정보기술학회 | 차량 내 반려동물 안전 위험 요소 감지 복합 센서 시스템
- 🥉 **동상** | 한국정보기술학회 | 개 짖는 소리 주파수 분석 및 신경망 종 분류 시스템
- 🥉 **동상** | 한국정보과학회 | IoT 다중센서 낙상사고 예방 & 수면환경 개선 영아용 침대
- 🏆 **최우수상** | 멀티캠퍼스 | 반려동물 커뮤니티 (세미프로젝트)
- 🏆 **최우수상** | 멀티캠퍼스 | Kodi 한국 여행 안내 플랫폼 (최종프로젝트)

---

## 📞 Contact

- **Blog**: [goingweb.tistory.com](https://goingweb.tistory.com/)
- **Email**: [eunseon7325@gmail.com](mailto:eunseon7325@gmail.com)

---

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=eunsoni&show_icons=true&theme=radical&hide_border=true" height="160"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=eunsoni&layout=compact&theme=radical&hide_border=true" height="160"/>
</div>

<div align="center">
  
**"비용·가용성·대기시간 지표 중심의 인프라 설계로 최적의 성능을 만들어갑니다"**

</div>
