# 🛒 고객 및 상품 관리 시스템 (E-Commerce Back-office)

> **팀원들의 원활한 협업과 효율적인 관리를 위한 이커머스 백오피스 프로젝트입니다.**

---

## 🏗 기술 스택 및 구조 (Tech Stack)

![Java](https://img.shields.io/badge/Java%2017-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring%20Data%20JPA-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-%234479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)

| 기술 스택 (Tech Stack) | 버전 (Version) |
| :--- | :--- |
| **Java** | 17 |
| **Spring Boot** | 4.0.2 |
| **Spring Dependency Management** | 1.1.7 |
| **Spring Data JPA** | - |
| **MySQL** | - |

- **Architecture**: Domain-Driven Design (Partial), Layered Architecture (Query/Command Service)

---

## 👨‍💻 팀원 소개 및 역할 분담

### **R&R (Role & Responsibilities)**

| 이름 | 역할 | 담당 과업 (Task) |
| :---: | :---: | :--- |
| <nobr>**정채림**</nobr> | <nobr>**Leader**</nobr> | 프로젝트 총괄, 일정 관리, 초기 환경 세팅(Git/S.A)<br>공통 Response/Exception 핸들러, 코드 병합 및 최종 QA |
| <nobr>**정민교**</nobr> | <nobr>**Presenter**</nobr> | 발표 자료 제작 및 리허설 주도<br>주문 조회(검색/정렬/페이징), 회의록 및 README 관리 |
| <nobr>**이지민**</nobr> | <nobr>**Sub Leader**</nobr> | 관리자 인증(회원가입/승인/세션 로그인)<br>도메인 로직 설계 및 코드 리뷰 주도 |
| <nobr>**신현민**</nobr> | <nobr>**Sub Leader**</nobr> | 상품 관리 총괄(등록/조회/수정/삭제)<br>재고 기반 자동 상태 변경 로직 구현 |
| <nobr>**이재민**</nobr> | <nobr>**Sub Leader**</nobr> | 주문 CUD(생성/취소)<br>트랜잭션 관리 및 재고 동시성 제어 핵심 담당 |
| <nobr>**이지혜**</nobr> | <nobr>**Recorder**</nobr> | 고객 관리(조회/수정/삭제/상태 변경)<br>회의록 정리 및 문서화 보조 |

---

## 📋 프로젝트 개요

본 프로젝트는 이커머스 운영에 필수적인 **관리자 전역 기능, 고객 응대, 상품 및 재고 관리, 그리고 주문 프로세스**를 효율적으로 처리하기 위한 백오피스 시스템입니다.

### **주요 특징**
- **계층별 책임 분리**: Query/Command Service 분리를 통한 가독성 및 유지보수성 향상
- **데이터 정합성**: 주문 시 재고 차감 및 취소 시 복구 로직의 트랜잭션 보장
- **확장성 있는 설계**: 공통 DTO와 페이징 처리를 통한 일관된 API 구조

---

## 🗂 ERD (Entity Relationship Diagram)

<img width="1280" height="842" alt="Image" src="https://github.com/user-attachments/assets/fb60e0e9-4fcb-48e9-a3d2-b563e266be9d" />

---

## 🛠 주요 구현 기능

### 1. Auth & Admin (관리자)
- **인증**: 관리자 회원가입, 세션 기반 로그인/로그아웃 구현
- **계정 관리
