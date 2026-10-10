# TypeSafe/Jev at >$100M ARR, $7.5B valuation 3 weeks after launch - 요약

**원문 URL**: https://www.latent.space/p/ainews-typesafejev-at-100m-arr-75b
**번역일**: 2026-10-10 12:28
**발행일**: 2026-10-10

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 간결한 브리핑입니다.

### 🔥 주요 뉴스
**[TypeSafe/Jev, 출시 3주 만에 >$100M ARR 달성]** — TypeSafe의 Jev API가 출시 3주 만에 연간 반복 매출(ARR) 1억 달러를 돌파하며 75억 달러의 가치를 달성했습니다. Sequoia는 Jev가 첫 주에 1억 달러 ARR을 넘어섰다고 밝혔습니다.
![X avatar for @CompleteSkeptic](https://pbs.substack.com/profile_images/1650708125685800960/7k6r0UZg.jpg)
**[‘결정 모델(Decision Model)’ 카테고리 부상]** — 여러 벤더들이 동시에 "결정 모델"을 출시하며 새로운 제품 카테고리가 형성되고 있습니다. 이 모델들은 자유 텍스트 대신 단일 포워드 패스로 확률, 목록 선택, 점수 등 타입이 지정된 답변을 반환합니다.
**[OpenAI Decisions API 출시]** — OpenAI가 GPT-6 Luna 기반의 Decisions API를 출시했습니다. 이 API는 텍스트와 이미지를 모두 받아 조건 참 확률, 목록 선택, 레벨 점수 등 세 가지 타입의 결정을 제공하며, M 입력 토큰당 $0.10의 비용으로 출력 요금은 없습니다.
**[Claude Managed Agents 동적 워크플로우 공개 베타]** — Anthropic이 Claude Managed Agents의 동적 워크플로우를 공개 베타로 출시했습니다. 리드 에이전트가 계획을 수립하고 최대 1,000개의 에이전트에 작업을 분산시킨 후 결과를 병합하는 방식입니다.

### 📊 모델 & 벤치마크
*   **Perplexity pplx-decider-v1.1-27b 출시 및 벤치마크** — Perplexity가 pplx-decider-v1.1-27b를 출시하며 Decision Bench 1,071개 사례에서 94.5%의 최고 정확도를 달성했다고 주장했습니다. 1K 결정당 $0.017의 비용이 부과됩니다.
*   **Cloudflare clef-omni 및 clef-flash 업데이트** — Cloudflare의 새로운 clef-omni는 오디오, 비디오, 이미지, 텍스트를 모두 처리하며, clef-flash는 Jev보다 저렴하고 약 2배 더 빠르다고 발표했습니다. 가중치는 Hugging Face에서 공개됩니다.
*   **Qwen-Image-2.1-Turbo 오픈 웨이트 출시** — Alibaba Qwen이 7B Qwen-Image-2.1의 가속화된 체크포인트인 Qwen-Image-2.1-Turbo를 오픈 웨이트로 출시했습니다. 8단계 2K 생성 및 자연어 편집을 지원하며, Pro 및 Turbo API를 통해 제공됩니다.
*   **StepFun Step 5 Preview 공개 및 벤치마크** — StepFun이 총 600B, 활성 27B의 희소 MoE 모델인 Step 5 Preview를 공개했습니다. 1M 컨텍스트와 비전을 지원하며, Hermes Index에서 33.89점을 기록하여 GPT-6 Luna와 동등한 성능을 보였습니다. 오픈 웨이트는 10월 15일 출시 예정입니다.
*   **Upstage Solar Mini 4 출시 및 벤치마크** — Upstage가 3B 활성, 524K 컨텍스트 및 208 tok/s를 가진 35B MoE 모델인 Solar Mini 4를 출시했습니다. AAII 점수 24점으로 3B 활성 모델 중 최고 성능을 기록했으며, Cline에서 무료로 제공됩니다.
*   **Gemini 4 Argon 벤치마크 및 초기 출시** — Gemini 4 Argon이 DeepSWE v1.1에서 77.9%의 점수를 기록하여 Opus 5.5의 74.2%를 능가했습니다. Fairwind Program 방어자 650명 이상에게 M 토큰당 $2/$10의 가격으로 먼저 출시됩니다.
*   **HeyGen Voice 및 Whistle 음성 모델 출시** — HeyGen Voice가 Artificial Analysis Controlled Voice TTS 아레나에서 ELO 1,201점으로 1위를 차지하며 1M 문자당 $30, 초당 40문자의 속도를 제공합니다. Whistle은 Whisper base에 필적하는 16.9MB 온디바이스 STT 모델로 공개되었습니다.
*   **멀티턴 이미지 편집 모델 평가** — Artificial Analysis가 30개의 연속적인 편집을 연결하는 멀티턴 이미지 편집 평가를 수행했습니다. Ideogram 4.5와 FLUX 3는 이미지의 95% 이상을 유지하며 로컬 편집을 수행한 반면, GPT Image 2.5 Sunburst는 매 턴마다 프레임의 대부분을 다시 렌더링하여 드리프트 현상을 보였습니다.
*   **새로운 OCR 벤치마크 공개** — Roboflow가 48개 모델을 다루는 새로운 OCR 벤치마크를 출시했으며, GPT-6 Astra가 텍스트 로컬라이제이션에서 선두를 달리고 있습니다. Datalab의 OmniParseBench는 90개 언어에 걸쳐 16K개의 테스트를 포함합니다.
*   **최신 아레나 벤치마크 결과** — Claude Haiku 5.5는 WebDev에서 $0.10/$0.50의 가격으로 GPT-6 Luna보다 6점 높은 점수를 기록하며 30위에 올랐습니다. ARC-AGI-3에서는 59.17%의 새로운 최고 점수가 달성되었습니다.

### 🛠️ 제품 & 도구
*   **OpenAI Decisions API 기능** — OpenAI Decisions API는 텍스트와 이미지를 모두 입력으로 받아 조건 참 확률, 목록에서 선택, 레벨에 대한 점수 등 세 가지 요청 타입을 지원합니다.
*   **Microsoft-Decision-1 포지셔닝** — Microsoft-Decision-1은 LLM 심사관 및 과학적 가설 스크리닝을 위한 용도로 포지셔닝되었습니다.
*   **Liquid d1 Vercel AI Gateway 통합** — Liquid d1이 Vercel AI Gateway에서 사용 가능해졌으며, 분류, 라우팅, 점수 매기기 작업에 대한 비전 지원을 제공합니다.
*   **vLLM Semantic Router Decision 2.0 출시** — vLLM Semantic Router Decision 2.0은 단일 입력에 대해 여러 질문에 대한 답변을 한 번의 패스로 옵션별 확률과 함께 제공합니다.
*   **LangSmith Jev 통합** — LangSmith는 Jev를 모든 트레이스에서 난이도와 정확성에 대한 별도의 타입이 지정된 답변을 반환하는 심사관으로 활용합니다.
*   **Unsloth 결정 모델 전환 무료 노트북 출시** — Unsloth가 8GB VRAM에서 Qwen3.5-4B를 결정 모델로 전환하는 무료 노트북을 출시했습니다.
*   **Claude Code Projects 기능 확장** — Claude Code Projects가 모든 Pro 및 Max 사용자에게 승인되었으며, 각 프로젝트는 병렬 스레드로 작업을 실행하고 세션은 로컬에서 실행될 수 있습니다.
*   **Opus 5.5 fast mode 출시** — Opus 5.5의 fast mode가 출시되었으나, 사용 크레딧에 따라 요금이 부과되며 구독에는 포함되지 않습니다.
*   **Codex Windows 샌드박스 업데이트** — Codex는 Microsoft Execution Containers (MXC) 기반의 새로운 Windows 샌드박스 모드를 도입하여 더 빠른 설정, 네트워크 적용 및 세분화된 파일 제어를 제공합니다.
*   **Codex Composer 예측 기능 베타 출시** — Codex가 다음 메시지를 제안하는 Composer 예측 기능을 Pro 사용자에게만 베타로 제공합니다.
*   **Devin 기능 확장** — Devin은 이제 관리되는 Devin들의 트리를 생성하여 실제 소요 시간을 가장 느린 브랜치로 추적할 수 있으며, GPT 사용을 위한 개인 ChatGPT 플랜을 받습니다.
*   **Grok Bot 이메일 주소 확보** — Grok Bot이 가입 및 스케줄링을 위한 자체 이메일 주소를 확보했습니다.
*   **Datology Curation Studio 출시** — Datology Curation Studio는 30B MoE를 위해 39개의 오픈 데이터셋에서 6배의 컴퓨팅 승수를 주장하며, $450K로 학습된 Thomson-1이 GPT-5.6 Sol을 이겼다고 인용합니다.
*   **Tinker 가격 인하 및 모델 추가** — Tinker는 최대 70%의 가격 인하를 단행하고 긴 컨텍스트와 짧은 컨텍스트의 가격을 동일하게 책정했으며, GLM-5.3-Flash 및 DeepSeek-v4.1-Flash 모델을 추가했습니다.

### 🔬 연구 & 논문
*   **Apple/CMU의 "Selection-based Structured Reasoning (SSR)" 연구** — Apple과 CMU의 공동 연구 "Selection-based Structured Reasoning (SSR)"은 에이전트 내부에 결정 모델과 유사한 아이디어를 적용합니다. KV-cache를 공유하는 배치 포워드 패스에서 6가지 자연어 전략을 평가하여 턴당 추론 레이턴시를 90% 이상 감소시켰습니다.
*   **DeepSeek 주기적 약점 발견 (ByteDance Seed)** — ByteDance Seed는 DeepSeek 모델에서 리트리벌 성능이 토큰이 압축 스트라이드에 상대적으로 어디에 위치하는지에 따라 달라지는 주기적인 약점을 발견했습니다. 이 패턴은 RoPE나 학습된 게이트 없이도 지속되며, V4.1의 스트라이드 2가 이 효과를 줄이지만 완전히 제거하지는 못합니다.
*   **Meta의 에이전트 가소성(Agent plasticity) 연구** — Meta는 학습 비용당 보유 이득을 측정하는 에이전트 가소성 연구를 통해 최고의 성능을 보이는 에이전트가 항상 가장 효율적인 학습자는 아니라는 점을 발견했습니다.
*   **MIMESIS: 9B 사용자 시뮬레이터 개발** — MIMESIS는 행동 충실도에서 Opus 5를 13.4점 앞서는 9B 사용자 시뮬레이터로 개발되었습니다.
*   **NVIDIA의 기반 모델 선택 연구** — NVIDIA는 기반 모델이 "결정적인 편집"을 재현할 수 있는지 여부에 따라 체크포인트를 순위 매기는 연구를 진행했으며, 이는 사후 학습된 SWE-bench Verified 점수를 추적하는 신호입니다.

### 💰 산업 동향
*   **TypeSafe/Jev, 출시 3주 만에 >$100M ARR, $7.5B 가치 달성** — TypeSafe의 Jev API가 출시 3주 만에 연간 반복 매출(ARR) 1억 달러를 돌파하며 75억 달러의 가치를 달성했습니다.
*   **결정 모델(Decision Model)의 제품 카테고리 부상** — 여러 벤더들이 동시에 "결정 모델"을 출시하며 자유 텍스트 대신 타입이 지정된 답변을 반환하는 새로운 AI 모델 카테고리가 빠르게 확산되고 있습니다.
*   **LangChain, 결정 모델 활용으로 비용 64% 절감** — LangChain은 각 작업을 가장 저렴하고 적절한 모델로 라우팅하는 결정 모델 활용을 통해 작업당 Open SWE 중앙값 비용을 64% 절감했다고 밝혔습니다.
*   **Vals AI, 멀티 에이전트 팀 효과 평가** — Vals AI는 Vibe Code Bench에서 GPT-6 Sol과 Opus 5.5를 단독 또는 팀으로 실행한 결과, 팀 구성 시 비용은 1.8~5.1배 증가했으나, 중간 노력의 Sol 팀만이 7.3점 향상으로 유의미한 개선을 보였습니다.

### ⚡ 인프라 & 하드웨어
*   **vLLM, GB200에서 처리량 7.8배 이상 증가 보고** — vLLM은 AgentX에서 동일한 상호작용성으로 MiniMax M3에서 GB200 처리량이 7.8배 이상 증가했다고 보고했습니다.
*   **Locality-aware MoE 기술 개발** — CUDA 13.4 로컬리티 도메인을 활용하여 각 SM이 로컬 HBM만 읽도록 하는 Locality-aware MoE 기술이 개발되어 MoE 디코드를 최대 1.2배 더 빠르게 만듭니다.
*   **SGLang, FP8 MLA 및 MoE 테일 퓨전으로 성능 향상** — SGLang은 128K 컨텍스트에서 FP8 MLA를 최대 20% 더 빠르게 하고, 디코드 단계당 276개의 론치를 제거하는 MoE 테일 퓨전을 통해 5.9%의 엔드투엔드 이득을 달성했습니다.
*   **TRL v1.15, 퓨즈드 LM 헤드 기본 활성화** — TRL v1.15는 퓨즈드 LM 헤드를 기본적으로 활성화하여 전체 로짓 텐서를 구체화하는 것을 방지합니다. 이로 인해 Gemma 3 1B에서 GRPO 시퀀스 길이가 28K에서 114K로, DPO는 10K에서 59K로 증가하며 학습 속도가 약 11% 빨라지고 피크 메모리가 52~82% 감소합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
