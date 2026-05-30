# Founders and Forward Deployed Engineers - 요약

**원문 URL**: https://www.latent.space/p/ainews-founders-and-forward-deployed
**번역일**: 2026-05-30 06:18
**발행일**: 2026-05-30

---

### 🔥 주요 뉴스
**[Anthropic Claude Opus 4.8 출시]** — Anthropic이 Claude Opus 4.8을 출시했습니다. 독립 벤치마크에서는 점진적 개선을 보였으나, 실제 사용 환경에서는 코딩 협업 및 API 플랫폼 변경을 통해 사용자 경험을 크게 향상시킨 '삶의 질 개선' 릴리스로 평가됩니다.
**[StepFun 3.7 Flash MoE 모델 공개]** — StepFun이 총 196B 파라미터(활성 11B)의 멀티모달 MoE 모델 Step 3.7 Flash를 공개했습니다. SWE-Bench Pro 56.26%, DeepSearchQA F1 92.82% 등 강력한 벤치마크 성능을 보이며, llama.cpp 데이-0 지원과 함께 로컬에서 약 128GB RAM으로 실행 가능합니다.
**[Google 및 OpenAI, 에이전트 스택 확장]** — Google은 Gemini API의 관리형 에이전트, Gemini Spark, Gemini Omni, Google Flow Agent를 통해 관리형 에이전트 스택을 확장했습니다. OpenAI는 ChatGPT 모바일 앱을 통해 Windows 컴퓨터 사용 및 모바일 원격 제어를 포함한 Codex 기능을 추가하며 에이전트 운영 표면을 넓혔습니다.
**[다중 턴 RL 학습 루프의 핵심 버그 발견 및 수정 제안]** — Hugging Face는 도구 사용 다중 턴 RL 학습 루프에서 모델 출력을 재토큰화할 때 발생하는 핵심 버그를 지적했습니다. 이는 모델이 실제로 샘플링하지 않은 시퀀스에 그래디언트가 적용되는 문제로, 엄격한 "토큰 인, 토큰 아웃" 규칙을 수정 사항으로 제안했습니다.
**[오픈 웨이트 모델의 성장 및 인프라 강화]** — AI 팀 3곳 중 1곳이 오픈 웨이트 모델을 실행하며, EpochAIResearch는 오픈 웨이트 모델이 프론티어 모델보다 약 4개월 뒤처진다고 추정했습니다. ggerganov는 llama.cpp의 로컬 배포를 용이하게 하는 llama.app을 출시했으며, NVIDIA는 4개의 오픈 모델 제품군을 Linux Foundation OpenMDW-1.1로 이전하여 라이선스 파편화를 줄였습니다.

### 📊 모델 & 벤치마크
*   Anthropic이 Claude Opus 4.8을 출시했습니다. 독립 벤치마크에서는 점진적 개선을 보였으나, 실제 사용 환경에서 코딩 협업 및 API 플랫폼 변경을 통해 사용자 경험을 크게 향상시켰습니다.
*   StepFun이 총 196B 파라미터(활성 11B, 1.8B ViT 내장)의 멀티모달 MoE 모델 Step 3.7 Flash를 공개했습니다. SWE-Bench Pro 56.26%, DeepSearchQA F1 92.82% 등 강력한 벤치마크 성능을 기록했습니다.
*   EpochAIResearch는 오픈 웨이트 모델이 이제 프론티어 독점 모델보다 약 4개월 뒤처진다고 추정했습니다.
*   GPIC(Generative Permissive Image Corpus)는 시각적 생성을 위한 1억 쌍의 허용 이미지 코퍼스와 100만 쌍의 벤치마크를 소개하며 연구 및 상업적 유용성을 강조했습니다.

### 🛠️ 제품 & 도구
*   Anthropic은 프롬프트 캐시를 깨뜨리지 않는 대화 중간 시스템 지침과 권위 있는 대화 중간 시스템 역할 업데이트를 출시했습니다.
*   LangChain의 Deep Agents v0.6은 하네스 프로필을 일급 객체로 만들어 Qwen/Kimi/DeepSeek에서 프론티어 API보다 20배 이상 낮은 비용으로 강력한 성능을 달성했습니다.
*   ggerganov가 llama.cpp의 공식 웹사이트, 통합 설치 프로그램, 쉬운 로컬 배포 및 타사 에이전트 통합을 목표로 하는 llama.app을 출시했습니다.
*   Ollama는 Ollama를 통해 로컬 우선 개인 AI인 OpenJarvis를 발표했습니다.
*   DSPy는 다가오는 4.0 버전에 앞서 프로그래밍 가능한 AI 시스템 온보딩에 중점을 둔 재설계된 문서/첫 페이지를 출시했습니다.
*   Google은 Gemini API의 관리형 에이전트(코드 실행, 웹 액세스, 파일 I/O를 갖춘 샌드박스형 Linux 환경 프로비저닝)를 선보였습니다.
*   Google은 미국 AI Ultra 구독자에게 24/7 개인 에이전트인 Gemini Spark를 출시했습니다.
*   Google은 Gemini Omni 멀티모달 생성/편집 데모를 계속 추진했으며, 비디오/영화 제작 워크플로우를 위한 Google Flow Agent를 발표했습니다.
*   OpenAI는 ChatGPT 모바일 앱에서 Windows 컴퓨터 사용 및 원격 제어를 포함한 Codex 기능을 추가했습니다.
*   OpenAI는 아첨, 사실성 및 다국어 성능 개선을 위해 gpt-5.5 instant를 업데이트했습니다.
*   OpenAI는 공중 보건 및 생물 방어를 위한 신뢰할 수 있는 액세스 생물학 도구인 Rosalind Biodefense를 발표했습니다.

### 🔬 연구 & 논문
*   Hugging Face는 도구 사용 다중 턴 RL 학습 루프에서 모델 출력을 재토큰화할 때 발생하는 핵심 버그를 지적하고, 엄격한 "토큰 인, 토큰 아웃" 규칙을 수정 사항으로 제안했습니다.
*   Omar Sar는 유효 피드백 컴퓨트(EFC)에 대한 작업을 표면화하며, 하네스 품질이 총 활동보다 에이전트 성공에 더 중요함을 시사했습니다.
*   Harvard/MIT의 양방향 진화 검색(BES)은 순방향 검색과 역방향 분해 및 진화 연산자를 결합하여 MuSiQue에서 Llama-3.2-3B-Instruct의 성능을 4.0%에서 7.0%로 향상시켰습니다.
*   Latent Terms 연구는 희소 BM25-준비 기능이 SAE를 통해 고정된 밀집 리트리버에서 추출될 수 있음을 보여주었습니다.
*   BeliefTrack은 최적화된 신념 상태 관리가 장기 추론 실패를 70% 이상 줄인다고 주장했습니다.
*   NVIDIA는 24 FPS로 스트리밍되는 생성형 다중 에이전트 월드 모델인 γ-World와 실시간 대화형 비디오 월드 모델 프레임워크인 minWM을 포함한 연구를 발표했습니다.
*   dair_ai는 LLM 깨우기 결정을 220MiB 시간 그래프 인코더로 대체하여 평균 F1을 +16.7 증가시키면서 4~83배 더 빠르게 실행되는 작업을 표면화했습니다.

### 💰 산업 동향
*   LangChain 보고서에 따르면 2026년 4월 기준 AI 팀 3곳 중 1곳이 오픈 웨이트 모델을 실행했으며, 이는 9개월 전 5곳 중 1곳에서 증가한 수치입니다.
*   Hugging Face의 모델 및 데이터셋 중 약 50%가 이제 비공개이며, HF의 스토리지/버킷 제공과 함께 증가하고 있습니다.
*   NVIDIA는 4개의 오픈 모델 제품군을 Linux Foundation OpenMDW-1.1로 이동하여 가중치/코드/문서/데이터 전반에 걸쳐 법적 파편화를 줄였습니다.

### ⚡ 인프라 & 하드웨어
*   vLLM_project는 네이티브 가중치 동기화 API와 비동기 RL을 위한 개선된 일시 정지/재개 기능을 출시했으며, 나중에 CPU 토큰화 병목 현상을 줄이기 위해 Rust BPE 토크나이저인 패스트토큰을 추가했습니다.
*   Hugging Face Jobs는 CPU/서버리스 GPU CI를 위해 GitHub 러너를 대체하는 것을 보여주었습니다.
*   StepFun 3.7 Flash 모델 아티팩트는 BF16, FP8, NVFP4, GGUF 형식으로 제공되며, llama.cpp 데이-0 지원 PR과 관련 MTP 작업이 함께 제공됩니다.
*   vLLM 야간 테스트에서 NVFP4 체크포인트를 사용한 StepFun 3.7 Flash는 2x Pro 6k에서 약 2200 tok/s에 도달했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
