# GLM > GPT? GLM-5.2 passes vibe check; Z.ai forecasts Open Fable by December - 요약

**원문 URL**: https://www.latent.space/p/ainews-glm-gpt-glm-52-passes-vibe
**번역일**: 2026-06-19 06:50
**발행일**: 2026-06-19

---

### 🔥 주요 뉴스
**[GLM-5.2, 프론티어 모델급 성능으로 주목]** — Zhipu의 GLM-5.2가 Jeremy Howard와 Artificial Analysis의 벤치마크에서 GPT-5.5 및 Opus 4.8과 동등하거나 능가하는 성능을 보이며 오픈 모델 중 프론티어급으로 평가받고 있습니다. IndexShare 기술로 1M 토큰 추론 비용을 절감하며, Hugging Face 및 로컬 GGUF를 통해 접근성을 확대합니다.
**[새로운 에이전틱 지식 작업 벤치마크 'AA-Briefcase' 공개]** — Artificial Analysis가 실제 장기 지식 작업을 평가하는 AA-Briefcase 벤치마크를 출시했습니다. 이 벤치마크에서 Claude Fable 5가 선두를 차지했으며, GLM-5.2는 비용 효율적인 강력한 오픈 모델로 평가받았으나, 최고 모델조차 3%의 작업에서만 모든 기준을 충족하여 실제 작업의 난이도를 보여주었습니다.
**[OpenAI, 시연 기반 워크플로우 자동화 도구 'Codex Record & Replay' 출시]** — OpenAI가 사용자가 워크플로우를 시연하면 검사 가능한 스킬로 전환해주는 Codex Record & Replay를 도입했습니다. 이는 에이전트 기반 자동화에 대한 강력한 수요를 반영하며, Claude Code의 Artifacts와 Cursor AI의 /automate 등 유사한 자동화 도구 출시가 이어지고 있습니다.
**[OpenAI, 의료 분야 AI 연구 및 GPT-5.5 Instant 건강 기능 강화]** — OpenAI는 보스턴 아동병원/하버드와의 연구를 통해 AI가 소아 희귀 질환 진단에 기여했음을 발표했습니다. 또한 GPT-5.5 Instant가 60개국 의사 피드백을 바탕으로 건강 관련 질문에서 프론티어 "사고" 모델과 동등한 성능을 달성했다고 밝혔습니다.

### 📊 모델 & 벤치마크
*   **GLM-5.2 출시 및 성능:** Zhipu가 GLM-5.2를 출시했습니다. 이 모델은 IndexShare 기술을 통해 1M 토큰 추론 비용을 절감하며, Artificial Analysis 벤치마크에서 GPT-5.5를 능가하고 Opus 4.8과 동등한 성능을 보였습니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/3af66988-dd32-43bd-b9bf-84636ea1ccf8_816x514.png)
*   **GLM-5.2 로컬 추론 지원:** GLM-5.2는 MIT 라이선스로 28.5T 토큰 사전 학습되었으며, 1M 컨텍스트 및 131k 출력 지원을 제공합니다. FP8의 경우 약 744-890GB, 동적 1비트 양자화의 경우 약 176-180GB의 추론 메모리가 필요하다고 추정됩니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/dad8658e-5b52-4d40-9757-5425bf9a5900_1188x434.png)
*   **Laguna M.1 오픈 웨이트 출시:** Poolside AI가 256K 컨텍스트를 지원하는 Laguna M.1 웨이트를 Apache 2.0 라이선스로 공개했습니다. 이 모델은 70개 레이어의 희소 MoE 아키텍처를 가지며, Apple Silicon에서 3비트 MLX 빌드로 약 26 tok/s의 성능을 시연했습니다.
*   **Cohere North Mini Code 접근성 확대:** Cohere가 4비트 양자화, Ollama 지원, 무료 OpenRouter 접근을 통해 North Mini Code의 접근성을 높였습니다.
*   **AA-Briefcase 벤치마크 공개:** Artificial Analysis가 실제 장기 지식 작업을 평가하는 AA-Briefcase 벤치마크를 출시했습니다. Claude Fable 5가 1587 ELO로 선두를 달렸고, GLM-5.2는 작업당 $2.40의 비용으로 1266 ELO를 기록했습니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/96e55c88-5f9d-4573-af94-501283bf9161_814x636.png)
*   **Terminal-Bench Challenges 도입:** @terminalbench가 장기적이고 토큰 집약적인 단일 작업을 위한 Terminal-Bench Challenges를 출시했습니다.
*   **SkillWeaver 에이전트 라우팅 접근법:** @omarsar0가 에이전트 라우팅을 구성 가능한 스킬 검색과 DAG 계획으로 처리하는 SkillWeaver를 강조했습니다.
*   **Agent Arena 인과 추적 접근 방식:** @arena가 조종 가능성, bash 복구, 도구 환각과 같은 신호를 통해 인간/AI 협업의 가치를 정량화하는 Agent Arena의 인과 추적 접근 방식을 설명했습니다.

### 🛠️ 제품 & 도구
*   **Noumena Code / ncode 출시:** @_xjdr이 수십에서 수백 개의 코딩 에이전트가 동시에 실행될 때 기존 SCM 워크플로우의 문제를 해결하는 Noumena Code / ncode를 제품화했습니다. 이는 가상 얕은 체크아웃, 커밋 스택, 클라우드 동기화 등을 통합합니다.
*   **OpenAI Codex Record & Replay 도입:** @OpenAIDevs가 사용자가 워크플로우를 시연하면 검사 가능한 스킬로 전환할 수 있는 Codex Record & Replay를 출시했습니다.
*   **Cursor AI /automate 출시:** @cursor_ai가 자연어 작업에서 트리거/지침/도구를 구성하고 Slack 이모지 및 GitHub 트리거를 추가하는 /automate 기능을 출시했습니다.
*   **Claude Code Artifacts 출시:** @ClaudeDevs가 에이전트가 진행 중인 작업을 공유 가능한 라이브 페이지로 전환할 수 있는 Artifacts를 Claude Code에 출시했습니다.
*   **Cognition Devin Review에 자동 보안 리뷰 추가:** @cognition이 Devin Review에 자동 보안 리뷰 기능을 추가하여, 에이전트 추론을 통해 낮은 심각도 발견 사항을 심각한 익스플로잇과 연결합니다.
*   **Ollama 로컬 배포 지원 확대:** @ollama가 오픈 로컬 배포 지원을 확대했습니다.
*   **Turbopuffer 요금 인하 및 i8 벡터 추가:** @turbopuffer가 기본 요금을 월 $64에서 $16로 인하하고, 양자화 인식 임베딩과 결합 시 스토리지/쿼리 비용을 최대 75% 절감하는 i8 벡터를 추가했습니다.
*   **LlamaIndex LiteParse v2.1 출시:** @llama_index와 @jerryjliu0가 가장 빠른 오픈, 모델 없는 PDF/문서 → 마크다운 파이프라인을 주장하는 LiteParse v2.1을 출시했습니다.

### 🔬 연구 & 논문
*   **OpenAI, 소아 희귀 질환 진단 AI 연구 발표:** @OpenAI가 Boston Children’s/Harvard와의 NEJM AI 연구를 통해 o3 Deep Research가 이전에 해결되지 않았던 376개 소아 희귀 질환 사례 중 18개에서 새로운 진단을 찾는 데 기여했음을 공유했습니다.
*   **OpenAI, 광범위한 정렬(Alignment) 연구 결과 공개:** @OpenAI가 모델이 광범위하고 지속적으로 유익하도록 학습시키는 연구를 소개했습니다. 건강 도메인 대화에 대한 RL이 진실성, 겸손, 인간 복지 관심 등 44/53개의 정렬 및 이점 평가를 개선했다고 주장했습니다.

### ⚡ 인프라 & 하드웨어
*   **Liquid AI, 다국어 리트리벌 모델 출시:** @liquidai가 11개 언어를 지원하며 자사 엔터프라이즈 스택에서 1.5ms의 종단 간 리트리벌 레이턴시를 주장하는 LFM2.5-Embedding-350M 및 LFM2.5-ColBERT-350M을 출시했습니다.
*   **CoreWeave Kimi K2.7 Code 서빙 성능 공개:** @CoreWeave가 Kimi K2.7 Code에 대해 289 tok/s의 서빙 성능을 주장하며, 공급자 측 가격/성능을 차별화 요소로 강조했습니다.
*   **vLLM 프로젝트, Ray Serve LLM + vLLM 처리량 개선:** @vllm_project가 직접 스트리밍, Ray V2 실행기 백엔드 등을 통해 프리필 중심 워크로드에서 최대 4.4배, 디코드 중심 워크로드에서 최대 24배의 처리량 개선을 보고했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
