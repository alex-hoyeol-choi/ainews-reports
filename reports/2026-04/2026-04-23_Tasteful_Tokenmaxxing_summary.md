# Tasteful Tokenmaxxing - 요약

**원문 URL**: https://www.latent.space/p/ainews-tasteful-tokenmaxxing
**번역일**: 2026-04-23 06:18
**발행일**: 2026-04-23

---

### 🔥 주요 뉴스
*   **Google, 8세대 TPU 및 Gemini 엔터프라이즈 에이전트 플랫폼 공개** — Google은 학습용 TPU 8t와 인퍼런스용 TPU 8i로 구성된 8세대 TPU를 발표하며, pod당 최대 3배의 컴퓨팅 성능과 백만 개의 TPU로 확장 가능한 인프라를 제시했습니다. 또한, 대규모 에이전트 구축 및 관리를 위한 Gemini Enterprise Agent Platform과 Workspace Intelligence 등 엔터프라이즈 AI 솔루션을 대거 출시했습니다.
*   **Alibaba Qwen3.6-27B, 강력한 오픈소스 코딩 모델로 출시** — Alibaba는 Apache 2.0 라이선스의 dense 모델 Qwen3.6-27B를 공개했습니다. 이 모델은 SWE-bench Verified 77.2점 등 주요 코딩 평가에서 더 큰 Qwen3.5-397B-A17B를 능가하며, 이미지 및 비디오에 대한 네이티브 시각-언어 추론을 지원합니다.
*   **OpenAI, PII 감지 및 마스킹을 위한 경량 프라이버시 모델 오픈소스화** — OpenAI는 PII(개인 식별 정보) 감지 및 수정을 위한 경량 Apache 2.0 오픈 모델인 Privacy Filter를 조용히 출시했습니다. 이 1.5B/50M MoE 토큰 분류 모델은 128k 컨텍스트 윈도우를 통해 대규모 데이터셋의 저비용 전처리를 가능하게 합니다.
*   **Xiaomi, 에이전트 기능 강화한 MiMo-V2.5 시리즈 발표** — Xiaomi는 소프트웨어 엔지니어링 및 장기 에이전트 분야에 특화된 MiMo-V2.5-Pro와 네이티브 옴니모달리티 및 1M 토큰 컨텍스트 윈도우를 갖춘 MiMo-V2.5를 발표했습니다. MiMo-V2.5-Pro는 SWE-bench Pro 57.2점 등 높은 벤치마크 성능과 1,000개 이상의 자율 도구 호출을 주장합니다.

### 📊 모델 & 벤치마크
*   **Alibaba Qwen3.6-27B 출시:** Apache 2.0 라이선스의 27B dense 모델로, SWE-bench Verified 77.2점 등 주요 코딩 평가에서 Qwen3.5-397B-A17B를 능가하며 이미지 및 비디오에 대한 네이티브 시각-언어 추론을 지원합니다. vLLM, Unsloth, ggml, Ollama 등 주요 생태계에서 즉시 지원을 시작했습니다.
*   **OpenAI Privacy Filter 오픈소스화:** PII 감지 및 마스킹을 위한 경량 Apache 2.0 오픈 모델로, 1.5B 전체 / 50M 활성 MoE 토큰 분류 모델이며 128k 컨텍스트 윈도우를 통해 대규모 코퍼스 및 로그의 저렴한 수정을 목표로 합니다.
*   **Xiaomi MiMo-V2.5 시리즈 발표:** MiMo-V2.5-Pro는 SWE-bench Pro 57.2점 등 소프트웨어 엔지니어링 및 장기 에이전트 분야에서 1,000개 이상의 자율 도구 호출을 주장하며, MiMo-V2.5는 네이티브 옴니모달리티와 1M 토큰 컨텍스트 윈도우를 추가합니다.

### 🛠️ 제품 & 도구
*   **Google Gemini Enterprise Agent Platform 출시:** Vertex AI가 대규모 에이전트 구축, 관리, 최적화를 위한 플랫폼으로 진화하며 Agent Studio, 200개 이상의 모델 접근, Gemini 3.1 Pro 등 Google 스택을 지원합니다.
*   **Google Workspace Intelligence GA:** 문서, 시트, 회의, 메일 위에 구축된 시맨틱 레이어로, Gemini Enterprise inbox/canvas/재사용 가능한 스킬, Agentic Data Cloud, Wiz 통합 보안 에이전트 등과 함께 출시되었습니다.
*   **Google Gemini Embedding 2 GA:** 텍스트, 이미지, 비디오, 오디오, 문서 전반에 걸친 통합 임베딩 모델로, Google Cloud Next에서 발표되었습니다.
*   **OpenAI ChatGPT 워크스페이스 에이전트 도입:** 문서, 이메일, 채팅, 코드 및 외부 시스템(Slack 기반 워크플로우 포함) 전반에서 작동하는 팀용 Codex 기반 에이전트를 출시했습니다.
*   **VS Code/Copilot BYOK/모델 지원:** Anthropic, Gemini, OpenAI, OpenRouter, Azure, Ollama 및 로컬 백엔드 등 다양한 제공업체를 지원하는 BYOK(bring-your-own-key)/모델 지원을 모든 플랜과 비즈니스/엔터프라이즈에 걸쳐 출시했습니다.
*   **Cursor Slack 호출 기능 추가:** 작업 시작 및 스트리밍 업데이트를 위해 Slack 호출 기능을 도입했습니다.

### 🔬 연구 & 논문
*   **Perplexity의 사후 학습 파이프라인 공개:** 검색 증강 SFT + RL 파이프라인을 통해 사실성, 인용 품질, 지시 따르기, 효율성을 개선하며, Qwen 기반 시스템이 GPT 계열 모델과 동등하거나 능가하는 사실성을 더 낮은 비용으로 달성할 수 있다고 밝혔습니다.
*   **Neural Garbage Collection 연구:** 프록시 목표 없이 추론과 KV-cache 유지/제거를 공동으로 학습하는 RL을 사용하는 새로운 방법을 소개했습니다.
*   **코딩 모델의 "최소 편집" 문제 연구:** 코딩 모델의 과도한 코드 재작성(Over-Editing) 문제를 다루며, 패치 거리와 인지 복잡성으로 과도한 편집을 측정하는 벤치마크를 제시하고 RL이 최소 편집 스타일 학습에 더 우수함을 발견했습니다.
*   **에이전트 데이터 프로토콜(ADP) 표준화 추진:** 오픈 에이전트 학습을 위한 데이터 기반으로서 오픈 트레이스의 중요성이 강조되었으며, ADP 표준화 노력이 진행 중입니다.

### ⚡ 인프라 & 하드웨어
*   **Google 8세대 TPU 발표:** 학습용 TPU 8t와 인퍼런스용 TPU 8i로 분할된 8세대 TPU를 소개했으며, 8t는 Ironwood 대비 pod당 거의 3배의 컴퓨팅 성능을 제공하고 8i는 낮은 레이턴시 인퍼런스 및 높은 처리량의 멀티 에이전트 워크로드를 지원합니다.
*   **Cohere의 W4A8 인퍼런스 vLLM 통합:** 프로덕션 W4A8 인퍼런스를 vLLM에 통합하여 Hopper에서 W4A16 대비 TTFT를 최대 58%, TPOT를 45% 빠르게 만들었으며, 채널당 FP8 스케일 양자화 및 CUTLASS LUT 역양자화를 포함합니다.
*   **SonicMoE의 Blackwell 처리량 증가:** Blackwell에서 SonicMoE의 fwd/bwd TFLOPS가 DeepGEMM 기준선보다 54%/35% 더 높았으며, 동일한 활성 파라미터에 대해 dense 모델과 동등한 활성화 메모리를 유지했습니다.
*   **Baseten의 RadixMLP 도입:** 재랭킹에서 공유 접두사 제거를 위한 RadixMLP를 도입하여 1.4~1.6배의 현실적인 속도 향상을 달성했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
