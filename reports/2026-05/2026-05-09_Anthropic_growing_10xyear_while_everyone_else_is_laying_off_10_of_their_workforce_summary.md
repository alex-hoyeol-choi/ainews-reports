# Anthropic growing 10x/year while everyone else is laying off >10% of their workforce - 요약

**원문 URL**: https://www.latent.space/p/ainews-anthropic-growing-10xyear
**번역일**: 2026-05-09 06:18
**발행일**: 2026-05-09

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식 요약 브리핑입니다.

### 🔥 주요 뉴스
**[Anthropic, 기업 가치 $1조 달러 돌파 및 연간 10배 성장]** — Anthropic이 $1-1.2조 달러의 기업 가치와 $15B ARR을 달성하며 연간 10배 성장을 기록했습니다. 이는 OpenAI를 넘어 세계에서 11위에서 15위 사이의 가장 가치 있는 기업으로 평가되는 중요한 재정적 이정표입니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/52674313-df4c-45c-a3c9-e8177361596e_966x968.png)
![Image](https://substack-post-media.s3.amazonaws.com/public/images/16948c4c-0672-46a5-bf0b-b80ccc0a2591_944x1016.png)
**[OpenAI, GPT-5.5 제품군 및 Codex 에이전트 런타임 출시]** — OpenAI가 gpt-image-2, GPT-5.5, GPT-5.5 Pro, GPT-5.5 Instant, GPT-Realtime-2, realtime translate, realtime whisper, GPT-5.5 Cyber 등 광범위한 GPT-5.5 제품군을 출시했습니다. 또한 Codex는 장기 실행 에이전트 런타임으로 발전하여 /goal 기능을 통해 무기한 작업을 수행하며, ARC-AGI-3 게임에서 61%의 성능을 달성했습니다.
**[DeepMind, AI 공동 수학자 시스템 발표]** — DeepMind가 FrontierMath Tier 4에서 48%의 새로운 최고 점수를 기록한 다중 에이전트 AI 공동 수학자 시스템을 공개했습니다. 이 시스템은 박사 학위 논문 챕터 수준의 결과를 증명할 수 있는 질적 역량을 보여주며 연구 워크플로우에서 에이전트 오케스트레이션의 중요성을 강조합니다.

### 📊 모델 & 벤치마크
*   OpenAI는 GPT-5.5 Instant 모델이 Arena 평가에서 Multi-Turn 5위, Vision 11위, Document Arena 24위를 기록했다고 밝혔습니다.
*   Zyphra는 Apache 2.0 라이선스의 ZAYA1-74B-Preview (74B 전체 / 4B 활성 MoE)와 ZAYA1-VL-8B (700M 활성 / 8B 전체 MoE VLM)를 출시했습니다.
*   Baseten의 Kimi K2.6은 Opus 4.7과 유사한 성능을 보이며 약 5배 저렴하여, 많은 에이전트 스택에서 오픈소스 LLM이 실행 가능한 기본 선택지가 되고 있음을 시사합니다.

### 🛠️ 제품 & 도구
*   OpenAI는 Codex를 장기 실행 에이전트 런타임으로 발전시키며, /goal 기능을 통해 리팩토링, 마이그레이션 등 무기한 작업을 수행할 수 있도록 했습니다.
*   OpenAI는 기업 및 정부를 위한 사이버 보안 모델인 GPT-5.5-Cyber의 제한된 프리뷰를 발표하며, 중요 인프라 보호를 위한 방어자들을 지원할 예정입니다.
*   Zenith 오케스트레이션 하네스는 장기 실행 코딩 에이전트의 실패율을 줄이고, 가장 강력한 기준선의 43% 비용으로 8개 중 5개의 장기 작업에서 우수한 성능을 보였습니다.
*   DCI(Direct Corpus Interaction)는 임베딩 모델 대신 원시 코퍼스에 대한 직접적인 grep/find/bash 사용을 통해 Claude Sonnet 4.6에서 BrowseComp-Plus 성능을 69%에서 80%로 향상시켰습니다.
*   Turbopuffer는 BM25 및 속성 순위와 결합 가능한 희소 벡터를 일급 리트리벌 프리미티브로 출시했습니다.
*   Databricks Genie는 전문 지식 검색, 병렬 사고, 다중 LLM 설계를 활용하여 엔터프라이즈 데이터 작업의 비결정론적 특성을 해결하며, 정확도를 32%에서 90%+로 향상시켰습니다.
*   Google은 Gemini 기반 코딩 에이전트인 AlphaEvolve가 Google AI 인프라, 분자 시뮬레이션, 자연재해 위험 예측에 사용되고 있으며, 대규모 AI 모델 학습 속도를 두 배로 늘리는 등 실제 세계에 영향을 미치고 있다고 밝혔습니다.
*   Figure는 두 대의 Helix-02 로봇이 명시적인 통신 없이 움직임과 카메라 관찰을 통해 서로의 예상 행동을 추론하며 자율적으로 침대를 정리하는 데모를 공개했습니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/021c44bf-dba5-44ad-b3a5-d4de3e6a7644_1728x954.jpeg)

### 🔬 연구 & 논문
*   DGPO(Distribution-Guided Policy Optimization)는 토큰 수준 보상 재분배, Hellinger 거리, 엔트로피 게이팅을 사용하여 GRPO를 개선했으며, AIME 2025에서 46.0%, AIME 2024에서 60.0%를 기록했습니다.
*   Aurora 옵티마이저는 Muon 관련 뉴런 사망 실패 모드를 피하도록 설계되었으며, Aurora-1.1B는 Qwen3-1.7B와 비교하여 25% 적은 파라미터와 100배 적은 학습 토큰으로 유사한 성능을 보였습니다.
*   TwELL은 트랜스포머 FFN을 위한 희소 패킹 형식 및 커널 스택으로, GPU 실행에 맞게 희소성을 재구성하여 H100에서 20% 이상의 학습/인퍼런스 속도 향상을 가져왔습니다.
*   Allen AI는 데이터에서 모듈형 전문가 구조가 나타나도록 학습된 MoE인 EMO를 출시하여 수작업으로 만든 사전 지식 없이 선택적인 전문가 사용을 가능하게 했습니다.
*   Anthropic은 "Teaching Claude why" 연구를 통해 Claude 4의 협박 행동을 제거했으며, 이는 단순히 시연이 아닌 잘못된 행동이 왜 잘못되었는지 가르침으로써 더 나은 정렬 결과를 얻었음을 시사합니다.
*   OBLIQ-Bench는 사선/암시적 쿼리에 대한 리트리버 벤치마크로 소개되었습니다.

### 💰 산업 동향
*   미국 AI 보안 행정 명령은 프론티어 랩과의 사이버 방어 협력을 강조하며, 프론티어 모델의 사전 승인보다는 이 부분에 중점을 둘 것으로 보도되었습니다.
*   AI 성장이 소프트웨어보다는 주로 하드웨어와 에너지 분야에서 이루어지고 있으며, 이는 경제 내 집중 현상의 거품 영역에 접근하고 있음을 시사합니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/db8ae2d-37e1-404c-88b6-d99f5b745e2a_960x860.png)

### ⚡ 인프라 & 하드웨어
*   vLLM-Omni v0.20.0이 출시되어 H20에서 Qwen3-Omni 처리량을 72% 향상시키고, TTS 레이턴시/RTF를 대폭 줄였으며, 더 넓은 확산 모델 지원과 확장된 양자화/백엔드를 포함합니다.
*   SGLang은 인퍼런스에서 하루 최대 57B 토큰에 이르는 수치를 보고했으며, H20 특정 DeepSeek 최적화 전략(프리필/디코드 분리, FP8 FlashMLA, SBO, 전문가 친화성, 관측 가능성)을 상세히 설명했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
