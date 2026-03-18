# Claude Cowork Dispatch: Anthropic's Answer to OpenClaw - 요약

**원문 URL**: https://www.latent.space/p/ainews-claude-cowork-dispatch-anthropics
**번역일**: 2026-03-18 06:42
**발행일**: 2026-03-18

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 뉴스레터 요약 브리핑입니다.

### 🔥 주요 뉴스
**[Anthropic, Claude Cowork 출시]** — Anthropic이 OpenClaw에 대한 답변으로 Claude Cowork를 출시했습니다. 이 제품은 원격 제어 기능을 포함하며, 샌드박싱과 Electron 기술을 활용하여 에이전트 기능을 강화한 새로운 제품입니다. 이는 에이전트 기반 워크플로우를 위한 Anthropic의 중요한 진출을 의미합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/319f7604-36d5-44d5-b37e-61de653f6941_1208x1334.png)
**[OpenAI, GPT-5.4 Mini/Nano 모델 출시]** — OpenAI가 GPT-5.4 mini와 GPT-5.4 nano를 출시하며, 이를 자사의 가장 유능한 소형 모델로 포지셔닝했습니다. GPT-5.4 mini는 이전 mini보다 2배 이상 빠르며, 코딩, 컴퓨터 사용, 멀티모달 이해, 서브 에이전트 작업에 최적화되었고, API에서 400k 컨텍스트 윈도우를 제공합니다. 이 모델들은 SWE-Bench Pro 및 OSWorld-Verified 평가에서 더 큰 GPT-5.4 성능에 근접한다고 주장됩니다.
**[Mistral AI, Mistral Small 4 모델 공개]** — Mistral AI가 1,190억 개의 파라미터와 256k 컨텍스트 길이를 가진 하이브리드 멀티모달 AI 모델인 Mistral Small 4를 Apache 2.0 라이선스로 출시했습니다. 이 모델은 128개의 전문가 중 4개를 활성화하는 MoE 아키텍처를 사용하며, 텍스트 및 이미지 입력을 지원하고 추론 레이턴시를 40% 줄였습니다. 다국어 지원 및 네이티브 함수 호출을 통한 고급 에이전트 기능도 포함합니다.
**[Unsloth Studio, 로컬 LLM 학습 및 실행 웹 UI 출시]** — Unsloth가 Mac, Windows, Linux에서 500개 이상의 LLM을 로컬에서 학습하고 실행할 수 있는 오픈소스 웹 UI인 Unsloth Studio를 출시했습니다. 이 도구는 70% 적은 VRAM으로 2배 빠른 학습, GGUF 지원, 합성 데이터 툴링, 툴 호출 및 코드 실행 기능을 제공합니다. 이는 로컬 LLM 개발 워크플로우를 간소화하는 데 기여할 것으로 예상됩니다.

### 📊 모델 & 벤치마크
*   **OpenAI GPT-5.4 Mini/Nano 성능:** GPT-5.4 mini는 SWE-Bench Pro 및 OSWorld-Verified 평가에서 더 큰 GPT-5.4 성능에 근접하며, GPT-5.4 Codex 할당량의 30%만 사용한다고 주장합니다. 가격은 mini의 경우 입력 $0.75/M, 출력 $4.5/M입니다.
*   **Qwen3.5-9B 문서 AI 벤치마크:** Alibaba의 Qwen3.5-9B는 문서 AI 벤치마크에서 77.0점으로 9위를 기록했으며, "Key Information Extraction" 및 "Table Understanding"에서 강점을 보였으나, "OmniDoc" 및 "IDP Core"에서는 GPT-5.4에 뒤처졌습니다.
*   **NVIDIA Nemotron 3 Ultra Base 모델 공개:** NVIDIA가 약 500B 규모의 Nemotron 3 Ultra Base 모델을 공개하며, 5배의 효율성과 높은 추론 정확도를 가진 "Best Open Base Model"이라고 주장했습니다. 이 모델은 MMLU Pro, Code HumanEval 등 여러 벤치마크에서 우수한 성능을 보였습니다.

### 🛠️ 제품 & 도구
*   **LangChain LangSmith Sandboxes 출시:** LangChain이 보안 임시 코드 실행을 위한 LangSmith Sandboxes를 도입했습니다.
*   **LangChain Open SWE 오픈소스화:** LangChain이 Stripe, Ramp, Coinbase에서 사용된 내부 시스템을 본뜬 백그라운드 코딩 에이전트인 Open SWE를 오픈소스화했습니다.
*   **Hermes Agent v0.3.0 출시:** Hermes Agent가 v0.3.0을 출시하며, 플러그인 아키텍처, CDP를 통한 실시간 Chrome 제어, IDE 통합, 로컬 Whisper 기반 음성 모드, PII 비식별화 기능을 포함했습니다.
*   **Hugging Face hf CLI 확장 기능 출시:** Hugging Face가 사용 가능한 하드웨어에 최적화된 로컬 모델/양자화를 자동 감지하고 로컬 코딩 에이전트를 실행하는 hf CLI 확장 기능을 출시했습니다.
*   **Ollama 웹 검색/가져오기 플러그인 추가:** Ollama가 웹 검색/가져오기 플러그인과 OpenClaw 워크플로우를 위한 헤드리스 실행 지원을 추가했습니다.
*   **LangChain Deep Agents 출시:** LangChain이 Claude Code 스타일의 에이전틱 하네스를 MIT 라이선스로 제공하는 Deep Agents를 출시했습니다.
*   **H Company Holotron-12B 출시:** H Company가 컴퓨터 사용 에이전트를 위해 NVIDIA와 함께 구축된 오픈 멀티모달 모델인 Holotron-12B를 출시했습니다.
*   **Perplexity Comet Enterprise 출시:** Perplexity가 rollout 컨트롤 및 CrowdStrike Falcon 통합을 통해 자사의 AI 브라우저를 엔터프라이즈 팀에 제공하는 Comet Enterprise를 발표했습니다.
*   **LTX 2.3 LORA 모델 공개:** 게임 Dispatch의 440개 클립으로 학습된 LTX 2.3 LORA 모델이 공개되었으며, 여러 캐릭터와 스타일을 구현하여 게임 개발 사전 시각화에 잠재력을 보였습니다.
*   **OldNokia UltraReal LoRA 출시:** 2000년대 중반 휴대폰 카메라의 미학을 재현하도록 재학습된 Nokia 2MP Camera LoRA인 OldNokia UltraReal이 Civitai와 Hugging Face에서 다운로드 가능하게 출시되었습니다.

### 🔬 연구 & 논문
*   **Moonshot Attention Residuals 논문 발표:** Moonshot이 "수직 어텐션" 또는 계층 간 어텐션을 다루는 Attention Residuals 논문을 arXiv에 발표했습니다. 이 연구는 각 계층이 이전 계층 상태를 쿼리하여 어텐션을 수평 시퀀스 상호작용에서 계층 간 메모리로 확장하는 아이디어를 제시합니다.
*   **Mamba-3 아키텍처 출시:** @_albertgu와 @tri_dao가 인퍼런스 효율성에 중점을 둔 Mamba-3를 출시했습니다. 이는 선형/상태 공간 모델의 경쟁력을 높이는 하이브리드 아키텍처로, 1.5B에서 가장 빠른 prefill+decode 성능을 주장합니다.

### 💰 산업 동향
*   **Anthropic CEO, 초급 화이트칼라 직업 50% 소멸 예측:** Anthropic CEO는 AI 기술 발전으로 인해 향후 3년 내에 초급 화이트칼라 직업의 50%가 사라질 것이라고 예측했습니다.
*   **NVIDIA GTC, 인퍼런스 및 에이전트 중심 메시징:** NVIDIA GTC에서 Jensen Huang은 미래 컴퓨터를 "토큰을 제조하는" 시스템으로 규정하며, 인퍼런스가 다음 용량 파동을 주도할 것이라고 강조했습니다.
*   **LangChain, NVIDIA Nemotron Coalition 합류:** LangChain이 자사 프레임워크의 10억 다운로드 돌파와 함께 NVIDIA Nemotron Coalition에 합류했습니다.
*   **NVIDIA, 1조 달러 AI 인프라 기회 재확인:** Jensen Huang은 2027년까지 1조 달러 규모의 AI 인프라 기회가 스택의 일부만을 다룰 것이며, 산업이 인퍼런스 인프라 구축의 매우 초기 단계에 있음을 재확인했습니다.
*   **NBC News 설문조사, AI에 대한 부정적 인식:** NBC News 설문조사 결과, 미국 유권자의 46%가 AI에 대해 부정적인 견해를 가지고 있으며, 이는 AI의 광범위한 사용에도 불구하고 대중의 회의론이 높음을 보여줍니다.

### ⚡ 인프라 & 하드웨어
*   **NVIDIA DGX Station, OEM 유통업체 통해 가용:** 고성능 AI 및 딥러닝 워크스테이션인 NVIDIA DGX Station이 이제 OEM 유통업체를 통해 85-90k USD 가격으로 구매 가능합니다. 이 장비는 고급 냉각 및 "코히어런트 메모리" 기능을 특징으로 합니다.
*   **llama.cpp, Nemotron 3 Nano 4B 지원:** @ggerganov가 llama.cpp에서 Nemotron 3 Nano 4B 지원을 강조했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
