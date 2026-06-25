# It's Meta-Harness Summer - 요약

**원문 URL**: https://www.latent.space/p/ainews-its-meta-harness-summer
**번역일**: 2026-06-25 06:50
**발행일**: 2026-06-25

---

다음은 AI 산업 동향에 대한 핵심 브리핑입니다.

### 🔥 주요 뉴스
**OpenAI, 맞춤형 AI 칩 'Jalapeño' 발표** — OpenAI는 Broadcom과 협력하여 LLM 인퍼런스를 위한 첫 번째 맞춤형 AI 칩인 Jalapeño를 공개했습니다. 이 칩은 ChatGPT, Codex, API 트래픽 및 미래 에이전트 제품에 사용될 예정이며, 컴퓨팅 경제성과 제품 동작의 독립성을 강화하려는 전략의 일환입니다.
**Anthropic, Slack 네이티브 Claude 에이전트 모델 출시** — Anthropic은 Slack/팀 워크플로우에 통합된 Claude 에이전트 모델을 발표했습니다. Claude는 자체 자격 증명을 가지며 모든 행동이 감사 가능하고 접근 권한이 중앙에서 철회될 수 있도록 설계되어, 엔터프라이즈 에이전트의 ID 및 권한 문제를 해결합니다.
**Alibaba Qwen, Qwen-AgentWorld 공개 및 오픈소스화** — Alibaba Qwen은 단일 모델 내에서 7가지 환경을 시뮬레이션하는 에이전트용 "언어 세계 모델"인 Qwen-AgentWorld를 소개했습니다. Qwen-AgentWorld-35B-A3B와 AgentWorldBench를 오픈소스화했으며, 35B MoE / 3B 활성, 256K 컨텍스트 모델을 제공합니다.
**GLM-5.2, 오픈 모델 벤치마크에서 강세 지속** — GLM-5.2는 Artificial Analysis 및 Agent Arena의 오픈 모델 순위에서 1위를 차지하며 현재 가장 강력한 오픈 웨이트 경쟁자로 평가받고 있습니다. 웹 작업에서 Opus 4.8과 유사한 품질에 약 2배 빠른 토큰 출력과 약 3배 저렴한 비용을 제공합니다.
**Anthropic, "적대적 디스틸레이션" 의혹 제기** — Anthropic은 Alibaba와 연계된 운영자들이 약 25,000개의 사기 계정과 2,880만 건의 Claude 교환을 사용하여 프론티어 역량을 Qwen급 시스템으로 디스틸레이션했다고 비난했습니다. 이는 "적대적 디스틸레이션" 논쟁을 국가 전략 수준으로 격상시킬 수 있는 중대한 사안입니다.

### 📊 모델 & 벤치마크
*   **GPT-5.5 Instant 업데이트:** OpenAI는 의도 이해, 제약 조건 처리, 대화 스타일이 개선된 GPT-5.5 Instant 개정판을 출시했습니다.
*   **GLM-5.2 벤치마크 성과:** GLM-5.2는 ARC-AGI-2에서 오픈소스 모델 중 가장 강력한 22.8%의 결과를 달성했으며, Code Arena: Frontend에서도 선두를 차지했습니다.
*   **OpenThoughts-Agent 벤치마크:** OpenThoughts-Agent 팀은 100K 예제 학습 세트를 구축하고 Qwen3-32B를 파인튜닝하여 7가지 에이전틱 벤치마크에서 평균 44.8%의 정확도를 달성했습니다.

### 🛠️ 제품 & 도구
*   **Anthropic의 Slack 네이티브 Claude 에이전트:** Claude가 Slack/팀 워크플로우에 통합되어 자체 자격 증명과 감사 가능한 행동을 제공하며, 에이전트 UX를 "도구"에서 "동료"로 전환합니다.
*   **SkyPilot Endpoints 출시:** SkyPilot은 자체 클러스터 전반에 걸쳐 통합 인퍼런스를 위한 Endpoints를 출시했습니다.
*   **Modal의 오픈소스 인퍼런스 설정:** Modal은 오픈소스 인퍼런스 설정이 레이턴시 면에서 독점 제공업체를 능가한다고 주장했습니다.
*   **Hugging Face의 Moon Bot:** Hugging Face는 셀프 호스팅, 맞춤형 도구, 감사 가능한 세션, 제로 락인(lock-in)을 강조하는 Slack 기반 코딩 에이전트 Moon Bot을 설명했습니다.
*   **Cursor x Notion 통합:** Cursor 작업이 이제 Notion에서 직접 Notion에서 위임될 수 있어, 에이전트 워크플로우가 기존 팀 소프트웨어로 확장되고 있음을 보여줍니다.

### 🔬 연구 & 논문
*   **Qwen-AgentWorld 연구:** Alibaba Qwen은 Qwen-AgentWorld를 통해 단일 모델 내에서 7가지 환경을 시뮬레이션하는 네이티브 언어 세계 모델을 제안하고, 시뮬레이터 구축 및 세계 모델링을 에이전트 사전 학습으로 활용하는 경로를 제시했습니다.
*   **OpenThoughts-Agent 연구:** @iScienceLuvr와 @RichardZ412는 100개 이상의 제어된 어블레이션(ablation)을 가진 에이전틱 모델을 위한 오픈 큐레이션/학습 파이프라인인 OpenThoughts-Agent를 강조했습니다.
*   **에이전트 메모리 연구:** @dair_ai는 에이전트 메모리가 최종 작업 성공으로만 판단되는 블랙박스가 아니라, 저장, 리트리벌, 업데이트, 통합, 라이프사이클 등 완전한 데이터 관리 레이어로 평가되어야 한다고 주장하는 논문을 지적했습니다.

### 💰 산업 동향
*   **Qualcomm의 Modular 인수:** Chris Lattner는 Qualcomm이 Modular를 인수한다고 발표했으며, Modular는 Mojo 오픈소스화가 순조롭게 진행 중이라고 밝혔습니다.
*   **Moonshot Kimi API, AWS Marketplace 입점:** Moonshot의 Kimi API가 AWS Marketplace에서 제공되어, 통합 청구 및 EDP 인출을 통해 기업 조달을 용이하게 합니다.
*   **Anthropic, AI 수출 통제 법적 도전:** Legion은 호스팅된 모델 접근이 가중치나 기술 데이터 수출과 동일하지 않다고 주장하며 트럼프 시대 AI 수출 통제에 대한 첫 번째 주요 법적 도전을 보고했습니다.
*   **Mirendil AI 출범:** Mirendil AI는 2억 달러의 시드 라운드와 과학을 위한 자체 가속 AI R&D에 대한 논문으로 출범했습니다.
*   **영국 국립 기초 AI 랩 설립:** 영국에서 BOLD Lab과 SOFAIR가 두 개의 새로운 국립 기초 AI 랩에 총 6천만 파운드의 시드 펀딩을 받았으며, UCL DARK는 BOLD에 합병되었습니다.
*   **Google DeepMind에서 Anthropic으로의 인재 이탈:** Bloomberg 보도에 따르면 Google DeepMind에서 Anthropic으로의 인재 이탈은 스타트업의 잠재력이 프론티어 인재를 계속해서 끌어들이고 있음을 강조합니다.

### ⚡ 인프라 & 하드웨어
*   **OpenAI, 맞춤형 AI 칩 'Jalapeño' 발표:** OpenAI는 Broadcom과 협력하여 LLM 인퍼런스를 위한 첫 번째 맞춤형 AI 칩인 Jalapeño를 발표했습니다. 이 칩은 TPU와 유사하며, 약 216GB HBM3E, ~7.1–7.4 TB/s 대역폭, ~10 PFLOPS FP4 성능을 가질 것으로 추정됩니다.
*   **NVIDIA NeMo AutoModel 학습 처리량 향상:** NVIDIA는 NeMo AutoModel이 Expert Parallelism, DeepEP, TransformerEngine 커널을 통해 MoE 모델의 학습 처리량을 3.4~3.7배 높인다고 밝혔습니다.
*   **Huawei의 SuperPOD 스케일 시스템 시연 가능성:** Huawei가 950 SuperPOD 스케일 시스템을 시연할 수 있다는 보고서가 나왔으며, 이는 상당한 규모의 대규모 국내 NPU 클러스터 생산을 의미합니다.
*   **Weaviate Engram GA 출시:** Weaviate의 Engram GA는 모든 것을 컨텍스트에 덤핑하는 대신, 메모리를 추출, 중복 제거, 조정 및 범위 지정하는 비동기 인프라로 정의됩니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
