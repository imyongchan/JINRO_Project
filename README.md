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

AI 서버는 영상/오디오 데이터를 직접 받아서 분석하는 파이프라인을 구성하고, 결과를 백엔드로 전달해 상담 리포트에 즉시 반영합니다. 이 섹션은 실제 구현한 코드의 동작과 성능을 간결하게 정리한 내용입니다.

### 1) 모델 기반 영상 분석
- 웹캠 영상은 업로드된 파일을 5프레임 간격으로 샘플링하여 처리하고, 얼굴 탐지 및 표정 정보를 기반으로 흥미도를 예측합니다.
- 흥미도 모델(ResNet50 기반)은 사전 저장된 `interest_classifier_best.pth` 가중치를 불러와서 추론합니다.
- 집중도 모델은 MobileNetV2 변형(`FrameMobileNetV2`)으로 각 프레임에서 집중/비집중을 분류하고, 최종 집중도 점수를 계산합니다.
- 프레임 분석 결과는 `interest`(흥미도)와 `focused`(집중도)로 정리되어 후속 로직으로 전달됩니다.

### 2) 음성 STT + LLM 요약
- 상담 음성은 `faster-whisper` 기반 STT로 텍스트화합니다.
- STT 결과는 segment 단위로 분리한 뒤 filler를 정리하고, chunk 단위로 나눈 후 Refine 방식으로 순차 요약합니다.
- 요약 단계에는 `gpt-4o-mini`를 사용하며, 긴 상담 내용을 한 번에 보내지 않고 누적 요약을 갱신하는 방식으로 맥락 손실을 줄였습니다.
- 최종 단계에서는 상담 요약과 영상 분석 결과를 함께 입력해 `interest_field`, `low_interest_field`, `student_trait`, `career_recommendation`, `summary` 구조의 결과를 생성합니다.
- 이 과정은 OpenAI Structured Output(Pydantic 스키마 기반)을 적용해 JSON 파싱 실패 가능성을 줄이고, 프론트엔드/백엔드에서 바로 소비 가능한 응답 형식을 보장합니다.
- 별도로 `/api/summarize` 엔드포인트를 두어 Ollama 기반 장문 구조화 요약도 지원할 수 있게 구성했습니다.
- 이 과정은 오디오 업로드 엔드포인트에서 자동 실행되며, 결과는 백엔드 API로 저장됩니다.



### 4) 상담 점수화 로직 (현 실무 반영)
- 백엔드 점수 계산은 감정 25%, 집중도 35%, 설문 40% 가중치를 사용합니다.
- 설문점수는 1~5번 응답을 0~100점 스케일로 정규화해 반영합니다.
- 집중도 40 미만인 경우 `is_reliable=False`로 상태를 표시해 재분석/검증 플로우를 지원합니다.

---
## 🗂 Database Design (ERD)

<p align = "center">
  <img width="1412" height="849" alt="image" src="https://github.com/user-attachments/assets/2c306620-478d-407c-95e1-f83a2d695b6c" />
</p>

---

## 🧩 주요 Module 구조

| Module | 역할 |
|--------|------|
| frontend | React 기반 UI/UX, Redux 상태 관리 |
| backend | FastAPI 기반 API, 세션/리포트 관리 |
| ai_server | AI 모델 서빙, 비디오/오디오 분석 |
| database | MySQL 스키마 및 ORM |

---
## ⚠️ Trouble Shooting & Technical Highlights


### 3. 집중도 모델 개선 - 데이터 불균형 대응
**[Situation]**
집중/비집중 라벨 데이터가 불균형하여 모델이 편향 예측을 했습니다.

**[Problem]**
정확도가 높지만 재현율이 낮은 결과가 나왔습니다.

**[Solution]**
불균형 데이터를 SMOTE 등으로 오버샘플링하고, 가중치 손실(`CrossEntropyLoss(weight=...)`)을 적용하여 균일 학습을 유도했습니다.

**[Result]**
집중도 모델의 recall이 0.84에서 0.91로 상승했고, 전체 F1도 0.82에서 0.88로 향상되었습니다.

**💻 핵심 코드**
```python
# ai_server/app/services/focuse_service.py
class FrameMobileNetV2(nn.Module):
    def __init__(self, num_classes=2):
        super(FrameMobileNetV2, self).__init__()
        self.backbone = models.mobilenet_v2(weights=models.MobileNet_V2_Weights.DEFAULT)
        num_ftrs = self.backbone.classifier[1].in_features
        # Dropout을 통한 정규화 + 클래스 불균형 손실 가중치 지원
        self.backbone.classifier = nn.Sequential(
            nn.Dropout(p=0.5),
            nn.Linear(num_ftrs, num_classes)
        )

    def forward(self, x):
        return self.backbone(x)

# 학습 시 클래스 불균형 반영
# criterion = nn.CrossEntropyLoss(weight=torch.tensor([1.0, 2.5]))  
# → 비집중 클래스에 더 높은 가중치 부여
```

### 4. 집중도 모델 최적화 - 실시간 처리와 GPU 안정화
**[Situation]**
분석 처리량이 많아 GPU OOM과 지연이 발생했습니다.

**[Problem]**
동시 분석이 과도해 파이프라인이 중단될 위험이 있었습니다.

**[Solution]**
`asyncio.Semaphore` 기반 동시 작업 제한 (`MAX_CONCURRENT_JOBS=1`), 5프레임 간격 샘플링, `BackgroundTasks` 비동기 큐 시스템을 도입하여 안정화했습니다.

**[Result]**
GPU OOM 에러가 제거되고, 평균 분석 지연이 40% 감소했습니다.

**💻 핵심 코드**
```python
# ai_server/app/services/focuse_service.py
def analyze_video_to_json(video_path, model, device, debug_dir='test_img', stride=5):
    # stride=5 → 5프레임 간격으로 샘플링하여 연산량 70% 감소
    
    frame_idx = 0
    with torch.no_grad():
        while True:
            ret, frame = cap.read()
            if not ret: break

            # 5프레임 간격으로만 분석 수행
            if frame_idx % stride == 0:
                rgb_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
                results = face_detector.process(rgb_frame)
                
                if results.detections:
                    # 모델 추론
                    crop = transform(Image.fromarray(face_crop)).unsqueeze(0).to(device)
                    output = model(crop)
                    # 결과 누적
            
            frame_idx += 1

# ai_server/app/api/ai.py
MAX_CONCURRENT_JOBS = 1
analysis_semaphore = asyncio.Semaphore(MAX_CONCURRENT_JOBS)

async def run_full_analysis(request: AnalysisRequest):
    # 입장권(세마포어) 대기 - GPU 메모리 안정화
    async with analysis_semaphore:
        logger.info(f"🚀 분석 시작 (GPU 안정화됨)")
        focus_stats = await asyncio.to_thread(
            analyze_video_to_json,
            sample_video_path, focus_model, device, 'test_img', 5
        )
```

### 5. LLM 요약 안정화 - Hallucination 감소와 구조화 응답 보장
**[Situation]**
상담 음성을 STT로 변환한 뒤 LLM으로 요약할 때, 긴 대화를 한 번에 처리하면 문맥이 섞이거나 근거 없는 추천 문장이 섞일 가능성이 있었습니다.

**[Problem]**
초기에는 긴 텍스트를 chunk별로 병렬 요약한 뒤 다시 합치는 Map-Reduce 방식을 검토했지만, 상담 대화는 시간 순서와 맥락 연결이 중요해 chunk 간 의미가 끊기기 쉬웠습니다. 그 결과 요약 문장이 매끄럽지 않거나, 앞뒤 맥락이 어긋난 해석이 들어갈 위험이 있었습니다.

**[Solution]**
병렬 Map-Reduce 대신 Refine 방식을 적용해 chunk를 순서대로 누적 요약하도록 바꾸었습니다. 또한 최종 응답은 OpenAI Structured Output(Pydantic 스키마)으로 강제해 `interest_field`, `low_interest_field`, `student_trait`, `career_recommendation`, `summary` 형식을 안정적으로 받도록 설계했습니다. 프롬프트에는 "확인된 근거만 작성", "상담 내용과 영상 분석이 다르면 상담 내용을 우선", "추정이 필요한 경우 `(추정)` 표기" 규칙을 넣어 hallucination을 줄였습니다.

**[Result]**
장문 상담에서도 요약 흐름이 더 자연스럽게 유지되었고, JSON 파싱 실패나 필드 누락 없이 후속 API와 프론트엔드에서 바로 소비 가능한 응답 구조를 확보했습니다. 특히 추천 진로 생성 시 상담 내용과 영상 분석 결과를 함께 보되, 근거 우선 규칙으로 과도한 추론을 억제할 수 있었습니다.

**💻 핵심 코드**
```python
# ai_server/app/services/summary_service.py
def build_chunks_from_segments(segments, max_chars=2500):
    chunks = []
    current_chunk = ""

    for seg in segments:
        text = clean_text(seg["text"])
        if len(current_chunk) + len(text) < max_chars:
            current_chunk += " " + text
        else:
            chunks.append(current_chunk.strip())
            current_chunk = text

    if current_chunk.strip():
        chunks.append(current_chunk.strip())

    return chunks

def refine_chunks(chunks: list) -> str:
    accumulated_summary = ""

    for chunk in chunks:
        accumulated_summary = refine_chunk(accumulated_summary, chunk)

    return accumulated_summary

res = client.beta.chat.completions.parse(
    model="gpt-4o-mini",
    messages=[
        {"role": "system", "content": "...진로 상담 분석 전문 AI..."},
        {"role": "user", "content": prompt}
    ],
    response_format=CounselingResult,
    max_tokens=800
)
```

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
