# Audio Streaming Web Service (MSA 기반)

## Overview
Kotlin과 Spring Boot를 기반으로 오디오 및 비디오 스트리밍 기능을 제공하는 웹 서비스를 구현한 프로젝트입니다.  
MSA(Microservice Architecture) 구조를 적용하고 Docker 및 Kubernetes를 활용하여 컨테이너 기반 서비스 배포 환경을 구성하였습니다.

---

## Role
- 백엔드 개발 및 서비스 구조 설계
- API 설계 및 데이터 처리 로직 구현
- MSA 및 컨테이너 환경 구축

---

## Tech Stack
- Backend: Kotlin, Spring Boot
- Database: MySQL (JPA)
- DevOps: Docker, Docker Compose, Kubernetes
- Server: Tomcat

---

## Architecture

- Controller / Service / Repository / Model 구조로 계층 분리
- Spring Data JPA를 활용한 데이터 관리
- MySQL 기반 데이터베이스 연동
- Docker Compose를 통한 웹 서버 + DB 멀티 컨테이너 구성

---

## Key Features

### 1. 사용자 인증 기능
- 회원가입 (Register API)
- 로그인 (Login API)
- 사용자 정보 조회 및 관리

### 2. 미디어 서비스 기능
- 오디오 및 비디오 업로드
- 트랙 정보 관리 (제목, 아티스트 등)
- 파일 시스템 기반 미디어 저장

### 3. CRUD 기능
- 사용자 및 트랙 데이터 생성, 조회, 수정, 삭제 기능 구현
- REST API 기반 서비스 구조 설계

### 4. 스트리밍 기능
- HTTP Range 요청 지원
- Content-Type 동적 설정을 통한 오디오/비디오 재생
- HTML5 audio/video 태그 기반 재생 지원

### 5. 좋아요 및 댓글 기능
- LikedTrack 엔티티를 통한 좋아요 기능 구현
- 댓글 작성, 조회, 수정, 삭제 기능 제공
- 사용자-콘텐츠 간 상호작용 기능 구현

---

## DevOps / Deployment

### Docker 기반 컨테이너 구성
- Spring Boot 서버와 MySQL을 각각 컨테이너로 구성
- docker-compose를 활용한 멀티 컨테이너 실행

### Docker Hub 활용
- 이미지 빌드 및 업로드 (Push)
- 외부 환경에서 이미지 Pull 및 실행 가능

### Kubernetes 기반 확장
- Deployment를 통한 서비스 확장 관리
- Service를 통한 외부 접근 구성
- PersistentVolume을 활용한 데이터 유지

---

## Result
- MSA 기반 웹 서비스 구조 이해 및 구현
- 컨테이너 기반 배포 환경 구축 경험 확보
- 백엔드 중심의 실무형 웹 서비스 개발 경험

---

## Note
프로젝트 용량 문제로 인해 전체 소스코드는 업로드하지 않았으며,  
구조 및 구현 내용 중심으로 정리하였습니다.
