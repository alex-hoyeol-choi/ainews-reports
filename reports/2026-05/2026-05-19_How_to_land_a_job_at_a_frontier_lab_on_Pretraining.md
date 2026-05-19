# How to land a job at a frontier lab (on Pretraining)

**원문 URL**: https://www.latent.space/p/ainews-how-to-land-a-job-at-a-frontier
**번역일**: 2026-05-19 12:19
**발행일**: 2026-05-19

---

[AINews] 프론티어 랩에 취업하는 방법 (사전 학습에 대하여)

### Google I/O를 하루 앞두고, 주목할 만한 블로그 게시물을 더 자세히 살펴볼 수 있게 되었습니다.
ShareGoogle I/O를 하루 앞둔 날입니다. 다음 주요 Gemini 릴리스가 미리 공개될 것으로 예상됩니다. 경쟁사들은 아마 조용한 한 주를 보낼 것입니다. 비록 Anthropic과 OpenAI가 오늘 각각 작은 성과를 거두었지만, Cursor는 합성 데이터/보상 해킹 및 Muon을 사용한 계속된 사전 학습에 대한 좋은 세부 정보와 함께 첫 번째 SpaceXAI 모델을 출시했습니다. 하지만 오늘 가장 오래 기억될 만한 주요 기사 후보는 Vlad Feinberg의 (이해할 수 있게도 Google/TPU 중심적인) 취업 준비, 특히 사전 학습에 대한 노트일 것입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/2e69d902-834c-41e83b07223f_1194x604.png)
특히 그는 작년 DeepMind의 Scaling handbook을 언급하며, 커널 작업이 중요한 부분이라고 말합니다.
> 모든 LLM 작업에서 가장 큰 병목 현상이자 가장 내부적인 루프는 LLM에 대한 추상적이고 논리적인 변경 사항을 실제로 실행 가능하게 만드는 성능 작업입니다. 모든 프로젝트에는 커널 수준에서 LLM을 튜닝할 수 있는 사람이 필요합니다. 이는 습득할 수 있는 기술이며, 랩으로 진입하는 가장 직접적인 경로입니다.
커널 개발을 위한 DSL에 대한 의외의 언급이 있습니다. 이에 대한 간결한 역사는 다음과 같습니다.

![X avatar for @yaroslavvb](https://pbs.substack.com/profile_images/917082138322788357/EBmj86nx.jpg)
스택의 이 수준에 있는 사람에게는 놀랍게도 그는 자동 연구(autoresearch) 및 AlphaEvolve와 같은 에이전트 작업(Agent Work)도 언급합니다. 그는 놀랍도록 간단한 연습 과제로 마무리합니다.

![X avatar for @swyx](https://pbs.substack.com/profile_images/1867875781676007424/RIF4Kt7U.jpg)
하지만 실제 채용 테스트는 다음 단락에 있습니다.
- 이를 위한 Chinchilla 법칙을 도출하십시오. 밀집(dense) 아키텍처와 MoE 아키텍처에서 어떻게 다른지 확인하십시오. 진정한 학습 경험을 원한다면 jax로 솔루션을 처음부터 직접 코딩하십시오.
- 다음으로, MoE 레이어에 jax.lax.ragged_dot을 사용했다고 가정하고, F > D에 대해 ragged dot보다 뛰어난 pallas 커널을 up/down 프로젝션을 융합하여 작성하십시오. 측정 가능한 순방향 패스 속도 향상을 발견하고 그 이유를 설명할 수 있는 설정을 찾으십시오.
이 내용을 커뮤니티의 다른 사람들에게 가르칠 수 있다면, 워크숍 연사로 모시고 싶습니다.
> 2026년 5월 16일-5월 18일 AI 뉴스. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
코딩 에이전트, 에이전트 운영, 그리고 채팅에서 자동화로의 전환
- 에이전트 인프라는 관측 가능성(observability) + 자동화 루프로 수렴하고 있습니다: 여러 게시물에서 프로덕션 에이전트를 위한 스택이 성숙해지고 있음을 지적합니다. LangSmith Engine은 에이전트를 위한 누락된 CI/CD 루프로서, 프로덕션 트레이스에서 실패를 자동으로 감지하고, 문제를 클러스터링하며, 수정/평가를 초안 작성하는 것으로 설명됩니다. LangChain은 또한 대규모 트레이스에 대한 낮은 레이턴시 쿼리 및 자체 호스팅/멀티 클라우드 요구 사항을 갖춘 에이전트 관측 가능성/평가 워크로드를 위한 특수 목적 데이터 레이어인 SmithDB를 강조했습니다 @krishdpi, @LangChain. 이와 동시에, Cognition은 Devin Auto-Triage를 출시하여, 장기 기억, 관리자/하위 에이전트 구조 및 PR 생성을 갖춘 버그, 경고 및 사고에 대한 상시 작동하는 "첫 번째 대응자"로 자리매김했습니다. Modal과 같은 초기 사용자들은 이를 일반적인 자체 개발 트리아지 자동화보다 더 유용하다고 설명합니다 @cognition, @walden_yan, @russelljkaplan. 공통적인 패턴은 "에이전트와 채팅"하는 것보다 트레이스, 메모리 및 평가에 묶인 지속적인 자동화에 가깝습니다.
- 코딩 에이전트를 위한 운영 패턴이 더욱 구체화되고 있습니다: Anthropic은 수백만 라인 규모의 모노레포, 레거시 시스템 및 마이크로서비스 전반에서 Claude Code를 실행하기 위한 모범 사례를 발표했으며, 프롬프트 캐시 진단을 추가하고 낮은 레이턴시 코딩 워크플로우를 위해 Fast 모드를 Opus 4.7으로 기본 설정했습니다 @ClaudeDevs, @ClaudeDevs, @ClaudeDevs. OpenAI는 Zoom 플러그인, 모바일/데스크톱 원격 실행, 그리고 "Mac을 깨어 있게 유지" 지원을 통해 Codex 워크플로우를 확장하여, 장시간 실행되는 작업이 휴대폰 앱에서 계속될 수 있도록 했습니다 @coreyching, @OpenAIDevs. Microsoft는 GitHub Copilot CLI 및 VS Code용 원격 제어를 GA(General Availability)로 전환했습니다 @code. 이 모든 것을 통해 제품 방향은 명확합니다: 단순히 대화형 완성(interactive completions)이 아니라 백그라운드 실행, 원격 감독 및 에이전트 팬아웃입니다.
- 실무자들은 동일한 정신 모델로 수렴하고 있습니다: 제약, 검증, 분해. François Chollet이 코딩 에이전트를 신중하게 배치된 검증 가능한 제약이 필요한 "눈먼 다람쥐"로 비유한 것은 하네스 중심 엔지니어링으로의 광범위한 전환과 간결하게 일치합니다 @fchollet. 관련 조언으로는 Python/ML 코드에서 assert를 많이 사용하여 빠르게 실패하도록 하는 것 @gabriberton, 장시간 실행되는 에이전트를 위해 종단 간(end-to-end) 및 점진적(incremental) 평가를 모두 구축하는 것 @palashshah, 그리고 에이전트 수를 조기에 최대화하기보다는 다중 에이전트 시스템을 단계별 성숙도 수준으로 구성하는 것이 포함됩니다 @shannholmberg. 실질적인 합의는 다음과 같습니다: 에이전트 품질은 프롬프트의 기발함(cleverness)만으로는 부족하며, 검증 표면, 분해 및 피드백 루프에 더 많이 의존합니다.
모델 릴리스, 순위 변화, 그리고 프론티어 코딩 모델
- 이번 배치에서 Cursor의 Composer 2.5는 단연 돋보이는 모델 출시입니다: Cursor는 Composer 2.5를 현재까지 가장 강력한 모델로 발표하며, 장시간 작업에 대한 더 나은 지속적인 작업과 더 신뢰할 수 있는 지시 따르기를 강조했습니다. 이어서 더 깊은 전략적 움직임을 공개했습니다: "SpaceXAI"를 사용하여 10배 더 많은 총 컴퓨팅과 Colossus 2의 백만 H100 등가물에 대한 접근 권한으로 훨씬 더 큰 모델을 처음부터 학습시키는 것입니다 @cursor_ai, @cursor_ai. 커뮤니티 반응은 모델의 효율성/비용-성능 프로필과 강력한 코딩 품질에 집중되었으며, 사용자들은 이를 Composer 2보다 훨씬 발전한 모델이라고 평가하고, 단순히 원시 벤치마크 성능 향상뿐만 아니라 메시지/업데이트에서 더 나은 협업 동작을 언급했습니다 @mntruell, @jonas_nelle, @kimmonismus.
- Alibaba의 Qwen 라인이 계속해서 순위를 올리고 있습니다: Qwen3.7 Preview는 Arena에 출시되었으며, Qwen3.7 Max Preview는 텍스트 부문 전체 13위(수학 7위, 전문가 9위, 소프트웨어 및 IT 9위, 코딩 10위 포함)를 차지했습니다. Qwen3.7 Plus Preview는 비전 부문 전체 16위에 도달하여, Arena 집계에 따르면 Alibaba는 텍스트 부문 6위, 비전 부문 5위 랩이 되었습니다 @arena, @Alibaba_Qwen. 이는 헤드라인 채팅 벤치마크뿐만 아니라 일반 및 전문 분야 모두에서 중국 랩들이 꾸준히 개선되고 있다는 광범위한 추세를 강화합니다.
- 메가 프론티어 아래에서 오픈 모델 및 멀티모달 릴리스가 계속되고 있습니다: ByteDance는 이미지/비디오 이해, 생성 및 편집을 위한 통합 멀티모달 모델로 설명되는 Lance를 오픈소스화했으며, 3B 비디오 + 3B 이미지 + 3B 디코더 구성 요소를 포함합니다 @bdsqlsz. Perplexity는 pplx-embed-0.6b의 계속 학습 변형으로 작은 오픈 다국어 ColBERT 모델을 출시했으며, MaxSim 커널 사용에 대한 노트를 함께 제공했습니다 @bo_wangbo. 이들은 프론티어 규모의 출시(launch)는 아니지만, 리트리벌 품질과 네이티브 멀티모달 통합이라는, 오픈 툴링이 여전히 중요한 두 가지 영역을 목표로 하기 때문에 기술적으로 의미가 있습니다.
인퍼런스, 배포, 그리고 로컬/엔터프라이즈 서빙
- llama.cpp에서 MTP를 통해 로컬 인퍼런스가 눈에 띄는 속도 향상을 얻었습니다: Georgi Gerganov는 llama.cpp에서 Qwen3.6 제품군에 대한 MTP 지원을 발표하며, 이를 로컬 AI의 중요한 이정표라고 불렀습니다 @ggerganov. 후속 보고서에 따르면, draft-MTP 플래그를 사용하여 A10G에서 Qwen3.6-27B dense 모델이 25 tok/s에서 45 tok/s로 (+78%) 처리량(throughput)이 크게 향상되었습니다 @victormustar. 이는 로컬 및 호스팅된 코딩/일반 어시스턴트 간의 사용성 격차를 상용 하드웨어에서 좁히기 때문에 중요합니다.
- 엔터프라이즈/온프레미스 배포 모멘텀이 여전히 강합니다: Hugging Face와 Dell은 NVIDIA B300이 탑재된 PowerEdge XE9780에 최적화된 Dell Enterprise Hub를 통해 Kimi K2.6, DeepSeek V4 Pro/Flash, GLM 5.1 및 MiniMax M2.7을 포함한 모델에 대한 원클릭 액세스를 홍보했습니다 @jeffboudier. Clement Delangue는 오픈소스 모델 기반의 온프레미스/로컬 AI가 GPU 부족에 대한 중요한 해답이 될 것이며, 비용, 레이턴시 및 안전성/데이터 제어 측면에서 이점을 가질 것이라고 주장했습니다 @ClementDelangue.
- 교차 하드웨어 인퍼런스 최적화가 더욱 정교해지고 있습니다: Zyphra는 AMD Instinct MI355X에서 종단 간 인퍼런스 벤치마크를 발표하며, Kimi K2.6, GLM 5.1 및 DeepSeek V3.2를 서빙할 때 AMD의 기준선 대비 강력한 성능 우위와 NVIDIA B200과의 격차를 좁혔다고 주장했습니다 @ZyphraAI. 이를 보완하여 Quentin Anthony는 벤치마킹이 하드웨어 한계와 현재 소프트웨어 상태를 구별해야 하는 이유에 대한 유용한 스레드를 게시하며, 많은 교차 스택 비교가 벤더 최대치, 달성 가능한 GEMM 성능 및 소프트웨어 성숙도를 혼동한다고 주장했습니다 @QuentinAnthon15. 인프라 엔지니어에게 이는 벤치마크 차트를 절대적인 진실이 아닌 스택 종속적인 스냅샷으로 취급해야 한다는 강력한 상기시켜주는 내용입니다.
연구: MoE, RL/데이터 혼합, 아키텍처 검색, 그리고 에이전트 평가
- 이번 주 여러 논문들은 더 큰 모델보다는 더 나은 학습 신호에 초점을 맞췄습니다: LeCun/Timor 등의 "On Training in Imagination" 요약은 모델 기반 RL에서 낮은 립시츠 상수(Lipschitz constants)를 가진 더 부드러운 세계/보상 모델이 오류 경계를 강화하고, 보상 모델이 종종 동적 모델보다 빠르게 스케일링되며, 많은 노이즈 있는 보상 레이블이 적은 고품질 레이블을 능가할 수 있지만, 편향된 보상은 특히 위험하다는 점을 강조했습니다 @TheTuringPost. Pedagogical RL에 대한 별도의 스레드는 올바른 추론 트레이스조차도 학생 정책에 비해 너무 놀랍다면 좋지 않은 학습 데이터가 될 수 있다고 주장했습니다. 이 방법은 특권 교사(privileged teacher)와 스파이크 인식 보상(spike-aware rewards), 그리고 놀라움 게이트 모방(surprisal-gated imitation)을 사용하여 학생이 실제로 학습할 수 있는 궤적을 생성합니다 @blc_16, @NoahZiems.
- 아키텍처 및 스케일링 연구는 여전히 매우 실용적입니다: Meta의 에이전틱 신경 아키텍처 발견(agentic neural architecture discovery)에 대한 AIRA 연구는 24시간 컴퓨팅 예산 내에서 검색을 계획 에이전트(AIRA-Compose)와 구현 에이전트(AIRA-Design)로 분할하여 350M, 1B, 3B 규모에서 Llama 3.2를 능가했기 때문에 주목을 받았습니다 @omarsar0, @dair_ai. 별도로, "Slicing and Dicing MoEs"는 2,000개 이상의 MoE LM 학습을 보고하며, 설계 공간의 대부분이 MoE 구성 노브(configuration knobs)에 대한 더 시끄러운 논의보다는 전문가 크기(expert size)와 전문가 수(expert count)로 귀결된다고 결론지었습니다 @margs_li.
- 데이터 선택/평가 방법론이 일류 연구 문제로 부상하고 있습니다: On-Policy Mix는 데이터 분포가 계속 변화함에 따라 올바른 데이터 믹스를 찾는 미해결 문제를 목표로 하며, 사전 학습, 중간 학습 및 지시 튜닝 전반에 걸쳐 적용 가능합니다 @michahu8. 평가 측면에서 Cameron Wolfe는 에이전트 평가 가이드를 발표했으며, 더 긴 Zhihu 요약은 에이전트 시대가 정적 지식이나 내부 CoT(chain-of-thought) 능력뿐만 아니라 위임 지능(delegation intelligence) — 즉, 언제 검색하고, 코딩하고, 추론하고, 도구를 호출할지 — 를 측정해야 한다고 주장했습니다 @cwolferesearch, @ZhihuFrontier. 이는 현재 제품 관행과 밀접하게 일치합니다: 어려운 부분은 텍스트 전용 추론이 아니라 점점 더 도구 선택과 검증 정책입니다.
생태계 동향: SDK, 수익 포착, 그리고 오픈 툴링
- Anthropic이 Stainless를 인수했습니다: Anthropic은 초기 API 시절부터 Anthropic SDK를 지원해 온 SDK 및 MCP 서버 플랫폼인 Stainless 인수를 발표했습니다 @AnthropicAI. 전략적으로 이는 모델 품질뿐만 아니라 개발자 인체 공학(ergonomics), SDK 생성 및 프로토콜 표면을 중심으로 한 지속적인 수직 통합을 시사합니다.
- 파운데이션 모델 제공업체 주변의 수익 집중이 증가하는 것으로 보입니다: 한 게시물은 34개 상위 AI 스타트업이 창출하는 AI 모델/애플리케이션 수익 중 Anthropic과 OpenAI의 점유율이 증가하고 있다고 주장했으며, 이는 모델 선택지가 확산되고 있음에도 불구하고 생태계가 경제적으로 통합될 수 있다는 신호입니다 @amir.
- 툴링 및 배포 큐레이션은 여전히 수요가 많습니다: The Turing Post가 vLLM, TGI, SGLang, llama.cpp, Ollama, BentoML, Kubeflow, MLflow 등을 포함한 파운데이션 모델 배포를 위한 13가지 오픈소스 도구를 정리한 게시물은 해당 세트에서 가장 실용적으로 유용한 큐레이션 게시물 중 하나였습니다 @TheTuringPost. 한편, Papers With Code는 AI 에이전트 지원 방식의 메서드 파싱, 리더보드 및 SOTA 추적을 통해 부활하고 있으며, 이는 연구 발견 가능성에 대한 새로운 초점을 강조합니다 @NielsRogge.
인기 트윗 (참여도 기준)
- Cursor의 Composer 2.5 + 더 큰 학습 추진: 가장 주목할 만하고 참여도가 높은 제품 뉴스는 Composer 2.5와 Cursor가 10배 더 많은 컴퓨팅으로 훨씬 더 큰 모델을 처음부터 학습시키고 있다는 공개였습니다 @cursor_ai, @cursor_ai.
- 개발자에게 영향을 미치는 OpenAI/Anthropic 제품 업데이트: Sam Altman은 최신 업데이트로 ChatGPT가 크게 개선되었다고 말했으며 @sama, Anthropic은 Claude Console에서 Fast 모드를 Opus 4.7로 기본 설정하고 프롬프트 캐시 진단을 출시했습니다 @ClaudeDevs, @ClaudeDevs.
- 지속적인 연구/엔지니어링 프레이밍: Richard Sutton의 "Bitter Lesson"에 대한 26단어 요약 — 컴퓨팅에 따라 확장되는 지식(예: 검색 및 학습)을 생성하는 방법에 집중 — 은 가장 많이 참여된 연구 관련 게시물 중 하나였으며, 에이전트 하네스, 검색 및 검증자 기반 시스템에 대한 이번 주 여러 주제와 공명했습니다 @RichardSSutton.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. LLM 안전성 벤치마크 및 제거 법의학

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-how-to-land-a-job-at-a-frontier&utm_source=paywall-free-trial&utm_medium=web&utm_content=198343451&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-how-to-land-a-job-at-a-frontier&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
