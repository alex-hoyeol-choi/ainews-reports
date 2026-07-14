# Codex usage up >10x in 6 months to 7M users, +1M in the past ~day; did Codex overtake Claude Code?? - 요약

**원문 URL**: https://www.latent.space/p/ainews-codex-usage-up-10x-in-6-months
**번역일**: 2026-07-14 06:53
**발행일**: 2026-07-14

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식 요약 브리핑입니다.

### 🔥 주요 뉴스
**[Codex/GPT-5.6 Sol 사용자 수 급증]** — GPT-5.6이 7월 9일 출시된 후, Codex 사용량이 6개월 만에 10배 증가하여 7월 12일 기준 600만 명, 24.5시간 후 700만 명을 달성했습니다. 이는 연초 대비 약 10배 성장한 수치입니다.
![X avatar for @thsottiaux](https://pbs.substack.com/profile_images/2075819673263001600/pj1vyX6I.jpg)
![X avatar for @thsottiaux](https://pbs.substack.com/profile_images/2075819673263001600/pj1vyX6I.jpg)
![](https://substack-post-media.s3.amazonaws.com/public/images/09c078c3-d47d-4ab1-91e5-b09ad5d082dd_1388x902.png)
**[Prime Intellect, 에이전트 RL 인프라 'Verifiers v1' 출시]** — Prime Intellect는 에이전틱 RL 및 평가를 위한 환경 스택을 재설계한 Verifiers v1을 출시했습니다. 롤아웃 트레이스 저장 방식을 메시지 DAG로 변경하여 트레이스 성장을 O(n²)에서 O(n)으로 개선했으며, 6개의 H200 노드에서 100B 추론 모델을 2일 이내에 학습시켰다고 주장합니다.
**[OpenAI, GPT-5.6 Sol 사용량 소모 문제 해결 위한 조정 발표]** — OpenAI는 ChatGPT Work/Codex의 GPT-5.6 Sol 사용량 소모 문제를 해결하기 위해 인퍼런스 최적화, 컨텍스트 윈도우 한도 372k에서 272k로 롤백, 일부 실험적 추론 변경 사항 되돌리기, 과도한 멀티 에이전트 동작 수정 등의 조치를 취했습니다.
**[xAI Grok Build, 개인 코드 무단 업로드 논란 및 대응]** — xAI의 Grok Build CLI가 코딩 태스크에 필요한 것보다 많은 전체 리포지토리(개인 코드 및 비밀 포함)를 Google Cloud 버킷에 업로드한다는 주장이 제기되었습니다. xAI는 Zero Data Retention(ZDR)을 사용하는 팀의 경우 데이터가 보존되지 않으며, /privacy 명령을 통해 보존을 비활성화하고 데이터를 삭제할 수 있다고 답변했습니다.

### 📊 모델 & 벤치마크
*   Arena 리더보드에서 GPT-5.6 Sol이 7.8K 실제 에이전틱 세션을 기반으로 에이전트 부문 2위에 올랐으며, Grok-4.5는 13위로 크게 상승했습니다.
*   Terra Max가 Fable 5 Max보다 점수에서 약간 앞서면서도 훨씬 낮은 비용을 보이는 등, 벤치마크가 토큰 가격에서 태스크당 비용으로 이동하는 추세가 나타났습니다.
*   Cognition은 Devin Fusion(Fable 5 사용)이 Opus 4.8보다 태스크당 비용이 더 낮을 수 있다고 보고했습니다.

### 🛠️ 제품 & 도구
*   Prime Intellect는 에이전틱 RL 및 평가를 위한 환경 스택을 대폭 재설계한 Verifiers v1을 출시했습니다.
*   OpenAI ChatGPTapp은 EEA 지역 WhatsApp에서 ChatGPT의 복귀를 발표했으며, 추가 시장에서 카카오/Viber 지원을 발표했습니다.
*   Factory는 사용자가 수동 편집 대신 UI 요소/파일을 가리키는 "디자인 모드"를 통해 하네스 설계의 새로운 관점을 제시했습니다.
*   LlamaCoder v4가 GLM 5.2를 기반으로 재구축되어 출시되었습니다.

### 🔬 연구 & 논문
*   지속 학습(Continual Learning)이 일류 시스템 문제로 재부상하며, Morpheus라는 영구적인 엔터프라이즈 시뮬레이션이 실제 RL을 위해 소개되었습니다.
*   LLM이 단기 기억을 장기 기억으로 통합하는 '수면' 단계와 재귀적 자기 개선을 위한 '꿈' 단계가 필요할 수 있다는 연구가 Knowledge Seeding과 함께 발표되었습니다.
*   Sakana AI는 모듈형 시스템에서 분산된 물리적 자기 인식 및 수리를 위한 Smart Cellular Bricks를 공개했습니다.
*   ByteDance는 시각적 데모에서 직접 추론/역학/계획을 학습하는 UniVR-34B를 발표했습니다.
*   Google DeepMind는 역사적 인퍼런스 워크플로우를 위한 Predicting the Past 스킬을 공개했습니다.
*   Anthropic은 30만 개 이상의 익명 대화 분석을 기반으로 Claude의 표현된 가치가 모델 및 언어에 따라 어떻게 다른지에 대한 연구를 발표했습니다.

### 💰 산업 동향
*   xAI의 Grok Build CLI가 개인 코드 및 비밀을 포함한 전체 리포지토리를 Google Cloud 버킷에 업로드한다는 논란이 발생했으며, xAI는 Zero Data Retention(ZDR) 정책을 강조하며 대응했습니다.
*   오픈 모델이 단순히 비용 절감뿐만 아니라 인간-AI 학습 루프에 대한 제어권과 기관 지식을 사내에 유지하는 것과 관련이 있다는 주장이 제기되었습니다.

### ⚡ 인프라 & 하드웨어
*   Hugging Face Transformers 모델이 이제 vLLM에서 네이티브 속도로 실행될 수 있도록 통합되어, 각 새로운 아키텍처를 두 번 구현해야 하는 부담이 줄어들었습니다.
*   새로운 양자화 방법이 미리 공개되었으며, 이는 기존 접근 방식(NVIDIA ModelOpt 포함)을 능가하여 더 나은 레이어별 정밀도 할당과 더 높은 벤치마크 점수를 제공한다고 주장합니다.
*   Unsloth는 GGUF, NVFP4, FP8을 아우르는 LLM 양자화 및 배포에 대한 AWS 가이드를 발표했습니다.
*   일부 사용자들이 GLM-5.2 및 Kimi K2.7 Code NVFP4를 8xB200 노드에서 사용하는 스택으로 실제 작업 파이프라인을 마이그레이션하여 매우 저렴한 비용으로 더 밀도 높은 보고서를 얻었다고 보고했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
