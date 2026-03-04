# Anthropic @ $19B ARR, Qwen team leaves, Gemini and GPT bump up fast models - 요약

**원문 URL**: https://www.latent.space/p/ainews-anthropic-19b-arr-qwen-team
**번역일**: 2026-03-04 07:28
**발행일**: 2026-03-04

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 뉴스 브리핑입니다.

### 🔥 주요 뉴스
*   **[Anthropic, 연간 매출 190억 달러 달성]** — Anthropic이 최근 190억 달러의 연간 반복 매출(ARR)을 달성했다고 확인되었습니다. 이는 OpenAI의 200억 달러에 근접한 수치로, AI 시장 내 경쟁 구도에 중요한 변화를 시사합니다.
*   **[Google, Gemini 3.1 Flash-Lite 출시]** — Google이 Gemini 3-시리즈의 가장 빠르고 비용 효율적인 엔드포인트인 Gemini 3.1 Flash-Lite (Preview)를 출시했습니다. 이 모델은 고볼륨 워크로드에 최적화되어 있으며, 2.5 Flash 대비 2.5배 빠른 첫 토큰 생성 시간을 제공합니다.
*   **[OpenAI, GPT-5.3 Instant 배포]** — OpenAI가 모든 ChatGPT 사용자에게 GPT-5.3 Instant를 배포했습니다. 이 버전은 이전 5.2 버전에 대한 사용자 불만을 반영하여 대화의 자연스러움을 개선하고 불필요한 거부 및 환각을 줄였습니다.
*   **[Alibaba Qwen 팀 핵심 인력 대규모 이탈]** — Alibaba의 Qwen 프로젝트에서 Justin Lin을 포함한 주요 기술 리더 및 선임 기여자들의 대규모 이탈이 발생했습니다. 이는 오픈소스 AI 생태계, 특히 Qwen 모델의 향후 개발 및 라이선싱 정책에 불확실성을 야기하고 있습니다.

### 📊 모델 & 벤치마크
*   Google Gemini 3.1 Flash-Lite (Preview)가 출시되었습니다. 이 모델은 LMArena에서 1432 Elo를 기록하고 86.9% GPQA Diamond 성능을 보이며, 1M 컨텍스트 윈도우를 유지합니다.
*   OpenAI GPT-5.3 Instant가 ChatGPT 사용자에게 배포되었으며, 환각이 검색 사용 시 26.8%, 미사용 시 19.7% 감소했다고 보고되었습니다.
*   OpenAI는 "생각보다 빨리" GPT-5.4가 출시될 것을 예고했습니다.
*   Qwen 3.5 모델이 출시되었으며, 0.8B 매개변수 모델에 비전 인코더를 포함하고 이전 세대 대비 성능이 크게 향상되었습니다.
*   Arena의 Document Arena가 출시되어 실제 PDF 추론 병렬 평가를 제공하며, Claude Opus 4.6이 이 벤치마크에서 선두를 차지했습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/5c5846dc-3d68-436a-8549-b9b4dd707c5d_1556x1004.png)

### 🛠️ 제품 & 도구
*   Google Gemini 3.1 Flash-Lite (Preview) API가 AI Studio 및 Vertex를 통해 배포되었습니다.
*   OpenAI의 "GPT‑5.3‑chat‑latest"가 API에 나타났습니다.
*   Databricks가 메모리를 절감하는 오픈소스 옵티마이저 구현인 FlashOptim (AdamW/SGD/Lion)을 출시했습니다.
*   Notion이 Meeting Notes를 위한 MCP/API 지원을 출시했습니다.
*   Cursor가 에이전트가 채팅 내에서 대화형 UI를 렌더링하는 MCP Apps를 출시했습니다.
*   Perplexity가 많은 모델을 오케스트레이션하고 관리형 보안 샌드박스를 통해 앱에 임베딩하는 "Computer" 플랫폼을 선보였습니다.

### 🔬 연구 & 논문
*   Together 연구팀이 Context Parallelism과 Sequence Parallel 스타일 헤드 청킹의 하이브리드를 통해 5M 컨텍스트 윈도우 8B 모델 학습 시 어텐션 메모리 사용량을 최대 87%까지 줄이는 방법을 발표했습니다.

### 💰 산업 동향
*   Anthropic이 190억 달러의 연간 반복 매출(ARR)을 달성하며 OpenAI에 근접한 시장 점유율을 보였습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/b8d40f52-7af5-4969-b941-896fbbd80306_1184x1702.png)
*   Alibaba Qwen 프로젝트에서 Justin Lin을 포함한 주요 기술 리더 및 선임 기여자들의 대규모 이탈이 확인되었습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/9b9024fe-bb8e-481d-898d-d61a0513b082_1264x856.png)
*   OpenAI의 사후 학습 VP였던 Max Schwarzer가 Anthropic으로 이직했습니다.
*   미 국방부가 Anthropic을 "공급망 위험"으로 분류하겠다고 위협하며, Anthropic은 대규모 국내 감시 및 자율 무기에 대한 안전 장치를 요구하고 있습니다.

### ⚡ 인프라 & 하드웨어
*   Databricks의 FlashOptim은 AdamW 학습 오버헤드를 매개변수당 약 16바이트에서 7바이트로 줄여, 예시 8B 파인튜닝 피크 메모리를 175GiB에서 113GiB로 감소시켰습니다.
*   SkyPilot이 RL 사후 학습을 위해 강력한 GPU, 저렴한 GPU, 고메모리 CPU에 걸쳐 워크로드를 분할하는 Job Groups 오케스트레이션 모델을 제공합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
