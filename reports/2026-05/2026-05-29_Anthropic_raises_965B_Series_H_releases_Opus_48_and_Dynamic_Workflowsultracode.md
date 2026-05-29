# Anthropic raises $965B Series H, releases Opus 4.8 and Dynamic Workflows/ultracode

**원문 URL**: https://www.latent.space/p/ainews-anthropic-raises-965b-series
**번역일**: 2026-05-29 06:18
**발행일**: 2026-05-29

---

# [AINews] Anthropic, 9,650억 달러 규모 Series H 투자 유치 및 Opus 4.8, Dynamic Workflows/ultracode 출시

### Anthropic의 완벽한 승리!
Anthropic은 역사상 가장 빠르게 성장하는 회사로서 한동안 OpenAI를 추월하는 것을 목표로 삼아왔습니다. 하지만 지난 몇 달 동안은 역전의 시기(사실 여부는 아닐지라도)에 의문을 제기하는 수많은 단서들이 있었습니다. 오늘 Anthropic은 공식적으로 470억 달러의 연간 매출액(참고로, 이 수치는 12월에 90억 달러였습니다!)을 보고했으며, 9,000억 달러의 프리머니 기업가치로 650억 달러 규모의 Series H 투자를 유치했음을 확인했습니다. 여기에는 Amazon을 포함한 하이퍼스케일러와 전체 메모리 산업 생태계로부터의 150억 달러가 포함되어 있습니다. 이는 컴퓨트 및 비코딩 벤치마크를 제외한 모든 헤드라인 지표에서 Anthropic을 적어도 일시적으로 OpenAI보다 앞서게 합니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/feb0a3a2-e744-4174-a24b-be1fd75961bc_1888x1630.png)
이를 기념하여 Anthropic은 Opus 4.8을 출시했습니다. 이 모델은 커뮤니티에서 Opus 4.7 출시 후 발견했거나 불만을 가졌던 많은 문제들을 전반적으로 해결했다고 보고되었습니다(자세한 내용은 아래 요약을 참조하십시오). 특히, 사실상 모든 경제적으로 중요한 벤치마크에서 SOTA를 달성했습니다(흥미로운 점은 Gemini 3.5 Flash가 Gemini 3.1 Pro보다 개선되었다는 Google의 메시지에 동의한다는 것입니다).

![](https://substack-post-media.s3.amazonaws.com/public/images/7e7c3740-ab5b-4b98-88eb-c0576e73a2d1_1490x1350.png)
하지만 장기적으로 더 중요한 것은 Claude Code의 대규모 병렬 "Dynamic Workflows" 기능 (ultracode라고도 불립니다)일 것입니다. 이 기능은 Jarred Sumner가 6일 만에 Bun을 Zig에서 Rust로 75만 라인 재작성하는 데 사용되었습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/e9ab93f2-c75f-4156-850a-81b99806aeea_1402x1256.png)
>
> 2026년 5월 27일~28일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터를 확인했으며, 추가 디스코드는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Anthropic은 대규모 신규 자금 조달을 발표하고 동시에 Claude Opus 4.8을 출시했습니다.
-   자본 측면에서 Anthropic은 Altimeter, Dragoneer, Greenoaks, Sequoia가 주도하는 Series H 라운드에서 9,650억 달러의 포스트머니 기업가치로 650억 달러를 유치했다고 밝혔습니다. 이 자금은 연구에 투자하고 증가하는 Claude 수요에 대한 역량을 확장하는 데 사용될 것이라고 말했습니다 (Anthropic).
-   회사는 또한 연간 매출액이 470억 달러를 넘어섰다고 공개했으며, 성장의 원인을 엔터프라이즈 배포와 일상적인 사용에 돌렸습니다 (Anthropic).
-   제품 측면에서 Anthropic은 Claude Opus 4.8을 출시했습니다. 이 모델은 Opus 4.7의 업데이트로서 "더 날카로운 판단력", "자신의 진행 상황에 대한 더 솔직함", 그리고 더 오랫동안 독립적으로 작업할 수 있는 능력을 동일한 가격으로 제공한다고 설명했습니다 (Claude).
-   Anthropic은 또한 Claude Code에 Dynamic Workflows를 출시했습니다. 이는 Claude가 작업을 계획하고 수백 개의 병렬 서브에이전트를 생성하여 대규모 작업을 처리하는 연구 프리뷰 오케스트레이션 시스템입니다 (ClaudeDevs). 독립적인 평가 게시물들은 4.8이 4.7에 비해 특히 장기적인 에이전틱 코딩 및 지식 작업에서 의미 있는 개선을 이루었음을 전반적으로 확인했습니다. 하지만 이것이 프론티어를 재설정하는 도약인지, 아니면 주로 OpenAI의 GPT-5.5-패밀리를 따라잡는 것인지에 대해서는 의견이 엇갈렸습니다.

## 사실 대 의견

### 사실 및 직접 진술된 주장
-   Anthropic은 Series H에서 9,650억 달러의 포스트머니 기업가치로 650억 달러를 유치했습니다 (Anthropic).
-   회사는 연간 매출액이 470억 달러를 넘어섰다고 말합니다 (Anthropic).
-   주요 투자자로 Altimeter, Dragoneer, Greenoaks, Sequoia가 지명되었습니다 (Anthropic).
-   Altimeter는 라운드를 주도했으며 현재까지 가장 큰 투자라고 공개적으로 확인했습니다 (Altimeter, Pauline Bhyang).
-   Anthropic은 Claude Opus 4.8을 출시했으며, Opus 4.7의 업데이트로서 향상된 판단력, 솔직함, 더 긴 자율 작업 능력을 동일한 가격으로 제공한다고 포지셔닝했습니다 (Claude).
-   Anthropic 엔지니어들은 4.8이 4.7 피드백에 대한 응답으로 "많은 수정 사항"과 더 나은 뉘앙스/자연스러움을 포함한다고 말했습니다 (Alex Albert).
-   Claude Code는 이제 오케스트레이션 계획을 작성하고 대규모 플릿/수백 개의 서브에이전트를 병렬로 실행하는 Dynamic Workflows를 지원합니다 (ClaudeDevs, Cat Wu).
-   Dynamic Workflows는 연구 프리뷰로 제공되며 Max, Team, Enterprise, API, Bedrock, Vertex AI, Foundry에서 작동한다고 합니다 (ClaudeDevs).
-   Anthropic/커뮤니티 게시물들은 웹/앱/Cowork에 노력 제어 기능이 추가되었고 Fast 모드 지원이 계속된다고 언급했습니다 (Mikey K, Sam Callister, Kimmonismus).

### 의견 / 해석
-   낙관적인 견해:
    *   Opus 4.8은 "Opus 5라고 불릴 수도 있었다" (Dan Shipper).
    *   "Anthropic이 게으름에 대한 치료법을 찾았다" (scaling01).
    *   솔직함/정확성 덕분에 "오랜만에 나온 첫 스마트 모델" (zephyr_z9).
    *   "Anthropic 구독을 취소했던 사람들이 다시 돌아올 것이다" (teortaxesTex).
-   회의적이거나 엇갈린 견해:
    *   Opus 4.8은 "사소한 업그레이드" (scaling01).
    *   Anthropic은 "속도를 주도하기보다는 OpenAI를 따라잡는 데 주력하고 있다" (kimmonismus).
    *   Andon Labs의 벤치마크 기반 비판: Vending Bench에서 Opus 4.7 / GPT-5.5보다 성능이 떨어졌고, Blueprint-Bench 2에서 기대 이하의 성능을 보였으며, 더 정렬되고/더 신중하며, "최대 추론이 최상의 추론 노력은 아니다" (andonlabs, andonlabs).
    *   Dynamic Workflows는 강력하지만 실제로 토큰 비용이 많이 들고 할당량을 빠르게 소진할 수 있습니다 (itsclivetime, Theo, Omar Sar0).

## 자금 조달 세부 사항 및 시사점
Anthropic의 자금 조달 수치는 헤드라인을 장식한 충격입니다: 9,650억 달러의 포스트머니 기업가치로 650억 달러를 유치했으며, 같은 발표에서 470억 달러의 연간 매출액을 공개했습니다 (Anthropic, Anthropic). 이러한 규모는 즉각적인 주목을 받았습니다. 이는 하이퍼스케일러급 자본 요구 사항과 모델 서빙 경제성을 가진 거의 1조 달러에 달하는 기업 가치로 운영되는 회사를 의미하기 때문입니다.
투자자 메시지는 엔터프라이즈 채택과 운영 실행에 강하게 초점을 맞췄습니다. Altimeter는 Claude가 "전체 엔터프라이즈의 기본 운영 체제"가 되고 있다고 설명했으며, Anthropic의 성능과 안전성 조합을 칭찬했습니다 (Altimeter). Pauline Bhyang은 Anthropic이 2022년부터 "세대적인 궤적"을 밟아왔으며, 5년도 채 안 되어 470억 달러의 연간 매출액을 넘어섰다는 점을 강조했습니다 (Pauline Bhyang).
주변 반응은 몇 가지 진영으로 나뉘었습니다:
-   **검증 진영:** 이 자금 규모는 Claude가 특히 코딩 및 에이전틱 워크플로우에서 핵심 엔터프라이즈 플랫폼이 되었다는 증거로 간주됩니다. Jamin Ball의 "Let’s go!!"와 같은 게시물은 단순한 시장 검증 반응이었습니다 (jaminball).
-   **규모/거품 우려 진영:** 일부는 이 발표를 전례 없는 규모로 부풀려진 전통적인 스타트업 자금 조달 수사법에 비유하며 반응했습니다. Jerry Liu는 "수십억"을 "수백만"으로 바꾸면 여느 고성장 스타트업의 자금 조달처럼 읽힌다고 농담했습니다 (jerryjliu0). 또 다른 비판적인 해석은 이 자금 조달을 Anthropic이 더 강력한 모델에 대해 점점 더 엄격하게 적용하는 안전 게이팅과 연결했습니다. 즉, 방대한 컴퓨트 접근과 선별적인 기능 출시가 결합된 것입니다 (menhguin).
-   **인프라 시사점:** Anthropic은 자금 유치를 Claude 수요를 위한 용량 확장과 명시적으로 연결했습니다 (Anthropic). 이는 새로운 4.8 기능, 특히 더 많은 노력을 요구하는 추론, 더 긴 독립 실행, 그리고 멀티 에이전트 워크플로우가 인퍼런스 집약적이기 때문에 중요합니다. 이번 자금 조달은 학습 자금뿐만 아니라 장기 실행 에이전트 워크로드의 서빙 비용을 보증하려는 직접적인 시도로 해석되어야 합니다.
한 가지 주목할 만한 맥락 트윗: 한 사용자는 Mythos 안전성 우려가 해결된 것으로 보이는 시점에 "Anthropic이 수백억 달러 규모의 인퍼런스 컴퓨트도 확보했다"고 추측했습니다 (menhguin). 이는 Anthropic에 의해 확인된 바 없는 추측이지만, 이번 라운드가 모델 R&D만큼이나 컴퓨트 공급 및 배포 규모에 관한 것이라는 일반적인 해석을 반영합니다.

## Opus 4.8: 공식 제품 포지셔닝
Anthropic의 공식 프레이밍은 벤치마크 점수뿐만 아니라 행동 품질에 대한 강조가 이례적으로 구체적입니다. 출시 트윗에 따르면 4.8은 다음을 특징으로 합니다:
-   더 날카로운 판단력
-   자신의 진행 상황에 대해 더 솔직함
-   더 오랫동안 독립적으로 작업할 수 있는 능력
-   4.7과 동일한 가격 (Claude)
Alex Albert는 4.8이 다음을 추가했다고 덧붙였습니다:
-   4.7 피드백을 기반으로 한 수정 사항 통합,
-   뉘앙스를 더 잘 이해,
-   대화에서 더 자연스럽게 느껴짐,
-   코딩 및 지식 작업 전반에서 더 강력해짐 (Alex Albert).
이 솔직함/정확성 측면은 주요 하위 테마가 되었습니다. 여러 Anthropic 직원과 외부 테스터들은 이 모델이 다음을 더 기꺼이 수행한다고 설명했습니다:
-   모르는 것을 말하고,
-   자신의 코드에서 결함을 표시하고,
-   불확실한 진행 상황을 얼버무리지 않고,
-   작업 완료를 잘못 암시하는 것을 멈춥니다 (Cat Wu, Mikey K, dejavucoder).
이는 Claude의 이전 평판이 강력한 코드 생성 능력에도 불구하고 불균일한 자기 모니터링(코드 리뷰에서 오탐, 과도하게 자신감 있는 진행 요약, 그리고 "게으르거나" 조기에 중단되는 작업 실행)을 포함했기 때문에 주목할 만합니다. 여러 커뮤니티 반응은 4.8이 이러한 실패 모드를 수정했다고 명시적으로 언급했습니다:
-   "게으름에 대한 치료법을 찾았다" (scaling01)
-   "역대 가장 게으르지 않은 모델?" (Teknium)
-   "다른 모든 Claude 버전보다 훨씬 덜 게으르다" (nrehiew_)

## 기술 세부 사항 및 수치

### 가격, 컨텍스트, 제어
가장 구체적이고 통합된 사양은 Artificial Analysis에서 나왔습니다:
-   컨텍스트 윈도우: 100만 토큰
-   가격: 입력/출력 토큰 100만 개당 $5 / $25
-   캐시 쓰기: 5분 TTL로 100만 개당 $6.25
-   캐시 히트: 100만 개당 $0.50
-   노력 설정은 Opus 4.7과 동일하게 유지되며; AA는 최대 노력을 테스트했습니다 (Artificial Analysis).
커뮤니티 게시물들은 또한 다음을 강조했습니다:
-   Opus 4.8에 Fast 모드를 사용할 수 있습니다.
-   이전 Fast 모드 경제성과 비교하여 약 2.5배 빠르고 3배 저렴합니다 (kimmonismus).
-   scaling01은 새로운 경제성을 다음과 같이 요약했습니다:
    *   Opus 4.8 Fast: 2.5배 빠르고, 일반 4.8보다 2배만 더 비쌉니다.
    *   Opus 4.7 Fast: 2.5배 빠르고, 일반 4.7보다 6배 더 비쌌습니다 (scaling01).
-   노력 제어 기능이 더 많은 제품 인터페이스에 새로 노출되어 사용자가 추론 강도를 높이거나 낮출 수 있게 했습니다 (sammcallister, mikeyk, kimmonismus).
이는 초기 사용자 보고서에서 추론 노력 선택이 특히 코딩 및 글쓰기에서 출력 품질과 비용을 크게 변화시킨다고 제안하기 때문에 중요합니다. Dan Shipper는 낮은 설정에서 더 약한 행동을 관찰한 후 코딩에는 xhigh를, 글쓰기에는 high를 권장했습니다 (Dan Shipper). Andon Labs도 일부 작업에서 최대 추론이 최상의 추론 노력은 아니라고 말했습니다 (andonlabs).

### 벤치마크: 가장 강력하게 보고된 수치
출시 트윗을 통해 주요 공식/반공식 수치가 공개되었습니다:
-   SWE-Bench Pro: 69.2%, Yuchen이 출시 자료를 인용하여 주장했으며, "GPT-5.5보다 10점 높다" (Yuchenj_UW).
-   FrontierSWE #1, Anthropic 관찰자들이 인용했으며 나중에 제3자 참조를 통해 확인되었습니다 (scaling01, scaling01).
-   APEX-SWE: Pass@1 45.3%, GPT-5.3 Codex의 41.5%보다 거의 4점 앞섰습니다 (mercor_ai).
-   GDPval-AA: 1890 ELO, Opus 4.7 대비 +137, GPT-5.5 xhigh 대비 +121, 이는 GPT-5.5 xhigh와의 일대일 대결에서 약 67%의 승률을 의미합니다 (Artificial Analysis).
-   Artificial Analysis Intelligence Index: 61.4, Opus 4.7 대비 +4.1, GPT-5.5 xhigh 대비 +1.2 앞섰습니다 (Artificial Analysis).
-   AA-Omniscience: 27.4, Gemini 3.1 Pro의 32.9에 이어 2위; 정확도 46.6%, 환각 35.9% (Artificial Analysis).
-   개선된 부분:
    *   Terminal-Bench Hard +6.8
    *   τ²-Bench Telecom +5.9
    *   IFBench +3.6
    *   AA-LCR, GPQA, SciCode에서는 상대적으로 변화가 없었습니다 (Artificial Analysis).
추가적인 정성적 벤치마크 관찰:
-   Cursor는 Opus 4.8이 CursorBench에서 4.7보다 훨씬 효율적으로 작동하며 어려운 작업에서 더 끈기 있다고 말했습니다 (Cursor).
-   Anthropic 직원들은 Claude Code의 장기적인 작업에서 강점을 강조했습니다 (ClaudeDevs).
-   일부 사용자들은 지식 작업 및 글쓰기에서 특히 큰 도약을 보고했습니다 (Dan Shipper, rishdotblog).

### 효율성 및 토큰 사용 세부 정보
Artificial Analysis는 다음과 같이 보고했습니다:
-   Opus 4.7과 비교하여 4.8은 다음을 통해 더 높은 GDPval 성능을 달성했습니다:
    *   작업당 턴 수 15% 감소
    *   출력 토큰 35% 감소
-   하지만 4.8은 여전히 2위 모델인 GPT-5.5보다 약 30% 더 많은 턴을 사용했습니다 (Artificial Analysis).
이는 출시 보도에서 가장 중요한 미묘한 발견 중 하나입니다:
-   4.8은 4.7보다 효율적입니다.
-   하지만 일부 워크로드에서 OpenAI에 비해 가장 인퍼런스 효율적인 프론티어 모델은 아닙니다.
이러한 긴장감은 커뮤니티 논평에서도 반복됩니다:
-   "여전히 GPT-5.5에 의해 토큰을 많이 소모당한다" (scaling01).
-   Theo와 다른 사람들은 Claude의 더 높은 에이전시, 더 많은 노력을 요구하는 모드가 실제로 할당량을 매우 빠르게 소진할 수 있다고 불평했습니다 (Theo, cremieuxrecueil).

### 긴 컨텍스트
게시물들은 Opus 4.6에서 4.8로의 긴 컨텍스트 개선을 강조했으며, 한 주장은 1M 컨텍스트의 Opus 4.8이 참조된 긴 컨텍스트 평가에서 GPT-5.5의 256K 점수와 거의 동일하다고 했습니다 (scaling01). Artificial Analysis도 1M 토큰 컨텍스트가 그대로 유지되었음을 확인했습니다 (Artificial Analysis).

### 안전성 / 견고성 / 환각
이것은 출시의 엇갈린 부분 중 하나였습니다.
긍정적:
-   Anthropic과 지지자들은 낮은 부정직성/더 나은 정확성을 강조했습니다.
-   "부정직성이 역대 최저 수준" (scaling01).
-   "눈에 띄게 더 솔직함" (Cat Wu).
-   "불확실한 것을 표시합니다" (Mikey K).
-   Artificial Analysis는 Anthropic이 Google/OpenAI 경쟁사보다 훨씬 낮은 환각률을 계속 보여준다고 말했습니다 (Artificial Analysis).
부정적 / 주의 사항:
-   scaling01은 Opus 4.8이 100번의 시도에서 프롬프트 인젝션 견고성을 개선하지 못한 오랜만의 첫 모델이라고 언급했습니다 (scaling01).
-   scaling01은 또한 이 모델을 Anthropic의 "가장 평가 인지도가 높은 모델"이라고 불렀습니다 (scaling01).
-   Andon Labs는 이 모델이 더 정렬되고/더 신중하며, "들킬까 봐 두려워하고", 일부 적대적/비즈니스 작업 벤치마크에서 성능이 떨어졌다고 말했습니다 (andonlabs).
-   nrehiew_는 보고된 평가에서 약간의 환각 개선이 있었지만, 일부 환각 테스트가 사용자들이 실제로 겪는 실패 모드를 반영하는지에 대해서는 의문을 제기했습니다 (nrehiew_, nrehiew_).

### 사이버 기능 게이팅 및 미래 모델 클래스
특히 중요한 전략적 세부 사항이 반응 게시물에 나타났습니다: Anthropic은 더 강력한 안전 장치 후에 "Opus보다 훨씬 더 높은 지능을 가진 새로운 클래스의 모델"을 출시할 계획이라고 밝힌 것으로 보입니다 (dejavucoder). 여러 관찰자들은 이를 사이버 민감 기능이 선택적으로 제한된 Mythos 클래스 출시로 해석했습니다:
-   "몇 주 안에 모든 고객에게 Mythos 클래스 모델을 출시할 것" (kimmonismus).
-   "그들은 적절한 안전 장치를 갖춘 Mythos 클래스 모델을 출시하고 있습니다. 즉, '출시하기에는 너무 위험한' 기능은 사용할 수 없습니다" (scaling01).
-   Cline은 Anthropic이 더 강력한 사이버 안전 장치를 추가한 후 Opus보다 더 높은 지능을 가진 새로운 모델을 출시할 계획을 발표했다고 요약했습니다 (Cline).
이는 단순한 제품 로드맵 소문이 아닙니다. 이는 Opus 4.8을 단계별 출시 전략으로 재구성합니다:
1.  상업적으로 안전하고/광범위하게 배포 가능한 일반 모델을 개선하고,
2.  제어 준비가 될 때까지 더 위험한 사이버 기능을 보류합니다.
이러한 절충안은 칭찬과 비판을 동시에 받았습니다:
-   지지: 안전 우선 프론티어 배포
-   회의적: Anthropic이 위험 태세를 유지하기 위해 원시 기능 가용성에서 일부 경쟁력을 희생하고 있을 수 있습니다 (teortaxesTex).

## Dynamic Workflows: 기본 모델을 넘어선 가장 중요한 기술적 추가 사항
Opus 4.8과 함께 제공되는 뛰어난 시스템 기능은 Claude Code의 Dynamic Workflows입니다.
공식 설명:
-   "Claude가 즉석에서 오케스트레이션 스크립트를 작성합니다."
-   그런 다음 대규모의 조정된 서브에이전트 플릿을 병렬로 가동합니다.
-   프롬프트에 "workflow"라는 단어를 사용하여 활성화합니다 (ClaudeDevs).
Anthropic 직원과 사용자들은 이 기능이 다음을 가능하게 한다고 설명했습니다:
-   Claude가 "엄격하게 따르는" 오케스트레이션 계획
-   수백 개의 에이전트
-   결과를 반환하기 전에 검증
-   매우 큰 마이그레이션/리팩터링/감사 작업 지원 (Cat Wu, Mikey K)
인용된 예시:
-   Bun을 Zig에서 Rust로 포팅하는 작업 (약 75만 라인, 테스트 스위트의 99.8% 통과, 첫 커밋부터 병합까지 11일 소요, 수백 개의 병렬 에이전트와 파일당 두 명의 검토자 사용) (Cat Wu).
-   10분 이내에 수백 개의 A/B 테스트 플래그를 병렬로 처리하여 오래된 플래그를 식별합니다 (Cat Wu).
이 출시는 더 넓은 개념에 대한 소규모 논쟁을 촉발했습니다:
-   일부 연구자들은 Anthropic이 재귀적 언어 모델/프롬프트에 대한 기호적 재귀와 유사한 아이디어를 본질적으로 제품화했다고 주장했습니다 (a1zhang, lateinteraction, lateinteraction).
-   다른 사람들은 "모델을 반복적으로 호출하는 것"은 새로운 것이 아니며, 많은 개발자들이 몇 달 동안 수동으로 이 작업을 해왔다고 반박했습니다 (omarsar0, jxmnop, willdepue).
더 실질적인 비판은 독창성이 아니라 비용과 하네스 품질이었습니다:
-   Omar Sar0는 에이전트 간 상호 작용은 효과적이지만 토큰 소모가 많다고 경고했습니다 (omarsar0).
-   Theo는 현재 툴링에서 충돌하는 병렬 편집과 낭비되는 토큰에 대해 불평했습니다 (Theo, cremieuxrecueil).
-   itsclivetime은 "수백 개의 병렬 서브에이전트"가 몇 초 만에 할당량을 소진할 것이라고 농담했습니다 (itsclivetime).
-   KLieret은 시스템 카드에서 멀티 에이전트가 최종 ProgramBench 품질을 개선하지 못할 수도 있지만, 평범한 솔루션에는 2배 더 빠르게 도달한다는 사실을 강조했습니다 (KLieret).
따라서 기술 사용자들의 합의는 다음과 같습니다:
-   Dynamic Workflows는 전략적으로 중요합니다.
-   이는 코딩 에이전트의 미래가 될 가능성이 높습니다.
-   하지만 현재 구현은 여전히 편집 충돌, 비용 폭증, 하네스 비효율성에 직면해 있습니다.

## Opus 4.8에 대한 다양한 의견

### 1) 강력한 지지: Anthropic이 돌아왔습니다.

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 무료 액세스 권한을 얻으세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-anthropic-raises-965b-series&utm_source=paywall-free-trial&utm_medium=web&utm_content=199680854&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인하세요.](https://substack.com/sign-in?redirect=%2Fp%2Fainews-anthropic-raises-965b-series&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
