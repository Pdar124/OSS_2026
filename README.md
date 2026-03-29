# 🐱 Campus Cat Mate (CCM)
> **캠퍼스 길고양이와 인간의 건강한 공존을 위한 실시간 돌봄 네트워크**

![Version](https://img.shields.io/badge/version-1.12-blue)
![Platform](https://img.shields.io/badge/platform-Mobile%20Web-orange)
![License](https://img.shields.io/badge/license-MIT-green)

캠퍼스 내 파편화된 고양이 정보를 통합하여 실시간 위치 정보를 제공하고, 중복 급여 방지 및 건강 상태를 체계적으로 관리하는 지능형 돌봄 시스템입니다.

---

## ✨ Key Features

### 📍 실시간 지도 및 위치 예측 (Real-time Map)
* **Encounter Check:** 학생들이 마주친 고양이의 위치와 시간을 간편하게 제보합니다.
* **Recency Weight:** 최근 제보 데이터에 가중치를 부여하여 고양이의 현재 예상 위치와 동선을 지도에 시각화합니다.

### 🧠 지능형 개체 식별 (Territory-based ID)
* **Territory Identification:** 고양이별 영역(Territory) 데이터와 GPS 좌표를 대조하여, 제보된 위치에서 가장 발견 확률이 높은 고양이를 사용자에게 자동 추천합니다.

### 🍱 체계적인 돌봄 관리 (Caregiver Log)
* **Diet Check:** 인증된 돌보미(Caregiver)가 사료 종류와 양을 기록하여 중복 급여를 방지합니다.
* **Health Monitoring:** 고양이의 건강 특이사항을 기록하고 과거 이력을 추적하여 이상 징후를 조기에 발견합니다.

### 📚 집단지성 고양이 위키 (Cat Wiki)
* **Cat Profile:** 이름, 나이, 성격, 주의사항 등 개체별 상세 정보를 관리합니다.
* **Optimistic Locking:** 다수의 사용자가 동시에 정보를 수정할 때 발생하는 충돌을 방지합니다.

---

## 🛠 Technical Solution & NFR

### ⚡ Technical Difficulties
* **영역 기반 식별:** 고유 영역 동물의 특성을 활용한 오제보 방지 로직 구현
* **루틴 보정 알고리즘:** 기상청 API 및 실시간 데이터를 연동한 이동 패턴 예측
* **동시성 제어:** 위키 편집 충돌 방지를 위한 낙관적 락(Optimistic Locking) 적용

### 📱 User Experience & Reliability
* **Mobile First UX:** 야외 제보 상황을 고려한 '원터치 위치 전송' 및 직관적인 UI 설계
* **Offline Buffering:** 네트워크 불안정 시 로컬 캐싱(Local Caching) 후 연결 시 자동 전송 기능
* **Data Integrity:** 모든 기록을 **Append-only Log** 형태로 보관하여 데이터 무결성 보장

---

## 👥 Roles

| Role | Description |
| :--- | :--- |
| **Student (Observer)** | 위치 제보, 신규 고양이 등록 요청, 실시간 정보 조회 |
| **Caregiver (Guardian)** | 전문 돌봄 로그(식단/건강) 작성, 위키 및 영역 정보 편집 |
| **Administrator** | 신규 등록 승인, 권한 관리, 시스템 통계 모니터링 |

---

## 📅 Revision History

| Version | Date | Description |
| :--- | :--- | :--- |
| **v1.00** | 03/27 | First Draft |
| **v1.10** | 03/27 | Actor Roles(Student, Caregiver, Admin) 상세화 |
| **v1.11** | 03/28 | 시스템 다이어그램 및 Glossary 정리 |
| **v1.12** | 03/28 | **Real-time Map 기능 추가 및 문서 고도화 (Current)** |

---

## 👤 Author

* **Name:** 박다래 (Darae Park)
* **Student ID:** 22411841
* **Email:** ret7258@naver.com
* **GitHub:** [@Pdar124](https://github.com/Pdar124)

> **Campus Cat Mate**는 고양이를 아끼는 마음이 유효한 데이터가 되어 더 나은 환경을 만드는 것을 목표로 합니다.
