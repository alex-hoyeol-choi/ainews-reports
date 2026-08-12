# How to steal a Reasoning Trace - 요약

**원문 URL**: https://www.latent.space/p/ainews-how-to-steal-a-reasoning-trace
**번역일**: 2026-08-12 12:05
**발행일**: 2026-08-12

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 산업 브리핑입니다.

### 🔥 주요 뉴스
*   **[프론티어 AI 모델 추론 트레이스 탈취 취약점 발견]** — 새로운 연구 논문에서 Claude, GPT, Gemini 등 프론티어 AI 모델의 암호화된 추론 트레이스를 디코딩하여 다른 모델이나 세션으로 포팅하는 방법이 시연되었습니다. 이 취약점을 통해 공개된 트레이스에서 62개의 API 키, 33개의 이메일 주소, 33개의 비밀번호 등 민감한 데이터가 발견되어 심각한 개인정보 및 보안 위험이 제기됩니다.
    ![Image](https://substack-post-media.s3.amazonaws.com/public/images/18b4c6ea-cef8-43ba-9ef6-4aa7ae493944_3300x1890.jpeg)
*   **[NVIDIA, 에이전트 워크로드 최적화 Nemotron 3.5 Lightning 출시]** — NVIDIA가 30B MoE 모델인 Nemotron 3.5 Lightning을 공개했습니다. 이 모델은 3.6B 활성 파라미터와 1M 컨텍스트를 지원하며, 최대 4배의 처리량과 Intelligence Index 24점을 기록하여 gpt-oss-120b와 유사한 성능을 보입니다.
    ![X avatar for @NVIDIAAI](https://pbs.substack.com/profile_images/1792994406114480128/y-52J4hB.jpg)
*   **[Meta, 로컬 에이전트 워크플로우 위한 Muse Glimmer 30B 공개]** — Meta가 Apache 2.0 라이선스의 30B 밀집형 멀티모달 오픈 웨이트 모델 Muse Glimmer를 출시했습니다. 이 모델은 뛰어난 KV-cache 효율성으로 단일 RTX 3090에서 262144 컨텍스트를 22-23GB VRAM으로 실행 가능하며, 에이전트 중심 벤치마크에서 경쟁력 있는 성능을 보입니다.
    ![Image](https://substack-post-media.s3.amazonaws.com/public/images/18b4c6ea-cef8-43ba-9ef6-4aa7ae493944_3300x1890.jpeg)
*   **[Attestable, AI 무결성 위한 영지식 증명 솔루션 출시 및 2천만 달러 투자 유치]** — Attestable이 AI 무결성을 위한 실용적인 영지식 증명(zero-knowledge proofs) 솔루션을 선보이며 2천만 달러의 시드 투자를 유치했습니다. 이 솔루션은 올바른 모델이 올바른 입력으로 실행되고 올바른 툴을 호출했음을 증명하여 에이전트 트레이스의 신뢰성을 높입니다.
*   **[xAI, 클라우드 기반 AI 팀원 Grok Bot 발표]** — xAI가 자체 클라우드 컴퓨터를 가진 AI 팀원 Grok Bot을 공개했습니다. 이 봇은 Slack 스레드 및 GitHub Actions 모니터링, 예약된 루틴 반복, 다른 봇 생성/관리 등 지속적인 작업을 수행할 수 있습니다.

### 📊 모델 & 벤치마크
*   NVIDIA Nemotron 3.5 Lightning: 30B MoE (3.6B 활성 파라미터) 모델이 출시되었으며, 1M 컨텍스트와 최대 4배 처리량을 제공하고 Intelligence Index에서 24점을 기록했습니다.
*   Meta Muse Glimmer 30B: Apache 2.0 라이선스의 30B 밀집형 멀티모달 오픈 웨이트 모델로, 에이전트 중심 학습에 최적화되었으며 뛰어난 KV-cache 효율성을 보입니다.
*   Qwen 3.8-27B: Alibaba의 Qwen 3.8-27B 오픈 웨이트 모델이 이번 주 출시될 예정이며, ModelScope에 Qwen3.8-2.4T-A95B가 등록되었습니다.
*   inclusionAI Ling-3.0-tiny: 약 1.3B 활성 파라미터를 가진 8B MoE 모델로, 저메모리 및 엣지 인퍼런스에 적합하며 AA Bench에서 25점을 기록했습니다.
*   LlamaIndex ExtractBench: 엔터프라이즈 문서 추출을 위한 결정론적 벤치마크를 출시했으며, 상용 VLM이 50페이지 이상 문서에서 낮은 재현율을 보임을 지적했습니다.
*   Artificial Analysis AA-AnalystAgent: 스프레드시트/문서 정량 분석을 위한 에이전틱 벤치마크를 공개했으며, Claude Opus 5가 54%로 선두를 달리고 Kimi K3가 최고의 오픈 웨이트 모델(39%)로 평가되었습니다.

### 🛠️ 제품 & 도구
*   Unsloth Desktop: Mac, Windows, Linux에서 모델을 로컬로 실행하고 학습시키는 오픈소스 데스크톱 앱을 출시했으며, 툴 호출, 샌드박스 코드 실행, RAG 등 엔드투엔드 로컬 AI 운영 환경을 목표로 합니다.
*   OpenAI ChatGPT 데스크톱 앱 (Linux): Linux용 ChatGPT 데스크톱 앱 프리뷰를 발표했으며, Ubuntu 24.04/26.04, Debian 13, Fedora 43/44 등 x64 및 ARM64 패키지를 지원합니다.
*   xAI Grok Bot: 자체 클라우드 컴퓨터를 가진 AI 팀원 개념의 Grok Bot을 발표했으며, 툴 로그인, 지속적인 작업 수행, 다른 봇 생성/관리 기능을 제공합니다.

### 🔬 연구 & 논문
*   프론티어 AI 모델 추론 트레이스 탈취: 암호화된 추론 블록을 약한 모델에 리플레이하여 CoT를 전사하고 민감한 데이터를 추출하는 새로운 공격 방식이 보고되었습니다.
*   결정론적 정수 전용 LLM 인퍼런스: A100, H100, Apple M5 Max 등 다양한 하드웨어에서 엔드투엔드 정수 연산을 사용하여 완전히 결정론적인 LLM 인퍼런스를 구현한 연구 결과가 발표되었습니다.

### 💰 산업 동향
*   Attestable 시드 투자: AI 무결성을 위한 영지식 증명 솔루션을 제공하는 Attestable이 2천만 달러의 시드 투자를 유치했습니다.
*   AI 텍스트 워터마킹 논의: EU 규제 압력 하에 AI 텍스트 워터마킹 및 텍스트 감지 API 도입에 대한 논의가 활발하며, 출력 품질 및 간결성 저해 가능성에 대한 우려가 제기되었습니다.
*   Together + IBM + NVIDIA 파트너십: IBM Cloud에서 엔터프라이즈 인퍼런스 인프라를 발표했습니다.

### ⚡ 인프라 & 하드웨어
*   결정론적 정수 전용 LLM 인퍼런스: A100, H100, Apple M5 Max, AMD EPYC, Intel Xeon 등에서 부동 소수점 연산 없이 완전히 결정론적인 LLM 인퍼런스가 가능하며, Qwen3-0.6B 테스트에서 fp16 대비 3.6배 빠른 디코딩 속도를 보였습니다.
*   Attestable의 ZK 오버헤드 감소: 영지식 증명(ZK proofs)의 오버헤드를 여러 자릿수만큼 줄여, 원시 인퍼런스 대비 한 자릿수(<10배) 오버헤드 내에서 실용적인 검증 가능한 인퍼런스를 가능하게 했습니다.
*   Muse Glimmer의 KV-cache 효율성: Meta Muse Glimmer 30B는 모든 레이어에 SWA가 적용되었음에도 불구하고 F16 KV 캐시 사용 시 131k 컨텍스트에 약 1.8 GiB만 사용하는 매우 효율적인 KV-cache 관리를 보여주었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
