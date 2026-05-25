# Dentio (HDX WILL)

## 프로젝트 개요

| 항목 | 내용 |
|------|------|
| 기간 | 2012.06 — 2013.06 (1년) |
| 역할 | Image System Engineering |
| 제품 | 치과용 디지털 파노라마 + 세팔로메트릭 X선 촬영장비 |
| 주요 협력 | Teledyne Dalsa (CMOS 센서) |

---

> HDX WILL(당시 윌메드) 재직 시절 참여한 제품으로, 파노라마(panorama)와 세팔로메트릭(cephalometric) 촬영을 하나의 장비로 통합한 All-in-One 치과용 X선 시스템이다.

## 프로젝트 배경

HDX WILL은 2008년 설립된 치과용 영상장비 업체다. Dentio는 기존 파노라마 단독 장비에 세팔로메트릭 촬영 기능을 통합한 제품으로, CMOS 센서 기반 디지털 영상 획득과 TDI(Time Delay Integration) 기술을 적용했다. 주요 스펙으로는 50-90 kV, 0.5mm focal spot, 16bit gray scale, Panorama 14.2초(Normal) / 7초(Fast), Cephalo 8.2초(Normal) / 4.2초(Fast) 스캔 시간을 지원했다.

---

## 담당 범위

- 제품 개발 컨셉에 대한 사내 기술 공유 및 논의
- X선 CMOS 센서 선정 및 공급사(Teledyne Dalsa) 엔지니어와의 기술 협업
- 센서 RAW 데이터로부터 최종 의료영상까지의 **Image Chain** 구현
- 제조 현장 지원을 위한 **Calibration Application** 개발
- 제품/생산 과정에서 발생하는 문제에 대한 진단 및 분석 대응

---

## 주요 기술 사항

### 센서 선정 및 Teledyne Dalsa 협업

Dentio에 사용할 CMOS 디텍터 선정 과정에 참여했으며, 공급사인 Teledyne Dalsa의 엔지니어들과 직접 기술 협업을 진행했다. 센서의 전기적 특성, 노이즈 프로파일, 프레임 레이트, 해상도 등이 의료영상 획득에 적합한지 평가하고, 장비 구조와 센서 간 인터페이스를 정의했다.

### Image Chain 구현

센서에서 출력되는 RAW 데이터를 최종 진단용 의료영상으로 변환하는 **Image Chain**을 구현했다. 이는 RAW 데이터 보정(Flat field correction, Gain/Offset 보정), 노이즈 저감, TDI 정렬, 16bit gray scale 매핑 등의 전처리 과정을 포함한다. 최종 영상은 Will-Master PACS를 통해 DICOM 포맷으로 저장·관리되었다.

### Calibration Application

제조 과정에서 각 장비별로 센서 편차를 보정하고 일정한 이미지 품질을 확보하기 위한 **Calibration Application**을 개발했다. 생산 라인에서 장비 조립 후 센서 특성을 측정하고 보정 파라미터를 산출하여 장비에 적용하는 도구로, 제조 품질 안정화에 기여했다.

### 문제 진단 및 분석

제품 개발 단계 및 초기 양산 과정에서 발생하는 이미지 이상(노이즈, 왜곡, 불균일 보정 실패 등)에 대한 원인 진단과 분석을 수행했다. 센서, 이미지 체인, 기구적 정렬 등 여러 레이어에서 문제의 근본 원인을 식별하고 해결 방안을 제시했다.

---

## 개발 환경

- **언어**: C/C++
- **센서**: Teledyne Dalsa CMOS 디텍터
- **이미지 포맷**: DICOM 3.0
- **플랫폼**: Windows
