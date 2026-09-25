# The Future of Latent Space - 요약

**원문 URL**: https://www.latent.space/p/ainews-the-future-of-latent-space
**번역일**: 2026-09-25 06:22
**발행일**: 2026-09-25

---

### 🔥 주요 뉴스
**[Anthropic, OpenAI 등 SOTA LLM 대거 출시 및 가격 인하]** — Claude Opus 5.5, GPT-6 Astra/Sol/Luna, Gemini 3.8 Flash, Xiaomi MiMo-V2.6-Pro 등 최신 LLM들이 대거 공개되었으며, Anthropic과 OpenAI는 가격 인하를 발표했습니다. 특히 Claude Opus 5.5는 SimpleBench에서 88.4%로 선두를 차지하고 비전 평가에서 Anthropic 최고의 모델로 평가받았습니다.
**[TypeSafe AI, 100억 달러 이상 가치로 10억 달러 이상 조달]** — TypeSafe AI가 Jev 의사결정 모델의 성공에 힘입어 100억 달러 이상의 기업 가치로 10억 달러 이상의 자금을 조달 중인 것으로 알려졌습니다. Jev는 RL로 학습되어 확률 기반의 유형화된 의사결정을 반환하며, GPT-6보다 약 277배 저렴한 비용으로 높은 정확도를 유지합니다.
**[Google, 4개의 TPU를 우주 궤도에 배치]** — Google이 SpaceX Transporter-18에 탑재된 Planet 프로토타입 위성을 통해 4개의 TPU(Tensor Processing Unit)를 성공적으로 우주 궤도에 띄웠습니다. 이는 AI 컴퓨팅 인프라의 새로운 지평을 여는 중요한 하드웨어 발표입니다.
**[Claude 에이전트, CRISPR 유사 효소 시스템 발견]** — Anthropic의 Claude 에이전트가 게놈 마이닝 워크플로우를 통해 이전에 특성화되지 않은 박테리오파지 시스템인 array-associated reverse transcriptases (ART)를 식별했습니다. 이는 AI가 독창적인 과학적 가설 생성에 기여할 수 있음을 보여주는 중요한 연구 결과입니다.
**[Hugging Face Transformers, GGUF 네이티브 지원]** — Hugging Face Transformers 라이브러리가 이제 `AutoModelForCausalLM.from_pretrained`를 통해 GGUF/llama.cpp 양자화 체크포인트를 직접 로드하는 기능을 지원합니다. 이는 로컬 LLM 배포 및 학습 워크플로우에 큰 영향을 미칠 것으로 예상됩니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/6eb94ca5-a315-4307-9f69-724a59c08af1_2132x1120.png)

### 📊 모델 & 벤치마크
*   **Claude Opus 5.5**가 SimpleBench에서 88.4%로 선두를 차지했으며, 비전 평가에서 Anthropic의 최고 비전 모델로 평가받았습니다. Terminal-Bench-Science에서 GPT-6 Astra와 함께 Fable 5.1을 약 20점 차이로 앞서고, Fable 5.1보다 약 60% 낮은 비용으로 제공됩니다.
*   **GPT-6 Astra**는 NetHack을 3번째 시도에서 이겼으며, **GPT-6 Luna [Max]**는 Code Arena WebDev에서 #24위를 기록하며 GPT-5.6 Luna보다 74점 높은 1593점을 달성했습니다.
*   **Gemini 3.8 Flash**는 1M 컨텍스트에서 291 tok/s의 속도로 AA Intelligence Index에서 41점을 기록했으며, Cline에서 무료로 제공됩니다.
*   **Xiaomi MiMo-V2.6-Pro**가 MIT 라이선스 하에 1M 컨텍스트를 가진 옴니모달 모델로 출시되었으며, AA 인덱스에서 46점을 기록하여 GPT-5.6 Sol의 47점 바로 뒤를 이었습니다. Xiaomi는 RL 코드와 학습 환경도 공개했습니다.
*   **Grok 4.7**이 Agent Arena에서 작업당 $1.14의 비용으로 #16위를 기록하며 데뷔했습니다.
*   **TypeSafe의 Jev**는 Calibrated Decisions를 위해 RL로 학습되었으며, 152ms의 중간 레이턴시와 1,000건 판단당 $0.044의 비용으로 GPT-6보다 약 277배 저렴하게 높은 정확도를 유지합니다.
*   **CLM**은 Jev의 오픈 웨이트 대안으로, Qwen3-8B를 위한 새로운 프로젝션 헤드로 구현되어 에이전트 스타일 벤치마크에서 4배–13배 낮은 레이턴시를 제공하며 Terminal-Bench 2.1 87.6%, DeepSWE 81.6%를 기록했습니다.
*   **Fastino의 GLiNER2.5-Decide**는 CPU에서 167ms, GPU에서 38–47ms로 스팬, 관계 및 제약 조건에 일치하는 구조화된 의사결정을 추가합니다.
*   **UkisAI Swift 제품군** (Swift1.5 27B, Swift Flash Next, Swift Bonsai 2)이 Qwen 기반 추론 모델로 출시되었으며, 과도한 사고 관련 토큰을 줄이고 GSPO RL 및 온-정책 디스틸레이션으로 정확도를 회복하도록 학습되었습니다.
*   **MiMo-V3**는 HySparse2를 핵심으로 하는 새로운 아키텍처를 채택하여 낮은 프리필 FLOPs, 감소된 KV-캐시 공간, 그리고 KV Bridging, KV Reuse, 토큰 수준 선택, 공유 KV-캐시 설계와 같은 메커니즘을 통한 더 나은 장문 컨텍스트 리트리벌을 제공합니다.
*   **Opus 5.5와 Astra**는 전적으로 코드를 통해 비디오와 애니메이션을 제작하는 능력을 시연했습니다.

### 🛠️ 제품 & 도구
*   **Claude Code 플랜**($200)이 이제 Codex를 능가하는 성능을 제공합니다.
*   **turbopuffer**가 네이티브 리랭킹에 Jev를 포함했습니다.
*   **LangChain Interrupt**에서 Managed Deep Agents 0.8을 출시하여 사용자 및 에이전트 메모리, HTTP 채널, 샌드박스 파일 API, 프록시 인증 샌드박스, 병렬 웹 검색 기능을 추가했습니다.
*   **LangSmith Fine-Tuning과 smithtune CLI**가 Baseten Loops 및 Fireworks에서 트레이스를 학습 후 데이터셋으로 전환하는 기능을 제공합니다.
*   **LangChain Engine v2**는 레드팀(red-teaming) 기능과 검증된 수정 사항을 추가했습니다.
*   **Perplexity Photon**은 Rust 기반의 리트리벌 및 랭킹 엔진으로 출시되었으며, 내부 p99 레이턴시를 약 800ms에서 65ms로 감소시키고, 고속 검색 API는 작업당 68% 낮은 비용으로 160ms p50 / 230ms p95로 실행됩니다.
*   **Perplexity의 로컬 에이전트**가 이제 AMD Ryzen AI Max에서 사용 가능합니다.
*   **Weaviate 1.39**는 쿼리 시점에 MMR 다양성을 GA(General Availability)로 만들었습니다.
*   **Quail**은 쿼리와 LLM 인퍼런스를 공동으로 계획하는 오픈소스 AI-SQL 엔진으로, 하나의 H100에서 분당 10억 개 이상의 입력 토큰을 처리합니다.
*   **Hugging Face Transformers**가 `AutoModelForCausalLM.from_pretrained(..., gguf_file=...)`를 통해 GGUF / llama.cpp 양자화 체크포인트를 직접 로드하는 것을 지원합니다.

### 🔬 연구 & 논문
*   **Anthropic의 Claude 에이전트**가 게놈 마이닝 워크플로우를 통해 이전에 특성화되지 않은 박테리오파지 시스템인 array-associated reverse transcriptases (ART)를 식별했습니다.
*   **Harness-Zero**는 최적화된 에이전트 하네스를 모델로 디스틸레이션하는 방법으로, 배포 시 하네스 없이 매크로 작업 성공률을 23.3%에서 44.3%로 상승시켰습니다.
*   **DeepMind의 XYEval** 연구는 자신감 있고 오해의 소지가 있는 사용자 힌트 하나를 주입하여 에이전트 점수를 상대적으로 최대 46.7%까지 낮출 수 있음을 보여주었습니다.
*   **NeurIPS 논문**은 하나의 MLP 뉴런을 억제하는 것이 1.7B에서 70B에 이르는 7개 모델에서 안전성 거부를 우회함을 보여주었습니다.
*   **Meta**는 컨텍스트 로트(context rot)에 대응하기 위해 행동 에이전트와 전용 메모리 에이전트를 짝지어 Sonnet 4.5의 성능을 37.6%에서 45.9%로 향상시켰습니다.
*   **SmolDataEnvs**는 단일 GPU에서 실행 가능한, 100억 개 미만 모델을 목표로 하는 5천 개 이상의 검증 가능한 데이터 과학 RL 환경을 출시했습니다.
*   **C5R**은 12주 만에 AI 운영 연구실과 SciUniverse 벤치마크를 구축했습니다.
*   **Odyssey의 Agora-2**는 하나의 공유 환경에서 최대 20명의 인간과 에이전트를 실시간으로 시뮬레이션하는 다중 에이전트 세계 모델입니다.
*   **Meta의 Muse Realtime Avatar**는 약 870ms의 응답 레이턴시를 목표로 합니다.
*   **Google Research**는 장편의 시간적으로 일관된 비디오를 위한 다중 에이전트 프레임워크를 발표했습니다.

### 💰 산업 동향
*   **TypeSafe AI**가 100억 달러 이상의 기업 가치로 10억 달러 이상의 자금을 조달 중인 것으로 알려졌습니다.
*   **Sakana AI**는 Jürgen Schmidhuber를 세계 모델 및 자체 개선 시스템을 목표로 하는 RSI Lab의 최고 과학 고문으로 임명했습니다.

### ⚡ 인프라 & 하드웨어
*   **Liquid AI DSpark**는 LFM2.5-VL-3B용 추측 디코딩 드래프터로, M5 Max에서 MLX를 사용하여 최대 3.13배의 디코딩 속도 향상을 제공합니다.
*   **AMD의 GLM-5.3**은 vLLM과 TileRT를 사용하여 8개의 MI355X에서 469 tok/s의 단일 사용자 디코드를 달성했습니다.
*   **Qualcomm**은 엣지 메모리 장벽을 위해 3D DRAM 통합을 사용한 HBC 대 HBM에 대해 논의했습니다.
*   **Google**은 SpaceX Transporter-18에 탑재된 Planet 프로토타입 위성에서 4개의 TPU를 궤도에 띄웠습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
