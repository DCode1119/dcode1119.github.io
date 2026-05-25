# WillCeph

## 프로젝트 개요

| 항목 | 내용 |
|------|------|
| 기간 | 2013.06 — 2014.03 (10개월) |
| 역할 | 교정 진단 소프트웨어 개발 |
| 제품 | 2D Cephalometric Analysis Software (HDX WILL) |
| 기술스택 | C/C++, MFC (Ribbon), GDI+ |

---

![WillCeph](../assets/images/willceph-screenshot.jpeg)

## 프로젝트 배경

WillCeph는 치과 교정 진단을 위한 2D 두부계측(Cephalometric) 분석 소프트웨어다. 환자 정보 및 영상 관리, 영상 Annotation, Annotation 기반 교정 분석법 적용, 치료 결과 예측 및 시뮬레이션을 지원하는 보조 소프트웨어로, HDX WILL(구 윌메드)에서 개발되었다.

---

## 담당 기능

- **영상 Annotation** — 두부계측 영상의 해부학적 기준점(Landmark)을 지정하고 관리하는 Annotation 구조 및 Viewer GUI 설계·개발
- **교정 분석법 적용** — Annotation된 기준점을 토대로 각종 치과 교정 분석법(Dental Orthodontic analysis)을 적용하여 계측값을 산출
- **예측 및 시뮬레이션** — VTO/STO 기반 진단 시뮬레이션, Growth Simulation(성장 예측), 치료 전후 비교 기능 구현
- 진단 결과 보고서 생성 및 Export 기능 구현

---

## 주요 기술 사항

### Annotation 기반 분석 구조

두부계측 영상에서 교정 진단에 필요한 Landmark(해부학적 기준점)를 지정하고, 이들 간의 각도와 거리를 계측하여 진단 지표로 활용하는 것이 핵심이다. MFC Ribbon 컨트롤을 기반으로 Viewer GUI를 구성하고, GDI+를 사용하여 영상 위에 Annotation을 표시하고 조작할 수 있도록 구현했다.

### 학술적 분석법의 소프트웨어 구현

다양한 교정 분석법(Steiner, Tweed, McNamara, Ricketts 등)을 학술 논문과 표준 교정 진단 기준을 토대로 소프트웨어에 구현했다. 각 분석법은 동일한 Landmark 집합에서 서로 다른 계측 항목과 기준을 사용하므로, 분석법 추가가 용이하도록 구조를 설계했다.

### VTO/STO 기반 치료 시뮬레이션

Annotation 결과를 바탕으로 VTO(Visual Treatment Objective) 및 STO(Surgical Treatment Objective) 시뮬레이션 기능을 구현했다. 치료 전후의 안면 골격 변화를 예측하여 시각화함으로써, 교정 치료 계획 수립과 환자 상담에 활용할 수 있도록 했다. 성장 예측(Growth Forecast) 기능을 통해 장기적인 치료 경과를 추정하는 것도 가능하다.

---

---

## 참고 자료

- HDX WILL, "WillCeph User's Guide"
  - https://hdxwillna.com/wp-content/uploads/2022/04/Will-Ceph-Users-Guide.pdf
  - 동 문서는 HDX WILL North America에서 배포하는 WillCeph 사용자 가이드로, 제품의 전체 기능 및 조작 방법을 포함한다.

---

## 개발 환경

- **언어**: C/C++
- **UI**: MFC (Ribbon Control)
- **그래픽**: GDI+
- **플랫폼**: Windows 기반 GUI 애플리케이션
