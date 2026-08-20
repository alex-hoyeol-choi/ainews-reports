# Death of Params: Z.ai CEO Jie Tang on GLM 5.3 and the new Post-training Scaling Law - 요약

**원문 URL**: https://www.latent.space/p/ainews-death-of-params-zai-ceo-jie
**번역일**: 2026-08-20 06:05
**발행일**: 2026-08-20

---

### 🔥 주요 뉴스
**[GLM 5.3 출시 및 새로운 스케일링 패러다임 제시]** — Z.ai CEO Jie Tang 교수는 GLM 5.3을 공개하며, 모델 성능이 파라미터 수뿐 아니라 데이터, 컴퓨트 사용처, 실행 조건 등 5가지 스케일링 조절 변수에 의해 결정된다고 강조했습니다. 특히 GLM 5.3은 장기적인 RL 환경에서의 학습을 통해 크게 개선되었으며, 이 학습 환경과 평가 프로세스는 완전히 합성적으로 구성되었습니다.
![X avatar for @jietang](https://pbs.substack.com/profile_images/2969848274/9650ac94b38c2872eecea8a7dfa376ef.jpeg)
![](https://substack-post-media.s3.amazonaws.com/public/images/1b1d78e9-d676-408c-9f84-8c9f244ef898_864x1821.png)

**[Ornith-1.5 오픈 모델 패밀리 출시]** — MIT 라이선스 기반의 Ornith-1.5가 9B 덴스, 35B MoE, 397B MoE 변형으로 출시되었으며, FP8, GGUF, MLX, NVFP4를 포함한 다양한 양자화 포맷을 지원합니다. 이 모델은 엔드-투-엔드 자기 개선 기능을 특징으로 하며, Terminal-Bench 2.1에서 86.1, SWE-Bench Verified에서 86 등 에이전틱/코딩 워크로드에서 강력한 성능을 보였습니다.

**[DeepSeek Harness (DSH) 오픈 에이전트 런타임 공개]** — DeepSeek Harness는 Cordis 플러그인 아키텍처 위에 구축된 의도적으로 얇은 셸로, 에이전트 루프를 포함한 모든 것이 플러그인으로 작동하는 오픈 에이전트 런타임입니다. 이는 사용자 확장 가능한 도구, 교체 가능한 제어 루프, 비즈니스 규칙 주입에 최적화되어 있으며, 초기 베타 사용자들은 일주일도 안 되어 100개 이상의 플러그인을 출시했습니다.

**[OpenRouter, Stripe에 인수]** — 토큰 라우팅 및 마켓플레이스 서비스인 OpenRouter가 Stripe에 합류한다고 발표되었습니다. 이는 토큰 라우팅/마켓플레이스 기능이 엣지 툴링을 넘어 핵심 인프라로 자리 잡고 있음을 시사하는 중요한 산업 동향으로 평가됩니다.

**[Gemini 3.7 Flash 출시 및 벤치마크 1위 달성]** — Google의 Gemini 3.7 Flash가 Artificial Analysis의 AA-AnalystAgent 벤치마크에서 60.0% pass^5, 70.5% pass@1로 1위를 차지했습니다. 이 모델은 태스크당 평균 1.32초, 0.54달러의 비용 효율성을 보이며, Gemini chat, Spark, AI Mode 등 Google 제품에 깊이 통합되고 있습니다.

### 📊 모델 & 벤치마크
*   Z.ai의 GLM 5.3이 장기적인 RL 환경에서의 학습을 통해 크게 개선되었으며, GLM 5.2와 동일한 기본 모델/아키텍처를 기반으로 합니다.
*   Ornith-1.5가 9B 덴스, 35B MoE, 397B MoE 변형으로 MIT 라이선스 하에 출시되었으며, Terminal-Bench 2.1: 86.1, SWE-Bench Verified: 86 등 에이전틱/코딩 벤치마크에서 강력한 성능을 기록했습니다.
*   UnslothAI가 Dynamic V3를 사용하여 새로운 Qwen3.8-27B GGUF를 출시했으며, 동일한 크기에서 약 10% 더 높은 정확도를 주장하고 8GB RAM에서 1비트 양자화 모델을 실행할 수 있습니다.
*   UnslothAI는 새로운 Divergence-300 메트릭을 공개하여 Terminal Bench, DeepSWE 등에서 더 긴 생성에 걸쳐 상위 1% 그리디 정확도를 확장합니다.
*   Agent Arena의 파레토 관점 평가에서 Claude Opus 5 (High)가 품질을 선도하며, Kimi K3, GLM 5.2, Grok 4.5, GPT-5.6 Luna 등 저비용 모델들이 가치 프론티어의 상당 부분을 정의했습니다.
*   Grok 4.6이 Legal Research Bench에서 48.1%로 49개 중 3위를 차지했으며, 500k 컨텍스트, 도구/이미지/파일 지원을 제공합니다.
*   GLM 5.3이 오픈 웨이트 모델 중 Terminal Bench에서 2위, Legal Bench에서 3위, Skills Bench에서 6위를 차지했습니다.
*   Microsoft Agent Lightning v1.0이 SWE-Bench Verified에서 Qwen3.5-9B의 성능을 41.8%에서 56.4%로 향상시켰다고 보고되었습니다.
*   Google의 Gemini 3.7 Flash가 Artificial Analysis의 AA-AnalystAgent에서 60.0% pass^5, 70.5% pass@1로 1위를 차지했습니다.

### 🛠️ 제품 & 도구
*   DeepSeek Harness (DSH)가 Cordis 플러그인 아키텍처 기반의 오픈 에이전트 런타임으로 공개되었습니다.
*   TrueFoundry가 프로덕션 에이전트를 위한 MIT 라이선스, 자체 호스팅 가능, 벤더 중립적인 하네스인 TrueForge를 오픈소스화했습니다.
*   ClaudeDevs는 Claude Managed Agents에 자체 호스팅 샌드박스 메모리 지원, 웹 도구 도메인 제어, 재설계된 다중 에이전트 세션 뷰어 등 새로운 기능을 추가했습니다.
*   OpenAI는 프론티어 모델에 대한 Zero Data Retention을 유지하면서 안전 위험을 감지하는 Private Safety Processing을 도입했습니다.
*   Replit이 GPT-5.6 Luna 기반의 Free Mode를 출시하여 SOTA급 모델을 무료로 제공합니다.
*   Anthropic Claude Code에 간결한 출력 스타일이 추가되어 개발자 인체 공학이 개선되었습니다.
*   Sentence Transformers v6.0이 출시되어 단일 벡터에서 다중 벡터 리트리벌로의 전환을 반영합니다.

### 🔬 연구 & 논문
*   Z.ai CEO Jie Tang 교수는 모델 스케일링이 파라미터 수 외에 데이터 품질, 인퍼런스 컴퓨트, 포스트-트레이닝 등 5가지 조절 변수에 의해 결정된다는 새로운 스케일링 법칙을 제시했습니다.
*   GLM-5.3의 큰 도약은 완전히 합성적으로 구성된 장기적인 RL 환경에서의 학습에서 비롯되었다고 발표되었습니다.
*   Microsoft Agent Lightning v1.0은 임의의 하네스를 엔드포인트 프록시를 통해 RL에 연결하여 재토큰화, 샘플 병합 등의 문제를 처리하며, Qwen3.5-9B의 SWE-Bench Verified 성능을 41.8%에서 56.4%로 향상시켰습니다.
*   TRL에서 온-폴리시 디스틸레이션이 생성 버퍼, 배치 처리된 교사 호출 등을 통해 40배 더 빨라졌음이 입증되었습니다.
*   prl에서 RL 실행 중 진행 중인 롤아웃을 동적으로 조정하는 적응형 동시성 기능이 발표되었습니다.
*   프로덕션 에이전트 앱 10개를 계측한 연구에서 비-LLM 구성 요소가 레이턴시를 지배하며, 태스크 인식 서빙, 상태 오프로딩, 도구 결과 캐싱이 레이턴시 및 메모리 사용량을 크게 개선할 수 있음을 발견했습니다.

### 💰 산업 동향
*   OpenRouter가 Stripe에 인수되어 토큰 라우팅/마켓플레이스가 핵심 인프라로 자리 잡고 있음을 시사합니다.
*   Google은 Gemini 3.7 Flash를 Gemini chat, Spark, AI Mode, AI Studio GitHub 동기화 등 자사 제품에 깊이 통합하고 있습니다.

### ⚡ 인프라 & 하드웨어
*   Qdrant가 필터링 가능한 HNSW를 출시하여 필터링된 ANN을 쿼리 시점이 아닌 인덱스에서 처리하며, 100만 개 벡터에 대한 1% 필터 벤치마크에서 ACORN 대비 99.8%의 재현율과 1.0ms의 성능을 보였습니다.
*   turbopuffer는 Linear가 델타 동기화 읽기 경로를 Postgres에서 turbopuffer로 옮겨 가장 큰 동기화 시간을 약 8초 단축했다고 발표했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
