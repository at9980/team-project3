# 에코(echo): 반려동물의 마음을 들여다 보는 챗봇

**에코(echo)**는 반려동물의 영상을 분석하여 감정과 이상행동, 통증여부를 알려주고, 사용자의 채팅을 통해 반려동물의 문제행동을 분석하여 솔루션을 제공해주는 AI 입니다. 사용자는 에코를 통해 반려동물의 감정과 행동을 더욱 잘 이해할 수 있으며, 반려동물의 통증을 사전에 캐치하여 조기에 치료할 수 있습니다.
반려동물과 보호자들의 삶의 질과 행복을 지켜주는 서비스를 제공하는 것이 목표입니다..

---

## 1. 프로젝트 개요

- **프로젝트 명**: 반사모 (반려동물을 사랑하는 사람들의 모임)
- **목표**: 반려동물의 감정 분석과 문제행동을 분석하여 솔루션을 제공하는 AI 멀티 서비스 개발
- **주요 기능**: 
  - 공감형 반응 및 질문 제공
  - 감정 분석 및 대화 유도
  - TTS(텍스트 음성 변환) 기능

---

## 2. 프로젝트 일정

- **9/18 or 9/19**: 첫 정식 미팅 (온라인)
- **9/27**: 참가팀 발표
- **~10/20**: 데모 버전 완성
- **10/21 ~ 10/23**: 리팩토링 및 최적화
- **10/24 ~ 10/26**: 테스트 및 디버깅
- **10/28**: 데모 버전 제출
- **11/8**: 본선팀 진출 발표

---

## 3. 팀 구성 및 역할

| **이름**     | **역할**         | **주 업무**                  | **부 업무**                 |
|--------------|------------------|------------------------------|-----------------------------|
| 김홍준       | PM               | 매니지먼트                   | 어시스턴스, TTS 작업         |
| 류윤선       | AI 개발          | AI 모델 개발                 | AI 모델 테스트, 프롬프트 엔지니어링 |
| 이현석       | 데이터           | 데이터 수집                  | 파인튜닝(RAG-Retriever)      |
| 박지환       | DB 구축/연동     | DB 구축                      | -                           |
| 안동현       | 풀스택           | 백엔드 개발                  | 프론트엔드 개발             |
| 김창미       | AI 개발          | AI (Yolo-v8) 개발            | DB 관리 (Docker)            |

---

## 4. 프로젝트 환경

| **구분**      | **설명**                                                                                |
|---------------|----------------------------------------------------------------------------------------|
| **개발환경**  | Python, JavaScript, TypeScript                                                         |
| **협업공간**  | Google Drive, Notion, Git, GitHub                                                      |
| **개발 도구** | Colab, Jupyter Notebook, VScode, AWS, Docker Compose                                   |
| **AI 솔루션** | OpenAI API(GPT-4o-mini), Langchain, Langchain-Memory Buffer, Prompt Engineering, RAG   |
| **웹 개발**   | React, Node.js + Express, React Native                                                 |
| **데이터**    | AI Hub 감정 분석 데이터셋, 유튜브 교통사고 통계 데이터                                  |

---

## 5. 시스템 아키텍처
![시스템 아키텍처](https://prod-files-secure.s3.us-west-2.amazonaws.com/1352b1ae-a6bb-4248-a0fd-73c3c63ea9d0/b6f481b8-c908-4f8f-9499-74d58a005d27/%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98.jpg)

---

## 6. 현재 진행 상황

1. **데이터**: 데이터 탐색 완료 → 크롤링 진행 중 → AI 분석 도구 선택 (앨런 유력)
2. **DB**: AWS 학습 중, MongoDB 구축 (재활용 가능)
3. **AI**: 사전 학습 모델 분석 및 파인튜닝 준비
4. **프로젝트 관리**:
   - **Notion**: 프로젝트 진행 상황 및 회의록 관리
   - **Google Drive**: 데이터 및 문서 관리
   - **GitHub**: 작업 공간 관리
   - **단톡방**: 실시간 커뮤니케이션

---

## 7. 실행 방법 (How to Run)

### 1. 의존성 설치
```bash
poetry shell
npm install
