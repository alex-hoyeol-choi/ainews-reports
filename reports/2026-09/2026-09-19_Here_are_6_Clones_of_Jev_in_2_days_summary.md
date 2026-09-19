# Here are 6 Clones of Jev in 2 days - 요약

**원문 URL**: https://www.latent.space/p/ainews-here-are-6-clones-of-jev-in
**번역일**: 2026-09-19 07:01
**발행일**: 2026-09-19

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식 요약 브리핑입니다.

### 🔥 주요 뉴스
**[Jev의 등장과 빠른 확산]** — 비생성형 의사결정 모델 Jev가 출시 이틀 만에 3,600만 회의 출시 영상 조회수를 기록하며 빠르게 확산되었습니다. Jev는 LLM의 빠른 "System 1" 보완재로 포지셔닝되며, 100% 합성 데이터로 학습된 것으로 알려졌습니다.
**[Anthropic과 Accenture의 AI 안전성 평가 파트너십]** — Anthropic이 프론티어 AI의 독립적인 평가를 위해 Accenture와 파트너십을 발표했습니다. 양사는 역량 구축을 위해 5년 동안 최소 10억 달러를 투자할 예정입니다.
**[캘리포니아 주정부의 AI 안전성 규제 강화 움직임]** — 캘리포니아 주지사 개빈 뉴섬이 킬 스위치, 외부 모니터 내장, 필수 안전 계획을 포함한 강력한 AI 안전성 법안을 권고할 전문가 패널 소집 행정 명령에 서명했습니다.

### 📊 모델 & 벤치마크
*   Jev의 클론 모델 6종(Laya, DiffusionGemmaJev, Bespoke Nimble, SemIf, Jevlike, Kev-0.5B)이 빠르게 등장했습니다.
*   Bespoke Nimble은 Qwen3.5-9B의 LoRA 파인튜닝으로, 자체 평가에서 기본 Qwen 대비 66%에서 90%로 성능을 향상시켰으며, Jev는 93%를 기록했습니다.
*   Kev-0.5B는 MacBook Pro에서 실행 가능한 Qwen2.5-0.5B 기반의 작은 Jev 유사 모델로 출시되었습니다.
*   RSI-Exam 벤치마크 업데이트에서 GPT-6-astra가 0.5126으로 1위를 유지하고, Fable 5.1이 0.4813으로 2위를 차지했습니다.
*   GPT-6 Astra가 FrontierMath의 또 다른 오픈 문제를 상호작용 세션에서 해결했습니다.
*   CUA-Bench가 실시간 키보드/마우스 사용을 테스트하는 6개의 게임으로 구성된 벤치마크로 출시되었으며, 모든 프론티어 모델은 20% 미만의 점수를 받았습니다.
*   작은 "System One" 컴퓨터 사용 모델 제품군의 첫 번째인 CUA-S1-FORMS가 오픈소스화되었습니다.
*   Grok Voice Transcribe 2.0이 음성 종료 후 0.49초 만에 스트리밍 최종 전사에서 2.7% WER에 도달하여 이전 버전의 3.9%에서 개선되었습니다.
*   H3 Max Lip Sync가 출시되어 자체 평가에서 속도와 품질 모두에서 1위를 차지했으며, 중앙값 생성 시간은 11초를 기록했습니다.
*   GPT-6 Astra는 Roboflow가 테스트한 가장 강력한 비전 모델로 보고되었으며, "고노력" 설정에서 mAP@50 83.6%의 탐지 정확도를 보였습니다.

### 🛠️ 제품 & 도구
*   Braintrust는 Jev를 평가 모델로 통합하여 채점 비용을 약 400배 절감했습니다.
*   Box는 Jev를 사고 보고서 에스컬레이션 경로 분류에 시연했습니다.
*   LangChain + Jev를 사용한 브라우저 사용이 시연되었으며, 위키피디아 게임 및 구조화된 워크플로우에서 강력함을 보였습니다.
*   Cline은 Jev에 브라우저를 제공하는 플러그인을 출시했습니다.
*   Claude Code v2.1.277은 CLAUDE.md가 없을 때 AGENTS.md를 확인하는 기능을 추가하여 AGENTS.md를 새로운 표준으로 인정했습니다.
*   SAIRfoundation은 연구 커뮤니티에 의해 형성된 수학을 위한 오픈 모델과 툴을 제안하는 Open Math Model을 출시했습니다.
*   Roboflow는 Auto Annotate에 GPT-6 Astra를 통합했습니다.

### 🔬 연구 & 논문
*   "An Empirical Study of Harness Design for Coding Agents" 논문은 벤치마크 결과가 기본 모델뿐만 아니라 하네스 구조, 컨텍스트 설정, 턴 예산, 툴 어포던스에 의해 형성됨을 강조했습니다.
*   ProgramAsWeights는 개발자가 AI 함수를 영어로 지정하고 컴파일한 다음, Wi-Fi 없이 CPU에서 작은 신경망 프로그램을 로컬로 실행하는 방식을 설명하며 코드와 모델을 공개했습니다.

### 💰 산업 동향
*   OpenAI는 내부 레포 침입 연구원에게 $6,500의 버그 바운티를 지급했습니다.

### ⚡ 인프라 & 하드웨어
*   대규모 디퓨전 LLM 학습을 위한 오픈소스 라이브러리인 Turbo-dLLM이 출시되었으며, Context-Sharded Block Parallelism을 통해 8x H100에서 1M 컨텍스트에서 최대 7.59배의 속도 향상을 보고했습니다.
*   DeepSeek V4.1 Flash는 컨텍스트를 1M 토큰으로 확장한 후 품질이 급격히 향상되었습니다.
*   ABC 및 ABC-130K 오픈 로봇 공학 데이터셋이 출시되었습니다. ABC-130K는 3,500시간, 130K+ 에피소드, 195개 작업을 포함하는 현재까지 가장 큰 오픈 텔레옵 데이터셋입니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
