# OpenAI GPT-next disproves 80 year old Erdős planar unit distance problem for under $1000 - 요약

**원문 URL**: https://www.latent.space/p/ainews-openai-gpt-next-disproves
**번역일**: 2026-05-21 12:19
**발행일**: 2026-05-21

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식 요약 브리핑입니다.

### 🔥 주요 뉴스
**[OpenAI, 80년 된 Erdős 문제 반증]** — OpenAI의 내부 범용 LLM(GPT 5.6 추정)이 80년 된 Erdős 평면 단위 거리 문제를 32시간 미만 또는 1,000달러 미만의 비용으로 반증하는 데 성공했습니다. 이는 전용 수학 시스템이 아닌 범용 모델이 새로운 구성 패밀리를 발견하며 이산 기하학 분야에서 중요한 과학적 돌파구를 마련한 사례입니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/0ff7bdc0-79ef-49ce-a5c0-f7db89d60637_1098x1582.png)
![Image](https://substack-post-media.s3.amazonaws.com/public/images/828cdb3-1d89-4582-9d70-0f251a57d77_753x620.png)
![Image](https://substack-post-media.s3.amazonaws.com/public/images/f77d343f-e4c1-4125-b78a-33728e06a6ba_1778x1490.png)
![Image](https://substack-post-media.s3.amazonaws.com/public/images/c9cfd22b-4a17-47a2-a2b0-d2ae5a911ece_1654x352.png)
**[Cohere Command A+ 오픈 웨이트 출시]** — Cohere가 자사의 가장 강력한 모델인 Command A+를 Apache 2.0 오픈 웨이트로 출시했습니다. 이 모델은 218B MoE / 25B 활성 파라미터로 구성되며 낮은 하드웨어 요구 사항에 최적화되어, 엔터프라이즈급 오픈 모델의 중요한 전환점으로 평가됩니다.
**[Google Gemini 3.5 Flash 및 Omni 출시]** — Google이 Gemini 앱에서 Gemini 3.5 Flash를 전 세계 무료 액세스로 출시하며, 기존 모델보다 4배 빠르고 비용은 절반 미만이라고 주장했습니다. 또한 비디오 및 혼합 입력 워크플로우를 위한 대화형 멀티모달 생성/편집 모델인 Gemini Omni를 선보였습니다.
**[Anthropic, SpaceX와 컴퓨팅 계약]** — Anthropic이 Colossus 2 용량을 확장하고 있으며, SpaceX와의 컴퓨팅 계약이 2029년 5월까지 월 12.5억 달러 규모에 달하는 것으로 알려졌습니다. 이는 AI 인프라 확장을 위한 대규모 투자 동향을 보여줍니다.

### 📊 모델 & 벤치마크
*   Cohere가 Command A+를 Apache 2.0 오픈 웨이트로 출시했습니다. 이 모델은 218B MoE / 25B 활성 파라미터, 멀티모달, 48개 언어를 지원하며, W4A4 양자화 시 2개의 H100으로도 실행 가능합니다.
*   Artificial Analysis는 Command A+를 Intelligence Index에서 37점으로 평가하며, Claude 4.5 Haiku 수준의 강력한 비-환각 행동과 괜찮은 속도를 보였으나, 과학적 추론 및 코딩 능력은 최고 성능 모델보다 약하다고 보고했습니다.
*   InferenceBench가 출시되어 AI R&D 자동화를 목표로 하며, 현재 프론티어 에이전트가 시스템 수준 엔지니어링 및 종속성 관리에 어려움을 겪고 역 스케일링 효과를 보인다고 보고했습니다.
*   Terminal-Bench Science가 출시되어 에이전트 평가를 코딩에서 실제 과학 워크플로우로 확장했습니다.
*   MINTEval이 빈번한 업데이트와 간섭이 있는 장문 컨텍스트 메모리 시스템을 목표로 출시되었으며, 138.8k~1.8M 토큰 컨텍스트에서 평균 정확도 27.9%를 기록했습니다.
*   SID-1이 RL 학습 에이전틱 검색 모델로 제시되었으며, RAG+리랭크보다 1.9배 높은 리콜, 24배 빠른 속도, GPT-5.1보다 99% 저렴한 비용을 주장했습니다.
*   Composer 2.5가 Artificial Analysis Coding Agent Index에서 62점을 기록하며, Opus/GPT-5.5 변형 모델보다 훨씬 낮은 비용으로 강력한 코딩 에이전트 성능을 보였습니다.
*   Qwen3.7 Preview (Max-Preview 및 Plus-Preview 포함)가 Arena에 출시되었으며, Artificial Analysis는 Qwen3.7 Max를 GPT 5.4 (xhigh)와 거의 동등한 5위로 평가했습니다.
*   Qwen은 중간 크기 밀집 모델 범위에서 파라미터 효율성을 최적화하기 위해 또 다른 27B 모델을 출시할 가능성이 높다고 로드맵을 통해 밝혔습니다.

### 🛠️ 제품 & 도구
*   Google이 Gemini 앱에서 Gemini 3.5 Flash를 전 세계 무료 액세스로 출시했으며, Gemini Omni는 비디오 및 혼합 입력 워크플로우를 위한 대화형 멀티모달 생성/편집 모델로 선보였습니다.
*   Google AI Studio는 엔드투엔드 개발자 워크플로우 및 모바일 액세스 방향으로 업데이트되었습니다.
*   Google DeepMind는 Google의 에이전트 스택을 위한 Science Skills를 출시하여 UniProt 및 AlphaFold DB와 같은 30개 이상의 생명 과학 소스를 통합했습니다.
*   LangChain이 LangSmith Sandboxes를 GA(General Availability)로 전환했습니다.
*   deepagents가 순수 도구 실행과 전체 샌드박스 사이의 중간 지점으로서 새로운 경량 코드 인터프리터 지원을 추가했습니다.
*   Perplexity는 답변 품질을 개선하면서 컨텍스트 토큰을 최대 70%까지 줄이는 쿼리 인식, 인용 보존 컨텍스트 압축 시스템을 설명했습니다.
*   Weaviate 1.37은 RAG/에이전트를 위한 벡터 리트리벌의 다양성을 개선하기 위해 MMR 리랭킹을 추가했습니다.
*   Cursor는 에이전트 워크스페이스에 자동화 기능을 추가했습니다.
*   VS Code는 더 나은 마크다운/HTML 미리보기, 원격 세션 연속성, 유틸리티 모델 구성 가능성을 출시했습니다.
*   OpenAI가 모바일용 Codex를 출시했습니다.

### 🔬 연구 & 논문
*   OpenAI의 내부 범용 LLM이 80년 된 Erdős 평면 단위 거리 문제를 반증하고 새로운 구성 패밀리를 발견했습니다.
*   ThoughtTrace는 실제 LLM 대화 중 사용자의 자가 보고된 생각을 담은 대규모 데이터셋(10,174개 생각 주석, 2,155개 다중 턴 대화 등)을 공개했습니다.

### 💰 산업 동향
*   Anthropic이 Colossus 2 용량을 확장하고 있으며, SpaceX와의 컴퓨팅 계약이 2029년 5월까지 월 12.5억 달러 규모에 달하는 것으로 알려졌습니다.
*   Exa가 2.2억 달러의 기업 가치로 2.5억 달러 규모의 시리즈 C 투자를 유치하며, 에이전트를 위한 웹 데이터를 정리하는 검색 연구소로 포지셔닝했습니다.

### ⚡ 인프라 & 하드웨어
*   Cohere Command A+는 W4A4 양자화 시 2개의 H100으로도 실행될 수 있도록 낮은 하드웨어 요구 사항에 최적화되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
