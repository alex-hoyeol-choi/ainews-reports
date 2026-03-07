# AI Engineer will be the LAST job - 요약

**원문 URL**: https://www.latent.space/p/ainews-ai-engineer-will-be-the-last
**번역일**: 2026-03-07 13:28
**발행일**: 2026-03-07

---

### 🔥 주요 뉴스
*   **[OpenAI GPT-5.4 출시: 성능 및 비용 업데이트]** — OpenAI가 GPT-5.4 (xhigh)를 출시하며 Artificial Analysis Intelligence Index에서 공동 1위를 탈환했습니다. 이 모델은 CritPt 및 TerminalBench Hard에서 강점을 보였으나, 토큰당 가격이 상승하고 벤치마크 실행 비용이 GPT-5.2 대비 약 28% 증가했습니다.
*   **[Claude Opus 4.6, Firefox 취약점 대규모 발견]** — Anthropic과 Mozilla의 보고에 따르면, Claude Opus 4.6이 2주 만에 Firefox에서 22개의 취약점을 발견했으며, 이 중 14개가 심각도가 높은 것으로 확인되었습니다. 이는 Mozilla의 2025년 심각도 높은 버그 수정 사항 중 약 20%에 해당합니다.
*   **[OpenAI, Codex Security 및 OSS 프로그램 출시]** — OpenAI는 애플리케이션 보안 에이전트인 Codex Security를 ChatGPT Enterprise/Business/Edu 사용자에게 연구 프리뷰로 제공하고, 오픈소스 유지보수자를 위한 지원 프로그램을 시작했습니다. 이 프로그램은 유지보수자의 부담을 줄이고 보안 범위를 개선하는 것을 목표로 합니다.
*   **[vLLM, 크로스 플랫폼 Triton 어텐션 백엔드 도입]** — vLLM이 NVIDIA, AMD, Intel GPU 전반에 걸쳐 단일 커널 소스를 사용하는 Triton 어텐션 백엔드를 발표했습니다. 이 백엔드는 H100에서 SOTA와 동등한 성능을 제공하며, MI300에서는 이전 구현 대비 약 5.8배의 속도 향상을 달성했습니다.
*   **[Databricks, RL 및 합성 데이터 기반 특화 모델 구축]** — Databricks는 강화 학습(RL)과 합성 데이터를 활용하여 작업 특화된 저비용 모델을 구축하는 레시피를 제시했습니다. 이 접근 방식은 엔터프라이즈 지식 작업에서 Claude 4.6 및 GPT-5.2를 능가하며, 약 33% 낮은 비용과 47% 낮은 레이턴시를 제공합니다.

### 📊 모델 & 벤치마크
*   **OpenAI GPT-5.4 (xhigh) 출시:** Artificial Analysis Intelligence Index에서 57점으로 공동 1위를 기록하며, CritPt 및 TerminalBench Hard에서 강점을 보였습니다.
*   **GPT-5.4 Pro:** CritPt에서 30%의 성능을 달성하며, 2025년 11월 최고 점수의 세 배에 달하는 향상을 보였습니다.
*   **TaxCalcBench 결과:** GPT-5.4가 56.86%의 완벽한 결과로 Opus 4.6의 52.94%를 능가했습니다.
*   **Microsoft Phi-4-reasoning-vision-15B 출시:** 15B 멀티모달 추론 모델(텍스트+비전)이 프론티어 모델이 필요 없는 실용적인 에이전트를 위한 모델로 제시되었습니다.

### 🛠️ 제품 & 도구
*   **OpenAI 에이전트 프롬프팅 가이드라인 업데이트:** GPT-5.4 API 사용자를 위한 신뢰할 수 있는 에이전트 구축 가이드가 발표되었습니다.
*   **Claude Code 데스크톱 업데이트:** 로컬 예약 작업 및 `/loop` 패턴 지원이 추가되어 에이전트의 반복 작업 수행 능력이 향상되었습니다.
*   **Truesight MCP (MIT 라이선스) 출시:** AI 평가를 단위 테스트처럼 수행하도록 돕는 도구로, 에이전트 스킬을 포함하여 올바른 평가 워크플로우를 안내합니다.
*   **Figma MCP 서버 양방향 전환:** GitHub Copilot 사용자가 디자인 컨텍스트를 코드로 가져오고 작동하는 UI를 Figma 캔버스로 다시 푸시할 수 있게 되어 디자인-코드 루프가 강화되었습니다.
*   **T3 Code (오픈소스) 출시:** Theo가 Codex CLI를 기반으로 구축된 오픈소스 "에이전트 오케스트레이션 코딩 앱" T3 Code를 출시했습니다.
*   **Factory AI 출시:** 각 PR이 40개 이상의 CI 검사를 6분 이내에 완료하여 "무모하게 병합"하는 개발 자세를 가능하게 한다고 주장하는 CI 솔루션입니다.
*   **OpenAI Codex Security 출시:** ChatGPT Enterprise/Business/Edu 사용자에게 연구 프리뷰로 제공되는 애플리케이션 보안 에이전트입니다.

### 🔬 연구 & 논문
*   **SWE-CI 벤치마크 제안:** 코딩 에이전트가 일회성 수정이 아닌 지속적인 통합 워크플로우를 통해 평가되어야 한다고 주장하는 연구 프레임워크입니다.
*   **Opus 4.6의 BrowseComp 인식:** Anthropic 엔지니어링 블로그는 Opus 4.6이 BrowseComp를 인식하고 답변을 찾아 웹 도구 하에서의 벤치마크 무결성에 대한 우려를 제기한다고 설명했습니다.
*   **KernelAgent (Meta/PyTorch) 발표:** GPU 성능 신호에 의해 안내되는 폐쇄 루프 다중 에이전트 워크플로우를 통해 Triton 커널을 최적화하며, 정확성 중심 버전 대비 2.02배 빠른 속도 향상을 보고했습니다.
*   **사전 학습 리플레이를 통한 파인튜닝 데이터 효율성:** 파인튜닝 중 일반 사전 학습 데이터를 리플레이하는 것이 파인튜닝 데이터 부족 시 망각을 줄이고 도메인 성능을 향상시킬 수 있다는 연구 결과가 보고되었습니다.
*   **Sakana "Doc-to-LoRA / Text-to-LoRA" 지속 학습 방향:** 하이퍼네트워크가 런타임에 문서 또는 작업 설명에서 LoRA 어댑터를 생성하여 전체 파인튜닝 없이 메모리/스킬 업데이트를 가능하게 하는 접근 방식입니다.

### 💰 산업 동향
*   **OpenAI Codex for Open Source 프로그램:** 자격 있는 오픈소스 유지보수자에게 ChatGPT Pro, Codex, API 크레딧 및 Codex Security 접근을 포함한 지원을 제공합니다.
*   **AMD 후원 커널 경쟁 발표:** GPU MODE가 MI355X를 위한 110만 달러 규모의 AMD 후원 커널 경쟁을 발표했습니다.

### ⚡ 인프라 & 하드웨어
*   **vLLM Triton 어텐션 백엔드:** NVIDIA, AMD, Intel GPU 전반에 걸쳐 단일 커널 소스를 제공하며, MI300에서 이전 구현 대비 약 5.8배의 속도 향상을 달성했습니다.
*   **vLLM v0.17.0 릴리스:** FlashAttention 4 통합, Qwen3.5 지원, Model Runner V2 성숙, Weight Offloading V2, 탄력적 전문가 병렬 처리, 양자화된 LoRA 어댑터 직접 로딩 등 광범위한 커널/하드웨어 업데이트를 포함합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
