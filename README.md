# 안녕하세요, 백엔드 & AI 인프라 엔지니어 김은선(리나)입니다 👋

<p align="center">
  <strong>AWS 기반 서버·네트워크·스토리지 최적화와 운영 자동화를 합니다</strong>
</p>

---

## 🧭 About

> 비용·가용성·대기시간 지표 중심으로 인프라를 설계/개선합니다.

- 🌐 **리전 이전, VPC Peering, 라우팅/보안그룹 설계 및 자동화**에 강점
- 🤖 **Stable Diffusion 모델 자산을 EFS/인스턴스 스토어로 공유·로컬화**해 배포 단순화

## 🔑 핵심 역량

| 분야 | 기술 스택 |
|------|-----------|
| **☁️ AWS 인프라** | EC2, EBS, EFS, S3, Lambda, CloudWatch, VPC, VPC Peering |
| **🌐 네트워킹** | 서버 마이그레이션, 라우팅/보안그룹 설계, 리전 이전 |
| **🤖 운영 자동화** | Lambda 스케일링, CloudWatch 모니터링, CI/CD |
| **💰 비용 최적화** | Savings Plans, Graviton 전환, GPU 크레딧 도입 |

## 🛠 Tech Stack

<table>
<tr>
<td><strong>☁️ Cloud/Infra</strong></td>
<td>AWS (EC2, EBS, EFS, S3, Lambda, CloudWatch, VPC), GCP, Docker</td>
</tr>
<tr>
<td><strong>🖥️ OS/Server</strong></td>
<td>Ubuntu, Amazon Linux, Windows Server, Raspberry Pi OS</td>
</tr>
<tr>
<td><strong>🌐 Network</strong></td>
<td>VPC, Subnet, Route Table, Security Group, NAT, IGW</td>
</tr>
<tr>
<td><strong>💾 DB/Cache</strong></td>
<td>MariaDB, MySQL, Redis, H2</td>
</tr>
<tr>
<td><strong>⚙️ Backend</strong></td>
<td>Java, Spring Boot, FastAPI, Python</td>
</tr>
<tr>
<td><strong>🎨 Frontend</strong></td>
<td>HTML, JavaScript, CSS</td>
</tr>
</table>

## 📊 주요 성과

<div align="center">

| 🚀 성과 | 📈 결과 |
|---------|---------|
| **QR 처리 성능** | `30s → 3s` **(90% 개선)** |
| **컴퓨팅 비용** | Graviton 전환으로 **20% 절감** |
| **스토리지 비용** | EBS `125GiB → 20GiB` **83% 절감** |
| **GPU 비용** | 크레딧 도입으로 **대부분 외부 지원** |
| **월 GPU 운영비** | 태그 기반 스케일링으로 **≤ 30만원** |

</div>

## 🚀 주요 프로젝트

### 🎞 Chiki Rental — AI 네컷 렌탈 서비스
> **Instagram**: [@chiki_rental](https://instagram.com/chiki_rental) | **Role**: AI Research Engineer

<details>
<summary><strong>📦 스토리지/모델 최적화</strong> (2025.07 ~ 현재)</summary>

- 🗂️ **인스턴스 스토어 활용**: 임시 스토리지 마운트로 EBS 비용 절감
- 🔄 **EFS 공유 구조**: 인스턴스·Docker 간 공통 모델 공유로 중복 제거
- 💾 **모델 로컬화**: SD 모델 구성 요소 추출로 외부 다운로드 없이 파이프라인 구성
- 🐳 **Docker 표준화**: AI 서버 이미지 패키징
- 💳 **GPU 크레딧 도입**: 인프라 비용 대폭 절감

</details>

<details>
<summary><strong>🌐 리전 이전 & VPC Peering</strong> (2025.04 ~ 2025.05)</summary>

- 📍 **서버 마이그레이션**: Seoul → Oregon (G5.xlarge 부족 해결)
- 🔗 **네트워킹 구성**: VPC Peering, 라우팅 테이블, 보안그룹 설계

</details>

<details>
<summary><strong>💰 컴퓨팅/비용 최적화</strong> (2024.12 ~ 2025.03)</summary>

- 🏗️ **Graviton 전환**: 컴퓨팅 비용 20% 절감
- 📋 **Savings Plans**: 장기 비용 안정화

</details>

---

### 🧠 Classendo — 교사용 학생 평가 자동화
> **Website**: [service.classendo.ai](https://service.classendo.ai/) | **Role**: Backend Developer

<details>
<summary><strong>⚖️ 로드밸런서 구조 개선</strong></summary>

**🔴 문제점**
```
ClassendoLB → FrontASG → Front Nginx → BackLB → BackASG → Back Nginx
```
- 이중 ALB/프록시로 경로 복잡
- 간헐적 오류 발생, 지연·관리 부담 증가

**🟢 해결책**
```
ClassendoLB → FrontASG 또는 ClassendoLB → BackASG 직결
```
- 홉 축소로 지연·장애요인 감소
- 운영 단순화

**📈 결과**: 서버 리소스 최적화, 예외처리+자동배포로 **장애 0건 유지**

</details>

## 💼 Experience

<table>
<tr>
<td>

### 🤖 AI Research Engineer Intern
**📍 (주)프로젝트빌드업** | `2025.07 ~ 현재`

- 🗂️ **스토리지 최적화**: 인스턴스 스토어 + EFS 활용으로 EBS 125GiB→20GiB 축소
- 💾 **모델 로컬화**: SD 모델 구성 요소 로컬 저장으로 외부 다운로드 제거
- 💳 **GPU 크레딧**: 직접 조사·신청·도입으로 인프라 비용 외부 지원 전환
- 🎪 **오프라인 운영**: 2025 대구힙합페스티벌 Chiki Rental 부스 스태프

</td>
</tr>
<tr>
<td>

### ⚙️ Backend Developer Intern  
**📍 (주)프로젝트빌드업** | `2024.12 ~ 2025.06`

- 🚀 **자동 스케일링**: Lambda+태그/트래픽 기반 스케일링 & CloudWatch 모니터링
- 🌐 **리전 이전**: Seoul→Oregon 마이그레이션 & VPC Peering 구성
- 💰 **비용 최적화**: Graviton 전환(20% 절감) & Savings Plans 적용

</td>
</tr>
</table>

## 🎓 Education & Certifications

<table>
<tr>
<td width="50%">

### 🏫 Education
- **☁️ AWS Summit 2025** 참가 `2025.05`
- **💻 카카오테크캠퍼스** 2기 Backend `2024.04~2024.11` 
- **🎓 경북대학교** 전자공학부(주)/컴퓨터학부(부) `2020.03~2024.08`
- **☕ 멀티캠퍼스** Java 풀스택 개발 `2023.09~2024.03`
- **🤖 대구AI허브** AI/자율주행 로봇 개발 `2023.07~2023.08`
- **🔬 학술동아리** AI & IoT 분야 `2022.03~2023.11`


</td>
<td width="50%">

### 📜 Certifications
- **🐧 리눅스마스터 2급** (1차 합격, 2024.08)
- **⚙️ 정보처리기사** (필기 합격, 2025.02)  
- **💾 SQLD** (취득, 2025.03)

</td>
</tr>
</table>

<details>
<summary><strong>🏆 주요 수상 내역</strong></summary>

| 🥇 등급 | 🏛️ 주관 | 📝 프로젝트 |
|---------|----------|-------------|
| **🥈 은상** | 한국정보기술학회 | 차량 내 반려동물 안전 위험 요소 감지 복합 센서 시스템 |
| **🥉 동상** | 한국정보기술학회 | 개 짖는 소리 주파수 분석 및 신경망 종 분류 시스템 |
| **🥉 동상** | 한국정보과학회 | IoT 다중센서 낙상사고 예방 & 수면환경 개선 영아용 침대 |
| **🏆 최우수상** | 멀티캠퍼스 | 반려동물 커뮤니티 (세미프로젝트) |
| **🏆 최우수상** | 멀티캠퍼스 | Kodi 한국 여행 안내 플랫폼 (최종프로젝트) |

</details>

---

## 📞 Contact

<div align="center">

| 📝 Blog | 📧 Email |
|---------|----------|
| **[goingweb.tistory.com](https://goingweb.tistory.com/)** | **[eunseon7325@gmail.com](mailto:eunseon7325@gmail.com)** |

</div>

---

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=eunsoni&show_icons=true&theme=radical&hide_border=true" height="160"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=eunsoni&layout=compact&theme=radical&hide_border=true" height="160"/>
</div>

<div align="center">
  
**💡 "비용·가용성·대기시간 지표 중심의 인프라 설계로 최적의 성능을 만들어갑니다"**

</div>