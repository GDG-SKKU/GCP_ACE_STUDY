# GDG SKKU Cloud Team - 3주차 스터디 정리

## 스터디 개요

- **일자**: 2025-01-04
- **참여자**: 강형준, 김민서, 박진석
- **주제**: GCP의 Instance Groups와 Cloud Load Balancing
- **발표자**: 김민서

## 스터디 목표

이번 스터디에서는 GCP의 Managed Instance Groups(MIG), Unmanaged Instance Groups(UIG), 및 Cloud Load Balancing의 개념과 기능을 이해하고, 실습을 통해 자동화 및 트래픽 분산 전략을 학습하는 것을 목표로 하였습니다.

## 학습 내용

### 1. Instance Groups

- **Instance Groups 정의**:
  - 유사한 가상 머신(VM)들을 그룹화하여 단일 엔터티로 관리
  - 일관된 구성 유지 및 관리 효율성 극대화
- **Instance Groups의 유형**:
  - **Managed Instance Group (MIG)**:
    - 인스턴스 템플릿 기반으로 동일한 VM 생성
    - 자동 스케일링, 자동 복구, 로드 분산 지원
    - 지역적 가용성을 보장하며 여러 존(zone)에 VM 분산 가능
  - **Unmanaged Instance Group (UIG)**:
    - 다양한 VM 구성 허용
    - 자동화 기능 미지원, 단순 그룹화 및 사용자 지정 구성 관리에 적합
- **MIG의 주요 기능**:
  - **Auto Scaling**: 사용자 수나 부하에 따라 VM 수 자동 조정
  - **Auto Healing**: 비정상 인스턴스를 자동 대체
  - **Rolling Updates**: 점진적 업데이트로 서비스 중단 방지
  - **Canary Deployment**: 일부 VM에 새 템플릿을 테스트 후 전체 적용

### 2. Cloud Load Balancing

- **Cloud Load Balancing 정의**:
  - 사용자 트래픽을 여러 지역 또는 단일 지역의 애플리케이션 인스턴스로 분산하는 관리형 서비스
- **주요 특징**:
  - 완전 분산된 소프트웨어 정의 서비스
  - 상태 확인을 기반으로 정상 인스턴스로 트래픽 라우팅
  - Auto Scaling 지원
  - 글로벌 로드 밸런싱으로 단일 Anycast IP 사용
  - 내부 및 외부 로드 밸런싱 모두 지원

### 3. 실습 과제

- **Managed Instance Group 설정**:
  - 인스턴스 템플릿 생성 및 MIG 구성
  - `gcloud compute instance-groups managed` 명령어로 설정
- **Auto Healing 테스트**:
  - VM 상태 확인 및 비정상 인스턴스 자동 교체
- **Cloud Load Balancer 구성**:
  - HTTP(S) 로드 밸런서를 통해 트래픽 분산
  - 상태 확인 및 SSL/TLS 설정 테스트

### 4. 퀴즈

- **문제 1**: HTTPS 웹 애플리케이션의 Auto Scaling 및 Auto Healing 설정 방법
- **문제 2**: GCP 로드 밸런싱 및 WebSocket 프로토콜 활용 방안

## 각 팀원의 역할

- **팀 리더**: 박진석
  - 스터디 방향 조정 및 실습 과제 관리
- **기술 발표**: 김민서
  - 주제 발표 및 실습 시 기술적 지원
- **실습 리뷰**: 강형준
  - 실습 결과 검토 및 피드백 제공

## 다음 스터디 계획

- **일자**: 2025-01-11
- **주제**: Section 10~15
- **발표자**: 박진석

## 느낀 점 및 피드백

![alt text](<스터디 스크린 샷 1.png>)
![alt text](<스터디 스크린 샷 2.png>)

- **김민서**: 다양한 인스턴스 그룹과 로드 밸런싱 기능을 실습하며 GCP의 강력함을 느꼈다.
- **강형준**: 실제 설정 명령어를 사용하면서 GCP의 자동화 기능을 더 깊이 이해할 수 있었다.
- **박진석**: 스터디를 통해 팀원들이 함께 성장하고 있음을 실감했다.

---

## 참고 자료

- `GCP_3rd_Study_Minseo_Kim.pdf`
- [Google Cloud 공식 문서](https://cloud.google.com/docs)

---
