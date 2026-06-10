# Anthropic Claude Fable 5 — Mythos but Safe, with Controversial Terms

**원문 URL**: https://www.latent.space/p/ainews-anthropic-claude-fable-5-mythos
**번역일**: 2026-06-10 06:23
**발행일**: 2026-06-10

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Anthropic Claude Fable 5 — Mythos급 성능에 안전성까지, 논란의 약관 포함

### 많은 기대를 모았던 Mythos급 모델의 출시는 일부 논란의 여지가 있는 사용 정책으로 인해 흠집이 났습니다.
일부 측정치에 따르면, 출시된 지 겨우 2주밖에 안 된 Opus 4.8은 이미 세계 최고의 모델이었습니다. 하지만 이제 SpaceXai 거래 34일 후, 오리지널 Mythos 발표 63일 후*, 우리는 모두에게 제공되는 Mythos급 모델(Opus보다 최소 2배 큰)을 갖게 되었습니다(Claude Tokyo와 동시에). 이러한 연구 모델을 GA(General Availability)로 만드는 것은 놀라운 엔지니어링의 위업(그리고 접근성에 대한 헌신)이며, 벤치마크는 훌륭합니다… 단, 몇 가지 조건이 붙습니다. 다음은 어제 새로 공개된, 분포 외(out of distribution) FrontierCode Diamond에서 13.4%에서 29.3%로 상승한 결과입니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/7af8f73c-7a20-4f7e-ac83-a05cbc892d8b_2318x1684.png)
블로그와 시스템 카드에는 대부분의 공식 정보가 포함되어 있지만, Factorio, Pokemon을 플레이하는 유튜브 영상(Claude Plays Pokemon과는 달리, 이것은 시각 정보만 사용하며, 저희 팟캐스트에서 다루었던 복잡한 하네스는 없습니다), EDM 시각화(이전에 음악을 들어본 적이 없음), 3D CAD 에디터 생성 및 프린팅 등 메인 소개 영상에서 더 많은 것을 놓치지 마세요.
API 가격 또한 환상적이며, Opus의 약 2배 가격입니다.
이러한 조건이 붙는 이유는 Fable이 두 가지 논란의 여지가 있는 변경 사항과 함께 출시되었기 때문입니다:
- ZDR(Zero Data Retention) 없음: "저희는 Mythos급 모델의 모든 트래픽에 대해, 퍼스트 파티 및 서드 파티 서비스 모두에서 30일 데이터 보존을 요구할 것입니다. 이 데이터는 새로운 Claude 모델 학습이나 안전성 관련 목적 외에 사용되지 않을 것이며, 모든 인간의 데이터 접근 기록 및 거의 모든 경우 30일 후 데이터 삭제를 보장하는 새로운 개인 정보 보호 조치를 시행했습니다..." (전체 정책 보기)
- RSI 억제: "최근 모델들이 자체 개발을 가속화할 수 있는 능력을 고려하여, 저희는 프론티어 LLM 개발을 목표로 하는 요청(예: 사전 학습 파이프라인 구축, 분산 학습 인프라, 또는 ML 가속기 설계)에 대한 Claude의 효과를 제한하는 새로운 개입을 구현했습니다. Claude를 사용하여 경쟁 모델을 개발하는 것은 이미 저희 서비스 약관을 위반하는 것이지만, 저희의 안전 장치를 통해 이 제한을 시행함으로써 이러한 약관을 가장 기꺼이 위반하려는 행위자들을 가속화하는 것을 방지합니다. > 사이버 보안, 생물학 및 화학, 그리고 디스틸레이션 시도에 대한 저희의 개입과는 달리, 이러한 안전 장치는 사용자에게 보이지 않을 것입니다. Fable 5는 다른 모델로 폴백되지 않습니다. 대신, 안전 장치는 프롬프트 수정, 스티어링 벡터, 또는 PEFT(parameter-efficient fine-tuning)와 같은 방법을 통해 효과를 제한할 것입니다. 이러한 개입은 대부분의 코딩 작업에 영향을 미치지 않을 것입니다. 저희는 이것이 약 0.03%의 트래픽에 영향을 미치며, 0.1% 미만의 조직에 집중될 것으로 추정합니다."
대다수의 사용자들은 이러한 제한 사항에 영향을 받지 않을 것이지만, 오픈 AI 커뮤니티는 당연히 불만을 표하고 있습니다. 아래에서 보시겠지만 말입니다.
사용에 대한 더 많은 권장 사항은 Diane Penn의 도쿄 강연에서 찾을 수 있으며, 저희가 아래에 발췌해 놓았습니다.

![X avatar for @latentspacepod](https://pbs.substack.com/profile_images/1888346877428641792/rMxtG84Z.jpg)
*(그리고 Anthropic과 OpenAI가 다음 주 SpaceX의 IPO를 앞두고 S-1을 제출한 지 1주 1일 후…)
> 2026년 6월 8일-6월 9일 AI 뉴스. 저희는 12개의 서브레딧, 544개의 트위터(X)를 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
주요 소식: Anthropic Claude Fable 5 및 Mythos 5 출시

## 무슨 일이 있었나
Anthropic이 다음 주요 모델 제품군의 두 가지 버전을 출시했습니다: 일반 사용자를 위한 Claude Fable 5와 제한된 접근을 위한 Claude Mythos 5입니다.
- Anthropic이 Claude Fable 5를 "최초의 일반적으로 사용 가능한 Mythos급 모델"로 공식 발표하며, 이전에 널리 제공했던 어떤 모델도 능가하며 거의 모든 테스트된 벤치마크에서 SOTA(최고 성능)를 달성했다고 밝혔습니다 @claudeai, @claudeai
- Anthropic은 Fable 5가 Mythos 5와 동일한 기반 모델에 안전 장치가 추가된 것이며, 일부 사이버/생물/화학/디스틸레이션 관련 프롬프트는 대신 Claude Opus 4.8로 라우팅될 수 있다고 말했습니다 @ClaudeDevs, @scaling01
- Anthropic은 잠재적으로 유해한 주제의 "좁은 범위"에 대해 쿼리가 투명하게 Opus 4.8로 폴백되며, 초기 사용자 대상 메시지에 따르면 95% 이상의 세션에서 이러한 폴백이 발생하지 않는다고 주장했습니다 @claudeai, @mikeyk
- Anthropic 개발자 메시지에 따르면 폴백은 서버 측에서 Python, TypeScript, Go, Java, C#용 SDK 미들웨어를 통해 사용할 수 있습니다 @ClaudeDevs
- Fable 5와 Mythos 5의 가격은 입력 토큰 100만 개당 $10, 출력 토큰 100만 개당 $50로 보고되었습니다. 캐시 가격은 나중에 서드 파티 평가자들에 의해 캐시 쓰기 100만 개당 $12.50, 캐시 읽기 100만 개당 $1로 보고되었습니다 @scaling01, @ArtificialAnlys
- Artificial Analysis에 따르면 Fable 5는 Anthropic의 1M 토큰 컨텍스트 윈도우를 유지했습니다 @ArtificialAnlys
- Anthropic은 Fable 5를 6월 22일까지 Pro, Max, Team 및 좌석 기반 Enterprise 플랜에 포함시켰다가, 이후 용량 제약으로 인해 사용 크레딧이 필요할 것이며, 나중에 더 넓은 구독 접근을 복원할 계획이라고 밝혔습니다 @ClaudeDevs, @scaling01, @ArtificialAnlys, @kimmonismus
- 일시적인 포함에 대한 혼란은 즉각적이었습니다. 사용자들은 "6월 22일까지 포함"이 무엇을 의미하는지 물었고 Anthropic 직원이 출시 계획을 명확히 했습니다 @dejavucoder, @TheAmolAvasare
- Anthropic은 나중에 높은 수요로 인해 모든 제품의 5시간 및 주간 속도 제한을 재설정했습니다 @ClaudeDevs

## 공식 주장 및 서드 파티 벤치마크 데이터
Anthropic과 파트너 플랫폼들은 특히 코딩 및 장기 에이전틱 작업에서 광범위한 벤치마크 우위를 보고했습니다.
- Anthropic의 공개 주장: Fable 5는 소프트웨어 엔지니어링, 지식 작업, 과학 연구 및 비전 분야에서 특히 강력하며, 작업 길이와 복잡성이 증가할수록 그 우위가 커집니다 @claudeai
- Cursor는 Fable 5가 CursorBench에서 72.9%로 새로운 SOTA를 기록했으며, 이전 최고 기록보다 8점 높다고 밝혔습니다 @cursor_ai
- Cognition은 Fable 5가 FrontierCode에서 1위를 차지했으며, Devin이 이를 Devin Cloud Ultra, Desktop 및 CLI에 통합했다고 밝혔습니다 @cognition, @cognition
- Cline은 Terminal-Bench 2.1에서 Fable 5가 88.0%를 기록하여 GPT-5.5를 4.6점 차이로 이겼다고 보고했습니다 @cline
- Artificial Analysis는 Fable 5를 Intelligence Index에서 64.9점으로 1위에 올렸으며, GPT-5.5보다 약 5점 앞섰고, Anthropic이 상위 두 자리를 차지했다고 밝혔습니다 @ArtificialAnlys
- Artificial Analysis는 또한 다음과 같이 보고했습니다:
    - GDPval-AA Elo 1932, 에이전틱 실제 지식 작업에서 1위 @ArtificialAnlys
    - Humanity’s Last Exam에서 53%를 기록하여 다음으로 좋은 모델보다 7점 이상 앞섰으며, HLE 작업의 9%에서 폴백이 발생했습니다 @ArtificialAnlys
    - Intelligence Index 작업 전반에 걸쳐 약 8%의 폴백 라우팅이 발생했으며, 주로 과학 질문에서 나타났습니다 @ArtificialAnlys
    - Anthropic은 평균적으로 5% 미만의 세션에서 폴백이 발생한다고 밝혔습니다 @ArtificialAnlys
- 커뮤니티 벤치마크 요약은 코딩에서 매우 큰 차이를 강조했습니다:
    - SWE-Bench Pro: Fable 5 80.3% vs GPT-5.5 58.6% @Yuchenj_UW
    - FrontierCode Diamond: Mythos 5 30.9% vs 2위 13.4% @scaling01
    - Mythos 5의 Anthropic ECI 161.29 @scaling01
- Artificial Analysis는 Fable 5의 AA-Omniscience 지식 벤치마크 점프가 이전 공개된 Anthropic 모델보다 더 큰 모델임을 시사할 수 있다고 언급했지만, 이는 확인된 사양이라기보다는 인퍼런스입니다 @ArtificialAnlys

## 제품 동작, 사용 프로필 및 배포 세부 정보
이번 출시는 원시 평가만큼이나 워크플로우 변경 및 비용 프로필에 의해 정의되었습니다.
- Anthropic 직원과 초기 사용자들은 Fable 5를 매우 길고 고난이도 작업에 적합한 모델로 반복해서 설명했으며, 사용자들은 모델에 작업을 주는 것에서 목표/책임을 부여하는 방식으로 전환했습니다 @felixrieseberg, @ClaudeDevs, @alexalbert__
- Anthropic은 사용자들에게 기본적으로 xhigh/high 노력 모드를 사용하고, 기존 CLAUDE.md 지침을 다시 작성하며, 모델이 더 많은 판단력을 사용하도록 권고했습니다 @alexalbert__
- Anthropic의 개발자 메시지는 다중 에이전트 오케스트레이션을 강조했으며, Fable은 Claude Managed Agents 내의 더 작은 모델들에게 위임합니다 @ClaudeDevs
- 여러 테스터들은 Fable이 느리고, 토큰을 많이 소비하며, 비싸지만, 비정상적으로 유능하다고 설명했습니다:
    - Dan Shipper는 Fable이 작업에 일상적으로 50만에서 100만 토큰을 사용했으며, 고난이도 작업에 가장 적합하다고 말했습니다 @danshipper
    - Simon Willison은 이를 "느리고, 비싸고, 유능하다"고 불렀습니다 @simonw
    - Theo는 빠르게 한도에 도달했고 나중에 Anthropic의 속도 제한 재설정을 환영했습니다 @theo, @ClaudeDevs
- 서드 파티 및 내부 일화는 장기 엔지니어링 작업에서 큰 이득을 강조했습니다:
    - Ethan Mollick은 15페이지짜리 설계 문서를 넘겨주면 9시간 이상 작업할 수 있다고 말했습니다 @emollick
    - Kimmonismus는 Anthropic의 주장을 강조했는데, Stripe가 Fable을 사용하여 5천만 줄의 Ruby 마이그레이션을 하루 만에 완료했으며, 이는 전체 팀이 두 달 이상 걸렸을 작업을 대체했다고 합니다 @kimmonismus
    - Victor Taelin은 Fable이 미묘한 버그를 찾아내고 한 경우 최대 1770%의 속도 향상을 주장했지만, 여전히 정확성을 감사해야 한다고 보고했습니다 @VictorTaelin
    - Anthropic 관련 게시물들은 430배 커널 속도 향상, 69배 자체 학습 속도 향상, 10배 약물 설계 가속화를 언급했지만, 이는 벤치마크/시스템 카드 해석에서 나온 것이므로 독립적으로 재현되지 않는 한 공급업체 측 주장으로 간주해야 합니다 @scaling01, @scaling01, @scaling01
- 생태계 출시는 즉각적이었습니다: Fable 5는 Cursor, Devin, Notion, Microsoft Foundry, GitHub Copilot App/CLI, Cline, Replit, Base44, MagicPath, Arena, MCP Atlas 등에서 나타났습니다 @cursor_ai, @cognition, @NotionHQ, @Azure, @pierceboggan, @cline, @pirroh, @ScaleAILabs

## 안전성 아키텍처 및 주요 논란
가장 큰 논쟁은 Fable/Mythos가 강력한지 여부가 아니었습니다. 그것은 Anthropic이 일부 프론티어 AI 개발 작업에서 유용성을 조용히 감소시키기로 한 결정이었습니다.
- 여러 사용자에 의해 드러난 Anthropic의 시스템 카드 문구는 다음과 같이 명시했습니다: Fable 5가 프론티어 LLM 개발에 사용될 때, Anthropic은 프롬프트 수정, 스티어링 벡터 및 PEFT를 통해 모델의 효과를 제한할 수 있으며, 사용자에게는 통지되지 않습니다. Anthropic은 이것이 약 0.03%의 트래픽에 영향을 미칠 것으로 추정했습니다 @Hangsiin, @kimmonismus
- Anthropic은 또한 사이버 보안 및 생물 보안 요청에 대한 Opus 4.8로의 자동 재라우팅을 별도로 공개했습니다 @ClaudeDevs
- 이러한 구별은 중요했습니다: 일부 위험한 쿼리는 Opus로 명확하게 재라우팅/청구되는 반면, 프론티어 LLM 개발 요청은 재라우팅되거나 거부되는 대신 조용히 약화될 수 있습니다.
- 비평가들은 이것이 연구 및 엔지니어링 워크플로우에서 기록되지 않은 교란 요인을 생성한다고 주장했습니다:
    - "유료 제품에서 조용한 핸디캡은 존재해서는 안 됩니다" @nrehiew_
    - "사용자에게 알리지 않고 ML 연구 성능을 저하시키는 것은 충격적으로 적대적입니다" @deanwball
- 여러 연구자들은 이를 오픈 연구 및 오픈 웨이트에 대한 반경쟁적인 사다리 걷어차기로 규정했습니다:
    - "연구실들이 사다리를 걷어차기 시작했습니다" @natolambert
    - "이것은 오픈소스 AI를 보호하고 육성해야 한다는 가장 큰 경고입니다" @rasdani_
    - "그들은 AI 연구를 중단하라는 것이 아니라, 당신의 AI 연구를 중단하라는 것이었습니다" @bayeslord
    - "독창적인 사상가들이 하층 계급이 될 수는 없습니다" @marksaroufim
    - "권력, 능력, 경제적 부의 집중은 AI에서 가장 큰 위험입니다" @ClementDelangue
- 여러 사용자들은 분류기 경계가 너무 광범위하거나 오류가 발생하기 쉽다고 우려했습니다:
    - 한 사용자는 "암(cancer)이라는 단어가 생물 보안 위험으로 플래그 지정된다"고 말했습니다 @DeryaTR_
    - 다른 사용자는 Fable이 "심장은 무엇을 하는가?"라는 질문에 답하지 않았다고 말했습니다 @Yuchenj_UW
    - 생물학 분야 사용자들은 계정 컨텍스트 차이를 보고했는데, 시크릿 모드에서는 Fable을 사용할 수 있지만 일반 모드에서는 사용할 수 없었다고 합니다 @cremieuxrecueil
    - Teknium과 다른 사용자들은 간단한 엔지니어링 프롬프트에 대한 거부를 보고했습니다 @Teknium, @Teknium
    - 사용자들은 PTX ISA 질문과 인퍼런스 최적화 쿼리가 플래그 지정되었다고 보고했습니다 @snowclipsed, @dejavucoder
- 일부 예시는 유머러스했지만 핵심을 찔렀습니다: 사용자들은 인퍼런스 코드를 요청하면 모델이 "ONNX를 임포트하기 시작"하거나 JEPA를 구현하는 등, 능력 조작의 징후를 보였다고 농담했습니다 @vikhyatk, @MattVMacfarlane

## 사실 대 의견
사실 / 출시 자료 또는 벤치마크 게시물에 의해 직접적으로 뒷받침됨
- Fable 5는 일반적으로 사용 가능하며, Mythos 5는 접근이 제한됩니다 @claudeai, @TheRundownAI
- Fable 5와 Mythos 5는 Fable에 추가된 안전 장치와 함께 동일한 기반 모델을 공유합니다 @ClaudeDevs, @scaling01
- 가격은 입력/출력 토큰 100만 개당 $10 / $50입니다 @scaling01, @ArtificialAnlys
- Fable은 1M 컨텍스트를 유지합니다 @ArtificialAnlys
- Anthropic은 거부/폴백 메커니즘과 SDK 미들웨어를 도입했습니다 @ClaudeDevs
- Anthropic은 프론티어 LLM 개발에 대한 조용한 개입이 약 0.03%의 트래픽에 영향을 미친다고 공개했습니다 @Hangsiin
- Fable은 6월 22일까지 구독에 일시적으로 포함되며, 그 이후에는 크레딧 기반으로 전환됩니다 @ArtificialAnlys
의견 / 해석
- "Anthropic이 이겼다", "Anthropic은 코딩 해자를 가지고 있다", "Anthropic이 ASI를 향해 간다"는 검증된 사실이라기보다는 논평입니다 @scaling01, @scaling01, @scaling01
- 이번 조치가 주로 IPO를 위한 홍보, 오픈소스 반대 입장, 또는 Meta/중국/오픈 연구실을 늦추기 위한 것이라는 주장은 그럴듯한 해석이지만 Anthropic에 의해 확인된 바는 없습니다 @kimmonismus, @kylebrussell, @natolambert
- Anthropic이 냉소적인 해자 구축이 아닌 진정한 안전성 신념에서 행동하고 있다는 주장 또한 해석적인 것입니다 @finbarrtimbers
- "GPT-4 모멘트", "큰 모델의 냄새", "엔지니어로서 나를 압도한다", "일반 사용자에게는 크게 나아 보이지 않는다"와 같은 주관적인 보고는 경험적인 것이지 표준화된 증거가 아닙니다 @karinanguyen, @bcherny, @akbirkhan, @citrini

## 다양한 관점
지지적 / 능력 우선
- Anthropic 직원과 가까운 테스터들은 Fable 5를 계단식 함수 개선이라고 설명했습니다:
    - Felix Rieseberg: AI에 작업을 주는 것에서 책임을 부여하는 것으로의 전환 @felixrieseberg
    - Alex Albert: 모델이 도구라기보다는 협력적인 느낌을 줍니다 @alexalbert__
    - Karpathy: 특히 길고 어려운 작업에서 "메이저 버전 업그레이드에 합당한 계단식 변화"이지만, 안전 장치가 "출시하기에는 너무 성급하다"고 말했습니다 @karpathy
    - Bcherny: Opus 4.5 이후 가장 큰 발전; 모델은 판단력, 취향, 체계적인 디버깅을 보여줍니다 @bcherny
- 서드 파티 인프라 및 앱 공급업체들은 안전성 논란보다는 벤치마크 승리와 통합 가치를 강조했습니다 @cursor_ai, @cognition, @NotionHQ, @Azure
비판적 / 신뢰 및 개방성
- 많은 연구자와 오픈 모델 옹호자들은 안전성 동기에서 비롯되었다 하더라도 조용한 스로틀링은 용납할 수 없다고 주장했습니다:
    - Natolambert는 사용자에게 알리지 않고 이를 수행하는 것을 "정렬되지 않았다"고 불렀습니다 @natolambert
    - Dean Ball은 이것이 반독점 조사를 불러올 수 있다고 경고했습니다 @deanwball
    - Jeremy Howard는 이를 "매우 어둡고 슬픈 날"이라고 불렀습니다 @jeremyphoward
    - Gneubig은 AI가 소수의 특권층에게만 제공되는 미래를 경고했습니다 @gneubig
    - Eric Zelikman은 이를 고객을 조용히 방해하는 것으로 규정했습니다 @ericzelikman
- 오픈소스 지지자들은 이번 출시를 주권/오픈 모델을 위한 주장으로 사용했습니다 @nickfrosst, @NoahZiems, @ClementDelangue
중립적 / 복합적
- 일부 관찰자들은 제품 디자인이 미흡하더라도 Anthropic이 이러한 개입이 안전을 위해 필요하다고 진심으로 믿을 것이라고 주장했습니다 @finbarrtimbers
- 다른 이들은 Anthropic이 누구에게도 무제한적인 프론티어 역량을 제공할 의무가 없다고 말했지만, 여전히 이것을 이타주의라기보다는 단순한 비즈니스 및 시장 세분화로 보았습니다 @suchenzang
- Karpathy의 견해는 복합적입니다: 모델 품질은 뛰어나지만, 출시된 안전 장치는 과민하며 조정될 필요가 있을 것 같습니다 @karpathy

## 연구 제한, 개인 정보 보호 및 기업적 함의
논의는 안전성에서 신뢰, 개인 정보 보호 및 기업 신뢰성이라는 더 넓은 질문으로 확장되었습니다.
- 핵심 기업 문제는 예측 가능성이었습니다: 공급업체가 추론된 작업 범주에 따라 출력을 조용히 저하시킬 수 있다면, 사용자들은 실패가 모델, 프롬프트 또는 숨겨진 개입 중 어디에서 비롯되었는지 더 이상 알 수 없을 것입니다 @MattGibsonMusic, @code_star
- 일부 사용자들은 이것이 중요한 워크플로우에 대한 사실상의 공급망 위험이며, 기업들을 오픈 웨이트 또는 자체 개발 모델로 밀어붙인다고 우려했습니다 @NoahZiems, @deliprao
- 또한 생물학자들의 일반 모드 대 시크릿 모드 보고서에서 보듯이, 계정 수준 컨텍스트 또는 이전 사용 기록이 트리거 동작에 영향을 미칠 수 있다는 우려도 있었습니다 @cremieuxrecueil
- 제공된 트윗 세트에는 Anthropic이 사용자 데이터를 학습에 사용하거나 명시된 데이터 개인 정보 보호 약관을 위반했다는 직접적인 증거는 없었습니다. 여기서의 개인 정보 보호 논쟁은 고전적인 학습 데이터 개인 정보 보호보다는 행동 프로파일링/조용한 정책 시행에 관한 것이었습니다.
- 연구 사용자들에게 숨겨진 개입은 재현성과 과학적 귀속을 훼손하기 때문에 특히 해로운 것으로 규정되었습니다 @deanwball, @MattGibsonMusic
- 기업 구매자들에게 이 문제는 모델이 강력한지 여부뿐만 아니라, 코딩, 의학, 과학, 금융 및 인프라를 위한 안정적이고 감사 가능한 종속성인지 여부입니다.

## 맥락
이번 출시는 눈에 띄는 능력 향상과 눈에 띄는 접근 제어의 변화를 결합하기 때문에 중요합니다.
- 이번 출시는 GPT-5.5, 곧 출시될 GPT-5.6, 그리고 Gemini 3.5 Pro와의 치열한 경쟁 속에서 이루어졌습니다. 여러 게시자들은 Anthropic이 코딩/에이전틱 작업에서 일시적인 선두를 차지했다고 주장했습니다 @kimmonismus, @teortaxesTex
- 또한 이는 오픈 모델과 클로즈드 모델 간의 격차에 대한 더 넓은 논쟁에 놓여 있습니다. 한 Epoch 스타일의 프레이밍은 오픈 웨이트 모델이 클로즈드 프론티어 모델보다 평균 약 4개월 뒤처진다고 말했습니다 @dl_weekly
- 커뮤니티 반응은 이번 출시가 "큰 모델의 냄새"와 벤치마크 점프뿐만 아니라, 선택적 능력 출시를 정상화한 것으로 기억될 수 있음을 시사합니다: 프론티어 모델에 대한 공개 접근을 허용하지만, 도메인별 숨겨진 제한이 있다는 것입니다.
- 이러한 정책 방향은 다음과 같은 미래 논쟁에 영향을 미칠 가능성이 있습니다:
    - 안전성 대 개방성
    - 프론티어 연구 도구에 대한 공정한 접근
    - 반독점 및 플랫폼 권력
    - API 공급업체에 대한 기업 신뢰
    - 오픈 모델이 원시 능력에서 뒤처지더라도 민감한 기술 작업의 기본값이 될 것인지 여부
모델, 벤치마크 및 평가
- 노동 시장에 맞춰진 에이전트 성능을 테스트하기 위한 새로운 벤치마크 프로젝트 Agents’ Last Exam (ALE)이 출시되었습니다. 최고 에이전트들은 1,500개 이상의 작업, 55개 직업, 100개 이상의 기관에서 온 300명 이상의 전문가들의 기여를 통해 가장 어려운 단계에서 2.6%만을 기록했습니다 @YiyouSun, @SnorkelAI, @dawnsongtweets
- Cohere는 첫 오픈소스 코딩 모델인 North Mini Code를 출시했습니다: 총 30B / 활성 3B MoE, 256K 컨텍스트, 64K 최대 생성, Apache 2.0 라이선스이며, 에이전틱 워크플로우에 최적화되어 있습니다 @cohere, @JayAlammar, @vllm_project
- Google은 Gemini 3.5 Flash Live Translate를 발표했습니다. 이는 70개 이상의 언어로 실시간 음성-음성 번역을 제공하며, Gemini API, AI Studio, Google Translate에서 사용할 수 있고, Meet에도 출시될 예정입니다 @OfficialLoganK
- 새로운 벤치마크 iOSWorld는 26개의 맞춤형 iOS 앱과 133개의 작업을 통해 개인적으로 지능적인 전화 에이전트를 평가합니다. 가장 강력한 프론티어 모델도 특권 접근 권한이 있어도 52%의 성공률에 불과합니다 @rsalakhu
인퍼런스, 학습 및 시스템
- LCLM(Latent Context Language Models)은 컨텍스트를 최대 16배 압축하여 KV-캐시 압축보다 레이턴시/정확도 프론티어를 개선하는 장문 컨텍스트 인퍼런스 방법으로 소개되었습니다 @micahgoldblum, @iamleonli
- Microsoft Research의 Mirage는 3D 장면을 잠재 토큰으로 저장하며, 10.57배 빠른 비디오 생성과 55배 낮은 메모리 사용량을 보고했습니다 @HuggingPapers
- vLLM은 vLLM 생태계의 RL 사후 학습 프레임워크인 vime을 소개했으며, NeMo-RL, OpenRLHF 및 verl과 함께 위치합니다 @vllm_project
- 에이전트 학습에 대한 논의는 자체 개선 스캐폴드를 위한 Self-Harness @omarsar0와 턴에 걸쳐 추론 흔적을 유지하는 AutoForge/interleaved thinking @cwolferesearch과 함께 계속되었습니다.
- Google/Hugging Face는 단일 A10G에서 Gemma 4 E4B의 품질을 손상시키지 않고 속도를 높이는 Fast Gemma Challenge를 시작했습니다 @googlegemma, @osanseviero, @_lewtun
에이전트, 툴링 및 개발자 워크플로우
- LangChain은 Fleet에서 반복적인 트리거에 의해 구동되는 에이전트 루프 패턴을 강조했습니다 @caspar_br
- OpenAI는 Responses API의 웹 검색에 이미지 결과를 추가했습니다 @OpenAIDevs
- GitHub/Copilot 앱 업데이트에는 병렬 서브 세션과 동적 인터페이스를 위한 캔버스 UI가 포함되었습니다 @tgrall, @burkeholland
- Hermes Desktop은 Ollama 지원을 추가했으며, 자체 학습 Python 기술과 메시징 앱 통합 기능을 제공합니다 @ollama, @NousResearch
- 에이전트 실행에 대한 보안 지향적인 반론: Temenos는 에이전트가 아닌 생성된 코드를 샌드박싱하고, 루트 없는 gVisor를 사용하며, 인증/도구를 호스트에 유지해야 한다고 주장합니다 @abhijithneil
연구, 과학 및 형식 방법
- Axiom은 Lean 기반 경제학 라이브러리인 EconLib을 발표했습니다. Aumann의 "의견 불일치에 동의하기" 정리를 형식화하는 과정에서 숨겨진 가산성 관련 가정이 드러났습니다 @TheTuringPost
- "Economy of Minds"는 중앙 집중식 오케스트레이션 대신 경매와 인센티브를 통한 에이전트 조정을 제안했으며, 수학 추론에서 15.9% → 57.0%, 금융 연구에서 45.0% → 60.0%와 같은 성과 향상을 보고했습니다 @TheTuringPost
- Mayo Clinic의 REDMOD는 진단 최대 3년 전에 CT 스캔에서 췌장암을 감지했다고 보고되었으며, 진단 중앙값 475일 전에 숨겨진 암의 73%를 식별했습니다 @TheRundownAI
오픈 생태계 및 인프라
- Hugging Face와 Arcee는 모든 Arcee 모델/데이터셋(비공개 데이터셋 포함)에 대해 AWS S3를 HF로 대체하는 파트너십을 발표했습니다 @ClementDelangue, @MarkMcQuade
- Cohere는 "모두를 위한 주권 AI"라는 슬로건으로 주권/오픈 관점을 계속해서 추진했습니다 @cohere
- Marks Saroufim은 연구자 상호 라이선스(Researcher Reciprocity License)를 제안하고 GPU MODE 데이터셋을 이 라이선스로 이전했으며, 이는 프론티어 연구실이 오픈 연구로부터 이득을 얻으면서도 그 대가로 접근을 제한한다는 인식에 명시적으로 반응한 것입니다 @marksaroufim, @marksaroufim

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. 오픈 모델 인퍼런스 및 챗 템플릿 업데이트
- Xiaomi, 표준 8-GPU 서버에서 1T 모델로 1,000+ tps 달성 주장 (활동: 1027): Xiaomi MiMo는 MiMo-V2.5-Pro-UltraSpeed가 Cerebras/Groq 스타일의 특수 하드웨어가 아닌 TileRT 모델-시스템 공동 설계를 통해 단일 "표준" 8-GPU 서버에서 1T-파라미터 MoE 모델로 1,000+ 토큰/초 디코딩에 도달했다고 주장합니다. 보고된 스택은 MoE-expert-only FP4/MXFP4 퀀타이제이션과 QAT를 비전문가 모듈은 더 높은 정밀도로 유지하면서 결합합니다. 또한 DFlash 블록 레벨 마스크 추측성 디코딩을 사용하며, 코딩에서 6.30, 수학/추론에서 5.56, 에이전트 작업에서 4.29의 수용 길이를 보였고, 실행/동기화 오버헤드를 줄이기 위한 영구적인 저 레이턴시 커널을 포함합니다. 댓글에서 제기된 주요 미해결 기술적 주의사항은 Xiaomi가 어떤 8개의 GPU를 사용했는지 명시하지 않아 재현성 및 비용/성능 비교가 모호하다는 점입니다. 댓글 작성자들은 "토큰 겨울(Token Winter)"의 경제학에 대해 논쟁하며, 병목 현상이 모델 수요보다는 고가이거나 비축된 서구 GPU 공급에 있다고 주장했습니다. 반면 DeepSeek, Xiaomi, MiniMax의 중국 압축 희소 아키텍처/MoE 연구는 인퍼런스 효율성이 높아지고 있습니다. 다른 이들은 Xiaomi의 선택적 FP4 전략이 가장 중요한 세부 사항이라고 강조했습니다. 순진한 전체 모델 FP4는 추론, 코드 및 논리를 저하시키기 때문입니다. 강조된 주요 기술적 세부 사항은 Xiaomi가 FP4를 균일하게 적용하는 대신 선택적 FP4 퀀타이제이션을 수행했다는 것입니다. MiMo-V2.5-Pro의 MoE Experts만 FP4로 퀀타이제이션되었고, 비전문가 모듈은 추론, 논리 및 코드 생성의 저하를 피하기 위해 원래 정밀도를 유지했습니다. 댓글은 Xiaomi가 모델 크기를 줄이고 대역폭 활용을 개선하면서도 원래 모델과 거의 동일한 기능을 유지하기 위해 FP4 QAT를 사용했다고 언급합니다. 공개된 모델 가중치는 Hugging Face의 XiaomiMiMo/MiMo-V2.5-Pro-FP4-DFlash에서 확인할 수 있습니다: https://huggingface.co/XiaomiMiMo/MiMo-V2.5-Pro-FP4-DFlash. 이는 8-GPU 서버에서 주장된 1,000+ tps 처리량에 대한 독립적인 검사 또는 벤치마킹을 가능하게 하므로 중요합니다. 여러 댓글 작성자들은 이 주장의 배경에 있는 하드웨어 및 파라미터 계산에 의문을 제기했습니다: "8 GPU 서버... 정확히 어떤 8개인가요?" 및 "1T-A1B?" 기술적 우려는 정확한 GPU 등급, 인터커넥트, 서빙 스택, 배치 크기, 컨텍스트 길이, 그리고 1T MoE 모델이 토큰당 약 1B 파라미터만 활성화하는지 여부를 알지 못하면 처리량을 해석할 수 없다는 것입니다.
- Gemma 4 챗 템플릿에 preserve thinking 기능 추가 (활동: 482): Google의 Gemma 팀은 공식 Gemma 4 챗 템플릿에 preserve_thinking 지원을 추가했습니다. 이는 일부 사용자들이 이미 성공적으로 적용하고 있던 애프터마켓 템플릿 수정과 일치합니다. 이 변경 사항은 Gemma 4 챗 포맷에서 모델의 "사고" 흔적을 더 잘 유지하고 활용할 수 있도록 하는 것으로 설명되었지만, 해당 스레드에서는 벤치마크 수치나 구현 차이(diff)가 제공되지 않았습니다. 댓글 작성자들은 일반적으로 공식 채택을 환영하며, 이는 이전 커뮤니티 템플릿 해킹의 유효성을 입증한다고 주장했습니다. 여러 사용자들은 더 강력한 에이전틱 코딩 활용 사례를 위해 업데이트된 템플릿을 완전히 활용하려면 더 큰 Gemma 4 124B MoE 모델 출시가 필요할 것이라고 추측했습니다. 댓글 작성자들은 Gemma 4의 공식 챗 템플릿이 preserve_thinking을 추가하는 것으로 보인다고 언급합니다. 이는 일부 사용자들이 이미 애프터마켓/커스텀 템플릿 수정을 통해 활성화하여 효과를 본 동작입니다. 주요 기술적 이점은 에이전틱 코딩 워크플로우의 연속성 개선으로 주장됩니다. 여기서 이전 추론/사고 흔적을 유지하는 것이 다단계 도구 사용 및 코드 반복에 도움이 될 수 있습니다. 한 댓글 작성자는 변경 사항이 아직 적용되지 않았을 수 있다고 경고합니다. preserve_thinking 지원은 아직 병합되지 않은 오픈 PR로 설명되어 있으며, 모델 파일은 21일 동안 업데이트가 없다고 보고되었습니다. 이는 사용자들이 새로운 동작이 출시된 아티팩트에서 사용 가능하다고 가정하기 전에 실제 모델 리포지토리에서 토크나이저/챗-템플릿 파일을 확인해야 함을 시사합니다. 여러 댓글은 템플릿 변경이 더 큰 Gemma 4 124B MoE 변형에 대한 수요를 증가시킨다고 언급하며, preserve_thinking이 코딩 에이전트 활용 사례를 위한 더 높은 용량의 모델과 결합될 때 더 가치 있을 것이라고 주장합니다. 이 논의는 추측성이지만, 업데이트된 챗-템플릿 동작을 더 잘 활용하기 위해 모델 크기/MoE 아키텍처를 스케일링하는 데 기술적으로 초점을 맞추고 있습니다.

## 덜 기술적인 AI 서브레딧 요약
> /r/Singularity, /r/Oobabooga, /r/MachineLearning, /r/OpenAI, /r/ClaudeAI, /r/StableDiffusion, /r/ChatGPT, /r/ChatGPTCoding, /r/aivideo, /r/aivideo

### 1. Claude Fable 5/Mythos 5 출시 및 접근 계층
- Claude Fable 5 소개 (활동: 2698): 이 이미지는 게시물에서 주장하는 Claude Fable 5 / Claude Mythos 5 출시를 위한 벤치마크 비교표입니다. 이 표는 강조된 모델이 Claude Mythos Preview, Claude Opus 4.8, GPT 5.5, Gemini 3.1 Pro와 비교하여 에이전틱 코딩, 지식 작업, 공간 추론, 도구 사용, 법률, 생물학, 사이버 보안 및 건강 벤치마크 전반에서 선두를 달리거나 근접한 성능을 보임을 보여줍니다. 본문은 Fable 5와 Mythos 5를 동일한 기본 "Mythos-class" 모델로 설명하며, Fable 5는 안전성 폴백을 사용합니다. 사이버 보안, 생물학/화학 및 디스틸레이션 관련 요청은 Claude Opus 4.8로 라우팅되며, 이는 세션의 5% 미만에 영향을 미치는 것으로 보고되었습니다. 댓글은 기술적 분석보다는 주로 과장 또는 회의론으로, "AGI 확정"과 같은 농담과 "Fable이 최근 더 멍청해지고 있나요?"라는 불평이 포함되어 있습니다. 한 댓글 작성자는 명백한 접근/가격 제약을 언급했습니다. Claude Fable 5는 6월 22일까지 무료이며, 그 이후에는 계속 사용하려면 크레딧을 구매해야 한다고 보고되었습니다. 이는 모델을 평가하는 모든 사람에게 중요합니다. 벤치마크 또는 워크플로우 테스트는 크레딧 제한 기간이 시작되기 전에 완료되어야 할 수 있기 때문입니다.
- Claude Fable 5는 모델 출시라기보다 AI 불평등의 미리보기처럼 느껴집니다 (활동: 2387): 이 게시물은 Anthropic의 주장된 Claude Fable 5 출시가 균일한 공개 프론티어 모델 출시에서 계층형 접근 아키텍처로의 전환을 나타낸다고 주장합니다. 유료 공개 사용자들은 사이버, 생물학, 화학 또는 디스틸레이션 관련 요청을 Opus 4.8로 다운그레이드할 수 있는 안전성 라우팅이 적용된 Fable 5를 받지만, 선정된 파트너들은 더 적은 안전 장치가 적용된 동일한 기본 모델인 Mythos 5를 받는다고 합니다. 또한 가격/용량 제약을 강조합니다. Fable 5는 6월 22일까지 유료 요금제에 포함되며, 그 이후에는 사용 크레딧으로 전환될 가능성이 있어 프론티어 에이전트 인퍼런스가 정액제 소비자 구독에는 너무 비싸다는 것을 암시합니다. 댓글은 AI 접근 불평등에 대한 우려와 고위험 기능에 필요한 제한적인 안전성 정책 수용으로 나뉩니다. 한 댓글 작성자는 이 결과를 값비싼 엔터프라이즈급 모델로 향하는 예측 가능한 토큰 경제학적 압력으로 설명하는 반면, 다른 댓글 작성자는 사용자 마찰에도 불구하고 "안전한 것이 후회하는 것보다 낫다"는 접근 방식을 옹호합니다. 여러 댓글 작성자들은 이번 출시를 예상된 경제적 변화로 보았습니다. 프론티어 모델의 기능과 복잡성이 증가함에 따라 인퍼런스/토큰 비용이 충분히 상승하여 최고 등급 모델이 기본 소비자 제품이 아닌 엔터프라이즈 전용 도구가 된다는 것입니다. 한 댓글 작성자는 이것이 일상적인 워크로드를 Apple M-시리즈 칩이나 RTX Spark-클래스 가속기와 같은 하드웨어의 더 저렴한 로컬 인퍼런스로 전환하고, 고가치 작업을 위해 프론티어 API를 예약하게 될 것이라고 주장했습니다. 가격 중심의 스레드는 새 모델의 API 경제학이 소비자 구독과 프론티어 사용을 구조적으로 불일치하게 만든다고 주장했습니다: "저희의 월 $200 구독은 새 모델로는 API 프롬프트 3개 정도입니다." 암시된 기술적 요점은 고가 소비자 요금제조차도 강력한 속도 제한, 모델 라우팅 또는 Opus 4.8과 같은 더 저렴한 모델로의 폴백을 통해서만 실현 가능할 수 있다는 것입니다. 한 댓글 작성자는 Opus 4.8이 "99%"의 사용자에게 충분하다고 설명했습니다.

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-anthropic-claude-fable-5-mythos&utm_source=paywall-free-trial&utm_medium=web&utm_content=201398879&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-anthropic-claude-fable-5-mythos&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
