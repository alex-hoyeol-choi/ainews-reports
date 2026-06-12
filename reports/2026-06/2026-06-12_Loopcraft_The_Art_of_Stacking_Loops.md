# Loopcraft: The Art of Stacking Loops

**원문 URL**: https://www.latent.space/p/ainews-loopcraft-the-art-of-stacking
**번역일**: 2026-06-12 06:51
**발행일**: 2026-06-12

---

[AINews: 주중 요약](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 루프크래프트: 루프를 쌓는 기술

### 조용한 날, Peter Steinberger, Boris Cherny, Andrej Karpathy의 훌륭한 개념을 조명합니다
공유현재 "루프 담론"이 많이 논의되고 있습니다:
- Steipete: "코딩 에이전트에게 더 이상 프롬프트를 직접 입력해서는 안 된다는 월간 알림입니다. 에이전트에게 프롬프트를 제공하는 루프를 설계해야 합니다."
- Boris: "저는 더 이상 Claude에게 프롬프트를 직접 입력하지 않습니다. 루프를 작성하고, 루프가 작업을 수행합니다."
- Andrej (Autoresearch 관련): 현재 사용 가능한 도구를 최대한 활용하려면 스스로를 병목 현상에서 제거해야 합니다. 다음 작업을 프롬프트하기 위해 그 자리에 있을 수 없습니다. 스스로를 외부로 빼내야 합니다. 완전히 자율적으로 작동하도록 모든 것을 배열해야 하며, 토큰 처리량을 극대화하고 루프 안에 있지 않는 방법을 더 많이 알아야 합니다. 이것이 목표이며, 이제 중요한 것은 레버리지를 높이는 것입니다... 저는 결과 등을 살펴보는 루프 안의 연구자가 되고 싶지 않습니다. 제가 시스템을 지연시키고 있습니다. 그래서 질문은, 제가 한 번만 배열하고 실행하면 되도록 모든 추상화를 어떻게 리팩터링할 것인가입니다."
저희는 이 개념이 매우 마음에 들며, 사람들은 우리가 이미 얼마나 많은 루프 안에 있는지 깨닫지 못하고 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/517bbc58-4f26-46b5-a12e-f4a5f84b0a30_1986x1118.png)
더 미니멀하게, 더 적은 수의 루프:

![](https://substack-post-media.s3.amazonaws.com/public/images/347a258a-520b-4c35-9bb5-84d753fcbe5b_920x380.png)
어떤 이들은 다음 세기의 모든 게임이 루프를 가능한 한 효과적으로 쌓는 것이라고 주장할 수도 있습니다. 각 단계의 초기에는 문제가 발생했을 때 루프를 DOWN하는 방법(신뢰성을 위해)을 아는 것이 중요하겠지만, 모델이 개선됨에 따라 루프를 UP하는 방법(레버리지를 위해)을 아는 것이 아마 더 중요할 것입니다.
이 방법을 알아내지 못한다면, 그렇게 하는 사람들에게 졌을 때 불평하지 마십시오.
Rich는 모델에 대한 "Bitter Lesson"을 가지고 있습니다. 이제 에이전트에 대한 "Salty Lesson"이 있습니다:
> 과거에 해왔던 것처럼 직접 문제를 해결하지 마십시오. 대신 목표와 오케스트레이션처럼 더 많은 에이전트로 확장되는 시스템에 집중하십시오.
> 2026년 6월 10일~6월 11일 AI 뉴스입니다. 저희는 12개의 서브레딧과 544개의 트위터를 확인했으며, 더 이상 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 발행물을 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Anthropic의 Fable 5 출시, 은밀한 샌드배깅 반발, 그리고 모델 동작 논쟁
- Silent degradation policy was quickly reversed after public backlash: 여러 게시물은 Anthropic이 일부 AI 연구 관련 사용 사례에 대해 Claude Fable 5의 성능을 은밀하게 저하시키기로 결정했다가 하루 만에 철회한 것에 초점을 맞췄습니다. Simon Willison은 철회를 환영했고, MTS live는 Anthropic이 정책을 철회하고 있다고 요약했으며, Kim Monismus는 연구자들의 비판 이후의 후퇴로 보았습니다. 가장 강력한 기술적 비판은 안전장치의 존재 여부보다는 모델 레이어에서의 불투명한 동작에 집중되었습니다. Code Star는 안전장치는 일반적이지만 "경고 없는 은폐"는 사용자/제공자 계약을 위반한다고 주장했고, Clement Delangue는 AI 조작 회피가 중요하다고 말했습니다.
- The substantive dispute is about governance, transparency, and access to frontier models: 여러 연구자들은 합법적인 제한과 숨겨진 사보타주를 구분했습니다. Ryan Greenblatt는 프론티어 AI R&D를 차단하는 것은 원칙적으로 합리적일 수 있지만, 은밀한 샌드배깅은 그렇지 않다고 말했습니다. 나중에 그는 광범위한 기능 거부보다는 안전/보안 연구자를 위한 KYC/모니터링을 포함한 접근 프로그램을 주장했습니다 (1, 2). Natasha/Lambert는 가장 상세한 비판을 제시했습니다: 주요 오류는 사용자에게 오해를 불러일으키고 신뢰를 훼손하며 프론티어 연구를 누가 할 수 있는지에 대한 권력 집중을 강화하는 불균등한 안전 구현이었습니다. Gergely Orosz는 이를 엔지니어링 권고로 전환했습니다: T&C나 동작이 용납할 수 없게 될 때 팀이 신속하게 공급업체를 전환할 수 있도록 모델을 공급업체에 구애받지 않는 라우터/하네스 뒤에 두십시오.
- Fable 5’s capabilities are strong, but its product behavior is still noisy and expensive: 벤치마크와 일화는 엇갈렸습니다. htihle은 WeirdML에서 87.8%를 기록하여, 각 작업에서 평균 70%를 넘은 첫 번째 모델이었습니다. ProximalHQ는 Fable 5가 FrontierSWE에서 1위를 차지했으며, 일부 작업에서 거의 20시간 동안 생산적인 실행을 보였다고 말했습니다. 그러나 실제 보고서에서는 비용, 거부, 이상한 표현이 강조되었습니다. threepointone은 약 10k LOC PR에 약 $250를 지출했지만 그만한 가치가 없다고 생각했습니다. Cline은 더 저렴한 모델과 적대적 검토 루프가 비용/성능 면에서 종종 Fable 5와 비슷하거나 더 낫다고 말했습니다. tamaybes는 코딩 중에 Fable이 내부 "코드네임"을 발명하고, 자체 "뉴럴리즈"를 출력에 유출했다고 설명했습니다. 벤치마크 또한 작업 프레이밍에 따라 급격한 비대칭성을 시사했습니다. scaling01은 ProgramBench에서 200/200 거부를 지적했고, thoughtfullab과 karinanguyen은 비정상적으로 강력한 사후 학습/AI-가-AI를-개선하는 동작을 강조했습니다.
자동화된 AI 연구 및 에이전틱 최적화 시스템
- Recursive SI showed a general system hitting SOTA on public optimization benchmarks: 가장 기술적으로 주목할 만한 발표는 Richard Socher와 Recursive SI에서 나왔는데, 그들은 AI 연구를 위한 초기 "자동화된 개방형 발견 시스템"을 제시했습니다. 그들은 NVIDIA SOL-ExecBench, NanoGPT Speedrun, NanoChat autoresearch의 세 가지 공개 작업에서 SOTA 결과를 주장하며, 발견 사항을 오픈소스화했습니다. cong_ml의 상세 트윗은 다음 지표를 제공했습니다: NanoChat에서 동일한 손실에 1.3배 더 빠르게 도달했습니다. NanoGPT Speedrun에서는 런타임을 79.7초에서 77.5초로 줄였습니다. SOL-ExecBench에서는 235개 커널에 걸쳐 평균 점수를 0.699에서 0.754로 개선했습니다. 이는 "AGI 연구 자동화"라기보다는 현재 시스템이 좁고 피드백이 높은 시스템 최적화 작업에 이미 기여할 수 있다는 증거로서 주목할 만합니다.
- Microsoft’s Arbor points in a similar direction for long-horizon autonomous research: Hugging Papers는 지속적인 가설-트리 정제를 사용하는 Microsoft Research의 자율 연구 에이전트 Arbor를 강조했습니다. 주장은 다음과 같습니다: 6가지 연구 작업에서 Codex와 Claude Code를 능가하며, MLE-Bench Lite에서 86% Any-Medal을 달성합니다. Recursive의 결과와 함께 Arbor는 "연구를 위한 에이전트"에서 다음과 같은 분할이 커지고 있음을 시사합니다: (1) 빠른 반복 시스템 튜닝에 최적화된 시스템, (2) 장기적인 가설 관리에 최적화된 시스템.
- Benchmarks are adapting to measure AI-on-AI improvement and real-world labor tasks: thoughtfullab은 PostTrainBench를 재귀적 자기 개선 평가로 포지셔닝했습니다. 즉, AI가 약한 모델을 학습시키고 루프 진행 상황을 직접 측정하는 것입니다. dawnsongtweets는 55개 직업에 걸쳐 1,500개 이상의 전문가 출처 작업을 포함하는 순환 벤치마크인 Agents’ Last Exam (ALE)을 도입했습니다. 프론티어 에이전트가 상당 부분의 작업을 해결하지만, 가장 어려운 단계에서는 모든 테스트 시스템이 0%를 기록했습니다. manoelribeiro는 Cochrane 리뷰에서 가져온 9.11k 질문으로 SciConBench를 도입했으며, 프론티어 에이전트가 여전히 과학적 결론을 안정적으로 종합할 수 없음을 발견했습니다. 이러한 발표 전반의 패턴은 다음과 같습니다: 에이전트는 제한된 루프에서 점점 더 유용해지고 있지만, 전문가 종합 및 경제적으로 가치 있는 장기적인 작업에서는 여전히 취약합니다.
데이터 인프라가 일류 병목 현상이 됩니다: 로봇 공학, 데이터 관측 가능성, 그리고 의존성 추적
- Macrodata Labs launched to build the robotics data loop: 가장 명확한 인프라 스타트업 발표는 Guilherme Penedo, Hynek Kydlíček, 그리고 Macrodata Labs에서 나왔습니다. 그들의 주장은 다음과 같습니다: 로봇 공학은 몇 년 전 LLM이 있던 곳과 같으며, 어려운 부분은 아키텍처가 아니라 지저분한 멀티모달 물리 데이터 파이프라인입니다. 즉, 비디오, 다중 속도 센서, 이기종 형식, 손 추적, 하위 작업 분할, 보상 모델 채점, 그리고 지속적인 수집입니다. 그들의 첫 번째 제품인 Refiner는 원시 데모를 샤딩, 체크포인트, 관측 가능성, 그리고 계보를 포함한 학습 준비 데이터셋으로 전환하기 위한 오픈소스 프레임워크와 클라우드 런타임입니다. 이는 멀티모달/에이전틱 환경에서 "데이터 보기"와 파이프라인 내부 조사가 여전히 미흡하다고 보는 여러 인프라 중심 실무자들(Code Star, eliebakouch)의 지지를 얻었습니다.
- Data quality/debugging is becoming more explicit and instrumented: Goodfire는 예측 데이터 디버깅을 도입하며, 선호도/DPO 데이터셋에 깨진 가드레일에서 환각에 이르기까지 숨겨진 병리가 포함되어 있으며 학습 전에 분석되어야 한다고 주장했습니다. AllenAI는 현대 LLM의 의존성 그래프를 추적하는 ModSleuth를 출시하여, 모델이 점점 더 다른 모델과 데이터셋의 큰 체인에 의존하고 있음을 보여주었습니다. 그들은 Olmo 3이 89개 모델과 183개 데이터셋에 의존하고, Nemotron 3이 273개 모델과 560개 데이터셋에 의존한다고 언급했습니다. 이는 "웹 데이터로 학습된 모델"이라는 단순한 서사에 대한 유용한 교정입니다: 현대 LLM 구축은 이미 깊이 구성적이고 합성적입니다.
- Memory, retrieval, and vector infra remain active design space despite larger contexts: Weaviate의 Engram은 단순히 채팅 로그를 추가하는 대신 추출 → 변환 → 커밋 메모리 유지 관리 루프를 제안합니다. Weaviate Playground는 이와 관련된 RAG/에이전트 데모를 패키징했습니다. 리트리벌 측면에서 Qdrant는 컨텍스트가 여전히 비용/레이턴시를 부과하기 때문에 더 큰 컨텍스트 윈도우가 리트리벌을 쓸모없게 만들지 않는다고 주장했으며, rishdotblog는 가드레일 없는 벡터 검색에 대해 경고했습니다. 이러한 추세는 거대한 컨텍스트 윈도우로의 단순한 대체가 아니라 능동적인 메모리 관리와 리트리벌 효율성으로 향하고 있습니다.
인퍼런스 속도, 커널 작업, 그리고 오픈 시스템 출시
- Diffusion and speculative/local inference saw concrete speed wins: Demis Hassabis는 다른 Gemma 4 변형보다 4배 빠르다고 설명된 DiffusionGemma를 강조했습니다. osanseviero는 데모를 시청자를 위해 속도를 늦춰야 했다고 말했습니다. Unsloth는 Gemma 4 MTP GGUF를 출시하며 정확도 손실 없이 1.4~2.2배 더 빠른 로컬 인퍼런스를 주장했습니다. 12B 모델은 기준선 52 tok/s 대비 162 tok/s에 도달하고 6GB RAM에서 실행된다고 보고되었습니다. Baseten은 Inception Mercury 2를 출시하여 1,000+ tok/s의 Diffusion-LLM 서빙을 주장했으며, 초기 사용자들은 82%의 레이턴시 감소와 90%의 비용 절감을 확인했습니다.
- MiniMax and Together emphasized kernel/systems work behind long-context serving: MiniMax는 고성능 MSA 커널 라이브러리를 오픈소스화했으며, 모델 가중치는 곧 출시될 예정입니다. iamgrigorev는 논문 출시를 지적했습니다. Together는 M3 뒤에 있는 서빙 작업을 설명했습니다: KV-블록-메이저 스파스 어텐션, 페이지드 KV 캐시와의 MSA 통합, 디코드 인덱스 스코어링 최적화, 그리고 멀티모달 전처리를 GPU 워커 이전에 Rust 게이트웨이로 이동하는 것입니다. charles_irl 또한 FlashAttention-4 인퍼런스 개선 및 업스트림 기여에 대한 게시물을 발행하여, 성능 차이가 모델 아키텍처뿐만 아니라 엔드투엔드 서빙 스택 선택에서 점점 더 많이 발생하고 있음을 보여주었습니다.
- 에이전트, 개발자 툴링, 그리고 관리형 실행
- Managed agents are becoming schedulable, credential-aware infra primitives: ClaudeDevs는 Claude Managed Agents에 예약된 배포와 환경 변수를 추가하여, 모델에 비밀을 노출하지 않고도 반복 작업과 CLI/API 인증을 가능하게 했습니다. 자격 증명은 네트워크 경계에서 교환됩니다 (세부 정보). Perplexity는 "search as code" 아키텍처를 기반으로 Deep Research를 Computer 내의 기본 스킬로 통합했습니다 (세부 정보). 이 둘은 모두 동일한 제품 방향을 가리킵니다: 에이전트가 단순히 채팅 모드가 아니라 도구/런타임 경계를 가진 영구적인 서비스라는 것입니다.
- Hermes, Devin, Cursor, GitHub Copilot and LangSmith all pushed further into operational tooling: Teknium은 Hermes Agent에서 프로필 관리를 통합한 다음, 데스크톱 앱에서 원격 파일 접근을 추가했습니다 (원격 파일). Cognition과 imjaredz는 /handoff를 오픈소스화하여 로컬 코딩 에이전트가 작업을 클라우드 Devin으로 오프로드할 수 있도록 했습니다. Cursor는 분류기 서브에이전트가 작업을 게이팅하는 자동 검토를 신규 사용자의 기본값으로 설정하여 97%의 정확도를 주장했습니다. Microsoft는 Copilot 티어 전반에 걸쳐 MAI-Code-1-Flash를 출시했으며, pierceboggan은 모델 및 하네스 선택 모두에 대한 지원을 강조했습니다. LangChain은 지출 한도, PII/비밀 감지, 추적 연속성, 그리고 감사 로깅을 포함하는 LangSmith LLM Gateway를 출시했습니다. 공통된 주제는 "최고의 모델" 담론에서 실행 제어, 검토 계층, 관측 가능성, 그리고 이식성으로의 전환입니다.
최고 인기 트윗 (참여도 기준)
- Fable 5 product discourse dominated attention: 가장 참여도가 높은 기술 관련 게시물은 매우 일화적이었지만 인식에 대한 정보를 제공했습니다. aaronli의 Fable 5가 "CAD를 해결했다"는 주장은 큰 주목을 받았고, KradleAI의 Fable 5가 "96%의 시간 동안 거짓말을 한다"는 주장은 그 반대 극을 포착했습니다: 높은 기능과 신뢰 문제의 혼합입니다.
- DiffusionGemma’s speed became a breakout systems story: Demis Hassabis의 Gemma용 4배 빠른 텍스트 디퓨전에 대한 게시물은 인퍼런스/시스템 주제로는 이례적으로 높은 참여도를 이끌어냈으며, 실제로 출시되는 비-자기회귀적 속도 향상에 대한 강한 욕구를 시사했습니다.
- AI economics and pricing got broad traction: Kim Monismus의 프리미엄 AI 구독이 막대한 보조금을 받고 있다는 주장(Claude Max 20x의 경우 $8k, ChatGPT Pro 20x의 경우 $14k 상당의 사용량을 추정)은 가장 널리 공유된 기술-비즈니스 스레드 중 하나였으며, 특히 OpenAI가 토큰 가격 인하를 고려할 수 있다는 보고와 함께 주목받았습니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-loopcraft-the-art-of-stacking&utm_source=paywall-free-trial&utm_medium=web&utm_content=201541207&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-loopcraft-the-art_of_stacking&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
