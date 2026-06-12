# Loopcraft: The Art of Stacking Loops - 요약

**원문 URL**: https://www.latent.space/p/ainews-loopcraft-the-art-of-stacking
**번역일**: 2026-06-12 06:51
**발행일**: 2026-06-12

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식 요약 브리핑입니다.

### 🔥 주요 뉴스
**[Anthropic Claude Fable 5 성능 저하 정책 철회]** — Anthropic은 일부 AI 연구 사용 사례에 대해 Claude Fable 5의 성능을 은밀히 저하시키려 했으나, 공개적인 반발로 하루 만에 정책을 철회했습니다. 이는 프론티어 모델의 거버넌스, 투명성, 접근성에 대한 중요한 논의를 촉발했습니다.
**[Recursive SI, 자동화된 AI 연구 시스템 공개]** — Richard Socher와 Recursive SI는 AI 연구를 위한 초기 "자동화된 개방형 발견 시스템"을 발표하며, NVIDIA SOL-ExecBench, NanoGPT Speedrun, NanoChat autoresearch 등 3가지 공개 작업에서 SOTA 결과를 달성하고 발견 사항을 오픈소스화했습니다. 이는 AI가 좁고 피드백이 높은 시스템 최적화 작업에 기여할 수 있음을 보여줍니다.
**[Microsoft Arbor, 장기 자율 연구 에이전트 공개]** — Microsoft Research는 지속적인 가설-트리 정제를 사용하는 자율 연구 에이전트 Arbor를 선보였습니다. Arbor는 6가지 연구 작업에서 Codex와 Claude Code를 능가하며, MLE-Bench Lite에서 86% Any-Medal을 달성했습니다.
**[Macrodata Labs, 로봇 공학 데이터 루프 구축을 위한 Refiner 출시]** — Guilherme Penedo, Hynek Kydlíček 등이 Macrodata Labs를 설립하고, 로봇 공학의 지저분한 멀티모달 물리 데이터 파이프라인 문제를 해결하기 위한 오픈소스 프레임워크 및 클라우드 런타임인 Refiner를 출시했습니다. 이는 로봇 공학 데이터 인프라의 핵심 병목 현상을 해결하는 데 중점을 둡니다.
**[DiffusionGemma, 4배 빠른 추론 속도 달성]** — Demis Hassabis는 다른 Gemma 4 변형보다 4배 빠르다고 설명된 DiffusionGemma를 강조했습니다. 이는 확산 모델 및 로컬 인퍼런스 분야에서 구체적인 속도 향상을 보여주는 중요한 발전입니다.

### 📊 모델 & 벤치마크
*   Anthropic Claude Fable 5는 WeirdML에서 87.8%를 기록하여, 각 작업에서 평균 70%를 넘은 첫 번째 모델이었으며, FrontierSWE에서 1위를 차지했습니다.
*   Unsloth는 정확도 손실 없이 1.4~2.2배 더 빠른 로컬 인퍼런스를 제공하는 Gemma 4 MTP GGUF를 출시했으며, 12B 모델은 6GB RAM에서 기준선 52 tok/s 대비 162 tok/s에 도달했습니다.
*   thoughtfullab은 AI가 약한 모델을 학습시키고 루프 진행 상황을 직접 측정하는 재귀적 자기 개선 평가 벤치마크인 PostTrainBench를 도입했습니다.
*   dawnsongtweets는 55개 직업에 걸쳐 1,500개 이상의 전문가 출처 작업을 포함하는 순환 벤치마크인 Agents’ Last Exam (ALE)을 도입했습니다.
*   manoelribeiro는 Cochrane 리뷰에서 가져온 9.11k 질문으로 SciConBench를 도입했으며, 프론티어 에이전트가 여전히 과학적 결론을 안정적으로 종합할 수 없음을 발견했습니다.

### 🛠️ 제품 & 도구
*   Macrodata Labs는 로봇 공학 데이터를 학습 준비 데이터셋으로 전환하기 위한 오픈소스 프레임워크 및 클라우드 런타임인 Refiner를 출시했습니다.
*   Goodfire는 선호도/DPO 데이터셋의 숨겨진 병리를 학습 전에 분석해야 한다고 주장하며 예측 데이터 디버깅을 도입했습니다.
*   AllenAI는 현대 LLM의 의존성 그래프를 추적하는 ModSleuth를 출시하여, Olmo 3이 89개 모델과 183개 데이터셋에, Nemotron 3이 273개 모델과 560개 데이터셋에 의존함을 보여주었습니다.
*   Weaviate의 Engram은 단순히 채팅 로그를 추가하는 대신 추출 → 변환 → 커밋 메모리 유지 관리 루프를 제안하며, Weaviate Playground는 이와 관련된 RAG/에이전트 데모를 패키징했습니다.
*   ClaudeDevs는 Claude Managed Agents에 예약된 배포와 환경 변수를 추가하여, 모델에 비밀을 노출하지 않고도 반복 작업과 CLI/API 인증을 가능하게 했습니다.
*   Perplexity는 "search as code" 아키텍처를 기반으로 Deep Research를 Computer 내의 기본 스킬로 통합했습니다.
*   Cognition과 imjaredz는 로컬 코딩 에이전트가 작업을 클라우드 Devin으로 오프로드할 수 있도록 /handoff를 오픈소스화했습니다.
*   Cursor는 분류기 서브에이전트가 작업을 게이팅하는 자동 검토를 신규 사용자의 기본값으로 설정하여 97%의 정확도를 주장했습니다.
*   Microsoft는 Copilot 티어 전반에 걸쳐 MAI-Code-1-Flash를 출시했습니다.
*   LangChain은 지출 한도, PII/비밀 감지, 추적 연속성, 감사 로깅을 포함하는 LangSmith LLM Gateway를 출시했습니다.

### 🔬 연구 & 논문
*   Richard Socher와 Recursive SI는 AI 연구를 위한 초기 "자동화된 개방형 발견 시스템"을 제시했으며, NVIDIA SOL-ExecBench, NanoGPT Speedrun, NanoChat autoresearch에서 SOTA 결과를 달성했습니다.
*   Microsoft Research는 지속적인 가설-트리 정제를 사용하는 자율 연구 에이전트 Arbor를 강조했으며, 6가지 연구 작업에서 Codex와 Claude Code를 능가하고 MLE-Bench Lite에서 86% Any-Medal을 달성했습니다.
*   MiniMax는 고성능 MSA 커널 라이브러리를 오픈소스화했으며, 관련 논문 출시를 지적했습니다.

### 💰 산업 동향
*   Anthropic이 일부 AI 연구 관련 사용 사례에 대해 Claude Fable 5의 성능을 은밀하게 저하시키기로 결정했다가 하루 만에 철회한 사건은 프론티어 AI R&D 접근 및 투명성에 대한 논쟁을 불러일으켰습니다.
*   Guilherme Penedo, Hynek Kydlíček 등이 로봇 공학 데이터 파이프라인 문제를 해결하기 위해 Macrodata Labs를 설립했습니다.

### ⚡ 인프라 & 하드웨어
*   Demis Hassabis는 다른 Gemma 4 변형보다 4배 빠르다고 설명된 DiffusionGemma를 강조했습니다.
*   Baseten은 1,000+ tok/s의 Diffusion-LLM 서빙을 주장하는 Inception Mercury 2를 출시했으며, 초기 사용자들은 82%의 레이턴시 감소와 90%의 비용 절감을 확인했습니다.
*   MiniMax는 고성능 MSA 커널 라이브러리를 오픈소스화했습니다.
*   Together는 M3 뒤에 있는 서빙 작업을 설명하며, KV-블록-메이저 스파스 어텐션, 페이지드 KV 캐시와의 MSA 통합, 디코드 인덱스 스코어링 최적화, 멀티모달 전처리를 GPU 워커 이전에 Rust 게이트웨이로 이동하는 등의 기술을 언급했습니다.
*   charles_irl은 FlashAttention-4 인퍼런스 개선 및 업스트림 기여에 대한 게시물을 발행하여, 성능 차이가 모델 아키텍처뿐만 아니라 엔드투엔드 서빙 스택 선택에서 발생하고 있음을 보여주었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
