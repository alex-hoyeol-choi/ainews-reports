# SpaceXAI launches Grok 4.5, first Opus-class model post Cursor acquisition

**원문 URL**: https://www.latent.space/p/ainews-spacexai-launches-grok-45
**번역일**: 2026-07-09 06:53
**발행일**: 2026-07-09

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] SpaceXAI, Cursor 인수 후 첫 Opus-클래스 모델 Grok 4.5 출시

### SpaceXAI는 지구상의 어떤 프론티어 랩보다 빠르게 움직이고 있습니다.
ShareGPT 5.6이 내일 출시될 예정인 가운데, 오늘은 GPT 5.5 동급 모델 출시에 사람들이 흥분할 수 있는 거의 마지막 날입니다. 그리고 SpaceXAI가 바로 그렇게 했습니다.

![X avatar for @cursor_ai](https://pbs.substack.com/profile_images/1970182748146180096/dhZeXi_X.jpg)
새로운 Grok 4.5는 Composer 시리즈(1.5T)와는 다른 웨이트 클래스이며, 견고한 평가에도 불구하고 현재 주력 모델인 Opus 및 GPTs와 매우 유사한 성능을 보입니다. OpenAI의 평가팀에 따르면 강력한 SWE-Bench Pro조차 이제 포화 상태이거나 치명적인 결함이 있어, FrontierCode를 포함한 소수의 후속 모델만 남게 될 것으로 보입니다.
학습 및 데이터 공개에 관해서는 이것이 저희가 가진 모든 정보입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/3dad0acc-e1ba-4ce4-9196-4ea6e56633a0_1628x1726.png)
> 2026년 7월 7일~7월 8일 AI 뉴스. 저희는 12개 서브레딧, 544개 트위터를 확인했으며 더 이상 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션임을 알려드립니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter Recap
주요 소식: Grok 4.5 출시

## 무슨 일이 있었나
xAI/"SpaceXAI"는 새로운 코딩 및 에이전트 중심의 프론티어 모델인 Grok 4.5를 공개적으로 출시했습니다. 이 모델은 절대적인 벤치마크 우위보다는 달러당 성능에 중점을 두었습니다.
- Elon Musk는 강력한 베타 피드백을 바탕으로 Grok 4.5가 "내일" 공개될 것이라고 처음 밝혔으며, 이를 "Opus-클래스"이지만 더 빠르고, 토큰 효율적이며, 저렴하다고 언급했습니다 @elonmusk.
- Musk는 나중에 Grok 4.5를 내부적으로 "Opus 4.7과 거의 비슷하지만 훨씬 빠르다"고 설명하면서, 벤치마크 추구보다는 Tesla 및 SpaceX 엔지니어들에게 유용성을 강조했습니다 @elonmusk.
- 공식 출시는 xAI 계정에서 이루어졌으며, Grok 4.5를 "코딩 및 에이전트를 위해 특별히 학습된 우리의 첫 모델"로, Cursor와 함께 학습되었으며 "선도적인 속도와 비용 효율성으로 프론티어 인텔리전스를 제공한다"고 설명했습니다 @SpaceXAI.
- Cursor는 xAI와 협력하여 Grok 4.5를 학습시켰다고 밝히며, 이를 "우리의 가장 강력한 모델"이라고 부르고 "소프트웨어 엔지니어링 이상을 위해 구축한 첫 모델"임을 강조했습니다 @cursor_ai.
- Cursor는 또한 "첫 주 동안 두 배 사용량"으로 제품 내 사용 가능성을 발표했습니다 @cursor_ai.
- Cursor는 "Grok 4.5와 Composer는 두 가지 다른 모델 웨이트 클래스"이며, Composer 2.5는 해당 더 작은 클래스의 향후 모델과 함께 계속 사용할 수 있을 것이라고 명확히 했습니다 @cursor_ai.
- 초기 생태계 지원이 즉시 나타났습니다: Grok 4.5는 Grok Build/API/Cursor에서 사용 가능해졌고 @milichab, Hermes Agent에 대한 출시 당일 지원이 발표되었으며 @Teknium, 나중에 Hermes Agent/Portal/OpenRouter/Grok 구독에서 실시간 사용 가능성이 확인되었습니다 @Teknium.
- Musk는 컨텍스트 윈도우가 "다음 주까지" 500k에서 1M으로 다시 이동할 가능성이 있다고 말했습니다 @elonmusk.

## 공식 주장 및 제품 세부 정보

### 포지셔닝
공식적으로 xAI의 메시지는 "최고의 종합 모델"이 아니라, Opus에 근접한 품질에 실질적으로 더 나은 경제성과 속도를 제공한다는 것이었습니다.
- "Opus-클래스 모델이지만 더 빠르고, 토큰 효율적이며, 저렴합니다" @elonmusk
- "코딩 및 에이전트를 위해 특별히 학습된 첫 모델" @SpaceXAI
- "선도적인 속도와 비용 효율성으로 프론티어 인텔리전스 제공" @SpaceXAI
- "가장 강력한 모델"이자 "소프트웨어 엔지니어링 이상을 위해 구축한 첫 모델" @cursor_ai
이러한 프레이밍은 중요합니다. xAI는 단순히 일반 채팅이 아니라, 최근 Anthropic/OpenAI/Cursor 스타일의 도구 사용 시스템이 지배해 온 코딩-에이전트 워크플로우 시장을 명확히 목표로 하고 있습니다.

### 가격 및 컨텍스트
밝혀진 구체적인 수치:
- 공식 가격: 입력 토큰 1M당 $2, 출력 토큰 1M당 $6 @scaling01
- Artificial Analysis는 동일한 가격대를 반복하며 다음과 같이 덧붙였습니다:캐시 히트는 75% 할인되어 토큰 1M당 $0.5200k 토큰을 초과하는 긴 입력은 두 배의 비용Grok 4.3의 1M에서 감소한 500k 컨텍스트 윈도우비전 입력 유지구성 가능한 추론 유지 @ArtificialAnlys
- Musk는 나중에 컨텍스트 윈도우가 곧 1M으로 다시 업그레이드될 것이라고 말했습니다 @elonmusk.
사용자들이 언급한 상대적 가격 비교:
- Grok 4.5: 입력 $2 / 출력 $6
- GPT-5.6: 입력 $5 / 출력 $30
- Opus 4.8: 입력 $5 / 출력 $25 @kimmonismus

### 모델 크기
Musk의 공개를 통해 제3자 보고서에서 밝혀진 한 가지 중요한 사양:
- Grok 4.5는 Grok 4.3보다 3배 큰 1.5T 파라미터입니다 @ArtificialAnlys
이는 주목할 만한 도약이며, 여러 관찰자들이 4.5를 반복적인 새로고침이 아닌 xAI의 진정한 플래그십 코딩-에이전트 티어 진입으로 해석한 핵심 이유일 것입니다.

## 벤치마크 및 독립 평가

### Artificial Analysis
Artificial Analysis는 트윗 세트에서 가장 실질적인 외부 평가를 제공했습니다.
주요 결과:
- Artificial Analysis Intelligence Index에서 54점으로 4위, Fable 5, GPT-5.5, Opus 4.8에 이어 @ArtificialAnlys
- 동일 인덱스에서 Grok 4.3 대비 16점 상승 @ArtificialAnlys
- GDPval-AA v2 Elo 1543점, 역시 4위로 Anthropic의 최신 Claude 릴리스에 이어 @ArtificialAnlys
- τ³-Banking에서 최고 점수 33%, GPT-5.5(xhigh)의 31%보다 높음 @ArtificialAnlys
- Grok Build에서 Artificial Analysis Coding Agent Index 점수 76점, "Codex의 GPT-5.5와 동등"하며 Claude Code의 Fable 5보다 낮음 @ArtificialAnlys
- Intelligence Index 작업당 비용: $0.31 @ArtificialAnlys
- GDPval 작업당 비용: $0.49 @ArtificialAnlys
- Coding Agent Index 작업당 비용: $2.59 @ArtificialAnlys
- Intelligence Index 작업당 평균 출력 토큰: 약 14k, Opus 4.8보다 60% 이상 낮음 @ArtificialAnlys
- Coding Agent Index 작업당 평균 총 토큰: 1.9M, Claude Code의 Fable 5는 7.2M, Codex의 GPT-5.5는 6.2M @ArtificialAnlys
Artificial Analysis의 해석은 명확했습니다: Grok 4.5는 성능 면에서 프론티어에 근접하지만, 효율성 면에서 이례적으로 강력하여 비용/성능의 파레토 프론티어에 위치합니다.
Musk는 Artificial Analysis의 평가를 명시적으로 강조했습니다 @elonmusk.

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-spacexai-launches-grok-45&utm_source=paywall-free-trial&utm_medium=web&utm_content=206247062&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-spacexai-launches-grok-45&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
