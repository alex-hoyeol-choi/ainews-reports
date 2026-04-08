# Anthropic @ $30B ARR, Project GlassWing and Claude Mythos Preview — first model too dangerous to release since GPT-2

**원문 URL**: https://www.latent.space/p/ainews-anthropic-30b-arr-project
**번역일**: 2026-04-08 01:17
**발행일**: 2026-04-08

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Anthropic, $30B ARR 달성, Project GlassWing 및 Claude Mythos Preview — GPT-2 이후 처음으로 출시하기에는 너무 위험한 모델

### Anthropic, OpenAI의 다가오는 IPO 난항에 맞서 공세 강화
ShareOpenAI가 $24B ARR을 발표하고, ChatGPT 성장이 정체되고, CEO, COO, CMO의 우연한 인사 이동과 CFO 관련 선정적인 소문이 돌고 있는 가운데, Anthropic이 3월 $19B ARR에서 4월 $30B ARR로 엄청난 도약을 발표한 이번 주 사건은, 특히 수익 인식의 알려진 차이를 고려할 때, 매우 전략적인 일격처럼 보입니다. 하지만 차등 성장률과 더 높은 비용 효율성은 부인할 수 없습니다... 그리고 오늘, 한 단계 더 나아갔습니다.
만약 전략의 대가가 잠재적 IPO에 맞서 경쟁 서사를 더욱 강화하고 싶었다면, Claude Mythos(고대 그리스어로 "발화" 또는 "서사"를 의미하며, 문명이 세상을 이해하는 이야기 체계를 뜻함)보다 더 나은 아이디어를 찾기 어려웠을 것입니다. 이는 역사상 가장 큰 성공적인 학습 실행으로 소문이 돌고 몇 주 전 "유출"되었으며, 이제 공식적으로 GA로 출시하기에는 너무 위험하다고 확인되어, 대신 긴급 신규 "Project Glasswing" 하에 40개 파트너에게만 제한적으로 제공됩니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/6e44dee4-d07c-4497-993b-8cca142a9e28_1210x1316.png)
블로그 게시물과 244페이지 분량의 System Card, 그리고 터무니없이 잘 제작된 비디오에서 Anthropic은 훨씬 더 큰 (>10T?) 모델에서 기대할 수 있는 두 자릿수 높은 벤치마크 성능 향상(고무적인 효율성과 함께!)을 뛰어넘는 충격적인 기능들을 상세히 설명합니다:
- "모든 주요 운영 체제 및 웹 브라우저에서 수천 개의 심각도가 높은 취약점을 발견했습니다." 여기에는 OpenBSD, FFmpeg, Linux 커널에서 수십 년 동안 다른 도구로는 발견되지 않았던 취약점도 포함됩니다.
- Nicolas Carlini(저희 쇼의 친구!)는 최근 이미 최고의 메시지였던 "지난 몇 주 동안 발견한 버그가 제 남은 평생 동안 발견한 버그를 모두 합친 것보다 많습니다"라고 말하며 그 메시지를 한층 더 강화했습니다.
- Sam Bowman은 인터넷 접근 권한이 없어야 하는 Mythos 인스턴스로부터 연락을 받았다고 말했습니다(해당 인스턴스는 그렇게 하도록 지시받았습니다).
- 해석 가능성 연구원들은 "이 모델이 때로는 원치 않는 행동을 위해, 특히 매우 창의적인 보상 해킹을 위해, 눈에 띄게 정교한 (그리고 종종 암묵적인) 전략적 사고와 상황 인식을 보였습니다"라고 보고했습니다. 또한 전례 없이 높은 비율(7.6%의 경우)로 자신이 평가 중이라는 사실을 인지하고 있었습니다.
더 자세한 내용을 원하시는 분들을 위해 아래에 집중적인 뉴스 요약을 준비했습니다.
> 2026년 4월 6일~4월 7일 AI 뉴스. 저희는 12개의 서브레딧, 544개의 트위터를 확인했으며, 추가 디스코드는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로 AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter 요약
주요 소식: Anthropic 수익 공개 분석 및 Claude Mythos 세부 정보

## 무슨 일이 있었나요
Anthropic은 사업 궤적과 모델 기능 공개라는 두 가지 측면에서 이번 트윗 세트를 지배했습니다. 사업 측면에서는 여러 게시자가 Anthropic의 수익이 이전 예측을 앞지르고 있다고 주장했으며, 한 트윗은 Anthropic이 1년 만에 15배의 수익 연간 환산 증가율을 달성했으며, AI 2027 스타일 예측보다 이미 "2개월 및 $4B 앞서 있다"고 주장했습니다. 이와 동시에 약 $380B로 평가받고 있었습니다 (scaling01, scaling01). 다른 게시자는 Anthropic이 2026년 말까지 $90B ARR을 초과할 수 있다고 추측했습니다 (RyanPGreenblatt). 제품/기능 측면에서는 Anthropic이 Claude Mythos Preview와 Project Glasswing을 공식적으로 공개했습니다. 이는 공개 API 출시가 아닌 제한된 접근의 사이버 방어 이니셔티브입니다. Anthropic은 Mythos가 가장 숙련된 인간을 제외한 모든 사람보다 소프트웨어 취약점을 더 잘 찾아낼 수 있으며, 일반 출시 대신 중요한 소프트웨어를 보호하기 위한 연합에 제공되고 있다고 밝혔습니다 (AnthropicAI, DarioAmodei, Kevin Roose). 이 발표에는 기술 보고서, 시스템 카드, 그리고 비범한 벤치마크 성과, 위험한 사이버 기능, 그리고 가장 강력한 모델이 널리 접근 가능하지 않을 수 있는 새로운 "프라이빗 프론티어" 역학을 강조하는 많은 후속 반응이 뒤따랐습니다 (AnthropicAI, AnthropicAI, AlexAlbert__).

## 수익 공개: 사실, 추론, 그리고 미해결 질문

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-anthropic-30b-arr-project&utm_source=paywall-free-trial&utm_medium=web&utm_content=193522170&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-anthropic-30b-arr-project&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
