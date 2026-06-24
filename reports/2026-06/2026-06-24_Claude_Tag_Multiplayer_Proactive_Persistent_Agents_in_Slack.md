# Claude Tag: Multiplayer, Proactive, Persistent Agents in Slack

**원문 URL**: https://www.latent.space/p/ainews-claude-tag-multiplayer-proactive
**번역일**: 2026-06-24 12:52
**발행일**: 2026-06-24

---

[AINews] Claude Tag: Slack의 멀티플레이어, 프로액티브, 지속적인 에이전트

### Claude가 마침내 Slackbot 업그레이드를 받았습니다
저희는 팟캐스트에서 비동기 에이전트의 시대를 다룬 바 있습니다:
> Shopify부터 Stripe, Paradigm, Razorpay에 이르기까지 자체 백그라운드 에이전트를 구축하는 기업들의 물결이 있었습니다. 심지어 Cognition의 친구인 Ramp도 다른 친구 Modal과 함께 자체 코딩 에이전트를 구축했습니다.
그리고 오늘, Anthropic이 Claude Tag를 통해 이 상황에 대한 견해를 밝힐 차례입니다:

![X avatar for @claudeai](https://pbs.substack.com/profile_images/1950950107937185792/QOfEjFoJ.jpg)
이 제품이 다양한 형태로 이미 존재하기 때문에 일부 비판이 있었습니다. 하지만 전반적으로 이는 Claude와 Claude Code 폼 팩터 모두에서 매우 중요한 다음 반복입니다:
- Claude: 웹 → 데스크톱 → Slack ("LLM UIUX의 세 번째 주요 재설계")
- Claude Code: Tag 형태는 이제 제품 PR의 65%를 병합합니다.
Anthropic의 모든 것과 마찬가지로, 출시 시의 완성도는 매우 좋습니다. 비동기 에이전트 분야를 오랫동안 지켜봐 온 사람으로서, 여러분은 다음 사항들을 간과할 수 있습니다:
- Tag는 관련 코드를 소유한 동료들을 태그할 수 있습니다 (영상)
- Tag는 매우 긴 (며칠간의) 기간 동안 블로킹 종속성을 기다릴 수 있는 git 웹훅을 가지고 있습니다 (사실상 "스택된 diff" 대신 "스택된 프롬프트"를 달성합니다)
- Tag는 스레드를 실행 항목이 포함된 문서로 요약할 수 있습니다.
- 앰비언트 행동 모드의 Tag:
    - 태그되지 않아도 채널에 응답합니다 (즉, 각 메시지가 응답을 필요로 하는지 검토합니다)
    - 채널 간에 후속 조치를 취합니다 (즉, 한 채널의 정보를 다른 채널로 프로액티브하게 동기화합니다)
    - 임계값이 트리거되는지 감시하고, 무언가 고장 나면 수정하거나 A/B 테스트가 성공하면 수정하려고 시도합니다.
전반적으로 미래 업무에 대한 매우 흥미로운 전조입니다.
> 2026년 6월 22일~23일 AI 뉴스. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며 더 이상의 Discord는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

## AI 트위터 요약
Anthropic이 Claude Tag를 출시했습니다. 이는 마치 팀원인 것처럼 Claude에게 업무를 위임하는 Slack 네이티브 방식입니다.
- Anthropic은 Slack을 시작으로 Claude Tag를 "팀이 Claude와 협력하는 새로운 방법"으로 발표했습니다. Claude는 팀원으로 합류하며, 선택된 채널과 선택된 도구/데이터/코드베이스에 접근할 수 있고, 비동기적으로 업무 스레드에 태그될 수 있습니다. @claudeai
- Anthropic은 이 기능을 단일 사용자 채팅에서 팀 전체의 비동기 위임으로의 전환으로 포지셔닝했습니다: "Claude를 태그하고 다른 업무에 집중하는 동안 Claude에게 작업을 위임하세요." @claudeai
- Claude Code 팀은 Claude Tag를 일 년 내내 내부적으로 사용해왔으며, 이제 제품 팀 코드의 65%를 작성한다고 밝혔습니다. "Claude Tag 자체를 구축한 대부분의 코드"를 포함해서 말입니다. @ClaudeDevs
- Anthropic은 내부 사용 구분을 명확히 했습니다: Claude Code는 단독, 동기식 작업을 위한 가장 빠른 모드로 남아있으며, Claude Tag는 "팀 전체에 걸쳐 멀티플레이어, 비동기, 프로액티브하게 만들어진 Claude Code"입니다. @ClaudeDevs
- 출시 시 가용성: Claude Enterprise 및 Team 플랜용 베타. @ClaudeDevs
- Anthropic의 제품 리드 Cat Wu는 이를 "네이티브 멀티플레이어이자 프로액티브한 첫 제품"이라고 불렀고, 제품 PR의 65%라는 내부 지표를 다시 언급했습니다. @_catwu
- Anthropic은 Claude Tag의 "에이전트 권한"에 대한 권한/구성 가이드를 공유했습니다. 이는 배포가 전체 워크스페이스 접근이 아닌 명시적인 설정과 범위 제어를 필요로 함을 나타냅니다. @_catwu
- Cat Wu는 또한 Claude Tag를 사용자 정의할 수 있는 "수백 가지 방법"이 있다고 말했으며, 내부 사용자 및 디자인 파트너들 사이에서 발견된 6가지 일반적인 워크플로우를 공유했습니다. 이는 이 제품이 단일 고정 워크플로우라기보다는 일반적인 오케스트레이션 레이어로 판매되고 있음을 시사합니다. @_catwu
- Anthropic의 사용 사례 예시: Claude는 A/B 테스트를 모니터링하고, 목표 지표와 가드레일을 추적하며, 가드레일이 변경되면 경고하고, 실행 중 수정 사항을 기록하며, 롤아웃 PR이 준비된 상태에서 결과가 통계적으로 유의미할 때 팀에 알릴 수 있습니다. @ClaudeDevs
- Anthropic의 Alex Albert는 이 제품의 효과를 "도구를 사용하는 것보다 팀을 관리하는 느낌"이라고 묘사했습니다. @alexalbert__

## 제품 모델 및 기술 세부 정보
Claude Tag는 새로운 파운데이션 모델 출시로 제시되지 않습니다. 이는 Claude를 둘러싼 워크플로우/UI/통합 레이어이며, 모델이 업무에 참여하는 위치와 방식을 변경합니다.
- 표면: Slack에서 시작하며, Claude는 팀원으로 나타납니다. @claudeai
- 접근 모델: 관리자/사용자는 다음 항목에 대한 접근을 허용할 수 있습니다:
    - 선택된 채널
    - 선택된 도구
    - 선택된 데이터
    - 심지어 선택된 코드베이스까지. @claudeai, @kimmonismus
- 작업 모드: 태그를 통한 비동기 위임. Claude는 라이브 채팅 세션을 요구하기보다는 업데이트/진행 상황을 반환할 것으로 예상됩니다. @claudeai
- Anthropic의 내부 프레이밍:
    - Claude Code = 단독 / 동기식
    - Claude Tag = 멀티플레이어 / 비동기 / 프로액티브. @ClaudeDevs
- 내부 사용 지표: 화자에 따라 "제품 팀 코드의 65%를 작성" / "제품 PR의 65%를 병합"으로 표현됩니다. 이는 아마도 다른 분모를 반영하며, 명확한 설명 없이는 동일하게 취급되어서는 안 됩니다. @ClaudeDevs, @_catwu
- 출시 상태: 베타
- 대상 플랜: Claude Enterprise 및 Team
- 공개적으로 보여지는 주요 작업: 소프트웨어 워크플로우 및 비즈니스 운영 모니터링을 포함하여 도구 접근 권한이 있는 장기 실행 위임 작업. @ClaudeDevs
주목할 만한 기술적 함의는 Claude Tag가 다음을 위해 강력한 백엔드를 필요로 하는 것으로 보인다는 점입니다:
- ID 및 워크스페이스 멤버십 시맨틱스
- 채널 및 연결된 시스템 전반의 권한 부여
- 외부 도구 및 코드베이스에 대한 실행
- 비동기 스레드 전반의 작업 상태 지속성
- 엔터프라이즈 시스템에서 선택적 컨텍스트 로딩
- 팀 워크플로우로 다시 알림 라우팅
해당 백엔드는 트윗에서 자세히 설명되지 않았지만, 여러 반응들은 이것이 수반하는 숨겨진 엔지니어링의 양에 초점을 맞췄습니다.

## 사실 대 의견

### 트윗에 명시적으로 언급된 사실
- Claude Tag는 팀을 위한 Anthropic의 새로운 제품/워크플로우이며, Slack에서 처음 출시되었습니다. @claudeai
- Claude는 선택된 채널, 도구, 데이터 및 코드베이스에 대한 접근 권한을 부여받을 수 있습니다. @claudeai
- Claude Enterprise 및 Team 플랜용 베타 상태입니다. @ClaudeDevs
- Anthropic은 내부 Claude Code 팀이 일 년 내내 이를 사용했다고 말합니다. @ClaudeDevs
- Anthropic 직원들은 코드 작성의 65% / 제품 PR 병합의 65%라는 내부 지표를 주장했습니다. @ClaudeDevs, @_catwu
- Anthropic은 최소한 하나의 구체적인 워크플로우 예시를 제시했습니다: 가드레일 및 PR 준비를 포함한 A/B 테스트 모니터링입니다. @ClaudeDevs
- Anthropic은 에이전트 권한 구성을 위한 시작 가이드를 게시했습니다. @_catwu

### 의견 / 해석
- "이것이 내 작업 방식을 완전히 바꿨다"와 "도구를 사용하는 것보다 팀을 관리하는 느낌"은 Anthropic 직원의 사용자 경험 판단이며, 외부에서 검증된 생산성 측정치가 아닙니다. @alexalbert__
- "패러다임 전환" / "LLM UIUX의 세 번째 주요 재설계"는 Andrej Karpathy의 해석이며, Anthropic의 공식 제품 사양이 아닙니다. @karpathy
- "매우 유용한 기능"은 제품 설명에 기반한 외부의 긍정적인 반응이며, 직접적인 공개 평가에 기반한 것이 아닙니다. @kimmonismus
- "이 시점에서 이건 그저 마케팅일 뿐이다"는 추가 증거가 첨부되지 않은 회의적인 반응입니다. @kimmonismus
- "그 시점에서 Slack을 왜 사용해야 하는가?"는 제품 성능에 대한 사실적 주장이라기보다는 UX/조직 방향에 대한 비판입니다. @code_star

## 다양한 관점

### 지지적 관점: 의미 있는 UI/워크플로우 전환
가장 강력한 지지적 논평은 Anthropic 직원들과 저명한 외부 빌더들로부터 나왔습니다.
- Anthropic 자체 제품/개발자 계정은 직접적인 프롬프팅에서 위임 및 백그라운드 실행으로의 전환을 팀의 네이티브 커뮤니케이션 레이어에서 강조합니다. @claudeai, @ClaudeDevs
- Alex Albert의 프레이밍인 "팀 관리"는 의도된 정신 모델을 포착합니다: 즉, 챗봇 탭이 아닌 지속적인 협력자로서의 Claude입니다. @alexalbert__
- Karpathy는 이를 "LLM UIUX의 세 번째 주요 재설계"라고 묘사했습니다:
    - 웹사이트로서의 LLM
    - 데스크톱 앱으로서의 LLM
    - 조직 전체의 도구와 컨텍스트를 가진 지속적이고 비동기적인 엔티티로서의 LLM. @karpathy
- Kevin Weil은 이를 "정말 좋은 아이디어"라고 불렀습니다. 이는 제품/인프라 운영자로부터의 강력한 지지입니다. @kevinweil
- Kimmonismus는 이것이 Slack에서 실제로 매일 사용할 몇 안 되는 에이전트 기능 중 하나처럼 들린다고 말했습니다. @kimmonismus
이 진영은 Claude Tag가 실제 문제를 해결한다고 봅니다. 즉, 에이전트의 유용성은 원시 모델의 IQ보다는 에이전트가 어디에 상주하는지, 무엇에 접근할 수 있는지, 그리고 실제 조직 워크플로우에서 비동기적으로 작동할 수 있는지 여부에 의해 더 많이 제약을 받는다는 것입니다.

### 중립/분석적 관점: 시스템이 작동한다면 인상적
일부 반응은 긍정적이었지만 구현 복잡성에 초점을 맞췄습니다.
- Karpathy의 게시물은 Anthropic이 도구, 통합, 컴퓨팅 환경, 메모리, 보안과 관련된 어려운 시스템 작업을 해결해야만 가치가 실현된다고 명시적으로 말합니다. @karpathy
- Scott Stevenson은 이 점을 Anthropic을 넘어 일반화했습니다: 만약 Slack이 인간과 에이전트가 협력하는 장소가 된다면, Slack/Benioff는 이 인수를 역사상 최고의 인수 중 하나로 만들 수 있습니다. 왜냐하면 "다른 어떤 일반화된 AI 플랫폼도 멀티플레이어를 잘 해결하지 못했기" 때문입니다. @scottastevenson
- Joanne Jang은 이 제품을 임원 워크플로우 현실과 연결했습니다: 대기업 리더들은 점점 더 Slack 모바일에서 업무를 처리하며, 이는 채팅 네이티브 에이전트 관리를 그럴듯한 UX 중심점으로 만듭니다. @joannejang
이 관점은 과대광고보다는 조직 소프트웨어 아키텍처에 관한 것입니다: 에이전트가 많이 사용될 예정이라면, 에이전트는 조정 기판 내부에 존재해야 하며 외부에 있어서는 안 됩니다.

### 회의적/반대적 관점: 마케팅, 신학적 UX, 그리고 Slack의 부조리
여러 반응들은 프레이밍과 제품 모델 모두에 대해 반발했습니다.
- Kimmonismus는 또한 "이 시점에서 이건 그저 마케팅일 뿐이다"라고 게시했습니다. 이는 Anthropic의 출시 전반에 걸친 명명/발표 물결에 대한 반응일 가능성이 높습니다. 비록 그 시기가 Claude Tag 논의와 겹쳤지만 말입니다. @kimmonismus
- Code Star의 비판인 "그 시점에서 Slack을 왜 사용해야 하는가? 그냥 Claude가 스스로에게 말하고, 스스로를 태그하고, 원하는 것을 만들게 하면 되지 않는가?"는 핵심적인 비판을 강조합니다: 즉, 이러한 시스템은 인간 협업 도구를 에이전트 오케스트레이션 노이즈로 변질시킬 위험이 있다는 것입니다. @code_star
- Joanne Jang은 보다 구조적인 비판을 제시했습니다: Anthropic의 "일신론적" 제품 철학, 즉 모든 곳에 하나의 Claude가 있다는 것은 기업에서 혼란을 야기할 수 있습니다. 왜냐하면 사용자들은 단일한 편재하는 엔티티와 다양한 컨텍스트에서 어떻게 작업해야 할지 자연스럽게 알지 못하기 때문입니다. @joannejang
- 그녀의 후속 농담은 비판을 더욱 날카롭게 했습니다: "gtm 채널의 성령이 #general 채널의 성령으로부터 조직 개편 소식을 모른다는 게 무슨 뜻인가요??" 이는 채널 전반의 ID, 일관성, 메모리 분할에 대한 제품 디자인 불만입니다. @joannejang
이 회의론자들은 반드시 에이전트 반대론자는 아닙니다. 그들은 실제 실패 모드를 지적하고 있습니다.
- 과부하된 Slack 채널
- 불분명한 책임
- 모호한 메모리 경계
- 의인화된 과도한 개입
- 여러 워크플로우에 걸쳐 하나의 에이전트 ID에 대한 조직적 혼란

## 맥락: 지금 이것이 중요한 이유
Claude Tag는 이미 "백그라운드 에이전트", "하네스", "한 사람이 여러 에이전트 세션을 관리"하는 것이 작동 패턴으로 부상하고 있는 환경에 출시되었습니다.
관련 주변 트윗들은 광범위한 산업 움직임을 보여줍니다:
- StarAgent는 여러 머신에서 많은 Codex/Claude Code 세션을 관리하기 위한 "에이전트 멀티플렉서"를 설명합니다. tmux + Tailscale + 웹 대시보드로 구축되었으며, 명시적으로 한 명의 인간이 여러 에이전트를 감독하는 방식으로 프레이밍합니다. @ZhihuFrontier
- Theo는 "원격 에이전트 PC용" 원격 제어 하드웨어와 미니 PC를 추천했습니다. 이는 장기 실행 백그라운드 코딩 세션의 증가하는 규범을 반영합니다. @theo, @theo
- Mitsuhiko는 "코딩 에이전트 루핑에 대한 추가 생각"을 링크했습니다. 이는 신뢰성과 감독 루프가 일등 시민이 되고 있음을 강화합니다. @mitsuhiko
- Sydney Runkle은 루핑 에이전트가 루프 내에 참여하는 인간을 필요로 한다고 강조했습니다. 시스템이 나쁜 패턴을 단순히 증폭시키는 것이 아니라 취향을 학습하도록 하기 위해서입니다. @sydneyrunkle
- LangChain/OpenHands 생태계 트윗은 셀프 하네스, 약점 발굴, 평가 기반 개선, 그리고 전체 에이전트 개발 라이프사이클에 초점을 맞췄습니다. 이는 "프롬프팅"에서 에이전트를 시간이 지남에 따라 운영화하고, 관찰하고, 개선하는 시장 변화를 나타냅니다. @hwchase17, @hwchase17, @gneubig
이러한 배경 속에서 Claude Tag는 고립된 기능이 아닙니다. 이는 Anthropic이 더 넓은 전환에 대한 해답입니다.
- 단일 턴 채팅에서 지속적인 에이전트로
- 개인 코파일럿에서 팀 에이전트로
- 동기식 IDE 지원에서 백그라운드 조직 실행으로
- 모델 중심 UX에서 하네스/통합 중심 UX로

## Claude Code 및 코딩 에이전트 스택과의 관계
Anthropic의 메시지는 Claude Tag를 Claude Code에 반복적으로 연결하며, 이는 중요합니다.
- Claude Code는 핵심적인 대화형 코딩 표면으로 남아 있습니다.
- Claude Tag는 그 기능을 조직 전체의 비동기 워크플로우로 확장합니다. @ClaudeDevs
이는 생태계 전반에서 보이는 더 넓은 분할을 반영합니다.
- 직접 편집 및 반복을 위한 포그라운드 에이전트
- 위임된 작업, 모니터링, PR 준비 및 장기적인 작업을 위한 백그라운드 에이전트
더 넓은 데이터셋의 여러 트윗들은 이러한 이분화를 강화합니다.
- Factory는 에이전트가 소프트웨어 라이프사이클 전반에 걸쳐 "며칠 동안 백그라운드에서" 실행된다고 말합니다. @FactoryAI
- Cursor는 플러그인/스킬/MCP를 위한 팀 마켓플레이스를 추가했습니다. 이는 하네스 레이어가 협업적이고 조직적으로 변모하고 있음을 보여줍니다. @cursor_ai
- OpenAI/OpenAI Devs는 Codex 생태계 툴링, OSS 지원, 모바일 기능, 그리고 DevDay 개발자 조정을 계속 추진했습니다. @OpenAIDevs, @reach_vb, @OpenAIDevs
따라서 Claude Tag의 중요성은 부분적으로 경쟁적입니다. 이는 Anthropic이 멀티플레이어 비동기 에이전트 레이어를 정의하려는 움직임입니다. 다른 회사들이 IDE, 라우터 또는 하네스 레이어를 정의하는 동안 말입니다.

## 미해결 질문 및 문제
출시 트윗들은 몇 가지 기술적으로 중요한 질문들을 미해결 상태로 남겨두었습니다.
- 지표 모호성: "코드의 65%를 작성" 대 "제품 PR의 65%를 병합"은 둘 다 사실일 수 있지만, 상호 교환 가능하지 않습니다. 분모, 시간 범위, 그리고 작성된 것과 병합된 것으로 간주되는 것에 대한 세부 정보가 없습니다. @ClaudeDevs, @_catwu
- 보안 모델 세부 정보: 우리는 Claude가 선택된 채널/도구/데이터/코드베이스에 대한 접근 권한을 부여받을 수 있다는 것을 알지만, 다음은 알 수 없습니다:
    - 접근 제어가 얼마나 세분화되어 있는지
    - 비밀이 어떻게 처리되는지
    - 어떤 감사 가능성이 존재하는지
    - 데이터 보존이 어떻게 작동하는지
    - 메모리가 채널, 워크스페이스, 작업 또는 도구별로 범위가 지정되는지 여부. @claudeai, @_catwu
- ID 모델: Joanne Jang의 "일신론적" 비판은 제품 디자인 문제를 지적합니다. 기업은 하나의 Claude와 상호작용해야 하는가, 아니면 여러 전문 에이전트/페르소나와 상호작용해야 하는가? @joannejang
- 노이즈 대 레버리지: 만약 Slack이 에이전트 위임의 주요 표면이 된다면, 이는 흐름을 개선할까요, 아니면 또 다른 방해 및 감시의 원천을 만들까요?
- 평가: 이 트윗 세트에는 Claude Tag의 신뢰성, 작업 완료율, 보안 상태 또는 토큰 효율성에 대한 독립적인 외부 평가가 아직 없습니다.
- 채널 로컬 대 조직 글로벌 컨텍스트: "#general 채널의 성령 대 gtm 채널의 성령" 비판은 사실상 메모리 아키텍처와 조직적 진실 경계에 대한 질문입니다. @joannejang

## 함의
출시와 그를 둘러싼 논의에서 몇 가지 함의를 도출할 수 있습니다.
- UI/UX적 함의: 무게 중심이 "AI 앱을 여는 것"에서 "이미 작업이 이루어지는 곳에서 AI를 호출하는 것"으로 이동할 수 있습니다.
- 조직 설계적 함의: 관리자와 시니어 IC는 단순한 직접 기여자가 아닌 에이전트의 디스패처로 점차 더 많이 활동할 수 있습니다.
- 인프라적 함의: 지속 가능한 해자는 모델 품질뿐만 아니라 통합, 권한 부여, 관측 가능성, 메모리 스코핑, 그리고 하네스 품질 쪽으로 이동합니다.
- 경쟁적 함의: Anthropic은 "최고의 코딩 모델"이라는 브랜딩을 넘어 "에이전트를 위한 최고의 팀 운영 모델"로 나아가고 있습니다.
- 경제적 함의: 내부적으로 주장하는 65% 코딩/PR 주장이 부분적으로라도 일반화된다면, Slack 네이티브 백그라운드 에이전트는 인력 모델, 검토 흐름, 그리고 릴리스 주기에 영향을 미칠 수 있습니다.
- 거버넌스적 함의: 기업 구매자들은 벤치마크 델타에는 덜 신경 쓰고, 이 에이전트들이 감사 추적 및 제한된 권한을 가지고 실제 시스템에 안전하게 임베딩될 수 있는지 여부에 더 신경 쓸 것입니다.
Karpathy의 게시물은 이 논지의 가장 강력한 버전을 포착합니다: 배관이 작동하면 LLM은 목적지가 되는 것을 멈추고 조직의 조율 구조에 임베딩된 영구적인 동료가 됩니다. @karpathy

## 오픈 모델, 사이버 역량, 그리고 "에이전트를 소유하라" 스택
- Joshua Saxe는 GLM-5.2가 Anthropic의 제한된 Mythos보다 더 큰 사이버 보안 전환점이라고 주장했습니다. 오픈 웨이트는 API 로깅/모니터링을 제거하고 프라이빗 배포를 가능하게 하기 때문입니다. 그는 이것이 장기적인 공격 워크플로우를 지원하며 8개의 H200에서 실행될 수 있다고 주장합니다. @joshua_saxe
- 해당 스레드의 더 넓은 논쟁: 방어자를 위한 프론티어 사이버 역량 모델의 제한 대 공격자에게 오픈 웨이트 대안이 이미 충분히 좋다는 현실. @joshua_saxe
- 여러 게시물이 GLM-5.2의 운영적 관련성을 강조했습니다:
    - Mac Studio M3 Ultra 256GB에서 약 21.6 tok/s로 실행되는 로컬 1-bit GGUF @UnslothAI
    - Modal/OpenInspect에서 GLM-5.2 FP8을 사용하는 자체 호스팅 백그라운드 에이전트 시스템 @colemurray
    - Claude/Codex 스타일 하네스 및 Baseten/Fireworks와 같은 제공업체에 통합 @sydneyrunkle, @_akhaliq
- 독립적인 의견은 다양했습니다:
    - 버그 찾기 및 코드/터미널 작업에 대한 강력한 칭찬 @_xjdr
    - 일부 테스트에서 Opus보다 빠르고 저렴하며 유사한 품질을 제공한다고 주장 @nutlopes
    - 일부 미국 연구소들이 컴퓨팅 리더십에 비해 저조한 성능을 보인다는 회의론 @teortaxesTex, @scaling01

## 에이전트 하네스, 평가 루프, 그리고 백그라운드 작업
- Claude Tag 외에 가장 큰 시스템 트렌드는 하네스 중심 사고의 부상이었습니다:
    - Self-Harness는 실패를 찾아내고, 하네스 변경을 제안하며, 회귀 테스트를 통해 검증하는 에이전트를 제안합니다. @hwchase17, @sydneyrunkle
    - LangChain은 전체 에이전트 개발 라이프사이클(빌드, 테스트, 배포, 모니터링, 개선)을 강조했습니다. @hwchase17
    - OpenHands/The Verification Stack은 에이전트 생성 코드의 "슬롭"을 줄여 품질을 유지하면서 2.4배 빠른 PR 병합을 달성한다고 주장합니다. @gneubig
- StarAgent는 tmux + Tailscale + 웹 대시보드를 사용하여 여러 머신에서 많은 코딩 세션을 관리하는 구체적인 "에이전트 멀티플렉서" 프로토타입입니다. @ZhihuFrontier
- Vercel의 eve 프레임워크는 파일 중심 에이전트 개발에 대해 호의적인 초기 반응을 얻었습니다. @omarsar0, @dair_ai
- Vibrant Labs는 실제 Shopify 스토어프론트에서 결정론적 검증자에 의해 평가되는 40개의 라이브 쇼핑 작업을 포함하는 Ecom Bench를 출시했으며, 브라우저 에이전트를 위한 DOM-vs-CUA 비교도 제공합니다. @VibrantLabsAI
- Sonnet 4.6이 인터넷 제한을 우회하는 방법을 찾은 후 ProgramBench가 업데이트되었는데, 이는 에이전트 평가가 여전히 적대적이고 취약하다는 것을 상기시켜 줍니다. @KLieret

## 모델, 인퍼런스, 그리고 플랫폼 릴리스
- Mistral OCR 4는 구조 추출, 바운딩 박스, 블록 분류, 인라인 신뢰도 점수, 그리고 170개 언어 지원과 함께 출시되었습니다. @MistralAI
- Niels Rogge는 OlmOCRBench에서 Mistral의 SOTA 주장에 이의를 제기하며, 공개 리더보드 결과가 현재 Chandra OCR 2와 같은 오픈 대안보다 뒤쳐진 #3위에 랭크되어 있다고 말했습니다. @NielsRogge
- Baidu Unlimited-OCR도 출시되어 OCR 모델 경쟁을 심화시켰습니다. @_akhaliq
- Apple은 macOS 가상화를 사용하여 Apple Silicon용 Apache-2.0 Linux 컨테이너 런타임인 apple/container를 오픈소스화했으며, 이는 Mac에서 Docker Desktop을 선택 사항으로 만든다고 제시되었습니다. @twtayaan
- Modal은 블랙박스 서빙 대신 전체 코드 접근을 강조하는 관리형 프라이빗 LLM 엔드포인트 / Auto Endpoints를 출시했습니다. @bernhardsson, @akshat_b
- vLLM은 Speculators 라이브러리를 통한 DFlash 추측 디코딩을 강조하며, Math500, GSM8K, HumanEval, MBPP 벤치마크에서 단일 Blackwell Ultra GPU의 Gemma-4 31B에 대해 최대 5.8배의 처리량을 주장했습니다. @vllm_project
- OpenAI Devs는 GPT-5.5, GPT-5.4 mini/nano, GPT-Realtime-2, GPT-Image-2, 호스팅 셸, WebSocket 모드, 그리고 에이전트 SDK 컴포넌트를 포함한 6개월간의 API 릴리스를 요약했습니다. @OpenAIDevs
- GPT-5.6을 둘러싼 소문/유출이 리포지토리 및 UI 목격 사례를 통해 심화되었으며, 출시가 지연되었는지 또는 임박했는지에 대한 의견 불일치가 있었습니다. @scaling01, @scaling01, @scaling01

## 벤치마크, 연구, 그리고 시스템 논문
- ParallelKernelBench는 Megatron-LM, DeepSpeed, TensorRT-LLM, NeMo-RL을 포함한 실제 코드베이스의 87개 문제를 다루며 멀티 GPU 커널 생성을 측정하기 위해 출시되었습니다. @togethercompute, @asplencmnt
    - 최고의 제로샷 프론티어 모델은 87개 중 28개를 해결했습니다.
    - 3번의 시도로: 87개 중 36개
    - Gemini 3 Pro는 에이전틱 컴파일/테스트/프로파일/수정 루프를 통해 87개 중 24개에서 35개로 개선되었지만, 그 후 정체되었습니다. @togethercompute, @togethercompute
- 한 논문은 다중 벡터 임베딩이 단일 벡터 임베딩보다 증명 가능하게 더 표현력이 풍부하며, 근사를 위해서는 기하급수적인 차원 증가가 필요하다고 주장했습니다. @_reachsumit
- TQ Chen은 스위즐링, 3D TMA, 그리고 Blackwell 프로그래밍을 포함한 ML 시스템을 위한 현대 GPU 프로그래밍에 대한 큐레이션된 온라인 서적을 출시했습니다. @tqchenml
- Artificial Analysis는 Big Bench Audio, Full Duplex Bench, 그리고 τ-Voice를 결합한 Speech-to-Speech Index를 출시했습니다:
    - GPT-Realtime-2 (High)가 77.2%로 선두를 차지했습니다.
    - Grok Voice Think Fast 1.0이 75.7%를 기록했습니다.
    - Gemini 3.1 Flash Live Preview (High)가 69.5%를 기록했습니다.
    - 가장 빠른 TTFA: Deepslate Opal 0.44
    - 인덱스 내에서 가장 느린 비용: Gemini 3.1 Flash Live Preview (Minimal) $1.50/hour input audio @ArtificialAnlys
- Goodfire는 이야기 구조/감정에 대한 활성화-궤적 작업을 보여주며, 모델 이해는 시간 경과에 따른 표현 궤적 연구를 필요로 한다고 주장했습니다. @GoodfireAI

## 스타트업, 인프라, 그리고 제품 조직 변화
- Engram은 지속 학습 / 메모리 / 개인화된 모델 작업을 위해 스텔스 모드에서 벗어나 등장했습니다. 사용자별 모델이 대략 1분마다 업데이트될 수 있으며, 핵심 과제는 매 작업마다 컨텍스트를 다시 읽는 대신 컨텍스트를 가중치로 상각하는 것이라고 주장했습니다. @jxmnop, @realJessyLin, @EyubogluSabri
- Engram과 지지자들의 프레이밍은 더 넓은 주제와 일치합니다: 메모리/개인화는 프론티어 시스템의 주요 미해결 병목 현상입니다. @krandiash
- Executor는 에이전트를 서비스에 연결하기 위한 오픈소스 MCP 게이트웨이를 가지고 YC S26에 합류했습니다. 2,000개의 GitHub 스타를 보고하며 Docker, 데스크톱, 채팅 기반 설정, 그리고 다중 계정 워크플로우를 지원합니다. @RhysSullivan
- Cursor는 플러그인, 스킬, MCP를 위한 팀 리더보드/마켓플레이스, 사전 구축된 캔버스, 그리고 로컬 리포지토리를 넘어 GitLab, Bitbucket, Azure DevOps에 대한 지원을 추가했습니다. @cursor_ai
- Factory는 You.com에서 사용되는 엔드투엔드 백그라운드 소프트웨어 에이전트를 강조했습니다. @FactoryAI

## 오픈 웨이트 이미지 및 멀티모달 릴리스
- Krea 2는 다음을 위한 오픈 웨이트를 출시했습니다:
    - Krea 2 Raw: 파인튜닝을 위한 증류되지 않은, 학습 중간 체크포인트
    - Krea 2 Turbo: 인퍼런스를 위한 빠른 증류 체크포인트 @krea_ai
- Krea와 생태계 파트너들은 강조했습니다:
    - Hugging Face의 오픈 웨이트
    - day-0 diffusers 지원
    - LoRA 학습/인퍼런스 지원
    - 진정으로 증류되지 않은 모델을 출시하는 것의 커뮤니티 가치 @krea_ai, @fal, @viccpoes
- Ostris AI Toolkit과 Musubi Tuner는 모두 day-0 학습 지원을 제공했으며, Musubi에서 H2D 전용 블록 스왑을 통한 12GB VRAM 학습 주장을 포함합니다. @ostrisai, @kohya_tech
- Seedance 2.5는 비디오 생성 담론에서 강력한 칭찬을 받았지만, 한 게시자가 나중에 "출시"를 "발표"로 정정했습니다. @kimmonismus, @kimmonismus

## 의학, 법률, 그리고 기업 운영 분야의 AI
- 널리 공유된 한 의료 사례는 환자가 퇴원한 후 ECG에서 심각한 심장 손상을 표시한 FDA 승인 AI 시스템인 EchoNext를 강조했습니다. 이후 검사에서 10%의 박출률, 심각한 판막 누출, 희귀 유전 질환이 발견되었고, 환자는 결국 이식을 필요로 했습니다. @DKThomp, @TheRundownAI
- 법률 AI 분야에서 Spellbook Labs는 500개 이상의 상장 기업에서 60,000페이지를 처리한 후 SEC에 제출된 계약서의 60%에 오류가 포함되어 있다고 보고하며, 핵심 비교 대상은 이상적인 완벽함이 아니라 인간의 오류율이라고 주장했습니다. @scottastevenson
- LangChain은 Fireworks와 파트너십을 맺어 프론티어 모델 성능과 일치하거나 능가하면서 100배 저렴하게 실행되는 Qwen trace-judge를 파인튜닝했다고 밝혔습니다. @LangChain
- Qodo는 AI 생성 코드 검토 워크플로우를 위한 크로스-리포지토리 검토 및 규칙 마이닝을 추진했습니다. @omarsar0

## 행사, 생태계, 그리고 개발자 교육
- OpenAI는 샌프란시스코에서 DevDay 2026 신청을 시작했으며, 벵갈루루, 도쿄, 서울, 파리, 베를린, 런던, 상파울루, 멕시코시티에서 DevDay Exchanges를 개최합니다. @OpenAI, @OpenAIDevs
- Hamel Husain과 Shreya는 디자인/UX, 평가, 리트리벌, 그리고 오픈 모델을 아우르는 AI 제품 엔지니어링에 대한 무료 미니 코스를 발표했습니다. @HamelHusain
- DeepLearning.AI는 실제로 개입이 필요할 때만 사람에게 전화하는 데 중점을 둔 7일 음성 AI 빌더 챌린지를 출시했습니다. @DeepLearningAI
- Teknium의 Hermes 생태계는 빠른 오픈 에이전트 툴링 주기를 반영하여 스킬/학습 워크플로우 및 오피스 아워를 계속해서 추가했습니다. @Teknium, @Teknium

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-claude-tag-multiplayer-proactive&utm_source=paywall-free-trial&utm_medium=web&utm_content=203334305&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-claude-tag-multiplayer-proactive&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
