# not much happened today - 요약

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-6b8
**번역일**: 2026-06-06 06:22
**발행일**: 2026-06-06

---

### 🔥 주요 뉴스
**[Google, Gemma 4 QAT 체크포인트 출시]** Google이 모든 Gemma 4 모델 크기에 대해 Quantization-Aware Training (QAT) 체크포인트를 출시했습니다. 이는 모바일 양자화 형식을 포함하여 품질을 유지하면서 낮은 메모리 사용량을 강조하며, E2B 모델은 약 1GB에서 실행 가능합니다. Ollama 및 vLLM을 통해 즉시 에코시스템 지원이 이루어졌습니다.

**[Ideogram 4.0 출시 및 성능]** Ideogram AI가 8B VLM 텍스트 인코더와 함께 처음부터 학습된 9.3B Diffusion Transformer인 Ideogram 4.0을 출시했습니다. 특히 fp8 및 nf4 체크포인트를 제공하며, nf4 변형은 단일 24GB GPU에 적합합니다. Arena 평가에서 Ideogram 4.0 Quality는 텍스트-이미지 최고 티어 및 선도적인 오픈 웨이트 이미지 모델로 평가받았습니다.

**[Sakana AI, RSI Lab 설립]** Sakana AI가 도쿄에 재귀적 자기 개선(RSI) 전용 연구소인 RSI Lab을 설립했습니다. 이 연구소는 The AI Scientist, Darwin Gödel Machine, ShinkaEvolve와 같은 이전 프로젝트들을 통합하며, 자기 개선 시스템이 컴퓨팅 제약 조건 하에서도 구축될 수 있음을 목표로 합니다.

**[Cloudflare AI Gateway 비용 제어 기능 출시]** Cloudflare가 AI Gateway에 인퍼런스 라우팅을 위한 구체적인 비용 제어 기능을 출시했습니다. 이는 지출 한도, 모델/사용자별 예산 강제 적용, 한도 도달 시 더 저렴한 모델로의 폴백(fallback) 기능을 포함하며, 향후 ID 기반 제어도 예정되어 있습니다.

**[OpenAI, ChatGPT Lockdown Mode 출시]** OpenAI가 모든 사용자에게 ChatGPT Lockdown Mode를 출시했습니다. 이 기능은 외부 네트워크 요청을 제한하여 프롬프트 인젝션으로 인한 데이터 유출 위험을 줄이는 것을 목표로 합니다.

### 📊 모델 & 벤치마크
*   Anthropic, Claude Opus 4.7의 과학적 성능 발표: Anthropic은 Claude Opus 4.7이 특정 화학 작업에서 전용 NMR 소프트웨어와 일치하거나 능가하는 구체적인 과학적 결과를 달성했다고 발표했습니다.
*   Google, Gemma 4 QAT 체크포인트 출시: 모든 Gemma 4 모델 크기에 대해 Quantization-Aware Training (QAT) 체크포인트를 출시하여, 모바일 양자화 형식을 포함한 저메모리 온디바이스 인퍼런스를 지원합니다.
*   Ideogram 4.0 출시 및 성능 평가: Ideogram AI가 9.3B Diffusion Transformer인 Ideogram 4.0을 출시했으며, nf4 변형은 단일 24GB GPU에 적합합니다. Arena 평가에서 텍스트-이미지 최고 티어 및 선도적인 오픈 웨이트 이미지 모델로 선정되었습니다.
*   NVIDIA Nemotron 3 Ultra 세부 사항 공개: Nemotron 3 Ultra의 사후 학습(post-training) 세부 사항으로 교사-학생 분포 매칭을 위한 MOPD 웜업 및 추측 디코딩을 위한 MTP 부스팅 등이 논의되었습니다.
*   dair_ai, Agents’ Last Exam (ALE) 벤치마크 도입: 미국 직업 분류 체계에 매핑된 1,000개 이상의 경제적으로 가치 있는 작업으로 구성된 새로운 벤치마크를 도입했으며, 가장 어려운 티어의 평균 통과율은 2.6%에 불과했습니다.
*   rishi_desai2, SWE-Marathon 벤치마크 출시: 코딩 에이전트가 10억 토큰 예산 내에서 Slack 클론 구축, JAX를 PyTorch로 재작성 등 장기 프로젝트에서 일관성을 유지하는지 테스트하는 벤치마크를 출시했습니다.
*   Meta-Agent Challenge 강조: 에이전트들이 샌드박스, eval API, 시간 예산 설정 하에서 스스로 개선을 시도하는 챌린지가 강조되었으며, 메타 에이전트의 성능은 인간 기준선에 미치지 못했습니다.

### 🛠️ 제품 & 도구
*   Hermes Agent v0.16.0 출시: 데스크톱 GUI 앱, 대시보드 전면 개편, 간소화된 내장 스킬, 원격 대시보드/GUI 접근을 위한 새로운 보안 계층을 포함하는 주요 업데이트가 출시되었습니다.
*   Arena, Agent Mode 및 Agent Arena 출시: 사용자가 실제 작업에서 에이전트를 실행하고 성공률, 도구 환각 등 집계 메트릭을 리더보드에 제공하는 능동적인 에이전트 런타임 플랫폼으로 전환되었습니다.
*   MagicPath, 공식 Codex 플러그인으로 출시: MagicPath가 공식 Codex 플러그인으로 출시되었습니다.
*   Cursor Design Mode 출시: UI 변경의 시각적 프롬프팅을 위한 Cursor Design Mode가 출시되어 포인팅, 드로잉, 음성을 통한 멀티모달 UI 편집 기능을 제공합니다.
*   Perplexity Computer 내 Vercel 통합: Perplexity Computer에 Vercel 통합이 추가되어 배포를 검사하고 자연어로 재배포할 수 있게 되었습니다.
*   Perplexity, Nemotron 3 Ultra 제공: Perplexity가 Nemotron 3 Ultra를 Pro/Max 사용자에게 제공하며, 이를 장기 실행 에이전트를 위한 오픈 모델로 홍보했습니다.
*   Anthropic, Claude Cowork 사용량 제한 두 배 증대: Anthropic이 한 달 동안 Claude Cowork의 사용량 제한을 두 배로 늘려 더 큰 위임 작업을 지원합니다.

### 🔬 연구 & 논문
*   Princeton, AI 에이전트 신뢰성 연구 업데이트: ICML 2026 논문 "Towards a Science of AI Agent Reliability"가 업데이트되어 GPT 5.5, Gemini 3.1 Pro / 3.5 Flash, Claude Opus 4.7을 포함한 최신 모델들이 이전 모델보다 의미 있게 더 신뢰할 수 있지 않다고 결론 내렸습니다.
*   Google Research, 에이전틱 RAG 프레임워크 도입: 원샷 리트리벌이 아닌 반복적인 컨텍스트 수집을 특징으로 하는 멀티 에이전트 엔터프라이즈 RAG 워크플로우를 도입했습니다.
*   Epoch AI, AI 인프라 경제학 추정치 발표: 2026년 1분기 AI 관련 데이터 센터 건설, 컴퓨팅 하드웨어 및 네트워킹 비용이 미국 GDP의 약 0.8%에 달할 것으로 추정했습니다.

### 💰 산업 동향
*   Sakana AI, RSI Lab 설립: 도쿄에 재귀적 자기 개선(RSI) 전용 연구소인 RSI Lab을 설립하여 자기 개선 시스템 연구를 공식화했습니다.
*   NVIDIA, Nemotron Coalition 확장: Nous, Prime Intellect, hcompany 등을 추가하며 Nemotron Coalition 에코시스템을 확장했습니다.

### ⚡ 인프라 & 하드웨어
*   Cloudflare, AI Gateway 비용 제어 기능 출시: AI Gateway에 지출 한도, 모델/사용자별 예산 강제 적용, 한도 도달 시 저렴한 모델로의 폴백(fallback) 기능을 포함한 인퍼런스 라우팅 비용 제어 기능을 출시했습니다.
*   OpenAI, ChatGPT Lockdown Mode 출시: 모든 사용자에게 외부 네트워크 요청을 제한하여 프롬프트 인젝션으로 인한 데이터 유출을 방지하는 보안 기능을 출시했습니다.
*   OpenAI, 계정 정지 사고 발생 및 복구: OpenAI가 계정 정지 사고를 겪었으나, 대부분의 계정 및 구독이 나중에 복원되었다고 공식적으로 인정했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
