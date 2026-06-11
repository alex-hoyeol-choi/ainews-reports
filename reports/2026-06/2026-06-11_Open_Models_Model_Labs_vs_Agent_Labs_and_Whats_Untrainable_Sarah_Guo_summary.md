# Open Models, Model Labs vs Agent Labs, and What's Untrainable — Sarah Guo - 요약

**원문 URL**: https://www.latent.space/p/ainews-open-models-model-labs-vs
**번역일**: 2026-06-11 06:51
**발행일**: 2026-06-11

---

다음은 제공된 AI 뉴스레터 내용에서 핵심 신규 소식만을 추출한 브리핑입니다.

### 🔥 주요 뉴스
**[Anthropic Fable 5 출시 및 논란]** — Anthropic이 새로운 모델 Fable 5(Mythos)를 출시했으나, AI 연구 관련 프롬프트에 대한 모델 성능을 사전 공개 없이 저하시켰다는 비판에 직면했습니다. 또한, 일부 설정에서 30일간의 프롬프트/데이터 보존 기능이 옵트아웃 불가능하여 데이터 보존 및 록인(lock-in) 우려가 제기되었습니다.
**[Fable 5의 강력한 벤치마크 성능]** — 논란에도 불구하고 Fable 5는 Agent Arena에서 전반적으로 1위를 차지하고, SimpleBench 81.9%, CADGenBench 1위, PACT 협상 1위 등 에이전틱 및 코딩 워크로드에서 강력한 성능을 보였습니다. Perplexity와 Apple 개발자 플랫폼에 빠르게 통합되었습니다.
**[Google DiffusionGemma 오픈 웨이트 출시]** — Google이 Gemma 4 기반의 실험적인 26B MoE 확산 텍스트 모델인 DiffusionGemma를 Apache 2.0 라이선스로 오픈 웨이트로 출시했습니다. 이 모델은 자동회귀 방식 대신 텍스트 블록을 동시에 생성 및 정제하여 최대 4배 빠른 출력과 초당 1,000개 이상의 토큰 생성을 주장합니다.
**[AI 에이전트 벤치마크 방법론 변화]** — Agent Arena가 인간 선호도 기반에서 bash 오류, 도구 환각 등 객관적인 신호를 채굴하는 장기 트레이스 기반 에이전트 지표로 전환하는 새로운 방법론을 상세히 설명했습니다. 이는 에이전트 평가의 중요한 방향 전환을 의미합니다.
**[Anthropic의 AI 정책 제안]** — Dario Amodei가 "Policy on the AI Exponential"을 발표하며 AI 발전이 제도를 앞지르고 있다고 주장하고 더 강력한 프론티어 AI 감독을 촉구했습니다. 이는 불투명한 모델 변경으로 비판받는 시점에 나온 정책 제안으로 주목받고 있습니다.

### 📊 모델 & 벤치마크
*   Anthropic이 새로운 모델 Fable 5를 출시했습니다. 이 모델은 Agent Arena에서 전반적으로 1위를 차지했으며, SimpleBench 81.9%, CADGenBench 1위, PACT 협상 1위 등 에이전틱 및 코딩 워크로드에서 강력한 성능을 보였습니다.
*   Google이 Gemma 4 기반의 실험적인 26B MoE 확산 텍스트 모델인 DiffusionGemma를 Apache 2.0 라이선스로 오픈 웨이트로 출시했습니다. 이 모델은 자동회귀 방식 대신 텍스트 블록을 동시에 생성 및 정제하여 최대 4배 빠른 출력과 초당 1,000개 이상의 토큰 생성을 주장합니다.
*   ZyphraAI가 Apache 2.0 라이선스로 Zamba2-VL을 출시하며 하이브리드 SSM-Transformer 아이디어를 VLM으로 확장했습니다.
*   Agent Arena는 인간 선호도 대신 bash 오류, 도구 환각 등 객관적인 신호를 위해 장기 트레이스를 채굴하는 새로운 에이전트 평가 방법론을 상세히 설명했습니다.

### 🛠️ 제품 & 도구
*   Perplexity가 Pro/Max 사용자를 위한 Computer 기능에 Claude Fable 5를 오케스트레이터 모델로 추가했습니다.
*   Apple 개발자들은 다단계 추론, 더 긴 컨텍스트, 코드 사용을 위해 Claude의 Foundation Models 프레임워크 지원을 받게 되었습니다.
*   Teknium이 GUI 기반 Hermes Agent 프로필을 출시했으며, 메모리/스킬 업데이트를 위한 Write Gate 승인 제어 기능을 추가했습니다.
*   Weaviate가 Engram에서 그룹, 토픽, 스코프를 사용하여 구조화된 에이전트 메모리를 설명했습니다.
*   FactoryAI가 Factory Desktop에서 Missions를 출시했습니다.
*   Perceptroninc가 원샷 탐지기 대신 다중 호출 줌/추론 루프를 사용하는 밀집되고 모호한 시각적 탐지를 위한 Agentic Detection을 출시했습니다.
*   tonywu_71이 ColBERT/ColPali/LateOn에서 사용되는 MaxSim을 위한 융합된 Triton 커널인 late-interaction-kernels를 출시했습니다. 이는 PyTorch와 수치적으로 동등하면서도 메모리 사용량을 크게 줄였다고 주장합니다.

### 🔬 연구 & 논문
*   새로운 연구에 따르면 확산 비디오 모델이 일부 프로브에서 V-JEPA/VideoMAE보다 물리적 정보를 선형적으로 더 잘 인코딩하여 "비디오 생성 모델은 멍청한 물리 시뮬레이터"라는 통념에 도전했습니다.
*   edunov가 Pearl보다 약 5배 빠르면서도 품질을 유지한다고 보고된 플로우 맵 공동 폴딩 모델인 DeCAF-Pearl을 소개했습니다.

### 💰 산업 동향
*   Dario Amodei가 "Policy on the AI Exponential"을 발표하며 AI 발전이 제도를 앞지르고 있다고 주장하고 더 강력한 프론티어 AI 감독을 촉구했습니다.
*   Anthropic Fable/Mythos가 일부 설정에서 30일간의 프롬프트/데이터 보존 기능을 제공하며 옵트아웃이 불가능하다고 보고되어, 제로 보존 환경 및 유럽 일부 지역을 배제한다는 우려가 제기되었습니다.

### ⚡ 인프라 & 하드웨어
*   DiffusionGemma는 vLLM에서 기본적으로 지원되는 최초의 확산 LLM으로, 단일 H200에서 FP8로 배치 크기 1일 때 초당 1200개 이상의 출력 토큰을 기록했습니다.
*   danielhanchen은 llama.cpp와 GGUF를 통해 DiffusionGemma가 로컬에서 실행되는 것을 시연했으며, UnslothAI는 18GB급 하드웨어에서의 로컬 실행을 강조했습니다.
*   vllm_project가 인퍼런스 경제성을 중심으로 최적화된 커뮤니티 에이전트 하네스인 Inferoa를 강조했습니다.
*   Azaliamirh가 분산형 다중 에이전트 프레임워크인 DeLM을 소개했습니다. 이 프레임워크는 Gemini 3-Flash를 사용하여 중앙 집중식 대안의 절반 미만 비용으로 SWE-bench Verified 65.7%에 도달했다고 보고되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
