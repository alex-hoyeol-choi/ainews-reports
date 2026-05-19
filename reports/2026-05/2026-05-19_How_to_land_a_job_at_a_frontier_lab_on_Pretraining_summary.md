# How to land a job at a frontier lab (on Pretraining) - 요약

**원문 URL**: https://www.latent.space/p/ainews-how-to-land-a-job-at-a-frontier
**번역일**: 2026-05-19 12:19
**발행일**: 2026-05-19

---

### 🔥 주요 뉴스
**[Cursor, Composer 2.5 출시 및 'SpaceXAI' 이니셔티브 발표]** — Cursor는 최신 모델 Composer 2.5를 출시하며 장기 작업 및 지시 따르기 능력을 강화했다고 밝혔습니다. 또한, 'SpaceXAI' 이니셔티브를 통해 Colossus 2의 100만 H100 등가물에 접근하여 10배 더 많은 컴퓨팅으로 훨씬 큰 모델을 처음부터 학습시킬 계획을 공개했습니다.
**[Anthropic, SDK 플랫폼 Stainless 인수]** — Anthropic은 초기 API 시절부터 자사 SDK를 지원해 온 SDK 및 MCP 서버 플랫폼 Stainless를 인수했습니다. 이는 개발자 인체 공학 및 프로토콜 표면을 중심으로 한 지속적인 수직 통합 전략을 시사합니다.
**[llama.cpp, Qwen3.6 모델에 MTP 지원 추가로 로컬 추론 속도 대폭 향상]** — llama.cpp는 Qwen3.6 모델군에 MTP(Multi-Token Prediction) 지원을 발표하며 로컬 AI의 중요한 이정표를 세웠습니다. A10G에서 Qwen3.6-27B dense 모델의 처리량이 25 tok/s에서 45 tok/s로 78% 향상되는 등 상당한 속도 개선을 보였습니다.
**[ByteDance, 통합 멀티모달 모델 Lance 오픈소스화]** — ByteDance는 이미지/비디오 이해, 생성 및 편집을 위한 통합 멀티모달 모델 Lance를 오픈소스화했습니다. 이 모델은 3B 비디오, 3B 이미지, 3B 디코더 구성 요소를 포함합니다.

### 📊 모델 & 벤치마크
*   Cursor는 장기 작업에 대한 지속적인 성능과 신뢰성 높은 지시 따르기를 개선한 Composer 2.5를 출시했습니다.
*   Alibaba Qwen3.7 Max Preview는 Arena 텍스트 부문 전체 13위(수학 7위, 전문가 9위, 소프트웨어 및 IT 9위, 코딩 10위 포함)를 기록했으며, Qwen3.7 Plus Preview는 비전 부문 전체 16위에 올랐습니다.
*   ByteDance는 이미지/비디오 이해, 생성 및 편집을 위한 통합 멀티모달 모델 Lance를 오픈소스화했으며, 3B 비디오 + 3B 이미지 + 3B 디코더 구성 요소를 포함합니다.
*   Perplexity는 MaxSim 커널 사용에 대한 설명과 함께 작은 오픈 다국어 ColBERT 모델인 pplx-embed-0.6b의 계속 학습 변형을 출시했습니다.
*   Zyphra는 AMD Instinct MI355X에서 Kimi K2.6, GLM 5.1, DeepSeek V3.2 모델 서빙 시 AMD의 기준선 대비 강력한 성능 우위와 NVIDIA B200과의 격차를 좁혔다고 주장하는 종단 간 추론 벤치마크를 발표했습니다.

### 🛠️ 제품 & 도구
*   LangSmith Engine은 프로덕션 에이전트를 위한 CI/CD 루프로서, 프로덕션 트레이스에서 실패를 자동으로 감지하고 문제를 클러스터링하며 수정/평가를 초안 작성하는 기능을 제공합니다.
*   LangChain은 대규모 트레이스에 대한 낮은 레이턴시 쿼리 및 자체 호스팅/멀티 클라우드 요구 사항을 갖춘 에이전트 관측 가능성/평가 워크로드를 위한 특수 목적 데이터 레이어인 SmithDB를 강조했습니다.
*   Cognition은 버그, 경고 및 사고에 대한 상시 작동하는 "첫 번째 대응자"로, 장기 기억, 관리자/하위 에이전트 구조 및 PR 생성을 지원하는 Devin Auto-Triage를 출시했습니다.
*   Anthropic은 수백만 라인 규모의 모노레포, 레거시 시스템 및 마이크로서비스 전반에서 Claude Code를 실행하기 위한 모범 사례를 발표하고, 프롬프트 캐시 진단을 추가하며, 낮은 레이턴시 코딩 워크플로우를 위해 Fast 모드를 Opus 4.7으로 기본 설정했습니다.
*   OpenAI는 Zoom 플러그인, 모바일/데스크톱 원격 실행, 장시간 실행되는 작업이 휴대폰 앱에서 계속될 수 있도록 "Mac을 깨어 있게 유지" 지원을 추가하여 Codex 워크플로우를 확장했습니다.
*   Microsoft는 GitHub Copilot CLI와 VS Code용 원격 제어를 정식 출시(General Availability)했습니다.
*   Papers With Code는 메서드 파싱, 리더보드 및 SOTA 추적을 통해 AI 에이전트 지원 방식을 개선하며 연구 발견 가능성에 새로운 초점을 맞추고 있습니다.

### 🔬 연구 & 논문
*   "On Training in Imagination" 연구는 모델 기반 RL에서 낮은 립시츠 상수를 가진 더 부드러운 세계/보상 모델이 오류 경계를 강화하고, 보상 모델이 동적 모델보다 빠르게 스케일링되며, 많은 노이즈 있는 보상 레이블이 적은 고품질 레이블을 능가할 수 있지만 편향된 보상은 위험하다는 점을 강조했습니다.
*   Pedagogical RL에 대한 연구는 올바른 추론 트레이스라도 학생 정책에 비해 너무 놀랍다면 좋지 않은 학습 데이터가 될 수 있다고 주장하며, 특권 교사, 스파이크 인식 보상, 놀라움 게이트 모방을 사용하여 학생이 실제로 학습할 수 있는 궤적을 생성하는 방법을 제시했습니다.
*   Meta의 AIRA(Agentic Neural Architecture Discovery) 연구는 검색을 계획 에이전트(AIRA-Compose)와 구현 에이전트(AIRA-Design)로 분할하여 24시간 컴퓨팅 예산 내에서 350M, 1B, 3B 규모에서 Llama 3.2를 능가하는 신경 아키텍처를 발견했습니다.
*   "Slicing and Dicing MoEs" 논문은 2,000개 이상의 MoE LM 학습을 보고하며, MoE 설계 공간의 대부분이 전문가 크기(expert size)와 전문가 수(expert count)로 귀결된다고 결론지었습니다.
*   On-Policy Mix는 데이터 분포가 계속 변화함에 따라 올바른 데이터 믹스를 찾는 미해결 문제를 목표로 하며, 사전 학습, 중간 학습 및 지시 튜닝 전반에 걸쳐 적용 가능합니다.
*   에이전트 평가 가이드 및 Zhihu 요약은 에이전트 시대에는 정적 지식이나 내부 CoT 능력뿐만 아니라 위임 지능(delegation intelligence) — 즉, 언제 검색하고, 코딩하고, 추론하고, 도구를 호출할지 — 를 측정해야 한다고 주장했습니다.

### 💰 산업 동향
*   Anthropic은 초기 API 시절부터 자사 SDK를 지원해 온 SDK 및 MCP 서버 플랫폼 Stainless를 인수했습니다.
*   Cursor는 Colossus 2의 100만 H100 등가물에 접근하여 10배 더 많은 컴퓨팅으로 훨씬 큰 모델을 처음부터 학습시킬 계획인 'SpaceXAI' 이니셔티브를 공개했습니다.
*   Hugging Face와 Dell은 NVIDIA B300이 탑재된 Dell PowerEdge XE9780에 최적화된 Kimi K2.6, DeepSeek V4 Pro/Flash, GLM 5.1, MiniMax M2.7 모델에 대한 원클릭 액세스를 제공하는 Dell Enterprise Hub를 홍보했습니다.

### ⚡ 인프라 & 하드웨어
*   Georgi Gerganov는 llama.cpp에서 Qwen3.6 모델군에 대한 MTP(Multi-Token Prediction) 지원을 발표하며, A10G에서 Qwen3.6-27B dense 모델의 처리량이 25 tok/s에서 45 tok/s로 78% 향상되는 결과를 보였습니다.
*   Zyphra는 AMD Instinct MI355X에서 Kimi K2.6, GLM 5.1, DeepSeek V3.2 모델 서빙 시 AMD의 기준선 대비 강력한 성능 우위와 NVIDIA B200과의 격차를 좁혔다고 주장하는 종단 간 추론 벤치마크를 발표했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
