# GDG SKKU Cloud Team - 2주차 스터디 정리

## 스터디 개요

- **일자**: 2024-12-28
- **참여자**: 강형준, 김민서, 박진석
- **주제**: Gcloud CLI 및 Configuration 관리
- **발표자**: 강형준

## 스터디 목표

이번 스터디에서는 Gcloud CLI의 기본 명령어와 Configuration 설정 방법에 대해 학습하고, 실습을 통해 이를 익히는 것을 목표로 하였습니다. 이후 팀원 간 역할 분담 및 다음 학습 방향을 논의하였습니다.

## 학습 내용

### 1. Gcloud CLI 개요

- **Gcloud CLI 기능**:
  - 구글 클라우드 리소스 관리, 배포, CRUD 작업 수행
  - Compute Engine, Kubernetes, BigQuery 등 다양한 서비스와 연동
- **Gcloud CLI와 관련된 도구**:
  - Cloud Storage: `gsutil`
  - BigQuery: `bq`
  - Kubernetes: `kubectl`
- **사용 방법**: GCP의 Cloud Shell에서 바로 활용 가능, 별도 설치 불필요

### 2. Gcloud Configuration 설정

- **기본 명령어**:
  - `gcloud config list`: 현재 Configuration 확인
  - `gcloud config configurations list`: 모든 Configuration 목록 출력
  - `gcloud config set {SECTION}/{PROPERTY} VALUE`: 설정 값 변경
  - `gcloud config configurations create {NAME}`: 새로운 Configuration 생성
- **Configuration 관리**:
  - 프로젝트, 계정, 지역(region) 및 영역(zone) 설정
  - 우선순위: 명령어별 설정 > 로컬 설정 > 중앙 관리 설정

### 3. 실습 과제

- **Configuration 실습**:
  - 프로젝트 별 Configuration 생성 및 활성화
  - `gcloud compute instances create` 명령어로 VM 생성 및 옵션 활용
- **필터링 및 정렬**:
  - `gcloud compute instances list --filter`와 `--sort-by` 옵션 사용
  - 특정 리소스 상세 정보 확인: `gcloud compute regions describe {REGION}`

### 4. 퀴즈

- **문제 1**: 비활성화된 Configuration의 Kubernetes Engine 설정 확인 방법
- **문제 2**: 두 계정에서 서로 다른 Configuration을 활용하여 Compute Engine 인스턴스 생성 방법

## 다음 스터디 계획

- **일자**: 2025-01-04
- **주제**: Section 6 ~ 9
- **발표자**: 김민서

## 느낀 점 및 피드백

![alt text](<스터디 스크린샷 1.png>)
![alt text](<스터디 스크린샷 2.png>)

- **강형준**: 실습을 통해 Gcloud 명령어의 구조를 이해할 수 있었으며, CLI와 Configuration 관리의 중요성을 느꼈다.
- **김민서**: 구체적인 예제를 통해 GCP의 다양한 기능을 배우는 유익한 시간이었고, CLI 활용 능력을 키울 수 있었다.
- **박진석**: 팀원들과의 협업이 잘 이루어졌고, 다음 주 주제를 준비하는 데 필요한 방향을 명확히 설정할 수 있었다.

---

## 참고 자료

- `Week_2_GDG_SKKU_Cloud_Team_강형준.pdf`
- [Google Cloud 공식 문서](https://cloud.google.com/docs)

---
