# 주현철

17년 이상 경력의 C/C++ 소프트웨어 엔지니어입니다. 의료영상, 산업제어, 임베디드, 실시간 3D 콘텐츠 제작도구 등 다양한 도메인에서 제품 개발을 해왔습니다. 요구사항 분석부터 설계, 구현, 검증 및 운영까지 일관되게 책임지는 업무 방식을 유지하고 있습니다.

---

## 대표 프로젝트

### [CinevStudio](./projects/cinevstudio.md)

Unreal Engine 기반 3D 영상 콘텐츠 제작 소프트웨어. Camera Direction System, Sequence 편집, LLM 및 AI 모델 연동 기능을 설계하고 구현했습니다. AI 생성 결과물을 편집 가능한 제작 데이터로 변환하여 제작 파이프라인에 통합하는 구조를 적용했습니다.

### [MediLabel On-premise](./projects/medilabel.md)

인그래디언트(Ingradient)에서 개발한 딥러닝 기반 의료영상 Labeling 도구. 2D 슬라이스 기반 Annotation과 3D Volume 데이터 편집(Isocontour, Sculpting) 기능을 구현했습니다. TensorFlow AI 모델의 출력을 Label 데이터로 변환하는 레이어를 설계하여 모델 종류에 독립적인 통합 구조를 구성했습니다. (2022년 개발 중단으로 프로젝트 종료)

### [GIPAM3000 전면 HMI](./projects/gipam-hmi.md)

LS Electric GIPAM3000 디지털 전력보호 감시장치의 전면 HMI Application. Qt와 Embedded Linux 기반으로 보호계전기의 상태 표시, 보호 요소 설정 편집, MODBUS-TCP 통신 기능을 개발했습니다. Source Insight 정적 분석과 고객사 QA 협력을 통한 장시간 신뢰성 검증을 수행했습니다.

---

## Engineering

제품 개발에서 중요하게 생각하는 것은 문제를 어떤 레이어에서 해결할지 결정하는 것입니다. 동일한 기능 요구라도 데이터 모델, 통신 인터페이스, 사용자 경험 중 어느 계층에서 해결하느냐에 따라 시스템의 유지보수성과 확장성이 달라집니다.

2D-3D 데이터 간 일관성 유지, AI 모델 출력과 제작 데이터 간 변환 레이어 분리, 교차 플랫폼 추상화 — 이 구조적 결정들이 시간이 지나면서 시스템의 변경 비용을 결정했습니다.

---

## AI / Agent

최근 생성형 AI와 Agent 기반 개발 방식에 관심을 가지고 있습니다. LLM Function Calling을 활용하여 AI 모델의 출력을 구조화된 제작 명령어로 변환하고, 이를 제작 파이프라인에 통합한 경험이 있습니다. Agent를 통한 개발 자동화 및 워크플로우 통합을 실무에 적용 중입니다.

---

