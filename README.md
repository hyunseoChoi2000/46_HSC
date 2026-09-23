# 안녕하세요, 최현서입니다 👋

AI반도체융합과에서 공부하고 있습니다. 반도체 기반에 AI 기술이 결합된 분야(AI 반도체, 온디바이스 AI)에 관심을 두고,
컴퓨터 비전, 온디바이스 AI, 로봇 비전, 반도체 설계 분야의 프로젝트와 실습을 진행해 왔습니다.

## 🤖 AI · 컴퓨터 비전

### 🎤 Mock Interview AI — AI 면접 보조 프로그램
웹캠 영상·음성·답변을 실시간으로 분석해 면접 피드백을 제공하는 프로그램입니다.
- **구조**: Webcam/Mic → React(Vite) → WebSocket → FastAPI → 분석 모듈 → Gemini API → 피드백
- **영상 분석**: MediaPipe·OpenCV로 표정과 자세 분석
- **음성 분석**: librosa로 Mel Spectrogram, RMS, 무음 구간 분석 / Web Speech API 기반 실시간 STT
- **백엔드**: FastAPI Router, JWT 인증, WebSocket ConnectionManager, 파일 업로드

🔗 [Interview-Help-AI](https://github.com/Kangnagi/Interview-Help-AI)

### 🖐️ 다중 카메라 3D 손 추적을 위한 합성 데이터 생성 — 진행 중
카메라 3대를 이용한 3D 손 자세 추정을 목표로, 딥러닝 학습용 합성 데이터를 만들고 있습니다.
- Blender에서 양손 모델과 카메라 3대를 배치하고, 손 크기와 작업 공간의 비율 조정
- MediaPipe 21개 관절 기준으로 손 관절의 3D 좌표와 카메라별 2D 투영 좌표 추출
- 렌더링 이미지와 좌표 CSV를 연결하는 데이터셋 생성 파이프라인 구성

### ♻️ 재활용품 객체 탐지 및 세그멘테이션
YOLOv8 기반으로 학습하며 bbox 탐지에서 Segmentation으로 전환했습니다.
- 데이터 수집, 라벨링, 품질 검사를 직접 진행
- Precision, Recall, mAP 지표로 학습 결과 확인
- 유리와 투명 플라스틱의 오분류 원인을 분석하며, 모델 구조보다 **데이터 품질과 라벨링 기준**이 성능을 크게 좌우한다는 점을 확인

### ✊ 가위바위보 모델 학습 및 온디바이스 추론
- 가위·바위·보 3개 클래스로 YOLO11n 객체 탐지 모델을 학습하고 TFLite 형식으로 변환
- Raspberry Pi에서 MobileNetV2 기반 TFLite 모델로 카메라 실시간 추론 환경 실습

### 📄 PDF 질의응답 파이프라인 (RAG)
- PDF 문서를 분할하고 OpenAI 임베딩과 FAISS로 관련 문서 검색
- 검색된 문서를 LLM에 전달해 답변을 생성하는 구조 구현

## 🔬 반도체

### 디지털 반도체 설계 흐름 실습 (Synopsys)
RTL부터 물리 설계까지 디지털 설계 흐름을 실습했습니다.
- **Design Compiler**: 설계 읽기, .sdc 제약 조건 작성, 논리 합성
- **PrimeTime**: Timing Report 분석, Setup/Hold Violation 확인
- **Timing Closure**: ECO 적용, Buffer 삽입과 Cell Sizing
- **ICC2**: Placement 수행 후 WNS, TNS, 인스턴스 수, 면적 지표 확인

### 레이아웃 및 회로 설계 실습
- CMOS 레이아웃, NAND/NOR·전가산기·OP AMP 설계
- D 플립플롭 레이아웃, 6TR SRAM Cell 설계

### 반도체 장비 제어 실습
- PLC 기초와 GX Works2 래더 프로그래밍
- 솔레노이드 밸브·실린더 제어, MFC 유지보수
- 웨이퍼 핸들링과 챔버 Gate 시스템 운용

## 🦾 로보틱스

### ROS 2와 OpenManipulator-X 실습
- ROS 2 Humble 환경에서 OpenManipulator-X 조립 및 구동, Gazebo 시뮬레이션
- YOLO 인식 결과를 로봇 팔 Pick & Place로 연계
- MoveIt Servo 실행 과정에서 통신과 토크 설정 문제 해결
- IBVS(Image-Based Visual Servoing)의 개념과 적용 방법 학습

## 💻 사용해 본 도구와 기술

**AI/ML** `PyTorch` `YOLO` `OpenCV` `MediaPipe` `TensorFlow Lite` `librosa` `FAISS`

**반도체** `Design Compiler` `PrimeTime` `ICC2` `GX Works2`

**SW/시스템** `Python` `C/C++` `FastAPI` `React` `SQL` `Linux` `Git`

**로보틱스/HW** `ROS 2` `MoveIt Servo` `Gazebo` `Raspberry Pi` `Blender`

## 📫 Contact
- Email: gustj0527@naver.com
