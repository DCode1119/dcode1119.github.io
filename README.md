# Portfolio

## Introduce

- **Nickname**: DCode
- **Name**: 주현철
- **Contact**: decaffeine@naver.com

---

## Core Skills

| 분류 | 내용 |
|---|---|
| **언어** | C/C++ |
| **플랫폼 / 엔진** | Unreal Engine 4/5, Qt, MFC, Linux, Windows |
| **도메인** | Unreal Engine, AI/LLM 응용, 의료영상, 산업제어, 임베디드 |
| **Etc** | Git, GitLab, Perforce, CI/CD |

---

17년 이상 경력의 C/C++ 소프트웨어 엔지니어입니다. 임베디드 시스템에서 시작하여 의료영상, 산업제어를 거쳐 Unreal Engine 3D 제작도구와 AI/LLM 응용까지 도메인을 확장하며 제품을 개발해왔습니다. 분석, 설계, 구현, 검증, 운영 등 제품 전 과정을 고려하여 작업의 디테일을 정하고 의견을 교환하는 업무 스타일을 지향합니다.

---

## Engineering

제품 개발에서 중요하게 생각하는 것은 문제를 어떤 레이어에서 해결할지 결정하는 것입니다. 동일한 기능 요구라도 데이터 모델, 통신 인터페이스, 사용자 경험 중 어느 계층에서 해결하느냐에 따라 시스템의 유지보수성과 확장성이 달라집니다.

2D-3D 데이터 간 일관성 유지, AI 모델 출력과 제작 데이터 간 변환 레이어 분리, 교차 플랫폼 추상화 — 이 구조적 결정들이 시간이 지나면서 시스템의 변경 비용을 결정했습니다.

---

## AI 모델 활용

LLM 기반 제작 파이프라인(CinevStudio)과 학습모델 통합(MediLabel) 두 축으로 구성된다. CinevStudio에서는 LLM 기능의 REST API를 설계하고 AI 출력을 편집 가능한 제작 데이터로 변환하는 파이프라인을 구축했다. MediLabel에서는 TensorFlow 모델 출력을 Label 데이터로 변환하는 모델 독립적 레이어를 설계했다.

---

## Agent 기반 개발

사내 트렌드에서 시작하여 퇴사 후 개인 Unreal Engine 프로젝트에서 직접 Agent 개발 환경을 구성해 운영 중이다. 계층화된 문서로 Agent 행동을 정의하고, Goal-Driven Execution, 작업 일지/세션 복원, Safeguard 자동화, knowledge graph(graphify) 기반 코드 분석을 적용하고 있다.

---

## Major Projects

### [CinevStudio](./projects/cinevstudio.md)

Unreal Engine 기반 3D 영상 콘텐츠 제작 소프트웨어. Camera Direction System, Sequence 편집, LLM 및 AI 모델 연동 기능을 설계하고 구현했습니다. AI 생성 결과물을 편집 가능한 제작 데이터로 변환하여 제작 파이프라인에 통합하는 구조를 적용했습니다.

### [MediLabel On-premise](./projects/medilabel.md)

인그래디언트(Ingradient)에서 개발한 딥러닝 기반 의료영상 Labeling 도구. 2D 슬라이스 기반 Annotation과 3D Volume 데이터 편집(Isocontour, Sculpting) 기능을 구현했습니다. TensorFlow AI 모델의 출력을 Label 데이터로 변환하는 레이어를 설계하여 모델 종류에 독립적인 통합 구조를 구성했습니다. (2022년 개발 중단으로 프로젝트 종료)

### [GIPAM3000 전면 HMI](./projects/gipam-hmi.md)

LS Electric GIPAM3000 디지털 전력보호 감시장치의 전면 HMI Application. Qt와 Embedded Linux 기반으로 보호계전기의 상태 표시, 보호 요소 설정 편집, MODBUS-TCP 통신 기능을 개발했습니다. Source Insight 정적 분석과 고객사 QA 협력을 통한 장시간 신뢰성 검증을 수행했습니다.

---

## Legacy - Industrial Projects

### [UFSN — Underground Facility Sensor Network](./projects/minor/ufsn.md)

전자부품연구원(KETI) 외주 프로젝트. 도시 지하시설물 관리를 위한 USN 기반 센서 네트워크 시스템. PLC 통신, 유무선 이중화, lighttpd+PHP 웹서비스 구축.

### [PDK3200](./projects/minor/pdk3200.md)

Hybus(하이버스) OLED/LCD Tester & Demo Kit. 임베디드 SW + Windows Application 병행 개발, Pattern Generator(픽셀 직접 dot 출력).

---

## Legacy - Medical Projects

### [PaX-Primo](./projects/minor/pax-primo.md)

Vatech 치과용 디지털 파노라마 X선 촬영장비. WinCE 5.0 임베디드 시스템, FPGA 기반 Frame Grabber, Ethernet 단일 인터페이스.

### [WillCeph](./projects/minor/willceph.md)

HDX WILL 2D Cephalometric 분석 소프트웨어. MFC Ribbon + GDI+ 기반, Annotation/교정 분석법/VTO·STO 시뮬레이션.

### [Dentio](./projects/minor/dentio.md)

HDX WILL 파노라마 + 세팔로메트릭 겸용 X선 장비. Teledyne Dalsa CMOS 센서 협업, Image Chain 구현, Calibration Application 개발.

### [CMCIS — MDEC Protocol Gateway](./projects/minor/cmcis.md)

국책과제 CMCIS의 MDEC 프로토콜 게이트웨이 장비. 군 의료정보체계 프로토콜을 Ethernet TCP/IP로 변환, Linux 포팅, UART/USB 디바이스 드라이버 및 웹 기반 모니터링 UI 개발.

---