# Claude Haiku 5.5 — better than GPT-6 Luna at the same pricing

**원문 URL**: https://www.latent.space/p/ainews-claude-haiku-55-better-than
**번역일**: 2026-10-08 12:27
**발행일**: 2026-10-08

---

[AINews] Claude Haiku 5.5 — 동일한 가격으로 GPT-6 Luna보다 우수합니다

### 작은 모델들 만세!
Oct 08, 2026ShareAnthropic이 Haiku 4.5를 출시한 지 약 1년이 지났고, Sonnet과 Opus, Fable 5.5까지 연이어 출시되면서 약간 잊혀진 듯했습니다. 특히 OpenAI가 Astra 및 Sol 6와 함께 Luna 6를 출시하면서 더욱 그랬습니다.
자, 드디어 출시되었으며, 환영할 만한 업데이트입니다. 자세한 내용은 아래 요약에서 확인하십시오.

![X avatar for @ArtificialAnlys](https://pbs.substack.com/profile_images/2042402069320290304/A8C1lP07.jpg)
> 10/06/2026-10/7/2026 AI 뉴스입니다. 저희는 12개 서브레딧, 544개 트위터(X)를 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 다시 한번 알려드리자면, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter Recap
주요 소식: Anthropic이 Claude Haiku 5.5를 출시했습니다

## What happened
Anthropic이 약 1년 만에 Haiku 티어의 첫 업데이트인 Claude Haiku 5.5를 출시했습니다. 이 모델은 OpenAI의 GPT-6 Luna와 동일한 가격으로 책정되었으며, Anthropic은 같은 날 Sonnet 5.5와 구독 요금제의 가격을 인하했습니다.
- 사전 출시 신호. @scaling01은 발표 전에 "happy Haiku 5.5 day"라고 게시했습니다. @kimmonismus는 이 모델이 이미 Claude Code 업데이트에 등장했으며 "Luna-pricing"이 될 것이라고 예측했습니다. 그는 공식 게시물보다 먼저 가격을 게시했고 (@kimmonismus), 출시되었을 때 이를 확인했습니다 (@kimmonismus).
- 공식 출시. @claudeai와 @AnthropicAI는 이를 "우리가 출시한 가장 저렴하고 빠르며 유능한 소형 모델"이라고 불렀으며, 평균적으로 Haiku 4.5보다 실행 비용이 약 75% 저렴하다고 밝혔습니다.
- 가용성 및 의도된 사용. 이 모델은 Claude Platform과 Claude Code (@ClaudeDevs)에서 사용할 수 있습니다. Anthropic은 이를 Opus 5.5 또는 Sonnet 5.5와 페어링되는 서브에이전트(subagent)로 포지셔닝하며, 요약, 압축 및 데이터베이스 쿼리와 같은 대량의 비용에 민감한 작업에 사용하도록 합니다. @mikeyk는 이러한 분할을 "Opus는 심층적인 사고를 담당하고, Haiku는 대량 작업을 처리한다"고 설명했습니다.
- 계층형 가격 책정 (@ClaudeDevs):
| 프롬프트 길이 | 1M 토큰당 입력 / 출력 | 1M당 캐시 읽기 |
|---|---|---|
| Under 100K tokens | $0.10 / $0.50 | $0.01 |
| Over 100K tokens | $0.50 / $2.50 | $0.05 |
- Sonnet 5.5 가격 인하. 캐시 읽기 비용이 1M 토큰당 $0.20에서 $0.10으로 절반으로 줄었습니다. Anthropic은 이로 인해 Sonnet 5.5가 대부분의 장기 실행 또는 에이전틱(agentic) 작업에서 약 20% 더 저렴해진다고 밝혔습니다 (@claudeai).
- 구독자를 위한 API 크레딧. 월별 Claude Platform API 크레딧은 이제 Max 5x ($100), Max 20x ($200) 및 Team (최대 $500, 풀링됨) 플랜과 함께 제공됩니다. 이 크레딧은 Haiku 5.5를 포함한 모든 모델과 타사 하네스(harnesses)에서 작동합니다 (@ClaudeDevs).
- 당일 SDK 업데이트. 컴퓨터 사용 및 브라우저 사용 툴셋이 이제 Python 및 TypeScript Claude SDK에 내장되었습니다. SDK는 액션 루프를 실행하고 browser_use, Browserbase, E2B 또는 Daytona의 드라이버로 클릭 및 키 입력을 전송하므로, 개발자는 더 이상 해당 루프를 직접 작성할 필요가 없습니다 (@ClaudeDevs, quickstart).
- 출시 당일 파트너 배포:
    - Cursor: @cursor_ai는 더 짧은 요청에서 "Haiku 4.5보다 10배 저렴하다"고 주장하며 CursorBench 비교 자료를 게시했습니다 (@cursor_ai).
    - VS Code의 GitHub Copilot: @code는 "더 적은 토큰과 단계를 사용하면서도 많은 코딩 작업에서 Claude Sonnet 5와 동등한 성능을 보였다"고 보고했습니다.
    - Devin: @cognition은 FrontierCode 1.1에서 58.4%를 기록하여 Sonnet 5보다 앞섰으며, 작업당 비용은 약 8분의 1 수준이라고 보고했습니다. 또한 Fusion에서 Opus 5.5의 리드 하에 "사이드킥"으로 추천했습니다.
    - Arena: Agent Arena, Code Arena WebDev, Text, Document 및 Vision에 추가되었으며, 점수는 보류 중입니다 (@arena).
    - OpenDocRouter: 같은 날 추가되었습니다 (자세한 내용은 아래 참조).

## Independent evaluation: Artificial Analysis
@ArtificialAnlys는 가장 상세한 타사 수치 (평가별 분석, 비교 페이지)를 게시했습니다.
- Intelligence Index: 최대 노력(max effort) 시 43점으로, 이전 Haiku보다 26점 상승했습니다.
    - GLM-5.3 Flash (42), Gemini 3.8 Flash (41) 및 GPT-6 Luna (38)보다 약간 앞섭니다.
    - 2.8조 파라미터 오픈 웨이트(open-weights) 모델인 Kimi K3 (44)와 비슷합니다.
    - 최대 노력 시 Claude Sonnet 5.5 (56)보다 13점 뒤처집니다.
- 새로운 제어 기능. 이것은 Anthropic의 노력 설정(effort settings)과 적응형 사고(adaptive thinking)가 적용된 첫 번째 Haiku입니다.
- 토큰 사용량이 주요 주의사항입니다.
    - 최대 노력 시 Index 작업당 약 162k 출력 토큰을 사용하며, 이는 최대 노력 시 GPT-6 Luna (약 50k)의 약 3배에 달합니다.
    - xhigh에서 max로 전환하면 약 1.8배의 토큰으로 2점이 추가됩니다.
    - 동일한 점수에서도 여전히 더 장황합니다. Haiku 5.5는 높은 노력(high effort)으로 38점을 얻는 데 약 55k 토큰을 사용하는 반면, Luna는 최대 노력으로 38점을 얻는 데 약 50k 토큰을 사용합니다.
    - 낮은 노력 설정에서는 그 격차가 더 벌어집니다.
- 비용 수치는 잠정적입니다. Artificial Analysis는 아직 100K 토큰을 초과하는 5배 가격 단계를 모델링하지 않았습니다. 작업당 비용 수치는 추후 공개될 예정입니다.
- AA-Briefcase (사설 에이전틱(agentic) 지식 작업 평가): 1578 ELO. 이는 Kimi K3 및 GLM-5.3보다 앞서며, 최대 노력 시 Muse Spark 1.3과 비슷합니다.
- Terminal-Bench 4.0: 33%로, Haiku 4.5의 0%에서 상승했습니다.
    - GLM-5.3 Flash와 동등합니다.
    - Gemini 3.8 Flash (20%) 및 GPT-6 Luna (13%)보다 앞섭니다.
- 지식 대 환각 (AA-Omniscience):
| 모델 | 정확도 | 환각률 |
|---|---|---|
| Haiku 5.5 | 36% | 40% |
| Gemini 3.8 Flash | 55% | 55% |
| GPT-6 Luna | 44% | 77% |
Haiku의 낮은 정확도 중 일부는 모른다고 말하는 데 더 적극적이기 때문입니다.
- AutomationBench-AA: 35%로, Luna, Gemini 3.8 Flash 및 GLM-5.3 Flash의 53–60%에 비해 낮습니다. 출시 전 안전성 버그로 인해 모델이 과도하게 거부하는 현상이 발생했습니다. Anthropic은 수정 작업을 진행 중이며, Artificial Analysis는 평가를 다시 실행하여 점수가 상승할 것으로 예상하고 있습니다.
- 사양:
    - Haiku 4.5의 200k에서 1M 토큰 컨텍스트(context)로 증가했습니다.
    - 텍스트 및 이미지 입력, 텍스트 출력.
    - 5분 캐시 쓰기 비용은 1M 토큰당 $0.125 ($100K 초과 시 $0.625)입니다.

## Other benchmark claims (mostly vendor or secondhand)
- @ShayneRedford는 Anthropic이 보고한 성능 향상을 요약했습니다:
    - OSWorld (컴퓨터 사용): 15% → 72%.
    - TerminalBench: 0% → 39%. 이는 Artificial Analysis의 Terminal-Bench 4.0 독립 평가 33%와 다릅니다.
    - 지식 작업 및 추론(reasoning)에서 10–50% 향상.
    - 이들 대부분에서 Luna를 능가합니다.
    - 약 12k 최대 출력 토큰을 가진 1M 컨텍스트.
- @alexalbert__ (Anthropic)는 Haiku 4.5가 2025년 Oct 15에 출시되었으므로, 비교 기간이 1년 미만임을 강조했습니다.
- @TheRundownAI는 이 모델이 "다양한 벤치마크에서" GPT-6 Luna를 능가한다고 보고했습니다.
- 문서 파싱 (독립 평가, ParseBench):
    - @LoganMarkewich: 전반적으로 Luna와 비슷하며, 테이블에서는 약간 더 좋고, 차트 이해는 더 나쁩니다.
    - @jerryjliu0: 1,000페이지당 약 $1.2. 가격 대비 테이블 및 읽기 순서 처리 능력은 좋지만, 차트, 시맨틱 포맷팅 및 바운딩 박스에서는 약합니다.
- 일화적 증거:
    - @simonw는 가격 관련 메모를 작성하고 자신의 "pelican-on-a-bicycle" 테스트를 실행했습니다. 그는 Haiku 4.5보다 "훨씬 더 좋다"고 말했으며, Haiku 4.5는 10배 더 비쌉니다 (비교).
    - @AI_Screening은 Haiku 5.5가 Three.js 얼룩말 시뮬레이션에서 Luna를 "압도했다"고 말했습니다 (단일 프롬프트, 체계적이지 않음).

## Opinions and reactions
Bullish
- @kimmonismus: "GPT-6-Luna보다 훨씬 좋고, Sonnet 5.5에 가깝습니다… 저렴하고 똑똑합니다."
- @theo는 계층형 가격 책정을 선호합니다. 100K 토큰 미만에서 5분의 1 가격을 부과하는 것이 "모델의 용도를 정말 명확하게 해준다"고 말했습니다. 그는 또한 Anthropic 모델이 "비용/지능 차트에서 이렇게 왼쪽에 있는 것"이 인상적이라고 생각했으며 (@theo), 스트리밍으로 출시를 다루었습니다 (@theo).
- @draecomino: "최대 노력 시 Haiku는 프론티어 모델(frontier model)처럼 작동합니다."
- @kipperrii는 작고 저렴한 모델들이 "수많은 유용한 일"을 할 수 있게 되면서 이제 더 중요해졌다고 주장합니다.
- @scaling01은 ("겁나 싸다")라고 말했고, 나중에 (@scaling01) "5.5 모델들이 좋아 보입니다"라고 덧붙였습니다.
- Anthropic 측의 @NotTomBrown ("작지만 강력한")과 @edwinarbus는 모두 축하 메시지를 게시했습니다.
Competitive framing
- 이번 출시는 OpenAI의 GPT-6 Luna를 겨냥한 것으로 널리 해석됩니다: “rip gpt 6 luna” (@dejavucoder), “Luna를 요리할 시간” (@scaling01).
- @kimmonismus는 Sonnet 캐시 읽기 비용 인하를 Anthropic이 OpenAI를 압박하는 것으로 해석했습니다. API 크레딧에 대해서는 "OpenAI: 이제 당신 차례"라고 덧붙였습니다 (@kimmonismus).
- @teortaxesTex는 Anthropic이 이제 OpenAI의 Luna/Sol/Astra에 비해 "모든 연구소 중 가장 깊이 있는 제품 라인업" (Haiku/Sonnet/Opus/Fable 및 Mythos)을 갖추고 있다고 말합니다. 그는 여전히 Anthropic이 "제품에 덜 신경 쓴다"고 생각하며, 이를 2026년 내내 Anthropic이 얼마나 여유를 가졌는지 보여주는 신호로 해석합니다.
- ThursdAI의 @altryne은 중간 티어에 의문을 제기했습니다: "Opus가 비쌌을 때는 Sonnet이 합리적이었죠." 이 쇼는 Haiku 5.5를 다룰 예정입니다 (@thursdai_pod).
Caveats (mostly from the data, not loud critics)
- 헤드라인 가격은 실제 절감액을 과장할 수 있습니다.
    - 많은 토큰 사용량 (최대 노력 시 Luna의 약 3배)이 토큰당 할인 효과의 일부를 상쇄합니다.
    - 100K 토큰을 초과하는 프롬프트는 5배 더 많은 비용을 지불해야 하며, 이는 긴 컨텍스트(context) 에이전트 루프에 중요합니다.
    - 이 두 가지 효과는 Cursor의 "짧은 요청에서 10배 저렴"하다는 주장과 Anthropic의 "평균 75% 저렴"하다는 주장이 다른 이유를 설명할 수 있습니다.
- 사실 회상 능력은 Gemini 3.8 Flash 및 Luna보다 약합니다.
- 과도한 거부 버그로 인해 현재 자동화 점수가 낮게 나옵니다.
- 아직 벤치마크되지 않음: Arena 점수는 보류 중이며, 독립적인 작업당 비용 수치는 계층형 가격 책정 지원을 기다리고 있습니다.

## Context
- Haiku 4.5는 2025년 October부터 Anthropic의 소형 모델이었습니다. 그 이후로 OpenAI의 GPT-6 Luna, Gemini 3.8 Flash, GLM-5.3 Flash 및 DeepSeek V4.1 Flash가 저가형 시장에서 경쟁해 왔습니다.
- Haiku 5.5는 Luna의 정가와 정확히 일치합니다. 노력 제어(effort control) 기능과 1M 컨텍스트(context)를 추가했습니다.
- 이 모델은 다중 모델 에이전트 하네스(harnesses) 내에서 저렴한 작업자로 명시적으로 포지셔닝됩니다: Claude Code 서브에이전트(subagents), Devin Fusion, Copilot 서브에이전트(subagents), 그리고 압축 또는 요약 단계와 같은 작업에 사용됩니다.
- Anthropic은 Sonnet 캐시 읽기 비용 인하 및 구독 API 크레딧과 함께 이를 제공하여 에이전트 경제성(agent economics)에 대한 조율된 추진을 진행했습니다. 이러한 추진은 토큰 비용에 대한 광범위한 논쟁 속에서 이루어졌습니다 (아래 @theo 참조).

## Other News
OpenAI의 722개 수학 원고: 규모, 효율성 및 여파

## Keep reading with a 7-day free trial
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-claude-haiku-55-better-than&utm_source=paywall-free-trial&utm_medium=web&utm_content=219386492&coupon=5fe099d9)
[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-claude-haiku-55-better-than&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
