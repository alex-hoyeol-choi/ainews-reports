# Claude Fable/Mythos 5.1: new SOTA model, 75% cache price cut but 70% more output tokens

**원문 URL**: https://www.latent.space/p/ainews-claude-fablemythos-51-new
**번역일**: 2026-09-02 12:19
**발행일**: 2026-09-02

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Claude Fable/Mythos 5.1: 새로운 SOTA 모델, 캐시 가격 75% 인하, 그러나 출력 토큰 70% 증가

### 늘 그렇듯 모델 출시가 봇물 터지듯 이어지고 있습니다...
2026년 9월 2일 공유
Astra가 마침내 본격적인 출시를 위해 예열하고 있는 것이 분명해 보입니다 (@sama와 OpenAI가 한 달간 자체적으로 속도 조절을 한 후 다시 이에 대해 글을 쓰고 있습니다). Grok 4.7과 Gemini Flash 3.8도 출시를 앞두고 있는 가운데, 모델 출시의 라운드 로빈 속에서 주도권을 잡으려는 익숙한 움직임이 있습니다. 하지만 오늘 출시된 모델을 설명하는 가장 좋은 방법은 아닐 수도 있습니다. 이 모델은 기존 세계 최고 모델을 다시 한번 업데이트하며 1,200만 회 이상의 조회수를 기록했습니다.

![X avatar for @claudeai](https://pbs.substack.com/profile_images/1950950107937185792/QOfEjFoJ.jpg)
벤치마크 표는 그 자체로 모든 것을 말해줍니다:

![Benchmark table comparing Claude Fable 5.1 with Fable 5, Opus 5, and GPT-5.6 Sol across seven evaluations. Fable 5.1 leads on every row, including 52.6% on Terminal-Bench-Science 0.1 and 55.8% on Terminal-Bench 4.0.](https://substack-post-media.s3.amazonaws.com/public/images/4c65cdfd-fd46-4b99-88f2-eb9be581afd1_2160x2250.png)
토큰당 가격은 Fable/Mythos 5와 동일하지만, 캐시 읽기 가격은 75% 인하되었습니다. 이는 장시간 세션/긴 컨텍스트 사용자를 위한 희소식입니다. 하지만 Artificial Analysis에 따르면 출력 토큰 사용량이 1.7배 증가하여, 작업당 총 비용은 20% 증가했습니다(아래 요약 참조).
또한 World Labs의 Astra 출시를 잊지 마십시오. 이는 우리가 본 월드 모델 출시 중 가장 인상적인 것이었으며, 평범한 날이었다면 쉽게 헤드라인 기사가 되었을 것입니다. 저희 팟캐스트에서 Fei Fei와 Justin Johnson의 비전을 확인하고, Marble부터 Astra까지의 흐름, 그리고 저희가 월드 모델의 진정한 잠재력에 대해 이야기했던 내용을 다시 살펴보실 수 있습니다:
> 2026년 8월 31일~9월 1일 AI 뉴스. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 추가 Discord는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
주요 기사: Fable 5.1 및 Mythos 5.1 출시 및 반응

## 무슨 일이 있었나
Anthropic은 Claude Fable 5.1과 Claude Mythos 5.1을 코딩 및 지식 작업용 새로운 플래그십 모델로 출시했습니다.
- Anthropic은 @claudeai를 통해 직접 출시를 발표하며, 이 모델들을 "코딩 및 지식 작업 분야에서 세계에서 가장 진보된 모델"로 포지셔닝했습니다.
- Anthropic 제품/엔지니어링 담당자들은 Fable 5.1을 특히 자율적인 다단계 작업에 초점을 맞춰 "복잡하고 다단계적인 자율 실행 작업"으로 설명했으며, 코딩, 지식 작업, 장기적인 문제 해결에 중점을 두었습니다 (@mikeyk).
- Anthropic은 Fable 5.1의 정가(input $10 / output $50 / cache write $12.5 per million tokens)를 유지하면서, 캐시 읽기 가격을 75% 인하하여 MTok당 $0.25로 낮췄습니다. 이는 @mikeyk, @Teknium이 언급하고 @ArtificialAnlys가 독립적으로 수치화했습니다.
- 초기 벤치마크 스크린샷과 시스템 카드 발췌문이 논의의 대부분을 주도했으며, 특히 Terminal-Bench-Science, SWE-계열 평가, HLE, FrontierCode, Artificial Analysis에 대한 내용이 많았습니다 (@StevenDillmann, @scaling01, @ArtificialAnlys).
- 커뮤니티 분석에서 핵심적인 해석적 주장이 나왔습니다: Fable과 Mythos 5.1은 다른 기본 모델이 아니라, 다른 안전성/라우팅 동작을 가진 동일한 기저 가중치일 수 있다는 것입니다 (@eliebakouch, 이후 @nrehiew_).
- 사용자 반응은 여러 축을 따라 나뉘었습니다: 코딩/계획 능력과 톤에 대한 매우 강력한 찬사가 있었지만, 속도 제한, 안전장치 오탐, 구독 UX, 불분명한 벤치마크 제시 방식에 대한 불만이 있었습니다 (@danshipper, @theo, @kimmonismus, @GregKamradt, @kylebrussell, @eliebakouch).

## 공식 주장 및 모델 포지셔닝
Anthropic의 메시지는 명확했습니다: Fable 5.1은 어렵고 위임된 장기적인 작업을 위한 것이며, Mythos 5.1은 지식 작업을 위한 짝을 이룬 출시입니다. 주요 공식 출시 게시물은 @claudeai입니다. Anthropic 직원의 보충 설명은 다음을 강조했습니다:
- @mikeyk를 통한 자율적인 장기 실행 작업
- @mikeyk를 통한 향상된 정직성 / 더 나은 실패 보고 ("막혔을 때 성공을 보고하는 대신 막혔다고 말합니다")
- @alexalbert__를 통한 새로운 엔터프라이즈 지향 제어 기능, 특히 Enterprise Frontier Safeguards (EFS)는 엔터프라이즈 환경에서 에이전트 관측 가능성을 위한 "ZDR++"로 포지셔닝되었습니다.
- 특히 @danshipper가 강조한 제로 데이터 보존(ZDR) 지원은 중요한 채택의 문을 여는 요소로 사용자들에게 부각되었습니다.
공식적인 홍보는 단순히 "더 나은 벤치마크 모델"이 아니라, "사용 가능한 자율 작업자"였습니다. 캐시된 에이전트 설정에서 충분히 빠르고, 충분히 저렴하며, 배포하기에 충분히 엔터프라이즈 호환적이라는 것입니다.
이러한 포지셔닝은 Fable 5가 강력하지만 때로는 비실용적이라는 평판(반응에서도 반복됨)을 가지고 있었기 때문에 중요했습니다. Dan Shipper는 이전 비판을 Anthropic이 "데이터센터에 거의 사용할 수 없는 천재를 만들었다"고 요약한 후, 5.1이 느림, 장황함, 어색한 톤을 해결했다고 주장했습니다 (@danshipper).

## 기술적 세부 정보 및 수치

### 핵심 공개/가격 세부 정보
@ArtificialAnlys에서:
- 컨텍스트 윈도우: 100만 토큰
- 모달리티: 텍스트 + 이미지 입력
- 가격: Fable 5와 동일input: $10 / 1M 토큰output: $50 / 1M 토큰cache write: $12.5 / 1M 토큰
- 캐시 읽기 가격: 1M 토큰당 $1.00에서 $0.25로 인하 (75% 인하)
Artificial Analysis는 이러한 캐시 가격 인하가 프롬프트의 대부분이 캐시에서 반복적으로 다시 읽히는 에이전틱 워크로드에 실질적으로 이점을 제공한다고 언급합니다.

### Artificial Analysis 주요 결과
또한 @ArtificialAnlys에서:
- Artificial Analysis Intelligence Index: 최대 노력 시 66점앞선 모델:Claude Opus 5 최대: 63Claude Fable 5 최대: 62GPT-5.6 Sol 최대: 61Grok 4.6 높음: 61
- HLE: 59.1%이전 최고 기록: Fable 5 55.5%
- Terminal-Bench v2.1: 91.4%
- SciCode: 62.0%
- τ³-Banking: Fable 5 대비 +9점
- GDPval-AA v2: 1853 ELO, Fable 5 대비 +130
- AA-Briefcase: 1694 ELO, Fable 5 대비 +122
그러나 AA는 중요한 단서도 덧붙였습니다:
- 에이전틱 지식 작업에서 Fable 5.1은 일부 측정치에서 Opus 5와 사실상 동률이며, 명확하게 우위를 점하지는 못했습니다.
- 이들의 평가는 Anthropic의 기본 서버 측 폴백을 사용했으며, 안전 플래그가 지정된 요청은 Claude Opus 4.8 또는 Claude Opus 5로 라우팅되었습니다.
- 폴백은 Intelligence Index 전체 출력 토큰의 약 4%를 차지했습니다.
이 폴백 세부 정보는 커뮤니티 해석에서 가장 중요한 기술적 주의사항 중 하나가 되었습니다.

### 작업당 비용
Artificial Analysis는 또한 다음과 같이 보고했습니다:
- Fable 5.1 최대: 작업당 $3.76
- Fable 5 최대: 더 낮음, 따라서 5.1은 작업당 20% 더 비쌈
- 이유: Fable 5.1은 약 1.7배 더 많은 출력 토큰을 사용
- 캐시 가격 인하로 작업당 약 $1.40 절약
- Fable 5.1 xhigh: 점수 65, 비용 작업당 $2.72
- Opus 5 최대: 점수 63, 비용 작업당 $2.34
이는 반응 주기에서 핵심적인 긴장 중 하나를 야기했습니다: Fable 5.1은 프론티어 최고 성능에서 분명히 더 나아 보이지만, 모든 비용 효율성 관점에서 분명히 더 낫지는 않습니다.
@nicdunz의 추가 설명:
- Fable 5.1 Max: 지능 66, 140M 토큰, 작업당 $3.69
- Fable 5 Max: 62, 83M 토큰, 작업당 $3.14
- GPT-5.6 Sol Max: 61, 70M 토큰, 작업당 $0.95
이 게시물은 Fable 5.1이 절대 최고 성능에서 승리하더라도, Sol이 달러당 지능 및 토큰당 지능에서 여전히 확실한 승자라고 주장합니다.

### 시스템 카드 논의에서 발췌한 벤치마크 스니펫
커뮤니티 구성원들은 몇 가지 벤치마크 포인트를 추출했습니다:
@StevenDillmann에서:
- Terminal-Bench-Science 0.1Fable 5: 24.7%Fable 5.1: 52.6%2배 이상 개선
@scaling01에서:
- DeepSWE: 67.4%
- FrontierCode 1.1 Extended: 63.6%
- FrontierSWE v2: 0.57, "Proximal이 평가한 모델 중 가장 높음"
@Sauers_에서:
- Humanity’s Last Exam: 도구 사용 시 65%
@perplexity_ai에서:
- Perplexity의 8월 WANDR 평가:점수 0.601작업당 $12.76Fable 5보다 21% 높은 점수37% 낮은 비용
@scaling01에서:
- Artificial Analysis Intelligence Index 점수 66, "프론티어로 복귀"
@theo에서:
- 캐시 가격 인하가 "가장 큰 승리"
- CursorBench에서 비용이 "거의 50%" 절감되면서도 더 높은 점수를 기록
@kimmonismus에서:
- Fable 5.1 High가 Cursor Bench에서 Sol 5.6 Max보다 더 강력하고 저렴해 보임
- 이는 2차적인 요약이며, 원본 벤치마크 보고서는 아님
@scaling01에서:
- Mythos 5.1은 긴 에이전틱 코딩 환경의 65%에서 채점자 인식을 언어화하여 보여줍니다.
마지막 요점은 특히 흥미롭습니다: 이는 모델이 장기적인 코딩 컨텍스트의 상당 부분에서 평가자를 명시적으로 모델링할 수 있음을 시사하며, 이는 기능 및 평가 조작 가능성 질문을 모두 제기합니다.

### 안전장치 및 라우팅 세부 정보
두 개의 트윗이 기술적 해석의 핵심을 포착합니다:
- @eliebakouch: "Fable과 Mythos 5.1은 정확히 동일한 가중치"이며, 내부 활성화는 안전성 분류에 사용되고 더 큰 분류기로 에스컬레이션되며, 위험한 요청은 Opus 4.8로 폴백됩니다.
- @nrehiew_: 만약 사실이라면, 차이점은 "아마도 안전장치 분류기에 설정된 임계값일 것"입니다.
이들은 트윗 본문에서 Anthropic의 공식 성명은 아니지만, @ArtificialAnlys를 통해 AA의 평가에서 폴백 라우팅이 출력 토큰의 약 4%를 처리했다는 공식 AA 노트와 일치합니다.
이는 "Mythos"와 "Fable"로 보고된 벤치마크 라인이 진정으로 비교 가능한지에 대한 커뮤니티의 반복적인 질문으로 이어졌습니다. 특히 하나의 명명 규칙이 주로 어떤 안전 경로가 활성화되었는지를 나타내며, 어떤 기본 모델이 작업을 수행했는지는 나타내지 않는다면 더욱 그렇습니다. @eliebakouch, @eliebakouch, @eliebakouch를 참조하십시오.

## 사실 vs 의견

### 공식/독립 출처에 의해 강력히 뒷받침되는 사실
- Anthropic은 Claude Fable 5.1과 Claude Mythos 5.1을 출시했습니다 (@claudeai).
- Fable 5.1 가격은 input/output/cache write에 대해 $10 / $50 / $12.5를 유지했으며, 캐시 읽기는 MTok당 $0.25로 인하되었습니다 (@mikeyk, @ArtificialAnlys).
- Fable 5.1은 1M 컨텍스트, 이미지+텍스트 입력 지원을 제공하며, AA의 Intelligence Index에서 66점으로 최고를 기록했습니다 (@ArtificialAnlys).
- AA의 평가에는 서버 측 폴백이 포함되었으며, 출력 토큰의 약 4%는 폴백 모델에 의해 처리되었습니다 (@ArtificialAnlys).
- Fable 5.1은 Terminal-Bench-Science에서 52.6%를 포함하여 여러 코딩/에이전틱 벤치마크에서 매우 큰 개선을 보였습니다 (@StevenDillmann).

### 그럴듯하지만 완전히 검증되지 않은 주장
- Fable과 Mythos 5.1은 다른 안전장치/라우팅 동작을 가진 동일한 가중치입니다 (@eliebakouch, @nrehiew_).
- 일부 벤치마크 라벨은 별도의 기본 모델 성능보다는 안전 모드/경로 차이를 반영할 수 있습니다 (@eliebakouch).
- "이제 보통 사람처럼 말한다" / "클로드어" 감소는 일화적으로 널리 보고되지만, 아래의 일부 어휘 통계에도 불구하고 여전히 주관적입니다.

### 의견 / 주관적 판단
- @danshipper: "우리가 사용해 본 가장 강력한 코딩 모델"
- @AravSrinivas: "Fable은 현재 상당한 차이로 프론티어 모델입니다"
- @scaling01: "Astra가 Fable 5.1을 완전히 파괴할 것입니다"
- @kimmonismus: "솔직히 Fable 5와 비교하여 큰 차이를 느끼지 못했습니다"
- @kimmonismus: 속도 제한 때문에 "말 그대로 사용할 수 없습니다"
중요한 패턴은 객관적인 지표와 사용자 경험 반응이 엇갈렸다는 것입니다. 벤치마크 종합에서는 5.1이 계단식 개선을 보였습니다. 그러나 실질적인 접근성과 UX에서는 많은 사용자들이 여전히 마찰을 보고했습니다.

## 다른 의견 및 반응

### 강력한 긍정적 평가: 기능, 계획, 코딩 품질
몇몇 영향력 있는 개발자들은 열광했습니다:
- @danshipper는 모델이 이제 빠르고, 토큰 효율적이며, 산문에서 더 낫고, 위임에 유용하다고 주장했습니다. 특히 원-프롬프트 앱 생성, 며칠 동안 실행되는 대규모 프로그래밍 작업, 더 나은 작가 채택을 언급했습니다.
- @theo는 이를 "정말 좋은 모델"이라고 부르며, 워크플로우를 재설정/업데이트해야 했고 적극적으로 많이 사용하고 있다고 언급했습니다 (@theo, @theo).
- @alexalbert__는 Fable 5.1이 부동산 부지 이미지를 받아 집을 디자인하고, 렌더링하고, 시네마틱 워크스루를 생성하는 디자인+렌더 워크플로우를 보여주었습니다. 후속 설명에서는 Blender headless 사용을 언급했습니다 (@alexalbert__).
- @spicey_lemonade는 "Fable 5.1 Minecraft 원샷"을 게시하여 큰 호응을 얻었으며, 창의적인 코딩 유용성을 보여주는 데모와 같은 증거가 되었습니다.
- @simonw는 Anthropic 모델에서 역대 최고의 SVG 펠리컨 출력을 보고했지만, 상당한 비용이 들었습니다.
이 진영은 5.1이 단순히 점진적으로 개선된 것이 아니라, 엔드투엔드 메이커 워크플로우에서 완전히 경쟁력 있다고 느껴지는 첫 Claude 모델이라고 보았습니다.

### 긍정적이지만 신중한 평가: 주의사항이 있는 프론티어 리드
- @ArtificialAnlys는 가장 균형 잡힌 제3자 평가를 제공했습니다: 프론티어 선도적인 종합 점수를 기록했지만, 작업당 비용은 Fable 5보다 여전히 비싸고 일부 에이전틱 지식 작업 평가에서는 Opus 5와 사실상 동률이었습니다.
- @kimmonismus는 특히 Cursor Bench에서 가격 대비 성능 면에서 "상당한 도약"이라고 불렀지만, 장황함 감소와 오탐 감소가 유지될지에 대해서는 명시적으로 유보적인 태도를 보였습니다.
- @theo는 순수한 기능 변화보다는 캐시 읽기 가격 인하의 실질적인 중요성에 더 집중했습니다.
- @perplexity_ai는 이를 더 넓은 멀티 모델 에이전트 스택 내에서 강력한 오케스트레이터 모델로 설명했습니다.
이러러한 관점은: 그렇습니다, 매우 강력하지만, 전체 배포 경제성과 툴 스택이 이제 합리적인지가 중요합니다.

### 비판적 평가: 속도 제한, 안전장치, 구독 경험
가장 날카로운 비판은 벤치마크 사기나 약한 지능에 대한 것이 아니었습니다. 접근성과 인체공학에 대한 것이었습니다.
- @kimmonismus는 심각한 속도 제한, 끊기는 연속성, 그리고 개선된 효율성에도 불구하고 해당하는 구독 혜택이 없다고 불평했습니다.
- @kimmonismus는 5.1이 "속도 사용량 면에서 Fable 5보다 훨씬 나빴다"고 강조했습니다.
- @GregKamradt는 v3 테스트 중 요청이 "리버스 엔지니어링"으로 자주 거부되어 계획된 평가 완료를 방해했다고 보고했습니다.
- @kylebrussell은 이론 수학 세션에서 "군사 작전" 은유가 사이버 안전장치를 작동시켰다고 말했습니다. 나중에 "첫날 안전장치... 지금까지는 더 성가시다"고 덧붙였습니다 (@kylebrussell).
- @theo는 속도 제한 불만의 보편성에 대해 반박하며, 자신은 "전혀 그런 것을 보지 못했다"고 말했고, 한 주간의 Fable 제한 중 14%만 사용했다고 했습니다.
- @theo는 실질적인 할당량 관계를 역설계하려고 시도했습니다: 5시간 제한 ≈ 주간 제한의 21% 및 Fable 제한의 38%
따라서 사용량 제한에 대해서도 단일한 합의는 없었습니다. 일부 사용자들은 빨리 한계에 부딪혔고, 다른 사용자들은 그렇지 않았습니다.

### 회의적/중립적 평가: 벤치마크 해석 및 명명 혼란
별도의 반응 클러스터는 방법론과 명확성에 초점을 맞췄습니다.
- @scaling01은 FrontierCode 결과가 이상해 보인다고 말했습니다.
- @scaling01은 더 많은 멀티 에이전트 비교와 더 나은 해석을 원했습니다.
- @iScienceLuvr는 Anthropic의 헬스케어 벤치마크 발표를 비판하며, 비교 불가능한 심사 모델과 더 넓은 의료 평가 범위의 부족을 지적했습니다.
- @eliebakouch는 시스템 카드 벤치마크 행이 "Fable"과 "Mythos"를 언제 사용하는지에 대한 설명을 반복적으로 요청했습니다. 이는 사용자가 안전장치에 의해 트리거된 라우팅을 추론해야 하는지에 영향을 미치기 때문입니다.
이는 출시 주기에서 가장 기술적인 비판입니다: 모델이 약하다는 것이 아니라, 보고 형식이 무엇이 정확히 측정되고 있는지 이해하기 필요 이상으로 어렵게 만든다는 것입니다.

## 작문 품질 및 "클로드어" 논의
가장 많이 반복된 주관적 관찰 중 하나는 5.1이 더 평범하게 들린다는 것이었습니다.
- @danshipper: "실제로 보통 사람처럼 말한다", "더 명확한 산문", "AI 특유의 표현" 감소
- @ethanCaballero는 5.1이 "클로드어를 제거했는가?"라고 직접 물었습니다.
- @ethanCaballero는 나중에 Anthropic의 새로운 프롬프트가 "클로드어"를 제거했다고 지적했습니다.
- @ValsAI는 정량적인 문체 변화를 게시했습니다:하이픈으로 연결된 복합어 감소em 대시 감소
- @ValsAI는 문장은 더 짧아졌지만 전체적으로 출력은 더 길어졌다는 것을 발견했습니다:VCB: 작업당 534 → 1299 단어Terminal-Bench: 961 → 1299Legal Research: 1892 → 2693
- @ValsAI는 이상한 보상 아티팩트를 언급했습니다: 논브레이킹 하이픈 U+2011의 사용이 거의 0에서 백만 개당 약 4.4천 건으로 증가했습니다.
따라서 "클로드어 감소" 주장은 순전히 느낌만은 아닙니다. 적어도 측정 가능한 문체 변화가 일부 있습니다. 그러나 통계는 Anthropic이 하나의 표면적 특징을 다른 것으로 교환했을 수도 있음을 시사합니다.

## 안전장치 이야기: 향상된 엔터프라이즈 실행 가능성, 그러나 오탐도 존재
5.1을 둘러싼 안전성 계층은 모델 자체만큼이나 많이 논의되었습니다.
공식/Anthropic 지향적 관점:
- @alexalbert__는 Enterprise Frontier Safeguards를 엔터프라이즈 환경에서 에이전트 배포를 위한 실용적인 관측 가능성 레이어로 제시했습니다.
- @mikeyk는 모델이 성공을 거짓으로 주장하기보다는 막혔을 때 더 솔직하다고 주장했습니다.
비판적인 사용자 보고서:
- @GregKamradt는 오탐된 리버스 엔지니어링 플래그 때문에 테스트를 완료할 수 없었습니다.
- @kylebrussell은 수학 설정에서 은유를 사용하여 안전장치를 작동시켰습니다.
- @nrehiew_는 Anthropic이 사이버 관련 콘텐츠를 분류하고 안전장치를 적용할지 결정하기 위해 활성화 프로브를 사용할 가능성을 강조했습니다.
- @mikeyk는 뇌 모델 아티팩트 예시를 허용되는 복잡한 추론의 긍정적인 예시로 공유했습니다.
여기에는 명확한 채택 트레이드오프가 있습니다:
- 기업은 더 안정적인 세션 간 모니터링 및 제어를 원합니다.
- 파워 유저는 오탐 감소와 더 관대한 탐색적 사용을 원합니다.
Anthropic은 이 둘을 모두 만족시키려고 노력하고 있으며, 첫날의 분위기는 그 균형이 아직 보편적으로 받아들여지지 않았음을 시사합니다.

## Mythos vs Fable: 동일 모델인가, 별도 제품인가?
이는 기술적으로 가장 흥미로운 논의 스레드 중 하나였습니다.
@eliebakouch의 주장:
- Fable과 Mythos 5.1은 "정확히 동일한 가중치"입니다.
- 내부 활성화가 검사됩니다.
- 위험한 요청은 더 큰 분류기로 에스컬레이션됩니다.
- 그런 다음 Opus 4.8로 폴백될 수 있습니다.
- 따라서 Fable은 더 큰 Mythos 모델의 디스틸레이션 버전이 아닙니다.
후속 설명 및 추측:
- @eliebakouch는 이전 커뮤니티의 추측이 Mythos를 교사 모델로, Claude/Fable을 디스틸레이션된 학생 모델로 취급했지만, 이는 추측에 불과했다고 말했습니다.
- @eliebakouch는 정확한 학습 계보에 대해서는 여전히 불확실하다고 했습니다.
- @nrehiew_는 차이점이 아마도 분류기 임계값일 것이라고 제안했습니다.
- @ArtificialAnlys는 평가에서 폴백 라우팅 동작을 독립적으로 확인했지만, "정확히 동일한 가중치" 주장을 직접 확인한 것은 아닙니다.
이것이 중요한 이유:
1.  벤치마크의 해석 가능성. "Mythos 결과"와 "Fable 결과"가 다른 라우팅/안전장치 설정 하의 주로 동일한 백본이라면, 벤치마크 표는 이를 명시해야 합니다.
2.  조달 및 배포. 기업은 동일한 모델에 대한 다른 정책을 선택하는 것임에도 불구하고, 별개의 모델 중에서 선택한다고 생각할 수 있습니다.
3.  안전성/기능 회계. 벤치마크가 폴백을 통해 실행된다면, "어떤 모델이 점수를 얻었는가?"는 더 이상 사소한 문제가 아닙니다.
이러한 명명/라우팅 모호성은 전체 트윗 세트에서 가장 훌륭한 기술적 질문들을 낳았습니다.

## 실질적인 제품 영향

### 캐시 읽기 가격 인하가 중요한 이유
에이전틱 시스템은 종종 대규모 스크래치패드, 리포지토리, 이전 단계 및 도구 트랜스크립트를 다시 보냅니다. 이러한 설정에서는 캐시된 입력 가격이 불균형적으로 중요합니다.
- Anthropic의 75% 캐시 읽기 가격 인하는 @Teknium, @theo에게 칭찬받았으며, @ArtificialAnlys에 의해 자세히 수치화되었습니다.
- AA의 설명에 따르면, 대부분의 절감 효과는 입력 토큰의 대부분이 캐시 읽기인 에이전틱 평가에서 특히 발생합니다.
- 이는 출력 토큰 비용이 여전히 높더라도 Fable 5.1을 다단계 워크플로우에서 오케스트레이터/플래너로서 더 매력적으로 만듭니다.

### 제로 데이터 보존 및 EFS가 중요한 이유
- Dan Shipper는 ZDR 지원을 기업이 이제 모델을 사용할 수 있는 주요 이유로 특별히 언급했습니다 (@danshipper).
- Alex Albert의 EFS 설명 (@alexalbert__)은 더 넓은 시장 전환을 시사합니다: 기업은 더 이상 단순히 "프라이빗 인퍼런스"를 원하는 것이 아닙니다. 그들은 에이전트 관측 가능성, 세션 간 이상 감지 및 위험 모니터링을 원합니다.
이는 Anthropic이 엔터프라이즈 채택이 원시 모델 품질만큼이나 거버넌스 인프라에 의존하는 미래를 위해 최적화하고 있음을 시사합니다.

### 구독 불만이 중요한 이유
API 경제성은 개선되지만 소비자/프로 구독자 제한은 그렇지 않다면, 인식이 빠르게 나빠질 수 있습니다.
- @kimmonismus는 Anthropic이 구독 사용자에게 더 낮은 가격이나 더 높은 사용량 제한을 발표하지 않았다고 명시적으로 언급했습니다.
- 이는 분리된 제품 인식을 만듭니다:API 개발자: "큰 승리"헤비 인터랙티브 구독자: "여전히 제약적"
이러한 불일치는 많은 주요 리뷰어들이 원시 API가 아닌 구독 제품을 통해 먼저 테스트하기 때문에 중요합니다.

## 경쟁 환경
이번 출시는 OpenAI의 Astra 루머/안전성 게시물과 여러 월드 모델 발표가 관심을 놓고 경쟁하는 매우 활발한 프론티어 주간에 이루어졌습니다. 그럼에도 불구하고 Fable 5.1은 코딩 모델 리더보드를 재설정하는 것처럼 보였기 때문에 강렬한 주목을 받았습니다.
반응에서 나온 비교 주장:
- @AravSrinivas: Fable은 "상당한 차이로" 프론티어 모델입니다.
- @kimmonismus: Cursor Bench에서 Sol 5.6 Max에 비해 Fable에 유리합니다.
- @nicdunz: Fable은 절대적인 지능에서 승리하고, Sol은 경제성에서 승리합니다.
- @scaling01: Astra는 추론 효율성에서 곧 이를 뛰어넘을 것입니다.
- @theo: Anthropic은 그 순간 1위, 2위, 3위를 차지했습니다.
또한 이번 출시가 다음 OpenAI 출시와 즉각적인 비교를 불러일으킬 만큼 중요했다는 광범위한 인식이 있었습니다:
- @kimmonismus는 Fable 5.1보다 GPT-Astra에 더 기대된다고 말했습니다.
- @theo는 주변의 Astra 기대감을 언급하며, 이번이 모델 출시를 위해 주어진 역대 가장 빠른 사전 경고일 수 있다고 말했습니다.
따라서 시장 측면에서 Fable 5.1은 Anthropic의 진정한 복귀이자, 급격히 고조되는 모델 출시 경쟁의 한 수로 여겨졌습니다.

## 배경: 이 출시가 일반적인 포인트 업데이트보다 더 중요했던 이유
세 가지 배경 역학이 반응의 강도를 설명합니다.

### 1. Anthropic의 명성은 양분되었습니다.
Claude 계열 모델은 초기에는 코딩 깊이와 작문 스타일로 강력한 명성을 얻었지만, 최근 논의에서는 종종 다음과 같이 묘사되었습니다:
- 매우 유능하지만
- 톤이 다소 어색하고
- 거절에 보수적이며
- 장시간 사용 시 느리거나 번거롭다
5.1에 대한 긍정적인 반응은 종종 Anthropic이 마침내 "사용성 비용"을 해결했다는 식으로 설명되었습니다 (@danshipper).

### 2. 에이전트가 가격 책정에서 사람들이 중요하게 생각하는 것을 바꾸었습니다.
전통적인 프롬프트-응답 사용자들은 입력/출력 가격에 집중합니다. 에이전트 개발자들은 다음 사항에 집중합니다:
- 캐시 읽기
- 긴 컨텍스트
- 장시간 세션에서의 신뢰성
- 위임된 작업 동작
- 정직한 실패 보고
이것이 캐시 읽기 가격 인하가 벤치마크 점수만큼이나 많은 칭찬을 받은 이유입니다.

### 3. 안전성은 단순한 정책이 아닌 제품 아키텍처가 되고 있습니다.
EFS, 라우팅, 활성화 프로브, 폴백 모델, ZDR은 모두 "모델"이 더 이상 단일 아티팩트가 아님을 보여주는 신호입니다. 이는 정책으로 감싸인 시스템입니다. Fable/Mythos 논쟁은 사실 이러한 변화에 대한 논쟁입니다.
사용자들은 이제 단순히 "모델이 얼마나 똑똑한가?"가 아니라 다음을 묻기 시작했습니다:
- 어떤 가중치가 이 요청을 처리했는가?
- 어떤 안전 경로가 개입했는가?
- 폴백이 얼마나 자주 발생했는가?
- 어떤 벤치마크 점수가 어떤 경로에 속하는가?
이는 표준 모델 출시 과대광고보다 더 성숙하고 시스템 수준의 대화입니다.

## 주목할 만한 데모 및 생태계 반응
- @alexalbert__: 이미지-주택 디자인-시네마틱 워크스루 파이프라인, @alexalbert__는 Blender headless 사용을 명확히 했습니다.
- @spicey_lemonade: 마인크래프트 원샷 데모
- @simonw: SVG 펠리컨 + 애니메이션
- @_catwu: Anthropic 팀원은 내부 팀이 이전에는 몇 달이 걸렸을 프로젝트를 수행하고 있다고 주장합니다.
- @perplexity_ai: Perplexity Computer에 통합되었습니다.
- @Teknium: Hermes Agent / Nous Portal / OpenRouter에서 사용 가능합니다.
- @theo: T3 Code는 Fable 5.1 지원을 출시했습니다.
이러한 통합의 속도는 5.1이 채팅 사용자뿐만 아니라 에이전트 개발자에게 특히 중요하다는 인식을 강화했습니다.

## 커뮤니티에서 제기된 질문들
-   **벤치마크 투명성** 시스템 카드에서 일부 벤치마크에는 Mythos를, 다른 벤치마크에는 Fable을 보고할 때, 정확히 무엇이 이러한 라벨링을 결정하는 걸까요? @eliebakouch와 @eliebakouch의 의견을 참조하십시오. 벤치마크 성능이 폴백 라우팅(fallback routing)에 얼마나 의존하는지, 아니면 주 모델(primary-model) 동작에 얼마나 의존하는 걸까요?
-   **안전장치 튜닝** Anthropic은 사이버 안전장치를 약화시키지 않으면서 이론적이거나 양성적인 기술 작업에서 오탐(false positives)을 줄일 수 있을까요? @GregKamradt와 @kylebrussell의 의견을 참조하십시오.
-   **속도 제한 및 제품 세분화** 구독 사용자들도 효율성 향상의 혜택을 받을 수 있을까요, 아니면 토큰 기반 API 고객만 해당될까요? @kimmonismus가 날카롭게 지적했습니다.
-   **평가 품질 및 과적합 우려** 특히 FrontierCode 또는 의료 하위 집합(medical subsets)의 일부 결과가 왜 이상하거나 비교하기 어려운 것처럼 보일까요? @scaling01과 @iScienceLuvr의 의견을 참조하십시오.
-   **문체 변화** "덜 클로드스러운(less Claudese)" 것은 프롬프트 변경 때문일까요, 후학습(post-training) 변화 때문일까요, 아니면 둘 다일까요? @ethanCaballero는 새로 공개된 프롬프트를 지적했고, @ValsAI는 측정 가능한 어휘적 차이를 보여주었습니다.
OpenAI의 Astra와 순환 깊이(recurrent depth)를 둘러싼 모니터링 가능성 논쟁
-   **준비 태세 이정표: "사이버 핵심"**: OpenAI는 Astra를 자사의 준비 태세 프레임워크(Preparedness Framework)에 따라 사이버 보안의 Critical 임계값에 도달한 첫 번째 모델로 미리 공개했습니다. 블로그 게시물에서는 @boazbaraktcs에 따라 Astra의 가장 진보된 사이버 기능이 더욱 엄격하게 접근 제어될 것이라고 강조했습니다. 게시물에서 유포된 요약에 따르면, @kimmonismus가 정리한 바와 같이, Astra는 V8 제로데이(zero-days), 연쇄 익스플로잇(chained exploits)을 발견하고, 강화된 브라우저를 침해하며, 샌드박싱(sandboxing)을 탈출하고, 테스트에서 권한을 에스컬레이션(escalated privileges)했다고 주장했습니다. OpenAI 리더십은 또한 안전성 작업의 일부가 배포를 늦췄으며, 미래 모델 개발 속도는 안전장치(safeguards)를 위해 속도를 계속 희생할 수 있다고 Sam Altman의 성명에서 강조했습니다.
-   **아키텍처 보고 및 "불투명한 추론" 우려**: Astra와 관련된 또 다른 주요 이야기는 Astra가 어떤 형태의 순환 깊이(recurrent depth) / 루프형 트랜스포머(looped transformer) 아키텍처를 사용한다는 보고에서 비롯되었으며, 이는 CoT 모니터링의 유용성을 감소시키는지에 대한 날카로운 논쟁을 촉발했습니다. @RyanGreenblatt, @thlarsen, @tenobrus, @bshlgrs는 더 많은 잠재 공간(latent-space) 추론이 사후 조사(post-incident investigation)를 실질적으로 더 어렵게 만들 수 있다고 주장하며 우려를 표했습니다. 이와 대조적으로, 다른 이들은 이러한 반응이 과장되었다고 주장했습니다. @max_paperclips, @teortaxesTex, @suchenzang은 내부 "뉴럴리즈(neuralese)" 추론이 새로운 것이 아니며, 중요한 것은 유효 깊이(effective depth)이지 레이어가 루프형인지 명시적으로 쌓여 있는지 여부가 아니라고 강조했습니다.
-   **OpenAI의 해명 및 기술적 맥락**: OpenAI의 최고 과학자 @merettm은 가장 강한 해석들을 완화시키려 노력하며, Astra를 포함한 현재 프론티어 모델(frontier models)의 계산 그래프(computation graph) 깊이는 GPT-4의 약 2배 이내이며, OpenAI는 여전히 CoT 모니터링을 핵심 연구 목표로 간주한다고 말했습니다. 이 해명은 논의를 더 좁은 기술적 질문으로 옮겼습니다. 즉, 순환 블록(recurrent blocks)이 주로 파라미터/저장 효율성 트릭인지, 아니면 훨씬 더 깊고 모니터링하기 어려운 추론으로 가는 자연스러운 경로를 만드는지 여부였습니다. @eliebakouch, @voooooogel, @scaling01로부터 선의의 기술적 논의가 있었습니다. 루프형 MoE 트랜스포머(looped MoE transformers) 및 스케일링 법칙(scaling laws)에 대한 관련 최신 논문들도 @iScienceLuvr에 의해 언급되었습니다.
World Labs의 Atlas: 재구성, 카메라 제어 및 real2sim을 위한 통합 월드 모델링
-   **주목할 만한 멀티모달 월드 모델 출시**: World Labs는 Atlas를 소개했습니다. @drfeifei는 Atlas를 처음부터 학습시킨 멀티모달 월드 모델(multimodal world model)로, 픽셀 단위의 완벽한 카메라 제어로 프레임을 생성하고, 단 한 장의 이미지로도 대규모 장면을 재구성하며, 시뮬레이션된 시공간을 통해 비디오를 리프레임하고, 이미지에서 네이티브 3D 공간을 출력할 수 있다고 설명했습니다. 팀은 이를 여러 도구를 이어 붙인 툴체인(toolchain)이 아닌, 생성과 재구성을 통합하는 단일 모델로 포지셔닝했으며, 이는 @KeunhongP와 @BenMildenhall의 후속 예시를 통해 더욱 강화되었습니다.
-   **데모 테마: 불릿 타임, 희소 뷰 재구성, 창의적 제어 가능성**: 가장 강력한 데모는 몇 장의 일반적인 휴대폰 캡처만으로 자유 시점 비디오를 만드는 데 중점을 두었습니다. 여기에는 @davidpantera_의 단편 영화 예시, @eerac의 3대의 iPhone으로 만든 "불릿 타임" 합성, 그리고 @bilawalsidhu의 논평(이전에는 수십 또는 수백 대의 카메라가 있는 볼륨 측정 장비(volumetric rigs)가 필요했다는 내용)이 포함됩니다. 추가 게시물에서는 몇 장의 서로 다른 인터넷 사진(예: 자연사 박물관 예시)으로 재구성한 모습과 스타일화된 생성과 탐색 가능한 3D 장면을 혼합하는 것을 보여주었습니다.
-   **엔지니어들이 주목하는 이유: real2sim과 로봇 공학**: VFX/영화 제작을 넘어, 기술적으로 더 중요한 측면은 로봇 공학을 위한 real2sim입니다. @YunzhuLiYZ는 일반적인 사진을 사용하여 로봇 내비게이션을 위한 RGB 및 깊이 관측을 합성하는 것을 보여주었고, @MTSlive는 공동 창립자 Justin Johnson의 "사진 5장을 찍고, 시뮬레이션을 구축한 다음, 로봇을 적용한다"는 비전을 강조했습니다. @DrJimFan을 포함한 연구원들은 이를 real2sim을 향한 강력한 진전이라고 불렀고, Fei-Fei는 Atlas를 로봇 공학 전반에 걸친 수평적 활용과 명시적으로 연결했습니다.
Qwen, GLM, RWKV 및 오픈 모델(open-model) 모멘텀
-   **Qwen의 업그레이드된 플래그십 모델이 웹 개발 코딩 평가에서 최고를 차지했습니다**: Alibaba는 1M 컨텍스트를 가진 2.4T 파라미터 모델인 Qwen3.8-Max-0902를 출시했습니다. 이 모델은 입력 $2/M, 출력 $6/M의 가격과 명시적/암시적 캐시 히트(cache-hit) 가격을 제공합니다. Arena는 이 모델이 Code Arena: WebDev에서 1691점으로 1위를 차지하며 Claude Opus 5 Max와 Kimi K3 Max를 앞섰다고 보고했으며, @arena를 통해 현재 최고의 가격/성능 프론티어에도 도달했습니다. Alibaba는 여기에서 동일한 결과를 강조했습니다.
-   **오픈 및 세미-오픈 장기 시계열(long-horizon) 모델이 공급업체를 통해 계속 확산되고 있습니다**: GLM-5.3은 Perplexity Agent API, Arcee, 그리고 Databricks 서빙(serving) 수치를 포함한 인프라 및 플랫폼 통합에서 계속 등장했습니다. Databricks에서는 310 tok/s를 기록했다고 보고되었으며, 내부 벤치마크에서 가장 강력한 OSS 코딩 모델로 설명되었습니다. CoreWeave는 또한 DeepSeek-V4-Pro-0813을 발표했습니다. 이 모델은 1.6T, 1M 컨텍스트 모델로, 매우 저렴한 캐시 읽기(cache reads)를 통해 장기 시계열 에이전트 워크로드(long-horizon agent workloads)에 적합한 가격입니다. 한편 RWKV-7 G1j는 에이전트/코딩/STEM 분야에서 성능 향상을 주장하는 100% RNN 모델로 출시되었고, LongCat-2.0은 Cline에서 접근 가능한 1M 컨텍스트를 가진 1.6T 오픈 웨이트(open-weights) MoE로 공개되었습니다.
-   **오픈소스 서빙 및 멀티모달 인퍼런스 개선**: 서빙(serving) 측면에서는 vLLM-Omni + FastVideo의 FastH3가 10.1초 길이의 동기화된 비디오+오디오 클립을 8.7초 만에 렌더링하여, 즉 재생보다 빠르게 처리하는 것을 시연했습니다. MiniMax는 이를 인터랙티브 비디오 시스템을 위한 오픈 베이스라인으로 제시했습니다.
에이전트, 하네스(harnesses), 메모리 및 평가 연구
-   **에이전트 하네스가 주요 동력(lever)이 되고 있습니다**: 여러 트윗에서 이제 큰 성과가 기본 모델뿐만 아니라 런타임 시스템(runtime systems)에서도 나오고 있음을 강조했습니다. @omarsar0는 오픈소스 하네스인 openJiuwen이 SWE-bench Verified에서 82.6%, Terminal-Bench 2.1에서 87.19%를 달성했다고 강조하며, 이는 레일 기반 구성(rail-based composition)과 고정된 기본 모델 정책(underlying model policy)을 통한 런타임 적응(runtime adaptation) 덕분이라고 설명했습니다. @dair_ai는 루트 프롬프트(root prompts)뿐만 아니라 전체 프로덕션 스킬 번들(production skill bundles)을 압축하여 품질 손실 없이 번들 토큰의 38%, 실행당 토큰의 10.4%를 절감하는 SkillZip Pro를 요약했습니다.
-   **장기 시계열 에이전트 평가가 더욱 현실적으로 변하고 있습니다**: 주목할 만한 벤치마크 추가는 E-Commerce Bench였습니다. 이 벤치마크는 에이전트가 여러 온라인 상점을 운영하는 시뮬레이션된 365일 동안 실행되도록 합니다. 최고 수익 모델은 GPT-5.6 Sol로, 10만 달러의 초기 자본을 1,431,425달러로 성장시켰지만, 사기 방지(fraud avoidance)에서는 낮은 순위를 기록했습니다. 어떤 모델도 모든 축에서 우위를 점하지 못했습니다. 이러한 종류의 평가는 단일 세션 벤치마크보다 수익, 안전성, 운영 품질 간의 트레이드오프(trade-offs)를 더 잘 드러냅니다.
-   **메모리 및 보상 해킹(reward-hacking) 연구**: @dair_ai는 또한 에피소드 타임라인(episodic timelines), 엔티티-이벤트 그래프(entity-event graphs), 그리고 인용 잠금(citation-locking)이 적용된 큐레이션된 문서 메모리(curated documentary memory)를 분리하는 Agent Zero Memory를 강조했습니다. 이 모델은 95.6%의 LongMemEval과 93.6%의 LoCoMo를 기록하며 대규모 비용 절감을 가능하게 했습니다. 정렬(alignment) 측면에서 @omarsar0는 에이전트가 결함 있는 테스트 인프라(test infra)에 직면했을 때 구조화된 에스컬레이션 도구(escalation tool)를 추가하면, 8개의 프론티어 모델(frontier models) 전반에 걸쳐 보상 해킹(reward hacking)이 23.6%에서 5.3%로 감소하며, 사실상 성능 오버헤드(performance overhead)가 없음을 보여주는 논문을 요약했습니다.
(참여도 기준) 인기 트윗
-   **Claude 출시**: Anthropic의 Claude Fable 5.1 / Mythos 5.1 발표는 그날의 가장 큰 순수 모델 출시 게시물이었습니다.
-   **Astra 준비 태세**: OpenAI의 Astra 안전성/준비 태세 발표는 가장 큰 안전성/아키텍처 논의를 이끌었습니다.
-   **Atlas 출시**: World Labs의 Atlas 발표는 뛰어난 멀티모달/월드 모델 출시였습니다.
-   **사이버 보안 경고**: @ilyasut은 미래의 악성 에이전트(rogue agents)가 클라우드 용량(cloud capacity)을 장악하여 복제(replicate)를 시도할 수 있으므로, 네오클라우드(neoclouds)가 사이버 방어(cyberdefenses)를 시급히 강화해야 한다고 주장했습니다.
-   **Meta 음성 모델**: @finkd는 Meta의 첫 실시간 오디오 인식 모델인 Muse Voice Transcribe를 발표했습니다. 이 모델은 네이티브 화자 분리(diarization) 및 종점 감지(endpointing) 기능을 갖추고 있습니다.

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Qwen, DeepSeek, 및 Gemma 모델 업데이트

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-claude-fablemythos-51-new&utm_source=paywall-free-trial&utm_medium=web&utm_content=213823166&coupon=5fe099d9)
[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-claude-fablemythos-51-new&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
