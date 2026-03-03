# Truth in the time of Artifice - 요약

**원문 URL**: https://www.latent.space/p/ainews-truth-in-the-time-of-artifice
**번역일**: 2026-03-03 13:29
**발행일**: 2026-03-03

---

### 🔥 주요 뉴스
**[Qwen 3.5 "스몰" 오픈 모델 출시]** — Alibaba가 Qwen3.5-0.8B/2B/4B/9B 시리즈를 출시했습니다. 이 모델들은 네이티브 멀티모달 기능과 스케일드 RL을 특징으로 하며, 262K의 긴 컨텍스트(1M까지 확장 가능)를 지원하여 엣지 및 경량 에이전트 배포에 최적화되었습니다.
**[Apple Neural Engine(ANE) 학습 활용 역설계]** — 한 연구원이 문서화되지 않은 API를 사용하여 ANE에서 트랜스포머 학습 루프를 구축하여 CoreML을 우회하는 데 성공했습니다. 이는 M4 ANE의 6.6 TFLOPS/W 효율성과 19 TFLOPS FP16의 실제 처리량을 주장하며 온디바이스 학습 및 파인튜닝의 가능성을 열어주는 중요한 발전입니다.
**[미국 국방부(DoD)와 OpenAI 계약 수정안 공개]** — Sam Altman이 DoD와의 계약 수정안 언어를 게시했습니다. 이 수정안은 미국인에 대한 "의도적인" 국내 감시를 명시적으로 금지하지만, 정보 기관은 후속 수정 없이는 제외되며 "우발적 수집" 허점 가능성에 대한 논란이 있습니다.
**[ByteDance의 CUDA Agent 연구 발표]** — 프로파일링 기반 보상과 에이전틱 RL을 사용하여 고성능 CUDA 커널을 생성하는 CUDA Agent가 공개되었습니다. 이 기술은 KernelBench에서 SOTA를 달성하고 torch.compile 대비 상당한 성능 향상을 보였습니다.

### 📊 모델 & 벤치마크
*   **Alibaba, Qwen 3.5 "스몰" 오픈 모델 시리즈 출시:** Qwen3.5-0.8B, 2B, 4B, 9B (Base + Instruct) 모델이 출시되었습니다. 이 모델들은 네이티브 멀티모달 및 스케일드 RL을 특징으로 하며, 262K의 네이티브 컨텍스트(1M까지 확장 가능)를 지원하고 MMLU-Pro 82.5, MMMU 78.4, CountBench 97.2 등의 경쟁력 있는 벤치마크 점수를 기록했습니다.
*   **Codex 5.3, WeirdML 벤치마크에서 성능 향상:** Codex 5.3이 WeirdML 벤치마크에서 79.3%의 성능을 달성하여 Opus 4.6의 77.9%를 앞섰다는 보고가 있습니다.
*   **BullshitBench v2 업데이트:** 코딩, 의료, 법률, 금융, 물리학 분야의 100개 신규 질문을 추가하고 70개 이상의 모델 변형을 테스트하는 BullshitBench v2가 공개되었습니다. 이 벤치마크에서 Anthropic 모델이 우세하며, OpenAI 및 Google 모델은 개선되지 않고 있다고 주장합니다.

### 🛠️ 제품 & 도구
*   **Qwen 3.5 모델, Ollama 및 LM Studio 지원:** Qwen3.5 모델이 Ollama에서 `ollama run qwen3.5:9b|4b|2b|0.8b` 명령어로 사용 가능하며, 툴 호출, 사고, 멀티모달 기능이 포함되었습니다. LM Studio에서는 Qwen3.5-9B가 약 7GB의 로컬 풋프린트로 실행 가능하다고 홍보됩니다.
*   **iPhone 온디바이스 Qwen3.5 2B 6비트 데모:** MLX를 사용하여 iPhone 17 Pro에서 Qwen3.5 2B 6비트 모델이 실행되는 온디바이스 데모가 시연되었습니다.
*   **Docker Desktop, MLX 모델 지원 추가:** Docker Desktop의 "Model Runner"가 OpenAI 호환 API 워크플로우를 통해 MLX 모델을 실행할 수 있도록 지원을 추가하여 Apple Silicon 개발 환경을 강화했습니다.
*   **AMD, rocprof-trace-decoder 오픈소스화:** AMD가 SQTT trace defs를 포함하는 rocprof-trace-decoder를 오픈소스화하여 더 심층적인 명령어 수준의 타이밍 트레이스를 가능하게 했습니다.
*   **GitNexus 출시: 브라우저 기반 리포 지식 그래프:** 리포지토리를 대화형 D3 그래프로 파싱하고, 내장된 KuzuDB에 관계를 저장하여 Cypher를 통한 "그래프 RAG"를 제공하는 GitNexus가 출시되었습니다. 이 도구는 Web Workers를 사용하여 브라우저에서 작동하며 MIT 라이선스를 따릅니다.
*   **Stripe, LLM을 위한 토큰 기반 빌링 출시:** Stripe가 LLM 프록시를 통해 모델 호출을 라우팅하고 사용량을 자동으로 기록하는 "토큰 기반 빌링" 서비스를 출시했습니다.
*   **llama.cpp, 공식 Debian/Ubuntu 패키지화 추진:** llama.cpp의 공식 Debian/Ubuntu 패키지화를 위한 피드백 요청이 진행 중입니다.
*   **Weaviate, 에이전트 스킬 기반 통합 패턴 공개:** Weaviate가 일반적인 에이전트 툴을 위한 스킬 기반 통합 패턴을 게시했습니다.

### 🔬 연구 & 논문
*   **Meta, "Effective Theory of Wide and Deep Transformers" 논문 재배포:** 트랜스포머의 순방향/역방향 신호 전파, 너비 스케일링 규칙, 하이퍼파라미터 스케일링, NTK 분석, 옵티마이저 동작에 대한 60페이지 이상의 심층 분석 논문이 재배포되었으며, 비전 및 언어 트랜스포머에서 검증되었습니다.
*   **MuP / Muon 안정성 코너 케이스 연구:** 임베딩, LM 헤드, RMSNorm 레이어의 안정성 지표와 임베딩 및 LM 헤드가 Muon과 "잘 맞지 않는" 이유에 대한 연구가 논의되었습니다.
*   **ByteDance, CUDA Agent 연구 발표:** 프로파일링 기반 보상과 에이전틱 RL을 사용하여 고성능 CUDA 커널을 생성하는 CUDA Agent가 공개되었습니다. 이 기술은 KernelBench에서 SOTA를 달성하고 torch.compile 대비 상당한 성능 향상을 보였습니다.
*   **AGENTS.md / SKILL.md의 에이전트 효율성 연구:** 10개 리포지토리/124개 PR에 걸친 Codex 연구 보고서에 따르면, AGENTS.md가 중앙값 런타임을 약 28.6%, 토큰을 약 16.6% 감소시키는 데 기여했습니다.

### 💰 산업 동향
*   **미국 국방부(DoD)와 OpenAI 계약 수정안 공개 및 논란:** Sam Altman이 DoD와의 계약 수정안 언어를 게시했습니다. 이 수정안은 미국인에 대한 "의도적인" 국내 감시를 명시적으로 금지하지만, 정보 기관은 후속 수정 없이는 제외되며, "의도적/고의적"이라는 표현이 "우발적 수집" 허점을 보존할 수 있다는 법률 전문가들의 우려가 제기되었습니다.
*   **Anthropic, Claude Gov의 안전장치 주장:** Anthropic 관련 직원들은 Claude Gov 모델에 추가 학습, 안전장치 및 분류기 스택이 포함되어 있어 제약 없는 국가 안보 모델을 제공했다는 주장을 반박했습니다.

### ⚡ 인프라 & 하드웨어
*   **Apple Neural Engine(ANE) 학습 활용 역설계:** 한 연구원이 문서화되지 않은 API를 사용하여 ANE에 트랜스포머 학습 루프를 구축하여 CoreML을 우회하는 데 성공했습니다. M4 ANE는 6.6 TFLOPS/W의 효율성을, 실제 처리량은 19 TFLOPS FP16을 주장합니다.
*   **인퍼런스 하드웨어의 분화: Taalas HC ASIC 공개:** GPU와 Taalas HC(ASIC)의 인퍼런스 하드웨어 차이점이 설명되었습니다. HC1은 마스크 ROM에 가중치를 저장하는 "하드웨어로서의 모델"로, 사용자당 16-17k 토큰/초를 주장하며 "하나의 칩 = 하나의 모델"이라는 트레이드오프가 있습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
