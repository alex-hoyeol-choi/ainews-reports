# The Field Guide to Fable

**원문 URL**: https://www.latent.space/p/ainews-the-field-guide-to-fable
**번역일**: 2026-07-07 06:09
**발행일**: 2026-07-07

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Fable 필드 가이드

### 조용한 하루는 세계에서 가장 중요한 모델 출시를 소화하게 합니다... 현재까지.
Share(쇼의 친구!) General Intuition의 새로운 모델과 (쇼의 친구!) Shunyu Yao의 새로운 모델을 축하하고, 전 세계가 GPT-5.6 Sol Ultra의 출시를 기다리는 동안, 사람들은 내일 구독 보조금이 끝나기 전에 Fable 5의 한계를 찾기 위해 경쟁하고 있습니다.
Thariq는 "Field Guide to Fable" 블로그 시리즈를 작업 중이었고, 마침 재출시 당일에 기조연설이 예정되어 있었습니다. 그래서 그는 하룻밤 만에 전체 기조연설을 변경하여 오늘 공개된 가장 시의적절한 조언을 제공했습니다.
4가지 세그먼트는 다음과 같습니다 (제 시청 코멘트는 이탤릭체):
- 0:00 Fable 소개 및 배경 설정
- 2:32 Unhobbling Claude: Understanding model behavior
모델에 대한 제약은 종종 우리, 즉 "우리가 모델에 씌우는 하네스와 프롬프트 방식"에 의해 부과됩니다. 따라서 새로운 클래스의 모델을 접할 때, 우리는 모델을 과도하게 제한하여 (일명 족쇄를 채워) 볼 수 없었던 새로운 동작을 이끌어내기 위해 이러한 하네스와 프롬프트를 제거하거나 변경해야 합니다.
예시: 대부분의 사람들은 HTML의 비합리적인 효과에 대해 Thariq의 의견에 동의하게 되었습니다.
- 9:08 Finding your unknowns: Navigating the gap between map and territory
이미 이곳에 블로그 게시됨.
"unhobbling"의 가까운 사촌 격입니다. unhobbling이 오래된 지식을 제거하는 것이라면, 이것은 자신이 알지 못했던 것을 찾는 것입니다.
가장 쉬운 기술:
Claude에게 미지의 것에 대한 "blindspot pass"를 수행하도록 지시하기
"wildly different design directions"에 대해 브레인스토밍하기
나를 인터뷰하기 - /grill-me와 유사하지만, 영향력 있는 질문에 우선순위를 두기
참조 사용: 마이그레이션의 경우
implementation-notes.md 유지: 당신을 대신하여 내려진 불완전하게 명시된 결정들의 실행 기록
나를 퀴즈하기 - 나의 이해를 확인하기
- 14:29 Dealing with Grief: Reflecting on the emotional shift in coding productivity
예전에는 몇 주가 걸리던 일이 이제는 몇 시간 만에 끝납니다.
- 16:30 Being unreasonable: Demanding good, fast, and cheap results
"Tradeoffs are not real" - Fable이 더 유능하기 때문에, 당신은 더 야심차게 행동하고 트레이드오프를 받아들이지 않을 수 있습니다.
"Building is easy, generating value is still hard".
전반적으로, 세계가 최초의 Fable-클래스 모델에 적응함에 따라 우리가 그 함의를 파악하게 될 훌륭한 강연이었습니다.
> 2026년 7월 4일-7월 6일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 추가 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 모든 지난 호를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter Recap
Tencent Hunyuan의 Hy3 출시와 오픈 웨이트 프론티어
- Hy3, 진지한 오픈 모델로 등장: Tencent는 Apache 2.0 라이선스 하에 Hy3를 발표했습니다. 이는 21B 활성 파라미터, 192개의 전문가 / top-8 라우팅, GQA, 256K 컨텍스트, 그리고 스페큘레이티브 디코딩을 위한 3.8B MTP 레이어를 갖춘 295B MoE 모델입니다. 여러 게시물에서 이 모델이 추론, 코딩, 에이전틱 작업에서 훨씬 더 큰 시스템들과 경쟁할 수 있다고 평가했으며, 특히 툴-콜링 안정성 및 환각 방지 작업과 같은 신뢰성 개선에 중점을 두었습니다 @eliebakouch, @HuggingPapers, @ShunyuYao12.
- 인퍼런스 지원이 이례적으로 출시 당일부터 성숙했습니다: @vllm_project는 Hy3가 출시와 동시에 툴-콜 및 추론 파서, MTP 스페큘레이티브 디코딩을 포함하여 vLLM에서 기본적으로 실행되며 NVIDIA 및 AMD에서 검증된 지원을 제공한다고 밝혔습니다. 후속 게시물에서는 Tencent의 프로덕션 커널이 vLLM 메인으로 업스트림되었음을 상세히 설명했습니다. 여기에는 로드 밸런싱 디코드 스케줄링 및 퓨즈드 FP8 MoE 서빙이 포함되며, 혼합 길이 디코드에서 최대 2.95배의 성능 향상과 기본 백엔드 대비 TTFT 약 24%, TPOT 약 17%의 레이턴시 감소가 보고되었습니다 @vllm_project. 커뮤니티 반응이 매우 뜨거워 @Teknium은 Hy3를 Nous Portal에서 2주간 무료로 제공했습니다.
- 더 넓은 오픈 모델 컨텍스트: Hy3는 GLM-5.2와 즉시 비교되었으며, 일부 게시자들은 벤치마크 및 바이브-테스트 결과가 유지된다면 Tencent가 이제 오픈소스 랩의 최상위 계층에 합류했다고 주장했습니다 @teortaxesTex. 반면 다른 이들은 GLM-5.2가 여전히 실제로 가장 잘 사용할 수 있는 오픈 웨이트 모델이라고 주장했습니다 @tinygrad, @mbusigin. 핵심 요약은 다음과 같습니다: 오픈 프론티어가 빠르게 압축되고 있으며, 경쟁은 단순히 순위표의 차이보다는 배포 견고성에 점점 더 초점을 맞추고 있습니다.
에이전트 벤치마크, 하네스, 그리고 장기 실행 메모리
- AutomationBench-AA, 보다 현실적인 에이전트 평가 추가: @ArtificialAnlys는 Zapier의 AutomationBench에 대한 독립적인 리더보드를 출시했습니다. 이는 657개의 작업과 40개의 시뮬레이션된 SaaS 앱에서 목표와 가드레일을 모두 사용하여 에이전트를 평가합니다. Claude Fable 5가 48.6%로 선두를 차지했으며, Opus 4.8이 48.5%로 근소하게 뒤를 이었고, Gemini 3.5 Flash가 42.6%, GPT-5.5 xhigh가 42.1%를 기록했습니다. 순위보다 더 흥미로운 점은 모든 모델이 여전히 비즈니스 규칙을 위반한다는 것과, Gemini가 목표당 가드레일 위반 및 비용 효율성 측면에서 특히 강세를 보였다는 것입니다. 오픈 웨이트 모델은 여전히 의미 있게 뒤처져 있으며, GLM-5.2 max가 27.8%로 가장 높은 순위에 있는 오픈 모델입니다.
- 역량 지수는 다차원적으로 변화하고 있습니다: Artificial Analysis는 또한 단일 스칼라 모델 점수를 넘어 금융 및 회계, 법률, 의료, 전략 및 운영, 엔지니어링, 경제학 등 6가지 도메인별 지수를 도입했습니다 @ArtificialAnlys. 헤드라인은 익숙했습니다—Claude Fable 5와 Opus 4.8 폴백이 선두를 차지했습니다—하지만 더 유용한 통찰은 도메인별로 순위가 얼마나 급격하게 재편되는지, 그리고 가격/성능 프론티어가 얼마나 가파르게 되었는지입니다. 이는 작업당 비용 없이 벤치마크 점수를 보고하는 것이 점점 더 무의미해진다고 주장한 @fchollet의 의견과 일치합니다.
- 메모리 및 리트리벌은 지속적인 에이전트의 병목 현상으로 남아있습니다: 두 편의 논문이 여기서 주목을 받았습니다. 첫째, A-TMA는 장기 실행 어시스턴트에서 오래된 사실과 현재 사실이 함께 리트리벌되는 "고스트 메모리" 문제를 다룹니다. LTP 벤치마크에서 Graphiti에 이를 추가하면 충돌 정확도가 절대값으로 +0.240 향상되는 것으로 보고되었습니다 @omarsar0. 둘째, ReContext는 답변 생성 직전에 모델 내부 증거를 재생하여 8개의 128K 데이터셋에서 증거 활용을 개선하는 학습 없는 장문 컨텍스트 인퍼런스 하네스입니다 @dair_ai. 백만 토큰 인-컨텍스트 리트리벌을 위한 BlockSearch @dair_ai와 결합하면, 더 나은 메모리 동작이 학습될 뿐만 아니라 인퍼런스 시점에 점점 더 많이 엔지니어링되고 있다는 주제가 명확해집니다.
Anthropic의 J-Space / Global Workspace 결과
- 기계적 해석 가능성이 중심에 섰습니다: Anthropic은 Claude 내부에 J-space라고 부르는 활성화의 작은 부분집합을 중심으로 하는 글로벌 워크스페이스와 유사한 내부 구조를 주장하는 연구를 발표했습니다 @AnthropicAI, @AnthropicAI. 핵심 주장은 CoT(chain-of-thought) 추출이 아니라, 보고, 변조 및 유연한 추론에 사용 가능한 특권적인 내부 표현 기질의 식별입니다. Anthropic은 또한 오픈 웨이트 모델을 위한 Neuronpedia 데모를 출시했습니다 @AnthropicAI.
- 연구자들이 관심을 가진 이유: 해석 가능성 연구자들은 이 결과를 이전의 공개된 작업보다 모델의 "작업 메모리" 또는 내부 워크스페이스에 대한 더 강력한 증거로 보았습니다. 비록 그들이 프레이밍에 동의하지 않더라도 말입니다. @NeelNanda5는 이를 작업 메모리 유사 메커니즘에 대한 최고의 증거라고 불렀습니다. @Jack_W_Lindsey는 이 특권적인 공간을 이해하는 것이 LLM 인지에 핵심이 될 수 있다고 주장했습니다. 게시물들은 또한 실용적인 안전 측면을 강조했습니다: 이 워크스페이스는 숨겨진 개념을 표면화하고, 프롬프트 인젝션을 감지하며, 모델이 언어화되기 전에 내부의 사보타주 관련 기능을 노출할 수 있다고 보고되었습니다 @mlpowered, @LiorOnAI, @omarsar0.
- 그러나 "의식"이라는 언어는 논란이 되었습니다: Anthropic의 공개적인 프레이밍은 강한 반발을 불러일으켰습니다. 지지자들은 이 결과가 현상적 의식(phenomenal consciousness)보다는 접근 의식(access consciousness)의 기능적 유사성을 시사한다고 말했지만 @BorisMPower, 비평가들은 회사가 특권적인 잠재 활성화를 의식과 혼동함으로써 과장하고 있다고 주장했습니다 @AlanCowen. 심지어 일부 동정적인 견해조차도 더 큰 이야기는 철학이 아니라 모델을 감사하고 조종하기 위한 새로운 개입 지점이라는 점을 강조했습니다.
인퍼런스, 서빙 및 시스템 효율성
- 스페큘레이티브 디코딩은 여전히 뜨거운 인프라입니다: @lmsysorg는 SGLang에 DSpark를 추가하여 신뢰도 기반의 가변 길이 검증을 가능하게 했습니다. 이 방식은 높은 부하에서 모든 드래프트 토큰을 검증하는 것을 피하여, 고정 예산 스페큘레이티브 방식에 비해 처리량/레이턴시 트레이드오프를 개선합니다. DeepSeek-V4-Pro는 B300에서 batch=1일 때 383.7 tok/s에 도달했다고 보고되었습니다. Microsoft는 또한 출시 후 레이턴시 및 토큰 효율성을 개선하기 위해 GitHub Copilot 하네스에서 GPT-5.5의 프롬프트 수준 최적화를 논의했습니다 @code, @pierceboggan.
- 인퍼런스 효율성은 점점 더 전략적 병목 현상이 되고 있습니다: @jon_durbin은 학습뿐만 아니라 인퍼런스가 이제 "전체 게임"이라고 주장했습니다. 모든 데이터 파이프라인, RL 루프, 에이전트 런타임이 궁극적으로 테스트 시간 컴퓨팅으로 귀결되기 때문입니다. 이러한 관점은 하위 수준 커널 작업에서도 나타났습니다: Chutes는 MiniMax MSA 및 GatedDeltaNet-2에 대한 주요 속도 향상을 보고했으며, RTX Pro 6000 / SM120에서 ~7배의 희소 어텐션 학습 개선과 더 나은 퓨즈드 FP8 커널을 포함합니다 @jon_durbin.
- 모델 서빙을 넘어서는 인프라 출시: Cloudflare는 표준 HTTP 헤더를 통해 구성되는 Worker 진입점 앞에 지역별 계층형 캐시인 Workers Cache를 출시했습니다 @Cloudflare. OpenAI는 GPT-Realtime-2.1-mini를 출시하여, 이전 mini와 동일한 가격으로 미니 실시간 라인에 추론 및 툴 사용 기능을 제공했으며, 캐싱 개선을 통해 25% 이상의 p95 레이턴시 감소를 주장했습니다 @OpenAIDevs, @OpenAIDevs.
월드 모델, 음성 및 문서 AI
- MIRA는 주목할 만한 월드 모델 데모입니다: General Intuition과 Kyutai는 Epic Games와 함께 Rocket League를 위한 플레이 가능한 멀티플레이어 월드 모델인 MIRA를 소개했습니다. 이는 10k 시간의 봇 수집 데이터로 학습되었습니다 @gen_intuition. 이 모델은 20 fps로 실시간 실행되며, 게시물들은 단일 NVIDIA B200에서 명시적인 물리 또는 렌더링 엔진 없이 전체 2v2 경기를 실행하는 5B 파라미터 모델을 강조했습니다 @TheRundownAI. 이는 비디오/월드 모델 작업이 장난감 데모에서 인터랙티브 시뮬레이터로 이동하고 있다는 가장 명확한 신호 중 하나였습니다.
- 음성은 여전히 매우 경쟁적입니다: AssemblyAI는 Universal-3.5 Pro Realtime을 출시했습니다. 이는 AA-WER Streaming에서 4.1% WER을 기록하고, 재연결 없이 통화 중에 업데이트할 수 있는 컨텍스트 프라이밍 기능을 갖춘 스트리밍 STT 모델입니다 @ArtificialAnlys. TTS 측면에서는 Artificial Analysis가 Speechify Simba 3.2가 이제 Speech Arena에서 1233 Elo로 선두를 달리고 있으며, Gemini 3.1 Flash TTS, Sonic 3.5, Inworld Realtime TTS 1.5 Max를 앞서고, 또한 상위권 모델 중 가장 저렴하다고 밝혔습니다 @ArtificialAnlys.
- 문서-컨텍스트 파이프라인은 기본적으로 멀티모달이 되고 있습니다: LlamaIndex와 LanceDB는 지저분한 PDF를 위한 리트리벌 파이프라인을 설명했습니다. 이 파이프라인은 페이지, 청크, 추출된 자산을 연결된 멀티모달 테이블로 분리하며, 레이블링된 ESG-report 벤치마크에서 82%의 any-page-hit@5와 74%의 답변 정확도를 보고했습니다 @lancedb, @llama_index. 이는 에이전트를 위한 전용 "문서 컨텍스트 레이어"에 대한 Jerry Liu의 광범위한 주장과 일치합니다 @jerryjliu0.
가장 많은 참여를 얻은 트윗 (참여도 기준)
- Anthropic의 글로벌 워크스페이스 논문은 참여도를 지배했으며, Claude의 내부 워크스페이스/J-space에 대한 주요 발표가 다른 모든 것을 훨씬 능가했습니다 @AnthropicAI.
- Tencent Hy3는 특히 오픈소스 경쟁력 및 배포를 논의하는 기술 계정들 사이에서 가장 큰 순수 모델 출시 이야기였습니다 @teortaxesTex, @ShunyuYao12.
- MIRA의 플레이 가능한 월드 모델은 뛰어난 멀티모달/시스템 데모였습니다 @gen_intuition.
- Will Depue의 "Stargate for Data" 스레드는 가장 실질적인 전략 게시물이었으며, 컴퓨팅 단독이 아니라 데이터 수집이 프론티어 랩의 구속 조건이자 잠재적 해자가 된다고 주장했습니다 @willdepue.
- John Carmack의 메모리-시스템 스레드는 인퍼런스 하드웨어가 대규모 모델 서빙을 위해 HBM보다 훨씬 저렴한 메모리 계층과 결정론적 접근 패턴을 활용할 수 있다고 주장함으로써 상당한 기술적 관심을 끌었습니다 @ID_AA_Carmack.

---

# AI Reddit Recap

## /r/LocalLlama + /r/localLLM Recap

### 1. 대규모 오픈 웨이트 MoE 모델 출시
- longcat 2.0 (1.6T, ~48B active) 가중치가 MIT 라이선스로 오픈되었습니다 (활동: 638): LongCat 2.0 가중치는 elie와 ModelScope의 발표를 통해 MIT 라이선스 하에 오픈되었으며, 기술적 세부 사항은 LongCat 2.0 블로그 게시물에 있습니다. 이 모델은 1.6T의 총 파라미터와 인퍼런스당 약 48B의 활성 파라미터를 가진 매우 큰 MoE 시스템입니다. 댓글 작성자들은 공개된 가중치가 BF16에서 약 3.55 TB, FP8에서 2.05 TB를 차지한다고 언급했습니다. 댓글 작성자들은 멀티-테라바이트 가중치 크기로 인한 실제 배포 부담을 강조했으며, 중국의 Groupon/Uber Eats와 유사한 Meituan이 100% 국내 중국 칩으로 이 모델을 학습시켰다고 보고되어 지정학적/시장적 중요성에 대한 논의를 촉발했습니다.
댓글 작성자들은 LongCat 2.0의 규모와 배포 공간을 강조했습니다: 약 48B의 활성 파라미터를 가진 1.6T의 총 파라미터는 희소/MoE 스타일 아키텍처를 의미합니다. 한 사용자는 공개된 가중치가 BF16에서 약 3.55 TB, FP8에서 2.05 TB를 필요로 한다고 언급했는데, 이는 로컬 스토리지 또는 인퍼런스 인프라를 계획하는 모든 사람에게 중요합니다.
제기된 기술적 요점은 Meituan이 이 모델을 100% 국내 중국 칩으로 학습시켰다고 보고되었다는 것입니다. 댓글 작성자들은 이를 AI 하드웨어 공급망 독립성에 중요한 의미를 가진다고 보았습니다. 이는 Meituan이 전통적인 AI 랩이라기보다는 Groupon과 Uber Eats를 혼합한 것과 유사한 주요 중국 인터넷 기업이라는 점을 고려할 때 특히 주목할 만합니다.
여러 사용자는 관대한 MIT 라이선스와 Qwen 및 DeepSeek과 같은 프론티어 오픈 모델에 대한 벤치마크 계획에 초점을 맞췄습니다. 1.6T의 총 파라미터, 약 48B의 활성 파라미터, 그리고 오픈 웨이트의 조합은 인퍼런스 툴링이 그 아키텍처를 효율적으로 지원한다면 이 모델이 다른 하이엔드 MoE 오픈 모델과 비교하는 데 실용적일 수 있음을 시사합니다.

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-the-field-guide-to-fable&utm_source=paywall-free-trial&utm_medium=web&utm_content=205713711&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-the-field-guide-to-fable&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
