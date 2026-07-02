# not much happened today

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-900
**번역일**: 2026-07-02 12:10
**발행일**: 2026-07-02

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 오늘은 별다른 소식이 없었습니다

### 또 다른 조용한 하루였습니다.
ShareFable이 예정대로 재출시되었으며, AIE는 Fable에 대한 첫 번째 Field Guide 강연과 함께 Autoresearch, Cursor FDE를 아우르는 Richard MacManus의 AIEWF 3일차에 대한 훌륭한 보도, 그리고 Zach Lloyd의 어제 인기 강연인 Software Factories에 대한 후속 기사, 그리고 "핵심만 담은" 폐막 기조연설을 놓치지 않고 다루었습니다.
> 2026년 7월 1일자 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 추가 Discord는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
코딩 모델, 에이전트 하네스, 그리고 Fable 5 재출시
- Anthropic이 Claude Fable 5를 재활성화했지만, 안전성 대체 시스템이 눈에 띄게 적용되었습니다: 억눌렸던 수요가 하루 만에 폭발한 후, @claudeai는 Fable 5가 복귀했음을 발표했으며, 업데이트된 사이버 보안 안전장치로 인해 일부 요청이 Opus 4.8로 라우팅될 수 있으며, 생물학/화학 분류기가 현재로서는 지나치게 광범위하다는 설명도 덧붙였습니다 @claudeai. 재출시는 즉시 도구 생태계로 확산되었습니다: Cursor는 Fable 5가 자체 평가에서 선두를 차지했지만, 작업당 비용이 가장 높다고 밝혔습니다 @cursor_ai; Devin은 Cloud/Desktop/CLI 전반에 걸쳐 이를 추가했습니다 @cognition; Perplexity는 이를 오케스트레이터 모델로 복원했습니다 @perplexity_ai. Anthropic은 모델이 다시 활성화되자 사용자들의 속도 제한도 재설정했습니다 @ClaudeDevs.
- 흥미로운 이야기는 "모델이 돌아왔다"는 것보다 "사람들이 프론티어 모델의 제약 사항에 어떻게 적응하고 있는가"였습니다: 여러 빌더들이 단일 모델 의존성 대신 다중 모델 오케스트레이션으로 수렴했습니다. @theo는 Fable을 더 높은 가치의 추론/계획에만 사용하고, 구현, 검증 및 컴퓨터 사용 작업은 다른 모델에 위임하는 방식을 설명했습니다. 그는 종단 간 PR(Pull Request) 생성률에서 상당한 개선을 보고했습니다 @theo. 유사한 견해는 팀이 하나의 프론티어 모델을 중심으로 구축하기보다 모델 조합 전략을 설계해야 한다고 주장한 @omarsar0와, 신뢰할 수 있는 라우팅은 종종 작업을 먼저 해결해야 한다고 주장하며 "단순 작업 사전 분류기"에 반박한 @MParakhin으로부터 나왔습니다. 벤치마크 측면에서는 @kimmonismus가 Remote Labor Index에서 Fable 5가 16.10%를 기록했음을 강조했으며, @ArtificialAnlys는 Sonnet 5가 AA-Briefcase에서 2위를 차지했지만, 턴 수가 훨씬 많고 낮은 노력 설정에서는 비용-성능 트레이드오프가 약했다고 보고했습니다.
오픈 모델, 중국 연구소, 그리고 GLM-5.2를 둘러싼 확장되는 코딩 스택
- Z.ai는 단순히 체크포인트를 출시하는 것을 넘어 GLM-5.2를 중심으로 제품 영역을 구축하고 있습니다: 가장 구체적인 출시는 GLM-5.2의 공식 개발 환경인 ZCode로, BYOK(Bring Your Own Key) 지원, 크로스 플랫폼 가용성, 그리고 코딩 플랜 구독자를 위한 할당량 증대를 제공합니다 @Zai_org. @kimmonismus의 논평은 이를 GLM 워크플로우 및 장기 자율 작업을 위해 최적화된 AI 네이티브 코딩 IDE로 평가했습니다. 주변 생태계도 빠르게 움직이고 있습니다: LangChain은 코딩 플로우에서 GLM-5.2를 사용하는 가이드를 발표했으며 @LangChain, @hwchase17은 개발자들이 GLM-5.2를 일상적인 주력 도구로 전환하고 있음을 명시적으로 언급했습니다.
- 벤치마크 결과는 오픈 코딩 모델이 전반적인 프론티어 성능을 선도하지는 못하더라도 특정 격차를 좁히고 있음을 시사합니다: @mercor_ai는 GLM 5.2가 APEX-SWE에서 통합(Integration) 부문 Pass@1 55.3%를 기록하며 한 카테고리를 선도한 최초의 오픈 모델이며, 그곳에서 테스트된 전체 오픈 모델 중 최고라고 보고했습니다. Kimi K2.7이 그 뒤를 바짝 쫓았습니다. 이는 GLM이 서구의 최고 프론티어 모델들을 능가했다고 과장하는 것을 경계하면서도, 코딩 격차가 빠르게 줄어들고 있음을 인정했던 @scaling01의 의견을 보완합니다.
- 오픈 모델을 둘러싼 인퍼런스 작업이 중요한 부분을 차지하고 있습니다: @vllm_project는 DeepSeek 모델을 위한 네이티브 DSpark 추측 디코딩 지원을 vLLM에 추가했으며, MTP 대비 향상된 수용률로 8×B300에서 약 250 토큰/초를 기록했다고 보고했습니다. 또한 @mgoin_은 GLM-5.2 DSpark 프리뷰를 출시하며 약 1.5배 빠른 디코딩을 주장했습니다. 이와 별도로 @jon_durbin은 Qwen3-32B에 자체 개발 dflash 드래프터를 적용하여 동일 하드웨어에서 약 50% 더 높은 처리량을 달성했다고 보고했습니다.
에이전트 인프라: 메모리, 위키, 스킬 구성, 그리고 구조화된 워크플로우
- "위키 메모리"가 에이전트의 실용적인 설계 패턴으로 부상하고 있습니다: @sydneyrunkle은 위키 구조의 메모리를 간단하고 확장 가능한 기반으로 주장했으며, 이 아이디어는 빠르게 제품 출시로 이어졌습니다. LangChain은 `openwiki --init` 명령어로 에이전트가 활용할 수 있는 코드베이스 문서를 생성하고 유지 관리하는 도구인 OpenWiki를 출시했습니다 @BraceSproul, @LangChain. 이러한 동기는 여러 게시물에서 일관되게 나타납니다: 에이전트는 스레드 간에 작업 컨텍스트를 반복적으로 잃어버리며, 원시 로그 대신 유지 관리되고 검사 가능한 지식 계층이 필요하다는 것입니다 @caspar_br.
- 메모리 시스템은 리트리벌 전용에서 조정 및 유지 관리로 전환되고 있습니다: Weaviate의 Engram 제안이 대표적입니다. 후보 메모리는 추출되어 기존 메모리와 비교하여 변환된 다음 커밋되므로, 모순은 모든 쿼리에서가 아니라 한 번에 해결됩니다 @PrajjwalYd. @bpalit은 동일한 주장을 엔터프라이즈 환경으로 확장하며, 에이전트 메모리가 단순히 마크다운 파일 폴더가 아니라 관리되고, 권한을 인식하며, 공유되어야 한다고 주장합니다.
- 구조화된 구성이 '모델에 모든 도구를 제공하는' 순진한 접근 방식을 대체하고 있습니다: @omarsar0는 스킬 선택을 공동 자기회귀 구성 문제로 다루는 SkillComposer를 강조했으며, 스킬 없는 기준선 대비 SkillsBench에서 +23.1pp / +18.2pp의 개선을 보고했습니다. 프레임워크 측면에서는 Deep Agents가 재귀적 언어 모델 워크플로우 지원을 추가했으며 @sydneyrunkle, @hwchase17은 동적 서브 에이전트를 에이전틱 MapReduce와 같은 패턴에 연결했습니다. 더 명시적인 워크플로우 구조, 팬아웃/팬인 패턴, 코드 기반 오케스트레이션이라는 이 일반적인 방향은 제품 및 벤치마크 전반에 걸쳐 반복적으로 나타났습니다.
보안, 평가, 그리고 에이전틱 MapReduce
- Cognition의 Devin Security Swarm은 실제 엔터프라이즈 워크플로우에 특화된 에이전트 아키텍처의 명확한 사례 중 하나입니다: 이 시스템은 에이전틱 MapReduce를 사용하여 코드베이스 전반에 걸쳐 제한된 에이전트들을 팬아웃하고, 발견 사항을 집계하며, 확인된 취약점을 표면화하기 전에 악용 가능성을 검증합니다 @cognition. Cognition은 이것이 다른 대안보다 비용 효율적이고 더 정확하다고 주장하며, Fortune 500 파일럿에서 프로덕션 저장소의 천 개 이상의 취약점을 찾아 수정했다고 밝혔습니다 @walden_yan. @jakejluo 및 @levie와 같은 빌더들의 광범위한 반응은 이 패턴이 대규모 문서, 코드 및 지식 워크플로우로 일반화될 것이라는 것이었습니다.
- AI 에이전트 평가는 빠르게 자체적인 하위 분야가 되고 있습니다: @random_walker는 에이전트 평가를 발전시키는 여러 새로운 논문을 언급하며 이를 별개의 학문 분야로 설명했습니다. 실용적인 사례로는 에이전트 모드에서 Fable 5를 재활성화한 Agent Arena @arena, 메가와트당 에이전트 시스템 벤치마킹을 위한 AA-AgentPerf @ArtificialAnlys, 그리고 월드 모델이 단순히 그럴듯한 시뮬레이션을 생성하는 것이 아니라 실제로 좋은 의사 결정을 지원하는지 평가하는 WorldModelGym @RekaAILabs 등이 있습니다.
- AI 실패에 대한 더 나은 보고 파이프라인을 위한 노력도 있습니다: 사이버 및 AI 안전 연구자들을 아우르는 연합과 함께 출시된 FLARE-AI는 결함 및 사고 보고를 표준화하여 문제가 사일로화된 접수 양식으로 사라지지 않고 올바른 개발자와 레지스트리로 전달될 수 있도록 하는 것을 목표로 합니다 @ClementDelangue, @ShayneRedford.
주목할 만한 시스템, 인퍼런스, 그리고 아키텍처 작업
- NVIDIA의 TwoTower 결과는 생성 아키텍처에서 구체적인 속도/품질 트레이드오프를 보여주는 뛰어난 사례입니다: @NVIDIAAI는 Nemotron-Labs-TwoTower를 소개했는데, 이는 30B 모델을 두 개의 복사본 설정(two-copy setup)을 통해 토큰을 병렬로 작성하는 확산 스타일 언어 모델로 조정했습니다. 주장된 결과는 원래 모델 품질의 98.7%를 유지하면서 2.42배 더 빠른 생성을 달성했다는 것입니다. @LiorOnAI는 이 기술을 동결된 컨텍스트 모델과 학습된 작성기 모델을 재사용하여 처음부터 전체 재학습을 피하는 것이라고 요약했습니다.
- 온디바이스 및 브라우저 인퍼런스는 에이전틱 최적화 및 특수 런타임의 이점을 계속 누리고 있습니다: @googlegemma는 Fable 5로 작성된 커널 덕분에 WebGPU Gemma 4가 M4에서 255 토큰/초로 실행된다고 강조했습니다. @andimarafioti는 Cerebras 인퍼런스를 사용하는 Gemma 4 31B 기반의 완전히 오픈소스인 실시간 음성 스택을 시연했으며, OpenAI의 실시간 API에 대한 드롭인(drop-in) 대안을 목표로 합니다. 커널 수준에서는 Hugging Face의 커널 라이브러리가 이제 MiniMax의 MSA 커널을 노출하며 @RisingSayak, Triton-on-Mac도 관심을 끌었습니다 @QuixiAI.
- 바닐라 LLM 스케일링을 넘어선 아키텍처 연구도 부상했습니다: @gklambauer는 잠재 상태 예측 오류를 통한 테스트 시간 적응을 사용하는 LeCun이 이끄는 월드 모델 접근 방식인 AdaJEPA를 지적했습니다. @LiorOnAI는 NEO를 다음 프레임 예측뿐만 아니라 재사용 가능한 인과적 "프로그램"을 학습하는 것으로 요약했습니다. 그리고 @ziv_ravid는 "상상 속 학습"을 단순한 추측이 아닌 활발한 패러다임으로 강조했습니다.
최고 인기 트윗 (참여도 기준)
- Fable 5 가용성이 기술적 관심을 지배했습니다: @claudeai: "Fable 5가 돌아왔습니다.", 속도 제한 재설정에 대한 @ClaudeDevs, 그리고 CursorBench에서 Fable 5가 선두를 차지했다는 @cursor_ai.
- 광범위한 영향력을 가진 시스템/인프라 출시: TwoTower가 98.7% 품질 유지율로 2.42배 더 빠른 생성을 달성했다는 @NVIDIAAI.
- 오픈 모델 생태계 모멘텀: GLM-5.2용 ZCode를 출시한 @Zai_org와 8.3B 달러 가치로 800M 달러 규모의 Series C 투자를 발표한 @TogetherCompute.
- 고품질 도구 및 지식 계층 출시: @LangChain/OpenWiki 및 @cognition/Devin Security Swarm.

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. 오픈 웨이트 모델 출시 및 로컬 런타임 벤치마크

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-not-much-happened-today-900&utm_source=paywall-free-trial&utm_medium=web&utm_content=204582585&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-not-much-happened-today-900&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
