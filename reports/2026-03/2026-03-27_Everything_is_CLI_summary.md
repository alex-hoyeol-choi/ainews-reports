# Everything is CLI - 요약

**원문 URL**: https://www.latent.space/p/ainews-everything-is-cli
**번역일**: 2026-03-27 07:19
**발행일**: 2026-03-27

---

### 🔥 주요 뉴스
**[Google, 실시간 AI 에이전트용 Gemini 3.1 Flash Live 출시]** — Google이 음성 및 비전 에이전트를 위한 새로운 실시간 모델 Gemini 3.1 Flash Live를 공개했습니다. 이 모델은 낮은 레이턴시, 향상된 함수 호출, 시끄러운 환경에서의 견고성, 그리고 Gemini Live에서 2배 더 긴 대화 메모리를 특징으로 합니다. Artificial Analysis 벤치마크에서 높은 추론 시 2.98초의 TTFA로 95.9%의 Big Bench Audio 성능을 기록했습니다.

**[OpenAI, GPT-5.4 mini 및 nano 변형 모델 공개]** — Artificial Analysis에 따르면 OpenAI가 멀티모달이며 400k 컨텍스트를 지원하는 GPT-5.4 mini와 GPT-5.4 nano를 출시했습니다. 특히 GPT-5.4 nano는 Claude Haiku 4.5 및 Gemini 3.1 Flash-Lite Preview보다 우수한 벤치마크 성능과 더 저렴한 비용을 보였으나, 높은 장황함과 환각률이 단점으로 지적되었습니다.

**[Sakana AI, AI 연구 자동화에 대한 Nature 논문 발표]** — Sakana AI가 AI 연구의 엔드투엔드 자동화에 대한 Nature 논문을 발표하며, AI 과학의 스케일링 법칙을 제시했습니다. 이들은 더 강력한 파운데이션 모델이 더 우수한 과학 논문을 생성하며, 이는 더 나은 기본 모델과 더 많은 추론 컴퓨팅으로 개선될 수 있다고 주장합니다.

**[Meta, 뇌 인코더 TRIBE v2 출시]** — Meta AI가 700명 이상의 500시간 이상 fMRI 데이터로 학습된 트라이모달 뇌 인코더 TRIBE v2를 공개했습니다. 이 모델은 이전 방법보다 2~3배 향상된 성능을 보이며, 보지 못한 주체, 언어, 작업에 대한 제로샷 예측이 가능하다고 주장합니다.

**[Stripe, 에이전트 서비스 프로비저닝 CLI 'ShareProjects.dev' 출시]** — Stripe가 에이전트가 서비스를 즉시 프로비저닝할 수 있는 CLI 도구 ShareProjects.dev를 출시했습니다. `stripe projects add posthog/analytics`와 같은 명령어로 PostHog 계정 생성, API 키 발급, 결제 설정 등을 자동화할 수 있습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/a29a5ad3-a76b-4aa4-b5eb-58bb7e229370_665x500.jpeg)
![](https://substack-post-media.s3.amazonaws.com/public/images/4235a84e-655c-4e77-bced-3d73e105e793_1876x394.png)

### 📊 모델 & 벤치마크
*   **Google Gemini 3.1 Flash Live 출시:** 음성 및 비전 에이전트용 실시간 모델로, 낮은 레이턴시, 향상된 함수 호출, 70개 언어, 128k 컨텍스트, SynthID를 통한 생성 오디오 워터마킹을 지원합니다. Artificial Analysis 벤치마크에서 높은 추론 시 2.98초의 TTFA로 95.9%의 Big Bench Audio 성능을 기록했습니다.
*   **Mistral AI, Voxtral TTS 모델 공개:** 프로덕션 음성 에이전트를 위한 오픈 웨이트 TTS 모델로, 9개 언어를 지원하며 낮은 레이턴시와 약 90ms의 time-to-first-audio를 제공합니다. 선호도 테스트에서 ElevenLabs에 비해 유리한 결과를 보였습니다.
*   **Cohere, 첫 오디오 모델 Cohere Transcribe 출시:** Apache 2.0 라이선스의 음성 모델로, Hugging Face Open ASR 리더보드에서 영어 부문 최고 순위(5.42 WER)를 차지하며 14개 언어를 지원합니다.
*   **OpenAI GPT-5.4 mini 및 nano 변형 모델 보고:** Artificial Analysis에 의해 멀티모달, 400k 컨텍스트를 가진 두 모델이 보고되었으며, nano 변형은 Claude Haiku 4.5 및 Gemini 3.1 Flash-Lite Preview보다 우수한 벤치마크 성능과 비용 효율성을 보였습니다.
*   **Chroma, 검색 중심 모델 Context-1 오픈소스화:** SFT+RL로 8,000개 이상의 합성 작업을 통해 학습된 모델로, 프론티어 범용 모델보다 더 좋고, 빠르며, 저렴한 검색을 제공한다고 주장합니다.
*   **Meta, 트라이모달 뇌 인코더 TRIBE v2 출시:** 700명 이상의 500시간 이상 fMRI 데이터로 학습되었으며, 이전 방법보다 2~3배 향상된 성능으로 보지 못한 주체, 언어, 작업에 대한 제로샷 예측을 지원합니다.

### 🛠️ 제품 & 도구
*   **Stripe ShareProjects.dev CLI 출시:** 에이전트가 서비스를 즉시 프로비저닝할 수 있도록 돕는 CLI 도구로, PostHog와 같은 서비스 계정 생성, API 키 발급, 결제 설정 등을 자동화합니다.
*   **Ramp CLI 출시:** Ramp의 새로운 CLI 도구가 편리한 유스케이스와 함께 공개되었습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/6c2ebb50-77e8-4904-9bb1-d9b9e873bc3e_1096x1240.png)
*   **Sendblue CLI (iMessage) 및 Kapso CLI (WhatsApp) 출시:** iMessage와 WhatsApp을 위한 새로운 CLI 도구들이 각각 출시되었습니다.
*   **ElevenLabs CLI 출시:** ElevenLabs의 CLI 도구가 새롭게 공개되었습니다.
*   **Zai, GLM Coding Plan 사용자에게 GLM-5-Turbo 제공:** Zai가 GLM Coding Plan 사용자들에게 GLM-5-Turbo 모델을 제공하기 시작했습니다.
*   **Reka Edge 및 Flash 3, OpenRouter에 추가:** Reka의 Edge 및 Flash 3 모델이 OpenRouter에서 사용 가능해졌습니다.
*   **Google/Gemini, 다른 AI 앱에서 채팅 기록 및 선호도 가져오기 기능 출시:** Google/Gemini가 다른 AI 앱에서 채팅 기록 및 선호도를 가져오는 기능을 도입했습니다.
*   **Cline Kanban 출시:** 격리된 Git 워크트리에서 여러 CLI 코딩 에이전트를 병렬로 오케스트레이션하는 무료 오픈소스 로컬 웹 앱으로, Claude Code, Codex, Cline을 지원합니다.
*   **Teknium, GODMODE 스킬 공개:** 영구적인 탈옥을 위한 GODMODE 스킬을 공개하며, 기능과 안전성이 이제 하네스 레이어에서 제품화되고 있음을 강조했습니다.
*   **Google, Gemini API 스킬 구축 방법 발표:** 모델에 최신 API 및 SDK를 학습시켜 Gemini 3.1 Pro의 평가 테스트 통과율을 95%로 향상시킨 방법을 공개했습니다.
*   **OpenEnv, 에이전틱 RL 환경을 위한 오픈 표준으로 소개:** 비동기 API, 웹소켓 전송, MCP 네이티브 도구 검색, 어디든 배포 가능한 패키징을 갖춘 에이전틱 RL 환경을 위한 오픈 표준이 제시되었습니다.
*   **Anthropic, Claude Code 웹/모바일 세션용 자동 수정 기능 출시:** Claude Code 웹/모바일 세션을 위한 원격 PR 추적 자동 수정 기능을 출시하여, 무인 CI 실패 수정 및 댓글 해결을 가능하게 했습니다.

### 🔬 연구 & 논문
*   **Sakana AI, AI Scientist에 대한 Nature 논문 발표:** AI 연구의 엔드투엔드 자동화에 대한 논문으로, 더 강력한 파운데이션 모델이 더 우수한 과학 논문을 생산하는 AI 과학의 스케일링 법칙을 관찰했습니다.
*   **NVIDIA, ProRL Agent를 통한 에이전트 RL 프레임워크 개선 주장:** 롤아웃과 최적화를 분리하여 SWE-Bench Verified에서 Qwen 8B의 성능을 9.6%에서 18.0%로 거의 두 배 향상시키고 GPU 활용률을 높였다고 주장합니다.
*   **Cursor, "실시간 RL" 프로덕션 학습 패턴 공개:** 5시간마다 개선된 Composer 2 체크포인트를 출시하며, 이를 정적 모델 출시 주기 대신 제품화된 RL 피드백 루프로 제시했습니다.
*   **Kimi/Moonshot, Attention Residuals (AttnRes) 개념 설명:** 트랜스포머 깊이를 어텐션 문제로 전환하여, 레이어가 이전 레이어 출력에서 선택적으로 리트리브할 수 있도록 하는 새로운 아키텍처 개념입니다.
*   **TurboQuant, 압축 및 메모리 효율성 기술 주목:** PolarQuant와 1비트 오류 수정 (QJL)을 결합하여 거의 제로에 가까운 정확도 손실로 3비트와 유사한 압축을 달성하는 실용적인 방법입니다.
*   **IRPAPERS, 멀티모달 리트리벌의 중요성 강조:** 과학 PDF에서 OCR/텍스트 리트리벌과 이미지 페이지 리트리벌이 다른 쿼리에서 실패하며, 멀티모달 퓨전이 단독 사용보다 우수함을 보여주었습니다.

### 💰 산업 동향
*   **OpenAI, Sora 및 "성인 모드" 챗봇 개발 우선순위 하향 조정:** OpenAI가 핵심 생산성 노력에 집중하기 위해 Sora 및 "성인 모드" 챗봇을 포함한 사이드 프로젝트의 우선순위를 낮추고 있다고 보고되었습니다.

### ⚡ 인프라 & 하드웨어
*   **vLLM의 Mamba-1 CUDA 커널 버그 수정:** AI21이 GRPO 학습에서 로그 확률 불일치를 유발하는 uint32_t 오버플로우를 추적한 후, vLLM의 Mamba-1 CUDA 커널에 uint32_t를 size_t로 변경하는 미묘하지만 영향력 있는 프로덕션 버그 수정이 적용되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
