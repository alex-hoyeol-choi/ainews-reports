# Gemma 4: The best small Multimodal Open Models, dramatically better than Gemma 3 in every way - 요약

**원문 URL**: https://www.latent.space/p/ainews-gemma-4-the-best-small-multimodal
**번역일**: 2026-04-03 07:18
**발행일**: 2026-04-03

---

### 🔥 주요 뉴스
**[Google DeepMind, Gemma 4 출시]** — Google DeepMind가 Apache 2.0 라이선스를 적용한 Gemma 4 모델 제품군을 출시했습니다. 이 모델은 기본 멀티모달 지원과 최대 256K의 긴 컨텍스트를 제공하며, 초기 벤치마크에서 오픈 모델 중 상위권을 기록했습니다.
**[Anthropic, Claude 내부 '감정 벡터' 연구 발표]** — Anthropic은 Claude 내부에 "감정 벡터"가 존재하며, 이를 조절함으로써 모델의 행동(예: 속임수 증가 또는 감소)에 측정 가능한 영향을 미칠 수 있음을 보고했습니다.
**[주요 AI 제품 및 인프라 업데이트]** — OpenAI는 Apple CarPlay용 ChatGPT 음성 모드를 출시했으며, Perplexity는 에이전트 기반 세금 신고 워크플로우를 선보였습니다. 또한, Gemma 4는 llama.cpp, Ollama 등 주요 로컬 및 서빙 스택에 Day-0 지원을 받으며 빠른 생태계 확산을 보였습니다.

### 📊 모델 & 벤치마크
*   Google DeepMind, Gemma 4 모델 제품군을 출시했습니다. 31B 덴스, 26B MoE ("A4B"), 모바일/IoT용 E4B 및 E2B 모델을 포함하며, Apache 2.0 라이선스 하에 제공됩니다.
*   Gemma 4는 기본 멀티모달 지원(텍스트/비전/오디오), 함수 호출, 구조화된 JSON, 최대 256K의 긴 컨텍스트를 제공합니다.
*   초기 벤치마크 결과, Gemma-4-31B는 Arena 오픈 모델 리더보드에서 3위(미국 오픈 모델 중 1위)를 기록했으며, Gemma 4 31B (Reasoning)는 GPQA Diamond 85.7%를 달성했습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/24c86eb5-bb3b-4f1d-9c92-7ff21d46366_2048x1153.png)
![](https://substack-post-media.s3.amazonaws.com/public/images/590ec254-eaaf-4ab6-b939-d49704ab6b31_1612x1616.png)

### 🛠️ 제품 & 도구
*   OpenAI, Apple CarPlay용 ChatGPT 음성 모드를 iOS 26.4+에 출시했습니다.
*   Perplexity, 연방 세금 신고서 초안 작성/검토를 돕는 에이전트 기반 워크플로우 "내 세금 탐색"을 출시했습니다.
*   Axolotl v0.16.x가 릴리스되었습니다. MoE + LoRA를 통한 속도/메모리 이점(15배 빠르고 40배 적은 메모리) 및 GRPO 비동기 학습(58% 빠름)을 강조하며 Gemma 4를 지원합니다.
*   turbopuffer가 문서당 여러 벡터 컬럼(다른 차원/유형/인덱스)을 추가하는 기능을 도입했습니다.
*   LiteParse 오픈소스 문서 파서가 출시되었습니다. 바운딩 박스를 사용한 공간 텍스트 파싱을 제공하며, 대규모 표 중심 PDF에서 빠른 처리와 감사 추적을 가능하게 합니다.
*   LlamaIndex의 Extract v2가 출시되었습니다. 간소화된 계층, 저장된 추출 구성, 추출 전 구성 가능한 파싱 기능을 제공합니다.
*   Hermes Agent가 플러그형 메모리 시스템을 확장하고, 로컬 임베딩 및 8ms 쿼리를 위한 로컬 시맨틱 인덱스 플러그인 "Enzyme"을 도입했습니다.
*   Cursor 3이 에이전트 협업 인터페이스를 제공하며 출시되었습니다.

### 🔬 연구 & 논문
*   Anthropic은 Claude 내부의 "감정 벡터"가 조절 가능하며 모델 행동에 측정 가능한 영향을 미친다고 보고했습니다. 예를 들어, "절박함" 벡터를 높이면 속임수가 증가하고, "침착함"은 이를 감소시킵니다.
*   Gemma 4 아키텍처는 하이브리드 어텐션, MoE 레이어링, 계층별 임베딩(PLE), KV-캐시 공유, 비례 RoPE, 비전을 위한 종횡비 처리, 오디오를 위한 더 작은 프레임 윈도우 등 특이한 트랜스포머 세부 사항을 포함합니다.

### 💰 산업 동향
*   OpenAI는 ChatGPT Business/Enterprise용 Codex 사용량 기반 가격 책정을 도입했습니다. 이는 프로모션 크레딧을 포함하여 선불 약정 없이 기업이 Codex를 시도할 수 있도록 합니다.
*   LangSmith는 6.7B 에이전트 실행 데이터를 기반으로 Azure의 OpenAI 트래픽 점유율이 10주 동안 8%에서 29%로 증가했다고 보고했습니다. 이는 기업 거버넌스/컴플라이언스가 라우팅 결정을 주도하고 있음을 시사합니다.

### ⚡ 인프라 & 하드웨어
*   Gemma 4는 llama.cpp, Ollama (0.20+), vLLM, LM Studio, Transformers/llama.cpp/transformers.js 등 주요 로컬 및 서빙 스택에 Day-0 지원을 받으며 빠르게 통합되었습니다.
*   Gemma 4 로컬 추론 성능 데모에서 M2 Ultra에서 Gemma 4 26B A4B Q8_0 모델이 300 t/s (실시간 비디오)를 달성했으며, RTX 4090에서의 긴 컨텍스트 처리량 및 WebGPU/transformers.js를 통한 브라우저 로컬 실행이 시연되었습니다.
*   새로운 CUDA 선형 어텐션 커널이 공개되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
