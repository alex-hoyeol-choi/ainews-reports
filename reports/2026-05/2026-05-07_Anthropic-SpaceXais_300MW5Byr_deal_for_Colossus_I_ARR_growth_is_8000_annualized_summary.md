# Anthropic-SpaceXai's 300MW/$5B/yr deal for Colossus I, ARR growth is 8000% annualized - 요약

**원문 URL**: https://www.latent.space/p/ainews-anthropic-spacexais-300mw5byr
**번역일**: 2026-05-07 06:19
**발행일**: 2026-05-07

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 브리핑입니다.

### 🔥 주요 뉴스
**[Anthropic, SpaceX와 컴퓨팅 파트너십 체결 및 Claude 용량 대폭 증대 발표]** — Anthropic은 SpaceX와의 컴퓨팅 파트너십을 통해 Claude 제품의 용량을 "상당히 증가"시킬 것이라고 발표했습니다. 이 계약으로 Claude 인퍼런스는 "며칠 내로" SpaceX의 Colossus 1에서 증강될 예정입니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/d591a434-a112-4fb9-829a-30ff2e4efbf5_2260x1442.png)
![](https://substack-post-media.s3.amazonaws.com/public/images/1a49129f-2c6b-4bd5-bcbb-aa397b2627218_1072x1064.png)
**[OpenAI, 대규모 AI 학습 클러스터를 위한 오픈 네트워킹 프로토콜 MRC 출시]** — OpenAI는 대규모 AI 학습 클러스터의 네트워킹 병목 현상을 해결하기 위해 MRC(Multipath Reliable Connection) 프로토콜을 공개했습니다. 이 프로토콜은 이미 OpenAI의 가장 큰 슈퍼컴퓨터에 배포되었습니다.
**[Perplexity, 자체 인퍼런스 엔진 ROSE 구축 및 CuTeDSL 활용]** — Perplexity는 임베딩부터 조 단위 파라미터 LLM까지 지원하는 자체 인퍼런스 엔진 ROSE를 개발했다고 밝혔습니다. Hopper 및 Blackwell 아키텍처에서 특수 커널 개발을 가속화하기 위해 CuTeDSL을 사용합니다.
**[Zyphra, 10억 미만 파라미터 추론 MoE 모델 ZAYA1-8B 오픈 웨이트로 공개]** — Zyphra는 10억 미만의 활성 파라미터를 가진 추론 MoE 모델인 ZAYA1-8B를 Apache 2.0 라이선스로 출시했습니다. 이 모델은 강력한 수학 및 추론 효율성을 통해 훨씬 더 큰 시스템에 근접한다고 주장합니다.
**[Cognition, AI 생성 코드 검토를 위한 Devin Review 및 Quick Review/SWE-Check 출시]** — Cognition은 Windsurf 2.0에 Devin Review 및 Quick Review / SWE-Check 기능을 도입하여 AI 생성 코드 검토라는 새로운 병목 현상을 명시적으로 해결하고자 합니다.

### 📊 모델 & 벤치마크
*   **ProgramBench 출시** — 언어 모델이 처음부터 프로그램을 재구축할 수 있는지 평가하는 새로운 벤치마크 ProgramBench가 공개되었습니다.
*   **Terminal-Bench 2.1 업데이트** — TB2.0의 89개 작업 중 28개가 패치된 Terminal-Bench 2.1이 출시되었으며, 에이전트 벤치마크 유지보수의 중요성을 강조합니다.
*   **OBLIQ-Bench 공개** — 대규모 코퍼스에서 미묘하게 관련 있는 문서를 찾아내지 못하는 현재 리트리버의 한계를 다루는 1단계 리트리벌에 초점을 맞춘 새로운 IR 벤치마크 OBLIQ-Bench가 등장했습니다.
*   **Harvey, 장기 법률 에이전트 벤치마크 LAB 출시** — Harvey는 24개 실무 분야에 걸쳐 1,200개 작업을 다루는 오픈소스 장기 법률 에이전트 벤치마크 LAB을 발표했습니다.
*   **Google Gemma 4, Code Arena 오픈 모델 순위 상승** — Google의 Gemma 4 모델이 Code Arena에서 오픈 모델 파레토 프론티어를 이동시켰습니다. Gemma-4-31B는 #13위, Gemma-4-26B-A4B는 오픈 모델 중 #17위를 차지했습니다.
*   **Google Gemma-4용 DFlash 드래프트 모델 공개** — Google은 Gemma-4용 DFlash 드래프트 모델을 학습시킨 최고의 드래프트 모델 중 하나로 설명했으며, 특히 코딩과 수학 분야에서 강력한 성능을 보입니다.
*   **Qwopus3.6-35B-A3B-v1, 소비자 하드웨어에서 고성능 주장** — Qwopus3.6-35B-A3B-v1은 단일 RTX 5090에서 162 tok/s를 달성했다고 주장하며, 소비자 하드웨어에서 강력한 원샷 프론트엔드/웹 생성을 목표로 합니다.

### 🛠️ 제품 & 도구
*   **Anthropic Claude Code 사용량 제한 및 Opus API 속도 제한 대폭 상향** — Anthropic은 Pro, Max, Team 및 좌석 기반 Enterprise 사용자를 위한 Claude Code의 5시간 속도 제한을 두 배로 늘렸습니다. 또한 Pro 및 Max의 피크 시간 제한 감소를 제거하고 Opus 모델의 API 속도 제한을 상당히 증가시켰습니다.
*   **Anthropic, Claude Managed Agents를 위한 Dreaming 및 Outcomes 기능 공개** — Anthropic은 에이전트 플랫폼 야망을 강조하며 메모리/세션 간 컨텍스트를 위한 Dreaming과 루브릭/채점/목표 추적을 위한 Outcomes 기능을 선보였습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/410c6b30-1820-4dd4-b5b7-5bcaeb548a03_1790x990.png)
![](https://substack-post-media.s3.amazonaws.com/public/images/339addf2-fd81-4049-8f51-9042943b2fe5_1358x846.png)
*   **Cursor, 컨텍스트 사용량 분석 기능 추가** — Cursor는 규칙, 스킬, MCP 및 서브 에이전트 전반의 컨텍스트 사용량 분석을 추가하여 컨텍스트 문제 디버깅을 돕습니다.
*   **OpenAI, Codex 서브 에이전트 홍보** — OpenAI는 전문 에이전트 간에 작업을 분할하고 결과를 하나의 답변으로 병합하는 방법으로 Codex 서브 에이전트를 소개했습니다.
*   **Perplexity, Agent API에 Finance Search 추가** — Perplexity는 라이선스 데이터, 실시간 시장 데이터 및 인용을 포함하는 Finance Search를 Agent API에 통합했습니다.
*   **Google Gemini API, File Search에 멀티모달 리트리벌 기능 추가** — Google의 Gemini API는 단일 리트리벌 파이프라인에서 PDF 및 이미지를 위한 gemini-embedding-2를 사용하여 File Search에 멀티모달 리트리벌을 도입했습니다.
*   **HeadVis, 어텐션 헤드 연구를 위한 새로운 해석 가능성 도구 출시** — HeadVis는 어텐션 헤드를 연구하기 위한 새로운 해석 가능성 도구로 소개되었습니다.

### 🔬 연구 & 논문
*   **Genesis AI, 로봇 공학 네이티브 파운데이션 모델 GENE-26.5 소개** — Genesis AI는 언어, 비전, 고유수용성 감각, 촉각 및 행동 전반에 걸쳐 학습되는 로봇 공학 네이티브 파운데이션 모델 GENE-26.5를 공개했습니다.
*   **Meta FAIR, NeuroAI용 통합 벤치마크 프레임워크 NeuralBench 출시** — Meta FAIR은 36개의 EEG 작업과 94개의 데이터셋을 포함하는 MIT 라이선스 통합 벤치마크 프레임워크 NeuralBench를 NeuroAI용으로 발표했습니다.
*   **Sander Dieleman, 플로우 맵 및 확산 모델의 적분 학습에 대한 기술 게시물 발표** — Sander Dieleman은 플로우 맵, 더 빠른 샘플링을 위한 확산 모델의 적분 학습 및 관련 기술에 대한 심층적인 기술 게시물을 공개했습니다.
*   **François Fleuret, 강력한 시스템을 위한 추측성 레시피 제시** — François Fleuret는 잠재 확산과 유사한 추론, 실제 순환 상태, 월드 모델 사전-사전 학습을 포함하는 더 강력한 시스템을 위한 추측성 레시피를 스케치했습니다.
*   **Microsoft Research, 에이전트가 읽을 수 있는 해석 가능성 연구 "Agentic-imodels" 제안** — Microsoft Research는 코딩 에이전트가 다른 LLM에 해석 가능한 모델을 진화시키는 "Agentic-imodels"를 제안하며, 65개 테이블형 데이터셋에서 성능 향상을 보고했습니다.

### 💰 산업 동향
*   **Anthropic, 연간 8000%의 ARR 성장률 발표** — Anthropic은 지난 6개월간 80배의 놀라운 성장률을 기록하며 연간 8000%의 ARR(연간 반복 매출) 성장을 달성했다고 밝혔습니다.
*   **Anthropic-SpaceX 컴퓨팅 파트너십, 연간 약 50억 달러 규모로 추정** — Anthropic과 SpaceX 간의 컴퓨팅 계약은 일부에서 연간 약 50억 달러 규모로 추정되며, xAI를 Anthropic의 새로운 클라우드 제공업체로 만듭니다.
*   **DeepSeek, 450억 달러 기업 가치 목표로 자금 조달 논의 중** — DeepSeek은 주요 중국 국영 반도체 펀드가 주도하는 450억 달러의 기업 가치를 목표로 자금 조달을 논의 중인 것으로 알려졌습니다.

### ⚡ 인프라 & 하드웨어
*   **Perplexity, Hopper 및 Blackwell에서 CuTeDSL을 활용한 커널 개발 가속화** — Perplexity는 자체 인퍼런스 엔진 ROSE 개발 과정에서 Hopper 및 Blackwell 아키텍처에서 특수 커널 개발을 가속화하기 위해 CuTeDSL을 사용한다고 밝혔습니다.
*   **vLLM + Mooncake, 에이전틱 워크로드에서 강력한 시스템 결과 발표** — vLLM과 Mooncake는 재사용 가능한 프리픽스를 사용하는 에이전틱 워크로드에서 3.8배 처리량, 46배 낮은 P50 TTFT, 8.6배 낮은 엔드투엔드 레이턴시 등 강력한 성능 개선을 시연했습니다.
*   **Unsloth + NVIDIA, 홈 GPU LLM 학습 최적화 발표** — Unsloth와 NVIDIA는 팩 시퀀스 메타데이터 캐싱, 더블 버퍼 체크포인트 재로드, 더 빠른 MoE 라우팅 등 세 가지 학습 최적화를 통해 홈 GPU LLM 학습을 약 25% 더 빠르게 만들었다고 주장합니다.
*   **NVIDIA 연구, RL 내 무손실 추측 디코딩으로 성능 향상** — NVIDIA 연구는 정책 분포를 변경하지 않고 235B 규모에서 최대 약 2.5배 빠른 엔드투엔드 RL, 8B에서 약 1.8배 빠른 롤아웃 처리량을 제공하는 무손실 추측 디코딩 기술을 강조했습니다.
*   **Baseten, 클로즈드 웨이트 랩을 위한 Frontier Gateway 출시** — Baseten은 클로즈드 웨이트 랩을 위한 관리형 인프라, API, 인증, 속도 제한 및 빌링을 제공하는 Frontier Gateway를 출시했습니다.
*   **Poolside, Laguna XS.2 및 M.1의 빠른 프로덕션 전환 보고** — Poolside는 Laguna XS.2가 P50 TTFT 146ms, Laguna M.1이 605ms를 달성하며 7주 만에 시작부터 프로덕션까지 진행되었다고 보고했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
