# Replit Agent 4: The Knowledge Work Agent - 요약

**원문 URL**: https://www.latent.space/p/ainews-replit-agent-4-the-knowledge
**번역일**: 2026-03-12 12:41
**발행일**: 2026-03-12

---

### 🔥 주요 뉴스
**[NVIDIA Nemotron 3 Super 출시]** — NVIDIA는 1M 컨텍스트를 지원하는 120B 파라미터의 오픈 모델 Nemotron 3 Super를 출시했습니다. 이 모델은 하이브리드 Mamba-트랜스포머/SSM 잠재 MoE 아키텍처를 특징으로 하며, FP4에서 GPT-OSS-120B보다 최대 2.2배 빠른 추론 속도를 제공합니다.
**[Replit Agent 4 출시 및 기업 가치 급증]** — Replit은 코딩을 넘어 지식 작업 에이전트에 초점을 맞춘 Agent 4를 출시했으며, 지난 6개월간 기업 가치가 3배 증가하여 90억 달러에 달했습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/98f51887-ef65-46b8-88f3-275dddae978_1186x1494.png)
**[Perplexity Personal Computer 및 Enterprise 확장]** — Perplexity는 Mac mini에서 실행되며 로컬 파일/앱/세션 접근 및 원격 제어가 가능한 상시 작동 로컬/클라우드 하이브리드 에이전트인 Personal Computer를 발표했습니다. 또한 20개의 전문 모델과 400개 이상의 앱을 아우르는 Computer for Enterprise를 확장했습니다.
**[Anthropic Institute 출범 및 내부 RSI 역학 보고]** — Anthropic은 고급 AI에 대한 대중 담론 형성을 목표로 하는 The Anthropic Institute를 출범시켰습니다. 내부적으로 Claude가 미래 모델 개발 코드의 70-90%를 작성하고 일부 작업에서 인간 감독자보다 427배 빠르다는 주장이 제기되었습니다.
**[Claude Code 서비스 중단 사태]** — Claude Code의 로그인/인증 중단 사태가 발생하여 개발자들의 워크플로우에 가시적인 지장을 초래했습니다. 이는 프론티어 모델 서비스 중단이 잠재적인 '지능 브라운아웃'으로 이어질 수 있음을 시사합니다.

### 📊 모델 & 벤치마크
*   NVIDIA Nemotron 3 Super는 AA Intelligence Index에서 36점을 기록하여 gpt-oss-120b(33점)를 앞섰으며, GPU당 약 10% 더 높은 처리량과 최대 484 tok/s의 서빙 속도를 보였습니다.
*   M5 Max 128GB 14인치 노트북에서 Qwen3.5-122B-A10B-4bit는 16K 컨텍스트에서 1,239.7 t/s의 프롬프트 처리량을, gpt-oss-120b-MXFP4-Q8은 2,710.5 t/s를 달성했습니다.
*   Qwen3.5-35B-A3B Aggressive GGUF 모델이 출시되었으며, 35B 파라미터 중 약 3B 활성 파라미터를 가진 MoE 구조로 멀티모달 입력을 지원합니다.
*   Reka Edge는 물리 AI를 위한 프로덕션 중심 VLM으로, 선도적인 8B 모델보다 3배 적은 입력 토큰과 65% 더 빠른 처리량을 주장했습니다.

### 🛠️ 제품 & 도구
*   Replit Agent 4는 앱, 웹사이트, 슬라이드를 위한 병렬 에이전트와 함께 협력적이고 캔버스 같은 워크플로우를 제공합니다.
*   Perplexity는 Mac mini에서 실행되며 로컬 파일/앱/세션 접근 및 원격 제어가 가능한 Personal Computer를 출시했습니다.
*   Base44 Superagents는 비기술 사용자를 위해 Gmail, Slack, Stripe, CRM 등과의 '배터리 포함' 통합을 강조하며 출시되었습니다.
*   LangChain은 Deep Agents에 모델이 엄격한 토큰 임계값 대신 작업 경계에서 압축할 수 있도록 자율 컨텍스트 압축 기능을 추가했습니다.
*   Google Gemini Embedding 2가 출시되었으며, 텍스트, 이미지, 비디오, 오디오, PDF용 임베딩과 저차원 저장을 위한 Matryoshka embeddings를 포함합니다.

### 🔬 연구 & 논문
*   OpenAI Devs는 에이전트의 컴퓨터 접근에 대한 기술 보고서를 발표하여 실행 루프, 파일 시스템 컨텍스트, 네트워크 접근 및 가드레일을 다루었습니다.
*   PostTrainBench v1.0 벤치마크가 출시되어 프론티어 에이전트가 단순화된 환경에서 언어 모델을 포스트 트레인할 수 있는지 측정하고 AI R&D 자동화 진행 상황을 추적합니다.
*   EvoSkill은 실패로부터 재사용 가능한 스킬을 발견하고 개선하는 에이전트 시스템으로, OfficeQA에서 Claude Code + Opus 4.5의 정확 일치율을 60.6%에서 67.9%로 향상시켰습니다.
*   AgentIR은 에이전트의 추론 추적과 쿼리를 함께 임베딩하는 추론 인식 리트리버로, BrowseComp-Plus에서 68%의 정확도를 보고했습니다.
*   NIST에 대한 프린스턴의 응답은 명시적인 공격보다는 신뢰성 부족에서 발생하는 AI 에이전트 실패 모드를 정의, 측정, 완화할 필요성을 강조했습니다.
*   Qwen3.5의 멀티모달 아키텍처에 대한 상세 분석이 공개되었으며, Gated DeltaNet 선형 어텐션과 Gated 풀 어텐션을 혼합한 하이브리드 어텐션 스택을 특징으로 합니다.
*   Google은 AI 시스템이 표준 검진에서 놓친 간격 유방암의 25%를 식별한 사례와 대화형 임상 추론을 위한 AMIE가 안전하고 실행 가능하며 환자들에게 좋은 반응을 얻었다는 연구 결과를 공유했습니다.

### 💰 산업 동향
*   Replit의 기업 가치가 지난 6개월간 3배 증가하여 90억 달러에 달했습니다.
*   Anthropic은 ML 엔지니어링, 경제학, 사회 과학을 아우르는 임무를 통해 고급 AI에 대한 대중 담론을 형성하는 The Anthropic Institute를 출범시켰습니다.

### ⚡ 인프라 & 하드웨어
*   NVIDIA Nemotron 3 Super는 네이티브 멀티 토큰 예측(MTP)과 Qwen3.5-122B 대비 주요 KV-캐시 이점(8,192 바이트/토큰 vs 24,576 바이트/토큰)을 통해 빠른 추론 속도를 달성했습니다.
*   M5 Max 128GB 14인치 노트북이 Qwen3.5-122B-A10B-4bit 등 다양한 모델의 벤치마크에 사용되어 성능 지표를 제공했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
