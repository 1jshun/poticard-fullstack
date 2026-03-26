<br />
<div align="center">
  <img src="backend/logo.png" width="100" alt="Poticard Logo" />
  
  <h1>Poticard</h1>
  
  <p><b>나만의 커리어를 한 장의 카드로</b></p>
</div>
<hr />
<br />


## 1. 프로젝트 소개

PotiCard는 사용자가 직접 구직 및 이직용 포트폴리오를 작성하고 다양한 스타일을 적용할 수 있는 웹 서비스입니다. 완성된 포트폴리오를 바탕으로 핵심 키워드와 정보를 담은 디지털 명함을 생성하고 관리할 수 있습니다.

사용자는 자신의 프로젝트 경험을 포트폴리오로 구성하며 ai를 이용한 포트폴리오 첨삭을 통해 완성도를 높일 수 있습니다. 시스템은 이를 분석하여 주요 기술 스택과 역량을 자동으로 도출합니다. 이를 바탕으로 사용자는 디지털 명함을 만들어 자신의 전문성을 보다 명확하게 정리하고, 효율적인 자기 표현 수단으로 활용할 수 있습니다.

또한, 기업은 본 서비스를 통해 지원자의 디지털 명함과 포트폴리오를 확인하여 핵심 역량을 신속하게 파악할 수 있으며, 서비스 내 제공되는 1:1 채팅 및 화상 채팅 기능을 통해 인재 컨택 및 채용 과정에 즉각적으로 활용할 수 있습니다.


## 2. 🔗 바로가기

| 구분 | 링크 |
|:---|:---|
| **🌐 홈페이지** | [www.poti.kro.kr](https://www.poti.kro.kr) |
| **📖 API 명세서** | [Swagger UI](https://api.poti.kro.kr/swagger-ui/index.html) |
| **📖 상세 설명** | [Poticard WIKI](https://github.com/beyond-sw-camp/be24-3rd-DevOops-Poticard/wiki) |
| **🖥️ Frontend Repos** | [be24-2nd-DevOops-PotiCard](https://github.com/beyond-sw-camp/be24-2nd-DevOops-PotiCard) |
| **⚙️ Backend Repos** | [be24-3rd-DevOops-Poticard](https://github.com/beyond-sw-camp/be24-3rd-DevOops-Poticard) |

## 3. 기술 스택

<table width="100%">
<tr>
<th width="15%" align="center">Category</th>
<th width="85%" align="center">Tech Stack</th>
</tr>
<tr>
<td align="center"><b>Frontend</b></td>
<td>
<img src="https://img.shields.io/badge/Vue.js_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black">
<img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white">
</td>
</tr>
<tr>
<td align="center"><b>Backend</b></td>
<td>
<img src="https://img.shields.io/badge/Java_17-007396?style=flat-square&logo=openjdk&logoColor=white">
<img src="https://img.shields.io/badge/Spring_Boot_3.x-6DB33F?style=flat-square&logo=springboot&logoColor=white">
<img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white">
<img src="https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=flat-square">
<img src="https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white">
</td>
</tr>
<tr>
<td align="center"><b>AI / API</b></td>
<td>
<img src="https://img.shields.io/badge/Google_Gemini_AI-4285F4?style=flat-square&logo=googlegemini&logoColor=white">
<img src="https://img.shields.io/badge/OAuth2.0_G/K-EB4132?style=flat-square">
<img src="https://img.shields.io/badge/PortOne_Payment-FF5D32?style=flat-square">
</td>
</tr>
<tr>
<td align="center"><b>Infrastructure</b></td>
<td>
<img src="https://img.shields.io/badge/Docker_&_Compose-2496ED?style=flat-square&logo=docker&logoColor=white">
<img src="https://img.shields.io/badge/Oracle_Cloud-F80000?style=flat-square&logo=oracle&logoColor=white">
<img src="https://img.shields.io/badge/AWS_S3-569A31?style=flat-square&logo=amazons3&logoColor=white">
<img src="https://img.shields.io/badge/Ubuntu-E9433F?style=flat-square&logo=ubuntu&logoColor=white">
</td>
</tr>
<tr>
<td align="center"><b>Observability</b></td>
<td>
<img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white">
<img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white">
<img src="https://img.shields.io/badge/Jaeger-60D051?style=flat-square&logo=jaeger&logoColor=white">
</td>
</tr>
</table>

## 4. 실행 가이드
PotiCard는 Docker Compose를 통해 개발 환경을 통합 관리하고 있습니다.

### 1) 사전 준비
* [Docker Desktop](https://www.docker.com/products/docker-desktop/) 설치 및 실행
* Git 설치

### 2) 프로젝트 클론 및 환경 설정
```bash
# 1. 저장소 클론
git clone [https://github.com/1jshun/poticard-fullstack.git](https://github.com/1jshun/poticard-fullstack.git)
cd poticard-fullstack

# 2. 환경 변수 파일(.env) 생성
cp backend/.env.example backend/.env

# 이미지 빌드 및 컨테이너 실행
docker-compose up --build -d
