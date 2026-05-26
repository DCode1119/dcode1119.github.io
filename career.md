# 경력기술서

| 항목 | 내용 |
|------|------|
| 성명 | 주현철 (Ju Hyun Chul) |
| 연락처 | decaffeine@naver.com |
| 경력 | 17년 8개월 (2008.06 — 2026.03) |
| 주요 언어 | C/C++ |
| 전문 도메인 | Unreal Engine, AI/LLM 응용, 의료영상, 산업제어, 임베디드 |

---

## 경력 요약

C/C++ 기반 소프트웨어 엔지니어로 17년 이상 임베디드 시스템에서 시작하여 의료영상, 산업제어를 거쳐 Unreal Engine 3D 제작도구와 AI/LLM 응용까지 도메인을 확장하며 제품을 개발해왔다. 분석, 설계, 구현, 검증, 운영 등 제품 전 과정을 고려하여 작업의 디테일을 정하고 의견을 교환하는 업무 스타일을 지향한다. 최근 3D 콘텐츠 제작 프로젝트에서 Camera Direction System 설계와 LLM/AI 모델 연동 기능을 개발했다.

| 기간 | 회사 | 역할 | 주요 프로젝트 |
|------|------|------|-------------|
| 2022.11 — 2026.03 | 시나몬스튜디오 | 시니어 프로그래머 | CinevStudio — Unreal Engine 기반 3D 영상 제작도구 |
| 2020.04 — 2022.11 | 인그래디언트 | 시니어 프로그래머 | MediLabel On-premise — 의료영상 Annotation 도구 |
| 2017.01 — 2020.03 | 하이버스 | 개발팀장 과장 | GIPAM3000 전면 HMI — 전력보호감시장치 HMI |
| 2014.06 — 2016.12 | 하이버스 (프리랜서) | MDEC SW 개발 | CMCIS MDEC — 의료장비 프로토콜 게이트웨이 |
| 2012.06 — 2014.03 | 윌메드 | 개발팀 대리 | WillCeph, Dentio — 치과 진단장비 SW |
| 2010.04 — 2012.06 | 하이버스 | 개발팀 사원 | PDK3200, UFSN — 산업장비/센서네트워크 |
| 2008.06 — 2010.03 | 바텍 | 개발팀 사원 | PaX-Primo — 치과용 X선 장비 SW |

---

## 기술 역량

### 언어

C/C++을 주 언어로 사용해왔다. 도메인에 따라 다양한 프레임워크와 플랫폼 위에서 C++을 활용했다 — Qt (크로스플랫폼 UI), Unreal Engine (Camera System, Sequencer), VTK (의료영상 시각화), MFC (Windows GUI), Embedded C++ (임베디드 시스템). 언어 자체의 변화(C++11 이후 현대화)에 맞추어 코드를 유지보수하고, 팀 내 코드 리뷰를 통해 일관된 스타일을 유지하는 데 신경을 썼다.

### 플랫폼 및 프레임워크

| 플랫폼 | 경험 | 비고 |
|--------|------|------|
| Unreal Engine 4/5 | Camera Direction System, Sequence 편집, AI 연동 | 제품 코어 엔진으로 사용, UE4→UE5 마이그레이션 경험 |
| Qt (5/6) | 의료영상 Annotation UI, 산업 HMI, VTK 통합 | Windows + Embedded Linux 교차 플랫폼 |
| MFC | 의료영상 Viewer, Annotation, Ribbon UI | GDI+ 기반 2D 그래픽 |
| Embedded Linux | 크로스컴파일, 디바이스 드라이버 연동, Qt HMI | ARM 타겟, 메모리/성능 제약 대응 |
| WinCE 5.0 | FPGA 연동, Frame Grabber, 디바이스 드라이버 | 임베디드 전용 OS 경험 |

### 도메인

- **의료영상**: DICOM, CT/MRI/Panorama, 2D/3D Visualization, Annotation, Image Chain (RAW→DICOM), Calibration
- **Unreal Engine**: Unreal Engine 4/5, Camera System, Sequencer, MovieRenderQueue, LLM 연동, UE4→UE5 마이그레이션
- **산업제어**: MODBUS-TCP, 보호계전기 HMI, DOT Matrix LED UI, Watchdog, 정적 분석 기반 신뢰성 검증
- **임베디드**: 크로스컴파일, UART/USB/TCP/IP 디바이스 통신, 프로토콜 변환, 리소스 제약 대응
- **AI/LLM**: LLM Function Calling, TensorFlow 모델 통합, AI→제작데이터 변환 레이어, AI 기반 반자동 Annotation

### 개발 환경 및 도구

- **소스 관리**: Git, GitLab, Perforce, SVN
- **빌드 시스템**: CMake, Unreal Build System
- **CI/CD**: 빌드 자동화, 패키징, 배포 파이프라인 운영
- **정적 분석**: Source Insight 기반 코드 분석 및 고객사 리뷰

---

## 주요 프로젝트 상세

### 1. CinevStudio — 3D 영상 콘텐츠 제작 소프트웨어

**기간**: 2022.11 — 2026.03 (3년 5개월, 중간 2개월 이직 및 재입사)
**회사**: 시나몬스튜디오
**역할**: 클라이언트 개발 시니어 프로그래머 (설계·구현·검증 전담)
**기술스택**: C++, Unreal Engine 4/5, LLM Function Calling, Git

#### 프로젝트 개요

CINEV 서비스의 내부 3D 영상 콘텐츠 제작 엔진. 사용자의 텍스트 프롬프트를 LLM이 장면 정의로 변환하고, Unreal Engine이 3D Scene으로 구성하여 렌더링하는 파이프라인의 핵심을 담당했다.

```
사용자 프롬프트
  → LLM: 장면 정의 생성 (Shot 구성, 캐릭터 위치, 카메라, 대사 등)
  → 3D Scene 생성 (Unreal Engine 기반)
  → 렌더링 (MovieRenderQueue)
  → Web 사용자에게 결과 전달
```

#### 주요 설계 및 구현

**Camera Direction System.** 영화 촬영 이론의 구도, 앵글, 움직임 유형을 파라미터화하여 Shot 단위로 정의했다. AutoCamera는 이 Shot 정의와 장면 맥락을 입력받아 적절한 카메라 방향을 결정하는 규칙 기반 시스템으로, LLM이 결정한 Shot 의도를 실제 카메라 움직임으로 변환하는 중간 계층 역할을 한다.

카메라 데이터를 Sequence Keyframe 구조로 일반화하여 저장하고, Unreal Engine의 Camera Actor/Spline과 결합했다. 데이터 모델과 엔진 데이터를 분리하여 UE4→UE5 마이그레이션 시 Camera Data Model 자체는 영향을 받지 않는 구조를 유지했다.

**LLM 연동 및 AI 파이프라인.** LLM Function Calling을 활용해 AI 출력을 구조화된 제작 명령어로 변환했다. AI 생성 결과를 Sequence 데이터로 변환하여 편집 가능한 형태로 제공함으로써, 사람이 검토하고 수정할 수 있도록 했다. AI 결과의 불완전성을 보완하는 구조적 접근을 선택했다.

동기 HTTP 통신이 필요한 LLM 호출 특성상, Unreal Engine의 비동기 HTTP 모듈을 콜백에서 스레드 대기 방식으로 래핑하여 순차적 처리 파이프라인을 구현했다.

**UE5 마이그레이션 대응.** UE4에서 UE5로 전환 시 SequencePlayer 업데이트 메커니즘이 근본적으로 변경되었다. UE4의 `ForceEvaluate`가 UE5에서 의도대로 동작하지 않아, Scene을 명시적으로 갱신하는 우회 구현을 적용했다. 이 과정에서 과다 사용되던 `SetPlayPosition` 호출을 제거하는 부수 효과도 있었다.

**CLI 기반 렌더링 파이프라인.** MovieRenderQueue를 CLI에서 구동하고 Web API를 통해 LevelSequence 렌더링을 요청하는 구조를 구축했다. 컷 전환 시점 Motion Blur 문제와 Lumen 조명 Snapshot 문제를 해결했다.

**Grouped Action System.** 캐릭터 애니메이션 관리 모듈로, 각 Action을 GameplayTags 기반의 Plugin Asset Type으로 설계했다. POC 완료 후 팀에 이관했다.

#### 결과

- Camera Direction System을 통한 제작 워크플로우 개선
- LLM 및 AI 모델 연동으로 텍스트 기반 콘텐츠 생성 파이프라인 확보
- AI 생성 결과물을 편집 가능한 제작 데이터로 통합하는 구조 적용
- UE4→UE5 마이그레이션 대응 및 MovieScene 갱신 문제 해결
- CLI 기반 MovieRenderQueue 파이프라인 구축
- Git 브랜치 전략 및 CI/CD 파이프라인 운영 체계 구축

---

### 2. MediLabel On-premise — 의료영상 Annotation 도구

**기간**: 2020.04 — 2022.11 (2년 8개월, 개발 중단으로 종료)
**회사**: 인그래디언트 (구 재이랩스)
**역할**: 온프레미스 제품 개발 시니어 프로그래머
**기술스택**: C++, Qt, VTK, TensorFlow, REST API, Git

#### 프로젝트 개요

딥러닝 기반 의료영상(CT/MRI) 라벨링 소프트웨어. 2D Slice 기반 Annotation과 3D Volume 데이터 편집(Isocontour, Sculpting)을 지원하고, TensorFlow AI 모델의 분할 결과를 편집 가능한 Label 데이터로 제공하는 온프레미스 제품.

#### 주요 설계 및 구현

**2D-3D Annotation 데이터 일관성.** 2D Slice에서 Polygon으로 그린 영역을 3D Volume 데이터로 변환하고, 역변환도 가능한 구조를 설계했다. 2D 슬라이스 기반 조작 방식(의사/라벨러에게 익숙한)을 유지하면서 3D Volume과의 일관성을 확보했다.

**AI 모델 데이터 변환 레이어.** TensorFlow 모델 출력(세그멘테이션 마스크)을 Polygon/Volume Label 데이터로 변환하는 레이어를 별도 모듈로 분리했다. 노이즈 제거, 경계 스무딩, Label 우선순위 처리를 포함하여, 추후 다른 AI 모델(PyTorch, ONNX 등)로 교체되어도 제품 코어에 영향을 주지 않도록 했다.

**VTK 기반 3D Viewer.** VTK Render Window를 Qt Widget에 임베드하여 Volume Rendering 및 Polygon 조작을 통합했다. Isocontour(CT value 기반 자동 영역 추출)와 Sculpting(3D 브러시 편집) 기능을 구현했다.

#### 결과

- 의료영상 Annotation 온프레미스 제품 핵심 기능 안정화
- 2D/3D 간 일관된 Label 데이터 모델 설계
- AI 모델 독립적인 통합 구조 적용
- REST API 기반 Cloud 연동으로 온프레미스-Cloud 하이브리드 구조 확보
- 2022년 회사 사업 방향 전환으로 개발 중단

---

### 3. GIPAM3000 전면 HMI — 디지털 전력보호감시장치 HMI

**기간**: 2017.01 — 2020.03 (3년 3개월)
**회사**: 하이버스 (LS Electric 외주 프로젝트)
**역할**: 개발팀장 과장
**기술스택**: C++, Qt, Embedded Linux, MODBUS-TCP, SVN

#### 프로젝트 개요

LS Electric GIPAM3000 디지털 전력보호감시장치의 전면 HMI Application. Windows(개발환경)와 Embedded Linux(타겟) 교차 플랫폼에서 동작하며, 34종의 보호 요소 설정/계측값 표시/사고 이력 조회를 제한된 DOT Matrix LED와 버튼 인터페이스에서 제공한다.

#### 주요 설계 및 구현

**스크립트 기반 동적 UI 구성.** 보호 요소별 파라미터가 스프레드시트로 관리되는 환경에서, CSV 리소스 파일을 파싱하여 메뉴 계층을 동적으로 구성하고 MODBUS 통신 인터페이스를 자동 연결하는 방식을 채택했다. 새로운 보호 요소 추가 시 스프레드시트만 갱신하면 UI가 자동 반영된다. 제품별(FI형/T형)로 다른 보호 요소 구성을 유연하게 대응할 수 있었다.

**하드웨어가 없는 상태에서의 MODBUS 개발.** 초기 개발 단계에서 실제 MODBUS 장비가 없어, 시뮬레이션 서버 → 기존 MODBUS 장비 → 실제 GIPAM3000 순으로 단계적 검증을 진행했다. 하드웨어 개발 일정에 블로킹되지 않고 SW 개발을 병행할 수 있었다.

**프레임버퍼 렌더링 문제 해결.** DOT Matrix LED에서 화면 전환 시 Tearing과 잔상 문제가 발생했다. 이전 화면 완전 소거 후 새 화면 렌더링, 렌더링 완료까지 입력 차단 방식으로 해결했으나, 버튼 채터링으로 인한 입력 먹통 현상이 새로 발생했다. 입력 디바운스 처리와 모달/화면전환 상태 분리 관리로 최종 해결했다.

**Watchdog 기반 장애 복구.** Application이 주기적으로 Watchdog 타이머에 pulse를 전송하고, OS 레벨에서 pulse 미감지 시 강제 재부팅하는 구조로, 사람 개입 없는 복구 체계를 구현했다.

**정적 분석 기반 신뢰성 확보.** Source Insight 정적 분석을 정기 수행하여 메모리 누수, 널 포인터, 리소스 해제 누락을 조기에 발견했다. 고객사(LS Electric) SW 전담 조직과 분석 결과를 공유하고 리뷰했다. 고객사 QA와 협력하여 온도/습도/Surge 등 물리적 환경 조건을 포함한 실제 환경 기반 장시간 테스트를 수행했다.

#### 결과

- GIPAM3000 전면 HMI Application 안정화 및 제품 출시
- 데이터 모델과 UI 분리로 보호 요소 추가/변경 유연성 확보
- 스크립트 기반 동적 UI로 제품 모델별 대응 가능
- 교차 플랫폼 대응 (Windows + Embedded Linux)
- 정적 분석과 실제 환경 테스트를 통한 신뢰성 확보

---

### 4. CMCIS MDEC — 의료장비 프로토콜 게이트웨이

**기간**: 2014.06 — 2016.12 (2년 7개월)
**형태**: 프리랜서 (하이버스)
**기술스택**: C/C++, Linux (ARM), UART, USB, TCP/IP

#### 프로젝트 개요

국책과제 CMCIS의 MDEC(Medical Device Exchange Communication) 게이트웨이 장비 개발. 각기 다른 통신 프로토콜을 가진 6종의 심장학 의료장비 데이터를 수신하여 CMCIS 표준 프로토콜로 변환·중계하는 임베디드 시스템.

#### 주요 설계

장비별 통신 방식(UART/USB)과 데이터 포맷의 차이를 물리 계층과 프로토콜 계층으로 분리하여 장비 추가 시 변경 범위를 최소화했다. 실시간 생체 데이터 특성을 고려하여 패킷 손실 시 지연된 재전송보다 최신 데이터 위주 전송을 선택했다. 제한된 임베디드 환경에서 장비별 수신 버퍼와 처리 주기의 트레이드오프를 검토했다.

---

### 5. WillCeph — 치과 교정 진단 분석 소프트웨어

**기간**: 2013.06 — 2014.03 (10개월)
**회사**: 윌메드
**기술스택**: C/C++, MFC (Ribbon), GDI+

#### 주요 기능

두부계측(Cephalometric) 영상의 해부학적 기준점(Landmark) Annotation 구조 및 Viewer GUI 설계. Steiner, Tweed, McNamara, Ricketts 등 다양한 교정 분석법을 학술 기준에 맞춰 구현했다. VTO/STO 기반 치료 시뮬레이션과 성장 예측(Growth Simulation) 기능을 개발했다. 분석법 추가가 용이하도록 Landmark 집합과 분석 로직을 분리했다.

---

### 6. Dentio — 치과용 통합 X선 촬영장비

**기간**: 2012.06 — 2013.06 (1년)
**회사**: 윌메드
**기술스택**: C/C++, Teledyne Dalsa CMOS, DICOM

#### 주요 기능

파노라마와 세팔로메트릭 촬영을 통합한 All-in-One X선 시스템. 센서 공급사(Teledyne Dalsa) 엔지니어와 협업하여 CMOS 디텍터를 선정하고, RAW 데이터에서 최종 의료영상까지의 Image Chain(Flat field correction, Gain/Offset 보정, 노이즈 저감, TDI 정렬, 16bit gray scale 매핑)을 구현했다. 제조 현장의 장비별 센서 편차 보정을 위한 Calibration Application을 개발했다.

---

### 7. PDK3200 — OLED/LCD Tester & Demo Kit

**기간**: 2011.08 — 2012.06 (10개월)
**회사**: 하이버스
**기술스택**: Embedded SW, Windows Application, C/C++

임베디드(패널 구동 타이밍/신호 생성)와 Windows Application(테스트 시나리오 관리/UI)을 동시 개발. Pattern Generator는 이미지 렌더링이 아닌 픽셀 단위 dot 출력 방식으로, 다양한 해상도 LCD 패널에 정확한 픽셀 출력을 보장했다.

---

### 8. UFSN — 지하시설물 센서 네트워크

**기간**: 2010.04 — 2011.08 (16개월)
**기관**: 전자부품연구원(KETI) 외주
**기술스택**: PLC, 유무선 네트워크, lighttpd + PHP, C/C++

도시 지하시설물(배수로, 관로) 상태 모니터링을 위한 USN 기반 센서 네트워크 시스템. PLC 통신 인터페이스, 유무선 네트워크 이중화, 경량 웹서비스(lighttpd+PHP) 구축. 연구 성과는 한국정보통신설비학회 논문지에 게재.

---

### 9. PaX-Primo — 치과용 디지털 파노라마 X선 장비

**기간**: 2009.10 — 2010.03 (6개월)
**회사**: 바텍
**기술스택**: WinCE 5.0, Embedded C/C++, FPGA

WinCE 5.0 기반 임베디드 시스템. FPGA를 이용한 Frame Grabber를 직접 구현하여 센서 RAW 영상 데이터를 시스템 메모리에 공유 영역으로 매핑하고 응용 SW가 접근하는 구조를 개발했다. 외부와의 물리적 인터페이스를 Ethernet 하나로 단일화하여 PC가 필요 없던 기존 구성에서 장비 단독 납품이 가능하도록 했다.

---

## 엔지니어링 접근 방식

### 문제 해결의 레이어

제품 개발에서 중요하게 생각하는 것은 **문제를 어떤 레이어에서 해결할지 결정하는 것**이다. 동일한 기능 요구라도 데이터 모델, 통신 인터페이스, 사용자 경험 중 어느 계층에서 해결하느냐에 따라 시스템의 유지보수성과 확장성이 달라진다.

실제 사례:
- **CinevStudio**: Camera 데이터를 Sequence Keyframe 구조로 일반화하여 Unreal Engine 업데이트 영향에서 데이터 모델을 분리
- **MediLabel**: AI 모델 출력을 Label 데이터로 변환하는 레이어를 분리하여 모델 종류 교체에 독립적인 구조 확보
- **GIPAM3000**: 스프레드시트 기반 동적 UI 구성으로 보호 요소 추가 시 UI 코드 변경 불필요

### 구조적 판단의 기준

코드베이스의 변경 비용을 줄이기 위해 다음 질문을 일관되게 적용한다:

- 이 기능이 시간이 지나면서 어떻게 변할 것인가?
- 어떤 계층에 변경이 생겼을 때 영향 범위는 어디까지인가?
- 엔진이나 라이브러리 업데이트가 발생하면 어느 부분이 깨질 위험이 있는가?
- AI 모델의 출력 품질이 변해도 시스템이 동작할 수 있는가?

### 개발 방식

17년간 다양한 규모의 팀(2-3인 소규모부터 10인 이상 팀)에서 일해왔다. 소규모 팀일수록 개인의 end-to-end 책임 범위가 넓어 요구사항 분석부터 설계·구현·검증·운영까지 전 과정을 수행했다.

코드 리뷰와 정적 분석 도구를 활용한 품질 관리, Git 기반 브랜치 전략과 CI/CD 파이프라인 운영, 고객사 QA와의 협업을 통한 검증 등 팀의 개발 프로세스 개선에도 참여해왔다.

---

## AI 모델 활용 경험

AI 경험을 LLM 기반 제작 파이프라인과 학습모델 통합의 두 축으로 나눈다.

### LLM 기반 제작 파이프라인 (CinevStudio)

CinevStudio에서는 LLM을 제품 경험의 전면에 두었다. 사용자 텍스트 프롬프트 → LLM 장면 정의 → Unreal Engine 3D Scene → 렌더링으로 이어지는 파이프라인에서, LLM 기능의 REST API 설계와 Application 측 처리 구조를 담당했다.

**REST API 설계 및 Data Schema 협의.** LLM 기능을 Application에서 사용하기 위해 REST API 형태로 인터페이스를 정의했다. 요청/응답 데이터 구조(Schema)를 설계하고, AI 엔지니어 및 기획팀과 협의하여 API 명세를 확정했다. LLM 출력(JSON)은 Sequence 생성 명령어로 매핑되어 3D Scene 구성의 입력으로 사용되었다.

**AI 결과의 중간 표현.** LLM 응답을 그대로 사용하지 않고, 편집 가능한 Sequence Keyframe 데이터로 변환하는 중간 레이어를 두었다. 이를 통해 AI 생성 결과를 사용자가 검토하고 수정할 수 있도록 했다. AI 출력의 불완전성을 구조적으로 보완하는 접근으로, 제작자의 의도가 반영된 최종 Scene을 구성할 수 있게 했다.

**동기 HTTP 통신 처리.** Unreal Engine의 HTTP 모듈은 비동기 콜백 기반이지만, LLM 호출 후 결과를 기다려 다음 처리로 이어져야 하는 파이프라인 특성상 동기(blocking) 방식이 필요했다. 비동기 요청의 콜백에서 결과 도착까지 스레드를 대기시키는 래퍼를 구현하여 순차적 처리 흐름을 유지했다.

### 학습모델 통합 (MediLabel)

MediLabel에서는 TensorFlow 기반 의료영상 분할 모델의 출력을 제품 내 Label 데이터로 통합하는 변환 레이어를 설계했다. LLM과 달리 이 프로젝트는 학습모델의 출력(세그멘테이션 마스크)을 Polygon/Volume Label로 변환하여 Annotation 도구의 기능으로 제공하는 데 중점을 두었다.

**AI 모델 독립적 변환 레이어.** TensorFlow 세그멘테이션 마스크를 Label 데이터로 변환하는 모듈을 별도 레이어로 분리했다. 노이즈 제거, 경계 스무딩, Label 우선순위 처리를 포함하여, 추후 다른 AI 모델(PyTorch, ONNX 등)로 교체되어도 제품 코어에 영향을 주지 않도록 했다.

**2D-3D 데이터 일관성.** AI 모델 출력은 3D Volume(픽셀 단위 마스크)이지만, 실제 라벨러가 조작하는 단위는 2D Slice Polygon이었다. 2D Polygon과 3D Volume Label 간 양방향 변환 구조를 정의하여, AI 생성 결과를 익숙한 2D 조작 방식으로 편집할 수 있도록 했다.

---

## Agent 기반 개발 경험

전 직장에서 Agent 기반 개발 방식이 사내 트렌드로 자리잡기 시작하면서 관련 방법론을 습득하고 현업에 적용하기 시작했다. 퇴사 후 개인 Unreal Engine 프로젝트에서 Agent 기반 개발 환경을 직접 구성하여 운영 중이다.

### 문서 기반 Agent 행동 정의

Agent의 행동을 계층화된 문서로 정의했다. `AGENTS.md`에 핵심 원칙(Simplicity First, Surgical Changes, Goal-Driven Execution)을 두고, 구체적인 업무 절차는 `Doc/Process/` 디렉토리 아래 개별 문서로 분리했다. 상세 워크플로우가 `AGENTS.md`에 비대해지면 `Doc/Process/`로 이동시키는 규칙을 통해 문서 간 책임 범위를 유지했다.

- **AGENTS.md**: 핵심 원칙, 프로젝트 컨텍스트, 코딩 컨벤션
- **Doc/Process/**: 문서 관리, Git 운영, Safeguard, 세션 복원 절차
- **Doc/Planning/**: 기획, 백로그, 향후 작업
- **Doc/Daily/**: 작업 일지 (Agent Work / User Work 분리)

### Goal-Driven Execution

모든 작업을 검증 가능한 목표로 변환하는 방식을 적용했다. 단순한 지시("버그 수정") 대신 재현 조건과 확인 기준을 명시("재현 테스트 작성 → 통과 → 수정 → 테스트 재통과")하여 Agent가 독립적으로 반복 작업을 수행할 수 있도록 했다. 다단계 작업은 단계별 확인 조건을 사전에 정의하고 순차적으로 실행했다.

### 작업 일지와 세션 복원

매 작업 세션의 결과를 `Doc/Daily/{날짜}/notes.md`에 기록한다. Agent가 직접 수행한 코드 편집/분석/문서 갱신은 **Agent Work**, Agent 안내에 따라 사용자가 직접 실행한 Unreal Editor 조작(BP 편집, PIE 튜닝)은 **User Work**로 분리하여 기록한다. 각 작업 단위는 **목표 → 수정 파일 목록 → 검증 결과** 순서로 정리한다.

새 세션 시작 시 `SESSION_START.md`에 정의된 복원 순서(`AGENTS.md → Doc/README.md → 최신 Daily notes → Planning 문서`)를 통해 일관된 컨텍스트를 복원한다.

### Safeguard 자동화

반복되는 실패 패턴을 문서화 대신 자동화된 검사 도구로 방어한다. Git pre-commit hook, Python 검증 스크립트를 통해 오류 발생 → 원인 분석 → Safeguard 생성 → 시스템 통합 → 모니터링 사이클을 운영한다. 단순한 규칙 나열이 아니라 실행 가능한 검사로 실패를 차단하는 접근이다.

### 지식 그래프를 통한 코드베이스 분석

코드베이스 분석에 knowledge graph(graphify)를 활용한다. 소스 코드를 AST 기반 지식 그래프로 구축하고, 파일 검색(grep)보다 그래프 탐색을 우선하여 모듈 간 관계와 의존성을 파악한다. 코드 수정 후 그래프를 갱신하여 최신 상태를 유지한다.

---

## 도메인 경험 맵

```
2008                2012                2016                2020                2024
├─── 바텍 ───┤─── 윌메드 ────┤─── 하이버스(프리랜서) ─┤─── 인그래디언트 ─┤─── 시나몬스튜디오 ─┤
│            │              │                        │                   │
│ 의료영상    │ 의료영상      │ 의료장비 프로토콜        │ 의료영상 AI       │ 3D 콘텐츠 제작    │
│ (X선 장비)  │ (진단 SW)    │ (국책과제)              │ (Annotation)      │ (Unreal Engine)  │
│ WinCE      │ MFC/GDI+    │                        │ Qt/VTK           │ UE4/UE5          │
│ FPGA       │              │─── 하이버스 ───────────┤                   │ LLM/AI           │
│            │              │ 산업 HMI                │                   │                   │
│            │              │ Embedded Linux/Qt      │                   │                   │
│            │              │ MODBUS                 │                   │                   │
│            │              │                        │                   │                   │
│            │              │─── 하이버스(초기) ──────┤                   │                   │
│            │              │ OLED/LCD Tester        │                   │                   │
│            │              │ 센서네트워크            │                   │                   │
│            │              │                        │                   │                   │
├─ 임베디드 ─┤─── 의료영상 ───┤─── 의료 + 산업 ────────┤─── 의료영상 AI ───┤─── 3D + AI ──────┤
```

---

*이 문서는 경력기술서, 이력서 및 프로젝트 문서를 기반으로 작성되었습니다.*
