<p align = "center">
  <img width="762" height="247" alt="image" src="https://github.com/user-attachments/assets/4d1cbc62-e2e6-4b75-be44-f4e2d88b11ae" />
</p>




# 🐸 너, 내 진로가 되라 - AI 기반 진로 상담 플랫폼
> **학생의 감정, 집중도, 설문조사, 상담 대화를 진로 리포트로 연결하는 AI 보조형 진로 상담 서비스**
---
## 📌 Introduction (KOREA IT ACADEMY 최종 프로젝트)

**너, 내 진로가 되라** 웹캠으로 학생의 집중도와 흥미도를 분석하고, 상담 내용을 STT로 변환하여 LLM으로 요약 및 진로 추천까지 제공하는 AI 기반 진로 상담 플랫폼입니다. AI 기반 진로 상담 및 분석 서비스 '진로이즈백'은 기존 진로 상담의 한계를 극복하기 위해 개발되었습니다.

## 기존 진로 상담의 한계점 

### 1️⃣ 상담사의 경험 의존성 
- 상담사의 경험에 의존하여 학생의 실제 관심도와 집중도를 파악하기 어렵다.
### 2️⃣ 비언어적 표현의 부족한 기록 
- 말로 진행되는 상담 특성상 학생의 비언어적 표현이 많이 기록되지 않거나 집중되지 않는다.
### 3️⃣ 제한된 시간과 부족한 구조화된 자료 
- 제한된 시간 내에 상담이 이루어져 활용 가능한 구조화된 자료가 부족하다.
### 4️⃣ 정보 과부하로 인한 학생의 혼란 
- 직업 정보가 많아지면서 학생 스스로 무엇을 좋아하고 잘하는지 판단하기 어렵다.
### 5️⃣ 주관적인 상담 진행 
- 상담사의 경험에 기반하여 객관적인 근거보다는 주관적인 생각이 개입될 수 있다.

## 목표 
- 실시간 웹캠 기반으로 학생의 몰입도, 흥미도, 집중도를 점수화.
- 자가 설문 조사 결과를 점수화하여 통합.
- 상담 내용을 녹음하여 STT(Speech-to-Text)로 변환하고 LLM(Large Language Model)으로 요약 및 진로 추천까지 제공
- 정량/정성 데이터를 결합한 리포트 자동 생성.


---
## 📊 Project Overview

- 프로젝트명: 너, 내 진로가 되라
- 개발 기간: 2026.02.10 ~ 2026.03.31
- 팀명: 진로 이즈 백
- 개발 형태: 5인 팀 프로젝트

## 👥 팀 구성 및 역할 
- **강대광** : 집중도 분석 모델 개발/개방, 온보딩 플로우 설계 및 구현
- **김용찬** : LLM 기반 상담 분석 파이프라인 설계, 서버 아키텍처 및 배포 구축
- **안희원** : STT → LLM 파이프라인 구현, 사용자 세션/로그인 상태 관리
- **오경택** : AI 결과 병목 분석 및 모델 적용 최적화, AI 점수화 로직 설계
- **조진석** : 흥미도 분석 모델 개발, 시선 기반 정면 응시 기준 정의 및 모델링

---

## 🛠 Tech Stack

### Backend
- ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) **3.10+**
- ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

### Database
- ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

### Frontend
- ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) **19**
- ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
- ![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white)

### 🧠 AI Pipeline & Models

- **STT**
   ![Whisper](https://img.shields.io/badge/Faster--Whisper-FF6F00?style=flat-square&logo=openai&logoColor=white) :Speech-to-Text

- **집중도 분석**
   ![MobileNetV2](https://img.shields.io/badge/MobileNetV2-0A66C2?style=flat-square&logo=pytorch&logoColor=white): Frame 단위 집중/비집중 분류

- **흥미도 분석**
   ![ResNet50](https://img.shields.io/badge/ResNet50-8A2BE2?style=flat-square&logo=pytorch&logoColor=white) :표정/감정 분류

- **시선 추적**
   ![MediaPipe](https://img.shields.io/badge/MediaPipe-FaceMesh-00A1F1?style=flat-square&logo=google&logoColor=white) :정면 응시 판단

- **추가 실험 모델**
   ![Swin Transformer](https://img.shields.io/badge/Swin%20Transformer-FF1493?style=flat-square&logo=pytorch&logoColor=white) :성능 비교 및 개선 실험

- **LLM**
   ![GPT-4o-mini](https://img.shields.io/badge/GPT--4o--mini-412991?style=flat-square&logo=openai&logoColor=white) :상담 요약 및 진로 추천

### Deployment
- ![AWS](https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white)


### Collaboration
- ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) / ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
---
## ⚡ 주요 기능

---

### 1️⃣ 영상 선택 및 시청 (내담자측) 

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/7c0ce337-c2f2-4792-9e81-e8ceb9c57fc1" width=400 height="250" style="object-fit: contain;"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/6b5df915-8944-4ab0-84c7-d0d1c39e5b13" width=400 height="250" style="object-fit: contain;"/>
    </td>
  </tr>
</table>

- 대분류, 중분류, 소분류로 나뉜 카테고리에서 영상을 선택하여 시청.
- 영상 시청 시작과 동시에 웹캠 녹화를 시작하며 시선과 표정을 분석.

---

### 2️⃣ 설문조사 (내담자측)

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/06deec85-9797-406a-a215-7935736d5fb7" width=400 height="250" style="object-fit: contain;"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/b244afdb-840d-4bee-a4f0-72b2d23b568d"  width=400 height="250" style="object-fit: contain;"/>
    </td>
  </tr>
</table>

- 영상 시청 녹화가 끝나면 설문 조사로 넘어가 사용자의 주관적인 데이터를 수집.
- 완료시 웹켐영상은 AI서버에 내담자별 video파일에 저장되고 설문조사 내역은 DB에 JSON 형태로 저장.  

---

### 3️⃣ 일정관리 및 학생목록 (상담사측)

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/93c05ab8-fe7f-4c9d-87b1-a083160c39e0"  width=400 height="250" style="object-fit: contain;"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/b85545a8-af91-43a7-bf98-771aa0173ebb"  width=400 height="250" style="object-fit: contain;"/>
    </td>
  </tr>
</table>

- 영상3개를 다본 내담자의 데이터가 상담사쪽으로 넘어옴.
- 상담사가 내담자의 상담일정을 잡은 후 그 목록을 학생목록에서 볼 수 있음. 

---

### 5️⃣ 📚 AI 결과 분석 & 상담녹음 

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/5ae67959-8ef2-41cb-b4a7-0aac3dd0cf56" width=400 height="250" style="object-fit: contain;"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/f1ce087e-af81-45f5-ac4f-0e3258df9ea6" width=400 height="250" style="object-fit: contain;"/>
    </td>
  </tr>
</table>

- 웹캠 영상 분석을 통해 사용자의 시선과 집중도를 시각화한 그래프를 제공.
- 집중도, 흥미도, 주관적인 의견을 포함한 최종 점수표를 제공.
- 상담 중 녹음을 시작하고, 종료 시 STT로 텍스트 변환 후 LLM으로 넘겨 학생 성향 분석 및 진로 추천을 도출.

---

### 6️⃣ 최종리포트 작성 & PDF출력

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/dce633c8-b075-4c49-9cfc-b8611572c843" width=400 height="250" style="object-fit: contain;"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/4d8a2708-6dd5-44c4-ad6e-f458e04edd61" width=400 height="250" style="object-fit: contain;"/>
    </td>
  </tr>
</table>

- AI 분석 결과를 기반으로 상담사가 주관적인 내용을 추가하여 수정 및 저장.
- 최종 작성 완료 시 수정이 불가능하며, PDF 또는 텍스트 파일로 추출하여 학생에게 전달가능.


## 🤖 AI 개발

### 1) 모델 기반 영상 분석
- 웹캠 영상은 업로드된 파일을 5프레임 간격으로 샘플링하여 처리하고, 얼굴 탐지 및 표정 정보를 기반으로 흥미도를 예측.
- 흥미도 모델(ResNet50 기반)은 사전 저장된 `interest_classifier_best.pth` 가중치를 불러와서 추론.
- 집중도 모델은 MobileNetV2 변형(`FrameMobileNetV2`)으로 각 프레임에서 집중/비집중을 분류하고, 최종 집중도 점수를 계산.
- 프레임 분석 결과는 `interest`(흥미도)와 `focused`(집중도)로 정리되어 후속 로직으로 전달.

### 2) 음성 STT + LLM 요약
- 상담 음성은 `faster-whisper` 기반 STT로 텍스트화.
- STT 결과는 segment 단위로 분리한 뒤 filler를 정리하고, chunk 단위로 나눈 후 Refine 방식으로 순차 요약.
- 요약 단계에는 `gpt-4o-mini`를 사용하며, 긴 상담 내용을 한 번에 보내지 않고 누적 요약을 갱신하는 방식사용.
- 최종 단계에서는 상담 요약과 영상 분석 결과를 함께 입력해 `interest_field`, `low_interest_field`, `student_trait`, `career_recommendation`, `summary` 구조의 결과를 생성.


### 3) 상담 점수화 로직 
- 백엔드 점수 계산은 감정 25%, 집중도 35%, 설문 40% 가중치를 사용.
- 설문점수는 1~5번 응답을 0~100점 스케일로 정규화해 반영.
- 집중도 40 미만인 경우 `is_reliable=False`로 상태를 표시해 재분석/검증 플로우를 지원.

---
# 💥Trouble shooting - LLM , 서버배포 

### 1️⃣ LLM 응답 JSON 구조 불안정 문제

#### 📌 문제
- 프롬프트로 JSON 형식을 지정했으나 출력이 일관되지 않음
- key 누락, 타입 불일치 등으로 파싱 에러 발생

#### 🔍 원인
- LLM은 자연어 생성 기반이라 형식을 100% 보장하지 못함
- 프롬프트 방식은 강제성이 부족함

#### 💡 해결 방법
- 최종 응답은 OpenAI Structured Output(Pydantic 스키마)으로 강제해 `interest_field`, `low_interest_field`, `student_trait`, `career_recommendation`, `summary` 형식을 안정   적으로 받도록 설계

##### Before (프롬프트 기반)
```python
prompt = """
다음 JSON 형식으로 출력하세요:
{
  "interest_field": "...",
  "low_interest_field": "...",
  "student_trait": "...",
  "career_recommendation": [],
  "summary": "..."
}
"""
res = client.chat.completions.create(...)
```

##### After (Pydantic Structured Output)
```python
from pydantic import BaseModel

class CounselingResult(BaseModel):
    interest_field: str
    low_interest_field: str
    student_trait: str
    career_recommendation: list[str]
    summary: str

res = client.beta.chat.completions.parse(
    model="gpt-4o-mini",
    messages=[...],
    response_format=CounselingResult
)

result = res.choices[0].message.parsed
```

#### 📊 효과
- JSON 구조 100% 보장
- 파싱 에러 제거
  

---

### 2️⃣ 상담 요약 시 맥락 손실 문제

#### 📌 문제
- 초기에는 긴 텍스트를 chunk별로 병렬 요약한 뒤 다시 합치는 Map-Reduce 방식을 검토했지만, 상담 대화는 시간 순서와 맥락 연결이 중요해 chunk 간 의미가 끊기기 쉬웠음.
- 그 결과 요약 문장이 매끄럽지 않거나, 앞뒤 맥락이 어긋난 해석이 들어갈 위험이 있었음.
- 최종 요약 결과의 일관성이 떨어짐.

#### 🔍 원인
- Map-Reduce 방식 사용으로 각 chunk가 독립적으로 처리됨
- 상담 데이터는 순차적 흐름이 중요한데 반영되지 않음

#### 💡 해결 방법
-청크별 요약처리를 Map-Reduce 방식에서 하나의 청크요약이 다음 청크요약에서 누적될 수 있도록 Refine 방식으로 개선 

##### Before (Map-Reduce)
```python
def summarize_chunk(chunk):
    return llm(chunk)

summaries = [summarize_chunk(c) for c in chunks]
final = llm(" ".join(summaries))
```

##### After (Refine 방식)
```python
def refine_chunk(existing_summary: str, new_chunk: str, max_retries=3) -> str:
    if not existing_summary:
        prompt = f"""
    당신은 학교 진로 상담 전문 분석가입니다.
    아래 상담 녹취의 핵심 내용을 구조화된 형식으로 정리하세요.
    ....
    {existing_summary}

    새로운 내용:
    {new_chunk}

    기존 내용을 유지하며 요약을 갱신하세요.
    """
    return llm(prompt)

summary = ""

def refine_chunks(chunks: list) -> str:
    accumulated_summary = ""

    for i, chunk in enumerate(chunks):
        print(f"[Refine] {i+1}/{len(chunks)} 청크 처리 중...")
        accumulated_summary = refine_chunk(accumulated_summary, chunk)
```

#### 📊 효과
- 상담 흐름 유지 (맥락 보존)
- 요약 일관성 향상
- 분석 품질 개선

### 3️⃣ LLM Hallucination (환각) 문제

#### 📌 문제
- 상담 내용과 다른 정보가 생성되거나, 근거 없는 내용이 포함되는 현상 발생
- 영상 분석 결과와 상충되는 진로 추천이 나오는 경우 존재
- 모델이 확신형 문장으로 잘못된 정보를 생성하여 신뢰도 저하

#### 🔍 원인
- LLM의 확률 기반 생성 특성으로 인해 실제 데이터에 없는 내용 생성
- 입력 데이터(상담 요약, 영상 분석) 간 충돌 시 명확한 판단 기준 부재
- "좋은 답변"을 만들려는 과정에서 과도한 일반화 발생

#### 💡 해결 방법

##### Before (일반 프롬프트)
```python
prompt = f"""
상담 내용을 기반으로 진로를 추천하세요.
"""
```

##### After (Hallucination 제어 프롬프트 적용)
```python
prompt = f"""
[분석 원칙]
- 확인된 근거가 있는 내용만 작성하고, 근거 없이 단정하지 마세요
- 상담 내용과 영상 분석이 다를 경우 상담 내용을 우선하세요
- 추정이 필요한 경우 반드시 "(추정)"을 붙이세요

[상담 요약]
{text}

[영상분석]
{video_analyze}
"""
```

#### 📊 효과
- 근거 기반 응답 생성으로 신뢰도 향상
- 데이터 충돌 시 일관된 판단 기준 확보
- 불필요한 추측 및 허위 정보 생성 감소 (Hallucination 완화)

### 4️⃣ 서버 구조 및 배포 관련 문제

#### 📌 문제
- AI 모델 추론과 API 요청이 하나의 서버에서 처리되면서 응답 지연 발생
- 영상 처리 및 모델 추론 시 CPU/GPU 사용량 급증 → 전체 서버 성능 저하
- 하나의 도메인에서 여러 서버를 운영하기 어려움

#### 🔍 원인
- Backend(API, DB)와 AI 연산 작업이 동일 서버에서 동작
- 연산 작업(AI)이 I/O 작업(API 응답)에 영향을 주는 구조
- 트래픽 분산 및 라우팅 구조 부재

#### 💡 해결 방법

##### Before (단일 서버 구조)
```
Client → Backend (API + AI 처리 + DB)
```

##### After (서버 분리 + Nginx 라우팅)
```
Client → Nginx
            ├ /api → Backend Server
            └ /ai  → AI Server
```

- Nginx를 활용하여 URL 기반 라우팅 적용
- Backend와 AI Server를 물리적으로 분리
- AI Server는 연산 성능 중심 인스턴스로 구성

#### 📊 효과
- API 응답 속도 안정화
- AI 연산과 서비스 로직 분리로 병목 제거
- 서버 확장성 및 유지보수성 향상

---

### 5️⃣ 서버 간 통신 보안 문제

#### 📌 문제
- AI Server에 저장된 영상 및 음성 데이터는 민감 정보
- 외부 네트워크 노출 시 보안 위험 존재

#### 🔍 원인
- 초기 설계에서 서버 간 통신 보안 고려 부족
- Public IP 기반 통신 시 외부 접근 가능성 존재

#### 💡 해결 방법

##### Before (외부 노출 가능 구조)
```
Backend ↔ AI Server (Public IP)
```

##### After (Private IP 내부 통신)
```
Backend ↔ AI Server (Private IP)
```

- 동일 VPC 내 Private IP 기반 통신 적용
- 외부에서 AI Server 직접 접근 차단

#### 📊 효과
- 민감 데이터 외부 노출 방지
- 내부 네트워크 기반 안정적인 통신 확보
- 보안 수준 향상

---

### 6️⃣ 로그 관리 및 서버 운영 문제

#### 📌 문제
- 에러 발생 시 원인 추적이 어려움
- 로그가 누적되면서 서버 용량 및 성능 저하 발생

#### 🔍 원인
- 로그 관리 정책 부재
- 로그 파일 무제한 누적

#### 💡 해결 방법
환경변수에 로그파일 관리설정과 TimeRotatingFileHandler 적용하여 관리 


#####  (파일 기반 로그 + 자동 관리)
```python
handler = TimedRotatingFileHandler(
    filename=os.path.join(LOG_DIR_NAME, BACKEND_LOG_FILE),
    when=os.getenv("LOG_ROTATION_WHEN", "midnight"),
    interval=int(os.getenv("LOG_ROTATION_INTERVAL", 1)),
    backupCount=int(os.getenv("LOG_BACKUP_COUNT", 30)),
    encoding="utf-8"
)

```
(env)
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/3940f50d-8942-4da0-b2f9-1aaacc5d2a44" />

```bash
/app/logs/app.log
/app/logs/app_2026-04-01.log
/app/logs/app_2026-04-02.log
```

- 날짜 기준 로그 파일 자동 분리
- 일정 기간 이후 로그 자동 삭제 (log rotation)
- 에러 발생 시 시점별 추적 가능

#### 📊 효과
- 문제 발생 시 빠른 원인 분석 가능
- 서버 디스크 사용량 안정화
- 운영 안정성 향상
## 🗂 Database Design (ERD)

<p align = "center">
  <img width="1412" height="849" alt="image" src="https://github.com/user-attachments/assets/2c306620-478d-407c-95e1-f83a2d695b6c" />
</p>
---

## 🎥 데모 영상

- 프로젝트 발표 영상 : [발표 영상](https://www.youtube.com/watch?v=iKnmn_Ps-NU&list=PLedGoSru7949ULhxrVcR86nPq25uXOu1Q&index=2)
- 프로젝트 화면 영상 : [화면 영상](https://www.youtube.com/watch?v=Ni0QDxmP0FU&list=PLedGoSru7949ULhxrVcR86nPq25uXOu1Q&index=3)
---



## 🚀 로컬 실행 방법

이 프로젝트는 `frontend`, `backend`, `ai_server` 3개 프로세스로 실행됩니다.  
Git에는 `.venv`와 `.env`가 포함되지 않으므로, 다른 PC에서 처음 실행할 때는 아래 준비가 필요합니다.

### 1. 사전 준비

- Python 3.12
- Node.js
- MySQL
- `JINRO_PROJ/backend/.env`
- `JINRO_PROJ/ai_server/.env`

`.env` 파일은 각 폴더의 `.env.example`을 복사해서 작성할 수 있습니다.

```powershell
Copy-Item JINRO_PROJ\backend\.env.example JINRO_PROJ\backend\.env
Copy-Item JINRO_PROJ\ai_server\.env.example JINRO_PROJ\ai_server\.env
```

### 2. 최초 1회 설치

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r JINRO_PROJ\backend\requirements.txt
.\.venv\Scripts\python.exe -m pip install -r JINRO_PROJ\ai_server\requirements.txt
cd JINRO_PROJ\frontend
npm install
```

### 3. 실행

가장 쉬운 방법은 프로젝트 루트에서 아래 파일을 실행하는 것입니다.

```bat
run_local.bat
```

수동 실행이 필요하면 터미널 3개에서 각각 실행합니다.

```powershell
cd f:\Portfolio\JINRO_AI_PORTFOLIO\JINRO_PROJ\backend
..\..\.venv\Scripts\python.exe run.py
```

```powershell
cd f:\Portfolio\JINRO_AI_PORTFOLIO\JINRO_PROJ\ai_server
..\..\.venv\Scripts\python.exe run.py
```

```powershell
cd f:\Portfolio\JINRO_AI_PORTFOLIO\JINRO_PROJ\frontend
npm run dev
```

### 4. 접속 주소

실행 후 접속 주소는 아래와 같습니다.

- Frontend: `http://localhost:5173`
- Backend: `http://127.0.0.1:8000`
- AI Server: `http://127.0.0.1:8001`

### 5. 참고 사항

- Python 가상환경은 프로젝트 루트의 `.venv`를 사용합니다.
- 데이터베이스 연결 정보는 `JINRO_PROJ/backend/.env`에 설정해야 합니다.
- AI 요약 및 분석 관련 설정은 `JINRO_PROJ/ai_server/.env`에 설정해야 합니다.
- LLM 기반 상담 요약을 사용하려면 `JINRO_PROJ/ai_server/.env`에 `OPENAI_API_KEY`를 설정해야 합니다.
- AI 모델 파일이 없으면 서버는 실행되지만 일부 분석 기능은 제한될 수 있습니다.
