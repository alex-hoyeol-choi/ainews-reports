# not much happened today - 요약

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-07e
**번역일**: 2026-06-30 06:51
**발행일**: 2026-06-30

---

### 🔥 주요 뉴스
*   **Meta의 Brain2Qwerty v2 발표:** Meta는 비침습적 뇌 신호로부터 실시간으로 단어와 의미를 디코딩하는 Brain2Qwerty v2를 공개했습니다. 이 시스템은 이전 비침습적 결과 대비 78%의 단어 정확도를 달성하며 침습적 BCI와의 격차를 좁혔습니다.
*   **Cursor, iOS 및 원격 에이전트 출시:** Cursor는 iOS 앱과 항상 켜져 있는 클라우드 에이전트를 출시하여, 사용자가 휴대폰에서 컴퓨터의 에이전트를 원격으로 제어하고 PR diff 검토 및 알림을 받을 수 있도록 지원합니다. 이는 모바일 환경에서 AI 코딩 에이전트의 활용도를 크게 확장합니다.
*   **DeepSeek, DSpark 인퍼런스 시스템 공개:** DeepSeek은 추측 디코딩(speculative decoding)의 효율성을 높인 DSpark를 발표했습니다. DSpark는 Qwen3-4B에서 Eagle3 대비 30.9% 더 높은 수용 길이를 달성하며, 새로운 SOTA 단일 GPU 추측 디코딩 경로로 평가받고 있습니다.
*   **Snowflake Arctic RL, 성능 및 벤치마크 공개:** Snowflake는 VeRL 및 SkyRL과 통합되는 오픈소스 RL 프로젝트 Arctic RL을 출시했습니다. 이 프로젝트는 최대 6배의 액터 업데이트 가속과 3.5배의 엔드투엔드 속도 향상을 제공하며, Arctic-Text2SQL-R2가 엔터프라이즈 SQL 벤치마크에서 Gemini 3.1 Pro 및 Claude 4.7을 능가한다고 주장합니다.
*   **Arena, $100M ARR 달성:** AI 모델 평가 플랫폼 Arena는 제품 출시 8개월 만에 연간 반복 매출(ARR) 실행률 $100M에 도달했습니다. 이 플랫폼은 7억 건 이상의 대화와 8천2백만 건 이상의 투표를 기록하며, 배포 후(post-deployment) 및 에이전트 평가를 강조하고 있습니다.

### 📊 모델 & 벤치마크
*   Snowflake Arctic RL은 ZoRRo를 통해 최대 6배의 액터 업데이트 가속과 3.5배의 엔드투엔드 속도 향상을 제공하며, 32개의 H200에서 Text2SQL 학습 실행 시간을 약 5일에서 약 36시간으로 단축합니다.
*   Snowflake Arctic-Text2SQL-R2는 엔터프라이즈 SQL 벤치마크에서 Gemini 3.1 Pro 및 Claude 4.7의 테스트된 구성을 능가했다고 주장하며, text-to-SQL 및 멀티홉 QA를 위한 오픈 레시피를 제공합니다.
*   DeepSeek의 DSpark는 Qwen3-4B에서 Eagle3 대비 30.9%, DFlash 대비 16.3% 더 높은 수용 길이(accepted length)를 보고하며, DeepSeek-V4-Flash 및 V4-Pro의 프리뷰 엔진에 프로덕션 배포되었습니다.
*   Meituan은 총 1.6T / 활성 약 48B, 1M 컨텍스트, 35T 학습 토큰, n-그램 임베딩, 희소 어텐션(sparse attention)을 특징으로 하는 LongCat 2.0 / Owl Alpha 모델을 출시할 예정입니다.
*   Nemotron-TwoTower는 AR LLM을 확산 스타일 병렬 생성기(diffusion-style parallel generator)로 복제하여 30B 모델에 대해 2.42배의 처리량으로 98.7%의 AR 품질을 달성한다고 주장합니다.
*   GLM-5.2 753B (IQ1_S) 모델이 Unsloth 동적 IQ1_S 양자화를 사용하여 2개의 M5 Max 시스템에서 완전 로컬로 실행되어 약 16 tok/s의 생성 속도를 달성했습니다.
*   M3 Ultra Studio 256GB + M3 Max MBP 128GB에서 GLM-5.2-UD-IQ4_XS를 실행하는 llama.cpp RPC 스타일 벤치마크에서 2,377 컨텍스트 토큰에서 TTFT 3.09초로 13.03 tok/s를 기록했습니다.

### 🛠️ 제품 & 도구
*   Cursor는 iOS 앱과 항상 켜져 있는 클라우드 에이전트를 출시하여, 사용자가 휴대폰에서 컴퓨터의 에이전트를 원격으로 제어하고 앱 내에서 PR diff 검토 및 알림을 받을 수 있도록 지원합니다.
*   Cognition은 "Fable 수준"의 품질을 유지하면서 35% 비용 절감을 주장하는 하이브리드 모델 코딩 하네스인 Devin Fusion을 출시했습니다.
*   W&B는 W&B 내부에 자동 연구 에이전트(autoresearch agent)인 ARIA를 출시했습니다.
*   Agenticin은 마이크로 에이전트 라우팅(Micro-Agent routing) 기능을 홍보했습니다.
*   LlamaIndex는 하나의 에이전트 루프에서 시맨틱 검색, grep, 파일 목록화, 파일 읽기를 결합한 리트리벌 하네스(Retrieval Harness)를 소개했습니다.
*   ndstudio의 Rampart는 데이터가 클라이언트를 떠나기 전에 PII(개인 식별 정보)를 수정하는 14.7MB 브라우저 측 모델을 출시했습니다.
*   Azure Foundry에서 Claude Opus 4.8 및 Haiku 4.5가 GA(General Availability)되어, 고객이 Azure ID, 청구, 거버넌스 제어, 프롬프트 캐싱 및 사고 지원을 통해 Claude 모델을 실행할 수 있게 되었습니다.
*   Trace Judge 모델이 클로즈드 모델 비용의 약 1/100로 궤적 오류(trajectory errors)를 감지하는 평가 도구로 발표되었습니다.

### 🔬 연구 & 논문
*   Meta는 비침습적 기록으로부터 실시간으로 단어와 의미를 디코딩하는 Brain2Qwerty v2 시스템을 발표했으며, 이전 비침습적 결과에서 전체적으로 약 61%의 단어 정확도, 최고의 참가자의 경우 78%로 향상되었다고 밝혔습니다.
*   Meta는 Brain2Qwerty v1/v2의 학습 코드를 공개하고 BCBL이 v1 데이터셋을 공개할 예정입니다.
*   DeepSeek의 DSpark는 더 나은 초안 생성(draft generation)과 더 스마트한 검증 스케줄링(verification scheduling)에 중점을 둔 추측 디코딩(speculative decoding)의 중요한 단계로 소개되었습니다.
*   코딩 에이전트가 구동하는 Auto Research 워크플로우가 표준 HPO(하이퍼파라미터 최적화)를 넘어 단어 오류율을 줄이는 개선 사항을 발견하고 구현했다는 연구 결과가 Meta에 의해 언급되었습니다.

### 💰 산업 동향
*   Arena는 평가 제품 출시 8개월 만에 연간 반복 매출(ARR) 실행률 $100M에 도달했습니다.
*   Cline은 GLM 5.2, DeepSeek, Kimi, MiniMax, Qwen 등 모델에 대한 할인된 접근을 제공하는 월 $9.99 패스를 출시하여 오픈 웨이트 모델 접근을 제품화했습니다.
*   오픈소스 지지자들은 프론티어 API에 대한 단속이 개발자들을 그들이 통제하는 웨이트(weights)로 밀어붙여 역효과를 낼 수 있다고 주장했습니다.

### ⚡ 인프라 & 하드웨어
*   vLLM은 단일 OpenAI 호환 엔드포인트 뒤에 4개의 DGX Spark 박스로 Nemotron-3-Ultra 550B를 서빙하는 가이드를 강조하며, 프라이빗, 다중 노드 프론티어급 인퍼런스를 일반화하는 방법을 제시했습니다.
*   GLM-5.2 753B (IQ1_S) 모델이 llama.cpp RPC를 사용하여 단일 Thunderbolt 5 링크를 통해 각각 128GB의 통합 메모리를 가진 2개의 M5 Max 시스템에 웨이트를 샤딩하여 완전 로컬로 실행되었습니다.
*   Meituan의 LongCat 2.0 / Owl Alpha 모델은 5만 개의 중국 가속기에서 학습될 예정이며, 이는 국내 중국 하드웨어에서 이 규모로 학습된 잠재적으로 첫 번째 준-프론티어 모델로 평가됩니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
