# Everything is Conductor - 요약

**원문 URL**: https://www.latent.space/p/ainews-everything-is-conductor
**번역일**: 2026-05-15 06:18
**발행일**: 2026-05-15

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 브리핑입니다.

### 🔥 주요 뉴스
*   **[OpenAI, ChatGPT 모바일 앱에 Codex 통합 및 원격 제어 기능 추가]** — OpenAI는 ChatGPT 모바일 앱에 Codex를 탑재하여 사용자가 노트북, Mac mini 또는 데브박스에서 실행 중인 코딩 에이전트 세션을 원격으로 시작, 검토, 승인, 지시할 수 있도록 했습니다. 이는 개발자 워크플로우의 유연성을 크게 향상시키는 중요한 업데이트입니다.
*   **[GitHub, Copilot App 기술 프리뷰 출시]** — GitHub는 병렬 워크스트림, 레포/PR 라이프사이클 관리, 모델 유연성을 위한 데스크톱 환경을 제공하는 GitHub Copilot App의 기술 프리뷰를 발표했습니다. 이는 "에이전트 우선(agent-first)" 사용자 경험으로의 전환을 가속화하는 움직임입니다.
*   **[Figure, 휴머노이드 로봇 24시간 연속 자율 작동 시연]** — Figure는 소형 패키지 분류 작업에서 24시간 이상 연속 자율 작동에 성공하며 인간과 거의 동등한 처리량을 달성했다고 보고했습니다. Helix-02가 온보드에서 전적으로 작동하며 원격 조작(teleoperation)이 없었음을 명시적으로 주장하여 로봇 공학 분야의 중요한 이정표를 세웠습니다.
*   **[Anthropic, Claude Code 사용 제한 및 개발자 반발]** — Anthropic은 서드파티 래퍼(wrappers) 및 대량의 프로그래밍 방식 워크플로우에 대한 Claude Code 사용을 제한/재편했습니다. 이는 개발자 커뮤니티의 강한 반발을 불러일으키며 플랫폼 위험과 구독 기반 에이전트 워크플로우의 안정성에 대한 논의를 촉발했습니다.
*   **[LangChain, 에이전트 인프라 스택 대거 출시 (SmithDB, LangSmith Engine, LangChain Labs)]** — LangChain은 에이전트 트레이스 데이터를 위한 데이터베이스 SmithDB, 실패 클러스터링 및 개선 제안 엔진 LangSmith Engine, 그리고 에이전트의 지속 학습 연구를 위한 LangChain Labs를 발표하며 에이전트 개발 인프라를 강화했습니다.

### 📊 모델 & 벤치마크
*   **Zyphra, ZAYA1-8B-Diffusion-Preview 모델 출시:** 자기회귀 생성(autoregressive generation) 대비 4.6~7.7배 빠른 디코딩 속도를 제공하며, Diffusion LM의 효율성을 입증했습니다.
*   **Datadog, Toto 2.0 시계열 예측 모델 5종 공개:** Apache 2.0 라이선스 하에 4M에서 2.5B 파라미터에 이르는 5개의 오픈 웨이트 시계열 예측 모델을 출시하고, BOOM, GIFT-Eval, TIME 벤치마크에서 1위를 차지했습니다.
*   **Prime Intellect, nanoGPT 스피드런 벤치마크에서 자율 옵티마이저 성능 기록:** Opus 4.7이 2930 스텝, GPT-5.5가 2950 스텝에 도달하여 약 1만 회 실행 및 1만 4천 H200 시간 후 인간 기준선인 2990을 넘어섰습니다.
*   **Moonshot AI, Kimi K2.6이 Finance Agent Benchmark V2에서 1위:** Kimi K2.6이 Finance Agent Benchmark V2에서 오픈 웨이트 모델 중 1위를 기록했습니다.
*   **vLLM, Ring-2.6-1T 모델에 day-0 지원 추가:** Ring-2.6-1T 오픈 릴리스에 vLLM 지원이 즉시 제공됩니다.

### 🛠️ 제품 & 도구
*   **OpenAI, ChatGPT 모바일 앱에 Codex 통합:** 사용자가 노트북, Mac mini 또는 데브박스에서 실행 중인 Codex 작업을 원격으로 시작, 검토, 승인, 지시할 수 있습니다.
*   **OpenAI, Remote SSH 일반 가용성 및 비즈니스/엔터프라이즈 자동화 훅 발표:** 관리형 원격 환경에서 Remote SSH가 일반적으로 사용 가능하며, Codex 루프 중심의 비즈니스/엔터프라이즈 자동화를 위한 훅과 프로그래밍 방식 액세스 토큰이 추가될 예정입니다.
*   **GitHub, GitHub Copilot App 기술 프리뷰 출시:** 병렬 워크스트림, 레포/PR 라이프사이클 관리, 모델 유연성을 위한 데스크톱 환경을 제공합니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/cc0e389d-df44-481c-998d-5524cf58e696_1194x1250.png)
*   **VS Code, 멀티 에이전트 워크플로우를 위한 Agents 창 출시:** 멀티 에이전트, 멀티 프로젝트 워크플로우를 위한 새로운 Agents 창, 브라우저/모바일 지원(vscode.dev/agents), BYOK 개선 사항, 압축된 터미널 출력과 같은 토큰 효율성 기능을 포함합니다.
*   **Nous/Hermes Agent, Codex 런타임 통합 추가:** OpenAI 기반 턴을 Codex CLI/앱 서버를 통해 라우팅하고 ChatGPT 구독 기반 실행을 Hermes 세션에서 재사용합니다.
*   **Kimi, Kimi Web Bridge 출시:** Kimi Code CLI, Claude Code, Cursor, Codex, Hermes 등 다양한 코드 에이전트에 인간과 유사한 웹 상호 작용을 노출하는 브라우저 확장 프로그램입니다.
*   **LangChain, SmithDB 출시:** 에이전트 트레이스 데이터를 위해 특별히 구축된 데이터베이스입니다.
*   **LangChain, LangSmith Engine 출시:** 트레이스를 소비하고, 실패를 클러스터링하며, 잠재적인 코드 문제를 식별하고, 수정/평가를 제안하여 관찰 가능성을 개선 루프로 전환합니다.
*   **AtomicBot-ai, Qwen용 Multi-Token Prediction (MTP) 및 TurboQuant 지원 llama.cpp 포크 공개:** Qwen 3.6 27B/35B용 GGUF MTP 양자화와 함께, MacBook Pro M5 Max에서 21 tok/s에서 34 tok/s로 속도 향상을 보고했습니다.

### 🔬 연구 & 논문
*   **OpenAI, Codex용 Windows 샌드박스 기술 보고서 발표:** 코딩 에이전트의 유용성과 제한된 머신 액세스 간의 트레이드오프에 초점을 맞춘 기술 보고서를 공개했습니다.
*   **LangChain, LangChain Labs 발표:** 프로덕션 트레이스가 장기적으로 학습 신호, 평가, 목표 역량 개선으로 이어져야 한다는 가설을 가진 에이전트의 지속 학습에 대한 응용 연구 노력입니다.
*   **Goodfire, Llama의 산술 연산 메커니즘 연구 결과 발표:** Llama가 산술 연산을 위해 기하학적인 "모양 회전 계산기" / 푸리에 특징과 유사한 메커니즘을 사용하며, 조향 기반 증거를 제시한다고 주장했습니다.
*   **The Turing Post, LLM RL을 롤아웃 엔지니어링으로 구성하는 설문조사 발표:** LLM RL을 PPO 대 GRPO가 아닌 생성(Generate) / 필터(Filter) / 제어(Control) / 재생(Replay) 전반에 걸친 롤아웃 엔지니어링으로 구성하는 설문조사를 제시했습니다.
*   **Souradip Chakraborty, 특권 정보를 활용한 교육적 RL (Pedagogical RL) 연구:** 유용한 롤아웃을 적극적으로 찾는 교육적 RL에 대한 연구를 발표했습니다.

### 💰 산업 동향
*   **Anthropic, Claude Code 사용 제한 및 재편:** 서드파티 래퍼 및 대량의 프로그래밍 방식 워크플로우에 대한 Claude Code 사용을 제한/재편했습니다.

### ⚡ 인프라 & 하드웨어
*   **W&B/CoreWeave, CoreWeave Sandboxes 출시:** RL, 도구 사용, 평가 워크로드에서 격리된 실행을 위한 샌드박스를 출시했으며, 파괴적인 명령을 대규모로 명시적으로 테스트했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
