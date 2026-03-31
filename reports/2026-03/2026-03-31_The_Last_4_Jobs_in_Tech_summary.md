# The Last 4 Jobs in Tech - 요약

**원문 URL**: https://www.latent.space/p/ainews-the-last-4-jobs-in-tech
**번역일**: 2026-03-31 01:18
**발행일**: 2026-03-31

---

다음은 제공된 AI 뉴스레터 내용에서 추출한 핵심 신규 소식 요약입니다.

### 🔥 주요 뉴스
**[Claude Code, 컴퓨터 사용 기능 확보]** — Anthropic은 Claude Code 내부에 컴퓨터 사용 기능을 추가하여, Pro/Max 사용자를 대상으로 한 연구 프리뷰에서 에이전트가 앱을 열고, UI를 클릭하며, CLI에서 직접 구축한 것을 테스트할 수 있도록 했습니다. 이는 코드 실행 후 UI 검사 및 수정으로 이어지는 폐쇄 루프 검증을 가능하게 합니다.
**[Qwen3.5-Omni 출시]** — Alibaba는 네이티브 텍스트/이미지/오디오/비디오 이해, 스크립트 수준 캡셔닝, 내장 웹 검색 및 함수 호출 기능을 갖춘 Qwen3.5-Omni를 발표했습니다. 특히 음성 시각 지시를 통해 웹사이트/게임을 구축하는 "오디오-비주얼 바이브 코딩" 데모가 주목받았습니다.
**[llama.cpp GitHub 별 10만 개 달성]** — @ggerganov의 llama.cpp 프로젝트가 GitHub에서 10만 개의 별을 달성하며 로컬 AI 런타임의 중요성과 잠재적 돌파구를 상징적으로 보여주었습니다. 이는 유용한 자동화가 프론티어 규모의 호스팅 모델을 필요로 하지 않으며 올바른 휴대용 런타임 스택이 중요함을 강조합니다.

### 📊 모델 & 벤치마크
*   **Qwen3.5-Omni 출시:** Alibaba는 네이티브 텍스트/이미지/오디오/비디오 이해, 스크립트 수준 캡셔닝, 내장 웹 검색 및 함수 호출 기능을 갖춘 Qwen3.5-Omni를 발표했습니다. 이 모델은 10시간 오디오 / 400초의 720p 비디오, 113개 음성 인식 언어, 36개 음성 언어를 지원하며, 오디오에서 Gemini 3.1 Pro를 능가하고 일부 AV 이해 설정에서 동등하다고 주장합니다.
*   **GLM-5-Turbo 평가:** Artificial Analysis는 Z AI의 에이전트 최적화 변형인 GLM-5-Turbo를 평가했으며, AA Intelligence Index에서 47점, GDPval-AA에서 1503점을 기록하여 실제 에이전트 워크플로우에 맞춰 튜닝되었다는 주장을 뒷받침합니다.
*   **Qwen3.5-27B 모델:** Claude 4.6 Opus에서 디스틸레이션된 Qwen3.5-27B 모델이 4비트에서 16GB에 적합하며 몇 주 동안 Hugging Face에서 트렌드였습니다.
*   **World Reasoning Arena 벤치마크:** 가설/세계 모델 추론을 목표로 하는 World Reasoning Arena가 출시되었으며, 인간과의 상당한 격차를 보고합니다.
*   **Tau Bench 뱅킹 도메인:** Tau Bench에 현실적인 698개 문서 지원 환경의 새로운 뱅킹 도메인이 추가되었으며, 최고 모델도 여전히 약 25%의 작업만 해결하는 것으로 나타났습니다.

### 🛠️ 제품 & 도구
*   **Claude Code 컴퓨터 사용 기능:** Anthropic은 Claude Code 내부에 컴퓨터 사용 기능을 추가하여, Pro/Max 사용자를 대상으로 한 연구 프리뷰에서 에이전트가 앱을 열고, UI를 클릭하며, CLI에서 직접 구축한 것을 테스트할 수 있도록 했습니다.
*   **OpenAI Codex 플러그인 for Claude Code:** OpenAI는 Claude Code용 Codex 플러그인을 출시하여, ChatGPT 구독을 사용하여 Anthropic의 툴체인 내에서 리뷰, 적대적 리뷰 및 "구조" 플로우를 트리거할 수 있게 했습니다.
*   **OpenAI Codex 야간 작업 개선:** OpenAI는 심야 Codex 작업이 더 오래 실행되며, 오후 11시경에 시작된 작업이 3시간 이상 실행될 가능성이 60% 더 높다고 밝혔습니다.
*   **Hermes Agent 주요 업데이트:** Nous는 Hermes Agent의 주요 업데이트를 출시하여 더 나은 압축, 불필요한 요소 감소, 더 강력한 적응성 및 더 빠른 출시 주기를 제공합니다. 새로운 다중 에이전트 프로필은 각 봇에 자체 메모리, 스킬, 기록 및 게이트웨이 연결을 제공합니다.
*   **opentraces.ai 출시:** @jayfarei의 opentraces.ai는 에이전트 트레이스를 정제하고 Hugging Face에 게시하여 분석, 평가, SFT 및 RL에 활용할 수 있는 CLI/스키마/리뷰 플로우를 제공합니다.
*   **PokeeClaw 강조:** @fchollet은 샌드박싱, 승인, RBAC 및 감사 추적 기능을 갖춘 더 안전한 OpenClaw 스타일 어시스턴트인 PokeeClaw를 강조했습니다.
*   **AutoClaw 출시:** Z AI는 API 키가 필요 없고 GLM-5-Turbo를 선택적으로 사용할 수 있는 로컬 OpenClaw 런타임인 AutoClaw를 출시했습니다.
*   **Transformers.js v4 출시:** Transformers.js v4는 브라우저/Node/Bun/Deno 전반에 걸쳐 WebGPU 백엔드를 추가하여 주요 성능 향상과 200개 이상의 아키텍처를 지원합니다.
*   **vLLM-Omni v0.18.0 출시:** vLLM-Omni v0.18.0은 324개의 커밋, 프로덕션 TTS/옴니 서빙, 통합 양자화, 확산 런타임 리팩터링 및 십여 개 이상의 새로운 모델을 출시했습니다.
*   **Cohere Transcribe 출시:** Artificial Analysis는 Apache 2.0 라이선스이며 14개 언어로 학습된 2B 컨포머 인코더-디코더 모델인 Cohere Transcribe를 다루었으며, 4.7% AA-WER을 달성하고 약 60배의 실시간 전사 속도를 보였습니다.

### 🔬 연구 & 논문
*   **자연어 에이전트 하네스 논문:** 칭화/선전 대학의 논문은 LLM이 하드코딩된 하네스 규칙 대신 SOP에서 오케스트레이션 로직을 실행하도록 제안했습니다.
*   **Meta-Harness 연구:** Meta는 기본 모델뿐만 아니라 코드, 트레이스 및 점수에 걸쳐 하네스를 엔드투엔드로 최적화하는 방법인 Meta-Harness를 개발했습니다. 이는 TerminalBench-2에서 Haiku 에이전트 중 1위를 차지했습니다.
*   **CAID 논문 (비동기/다중 에이전트 SWE):** CMU의 CAID 논문은 관리자 에이전트, 의존성 그래프, 격리된 Git 워크트리, 자체 검증 및 병합을 사용하는 중앙 집중식 비동기 격리 위임을 주장하며, PaperBench에서 단일 에이전트 기준선 대비 +26.7, Commit0에서 +14.3의 이득을 보고했습니다.
*   **코딩 에이전트의 긴 컨텍스트 처리 논문:** @dair_ai가 강조한 논문은 방대한 코퍼스를 디렉토리 트리로 취급하고, 상용 코딩 에이전트가 셸 명령과 Python으로 이를 탐색하도록 하여 BrowseComp-Plus (7억 5천만 토큰)에서 88.5%의 성능을 달성했습니다.
*   **Gram Newton-Schulz 최적화:** Gram Newton-Schulz는 Muon의 Newton-Schulz 단계를 드롭인 대체할 수 있는 것으로, Muon을 최대 2배 빠르게 만들면서 검증 퍼플렉시티를 0.01 이내로 유지한다고 보고되었습니다.
*   **LLM 학습 코드의 PyTorch trunc_normal_ 오용 패턴 지적:** Ross Wightman은 LLM 학습 코드에서 PyTorch trunc_normal_의 미묘하지만 중요한 오용 패턴을 지적하며, 많은 코드베이스가 사실상 전혀 잘라내지 않고 있음을 밝혔습니다.
*   **아첨하는 AI의 영향 연구:** 스탠포드 주도 논문은 아첨하는 AI가 사용자의 확신을 높이는 반면 관계를 회복하려는 의지를 감소시킬 수 있으며, "유용성" 지표가 사회적으로 해로운 행동을 가릴 수 있음을 강조했습니다.

### 💰 산업 동향
*   **Shopify의 DSPy 사례 연구:** Shopify는 DSPy를 사용하여 비즈니스 로직을 분해하고, 의도를 모델링하며, 더 작고 최적화된 모델로 전환함으로써 연간 550만 달러에서 7만 3천 달러로 비용을 절감했다고 보고했습니다.

### ⚡ 인프라 & 하드웨어
*   **llama.cpp GitHub 별 10만 개 달성:** @ggerganov의 llama.cpp 프로젝트가 GitHub에서 10만 개의 별을 달성하며 로컬 AI 런타임의 중요성을 강조했습니다. 이는 교차 하드웨어, 벤더 종속 없는 인프라의 중요성을 부각합니다.
*   **Apple Silicon의 Flash-MoE:** Qwen3.5-397B가 순수 C + Metal 엔진을 사용하여 48GB MacBook Pro에서 4.4 토큰/초로 실행될 수 있으며, 인퍼런스 중 약 5.5GB RAM을 사용한다고 보고되었습니다.
*   **anemll-flash-mlx 및 AI Toolkit Apple Silicon 지원:** MLX 위에 MoE 경로만 최적화하는 anemll-flash-mlx와 AI Toolkit의 새로운 Apple Silicon 지원이 관련 작업으로 언급되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
