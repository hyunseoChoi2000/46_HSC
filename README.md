# 안녕하세요, 최현서입니다 👋

AI반도체융합과에서 공부하고 있습니다. 컴퓨터 비전, 온디바이스 AI, 로봇 비전, 반도체 설계 분야의 프로젝트와 실습을 진행해 왔습니다.

## 프로젝트와 실습 🛠️

### 🖐️ 다중 카메라 손 추적을 위한 데이터 생성 — 진행 중

카메라 3대를 이용한 손 자세 추정을 목표로 작업 중입니다. Blender에서 양손 모델과 카메라를 배치하고, 손 크기와 작업 공간의 비율을 조정했습니다. 손 관절의 3D 좌표와 카메라별 2D 투영 좌표를 추출하고, 이미지와 CSV 파일을 연결하는 데이터 생성 작업을 진행했습니다.

### ✊ 가위바위보 모델 학습 및 TFLite 변환

가위·바위·보 3개 클래스를 대상으로 YOLO11n 객체 탐지 모델을 학습하고, 학습된 모델을 TFLite 형식으로 변환했습니다. Raspberry Pi에서는 별도의 MobileNetV2 기반 가위바위보 TFLite 모델을 실행하며 카메라 추론 환경을 실습했습니다.

### ♻️ 재활용품 객체 탐지 모델 학습

YOLOv8 기반 객체 탐지 모델을 학습하고 Precision, Recall, mAP 등의 지표로 학습 결과를 확인했습니다.

### 🤖 ROS 2와 OpenManipulator-X 실습

ROS 2 Humble 환경에서 OpenManipulator-X를 구동하고 MoveIt Servo를 실행했습니다. 이 과정에서 통신과 토크 설정 문제를 다뤘으며, IBVS(Image-Based Visual Servoing)의 개념과 적용 방법을 공부했습니다.

### 📄 PDF 질의응답 파이프라인

PDF 문서를 분할하고 OpenAI 임베딩과 FAISS를 이용해 관련 문서를 검색하는 질의응답 파이프라인을 구성했습니다. 검색된 문서를 LLM에 전달해 답변을 생성하는 방식을 구현했습니다.

### 🔬 반도체 물리 설계 실습

ICC2를 이용한 물리 설계 흐름을 실습했습니다. Placement 단계를 수행하고 WNS, TNS, 인스턴스 수, 면적 등 결과 지표를 확인했습니다.

## 사용해 본 도구와 기술 💻

`Python` `YOLO` `TensorFlow Lite` `ROS 2` `MoveIt Servo` `Raspberry Pi` `Blender` `FAISS` `ICC2`
