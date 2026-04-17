# Anthropic Claude Opus 4.7 - literally one step better than 4.6 in every dimension

**원문 URL**: https://www.latent.space/p/ainews-anthropic-claude-opus-47-literally
**번역일**: 2026-04-17 06:36
**발행일**: 2026-04-17

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Anthropic Claude Opus 4.7 - 모든 면에서 4.6보다 문자 그대로 한 단계 더 발전했습니다

### 새로운 SOTA 모델이 지배력을 확고히 합니다.
공유목요일 아침은 권위 있는 AI 출시를 위한 시간이며, OpenAI가 GPT-Rosalind와 The New New Codex(놀라운 컴퓨터 사용 능력 포함)로 맹렬한 노력을 기울였지만, 오늘 주요 기사의 승자가 누구일지는 의문의 여지가 없었습니다. 지난 AINews 발행본을 자세히 살펴보셨다면 지난 한 주 동안 이 소문에 대해 보셨을 테지만, 오늘 Claude Opus 4.7 출시는 그러한 기대를 약간 상회했습니다.
핵심 차트는 다음과 같습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/7242e5f5-6105-4489-bc8b-143002fe7da6_1344x756.png)
기본적으로 4.7-low는 4.6-medium보다 엄격히 우수하고, 4.7-medium은 4.6-high보다 엄격히 우수하며, 4.7-high는 이제 4.6-max보다 우수합니다. 그리고 Claude Code가 기본으로 사용하는 새로운 xhigh 노력 수준이 있습니다. Anthropic은 새로운 토크나이저(새로운 사전 학습?)가 최대 35% 더 많은 토큰 사용량을 유발할 수 있다고 말하지만, 전반적인 추론 효율성이 너무 많이 향상되어 전체 토큰 사용량은 여전히 이전 모델 대비 최대 50% 감소했습니다. 진정한 시험은 SWE-Bench Pro에서 11점 더 높아진 기본 Claude Code가 사용자 자신의 사용 사례에서 눈에 띄게 더 나은 성능을 보이는지 여부입니다.
문자 그대로 직접 봐야 믿을 수 있는 또 다른 주목할 만한 기능은 "상당히 개선된 비전"입니다. Opus 4.7은 고해상도 이미지에 대한 비전이 더 좋습니다. 긴 쪽이 최대 2,576픽셀(약 3.75메가픽셀)인 이미지를 받아들일 수 있으며, 이는 이전 Claude 모델보다 세 배 이상 많은 수치입니다. 이는 미세한 시각적 디테일에 의존하는 풍부한 멀티모달 활용 사례를 가능하게 합니다: 밀도 높은 스크린샷을 읽는 컴퓨터 사용 에이전트, 복잡한 다이어그램에서 데이터 추출, 픽셀 단위의 정확한 참조가 필요한 작업 등입니다. 자세한 내용은 아래의 집중 주제 요약에서 확인하십시오.
> 2026년 4월 14일-4월 16일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 모든 과거 발행본을 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# 주요 소식: Claude Opus 4.7
Anthropic은 Claude Opus 4.7을 최신 최고 티어 Opus 모델로 공식 출시했습니다. 사용자 요약 및 출시 논의에 따르면 [@claudeai, @kimmonismus], Opus 4.7은 Opus 4.6보다 장기 실행 작업, 코딩, 명령어 준수, 자체 검증, 컴퓨터 사용 및 지식 작업에서 더 뛰어나며, 백만 입력/출력 토큰당 $5 / $25의 정가는 유지됩니다. 이번 출시는 벤치마크 성능 향상, 새로운 토크나이저, 더 높은 이미지 해상도 지원, 새로운 xhigh 추론 노력 수준, 토큰 비용 영향, 그리고 Opus 4.7이 직계 4.6 후속 모델인지, 새로운 기반 모델인지, 아니면 부분적으로 디스틸레이션된 "Mythos 인접" 시스템인지에 대한 이례적으로 활발한 기술적 논의를 촉발했습니다.

## 출시 세부 정보 및 제품 변경 사항
공식적인 설명. Anthropic의 출시 설명은 세 가지 행동 개선 사항을 강조했습니다: 장기 실행 작업 처리 개선, 더 정확한 명령어 준수, 그리고 응답 전 더 강력한 자체 검증 [@claudeai].
가용성.
- Claude 플랫폼/앱은 즉시 라이브로 보고되었습니다 [@dejavucoder].
- Claude Code는 출시와 동시에 지원했으며 xhigh를 기본 노력 수준으로 설정했습니다 [@_catwu, @_catwu].
- Anthropic은 또한 공개 베타로 작업 예산을 출시하거나 강조했으며, Claude Code에 /ultrareview 기능을 추가하고 Claude Code Max 사용자에게 더 넓은 Auto 모드 접근성을 제공했습니다 [@kimmonismus].
새로운 노력 티어.
- 여러 사용자가 high와 max 사이에 위치하는 새로운 xhigh 추론 노력 모드를 언급했습니다 [@scaling01, @scaling01].
- Cat Wu는 Claude Code가 이제 Opus 4.7에 대해 기본적으로 xhigh를 사용한다고 말했습니다 [@_catwu].
비전/컴퓨터 사용 변경 사항.
- 사용자 요약에 따르면 긴 쪽이 최대 2,576픽셀(약 3.75MP)인 이미지를 지원하며, 이는 이전 Claude 이미지 입력보다 3배 더 크다고 설명되었습니다 [@kimmonismus].
- Anthropic 직원 Alex Albert는 "고해상도 이미지 다운스케일링이 더 이상 없다"는 점과 UI/슬라이드/문서에서 더 나은 출력 품질을 강조했습니다 [@alexalbert__].
- 이는 더 나은 컴퓨터 사용 및 스크린샷 위주의 워크플로우와 반복적으로 연결되었습니다 [@dejavucoder, @omarsar0].
토크나이저 및 토큰 경제학.
- 여러 관찰자들이 Opus 4.7이 4.6과 다른 토크나이저를 사용한다는 것을 발견했습니다 [@natolambert, @nrehiew_].
- Kimmonismus는 Anthropic의 주의 사항을 요약했는데, 동일한 입력이 콘텐츠 유형에 따라 1.0~1.35배 더 많은 토큰으로 매핑될 수 있다는 내용입니다 [@kimmonismus].
- 이는 4.7이 사실상 새로운 기반 모델인지, 토크나이저가 교체된 연속 모델인지, 아니면 Mythos로부터의 일종의 중간 학습/디스틸레이션 브릿지인지에 대한 논쟁을 촉발했습니다 [@natolambert, @stochasticchasm, @eliebakouch, @maximelabonne].
- Anthropic 직원 Boris Cherny는 나중에 증가된 토큰 사용량을 상쇄하기 위해 모든 구독자의 한도를 늘렸다고 말했습니다 [@bcherny, @bcherny].

## 벤치마크 및 측정 가능한 진전

### Opus 4.6 대비 보고된 벤치마크 성능 향상
가장 많이 인용된 출시 수치는 외부 계정에서 공유한 벤치마크 스크린샷 및 요약에서 나왔습니다:
- SWE-bench Pro: 64.3%, 사용자들은 Opus 4.6 대비 약 +11점 상승을 언급했습니다 [@scaling01, @kimmonismus]
- SWE-bench Verified: 87.6%, 4.6 대비 약 +7점 상승 [@scaling01, @scaling01]
- TerminalBench 2.0: 69.4%, 약 +4점 상승 [@scaling01, @kimmonismus]
- Document reasoning: 80.6%, 타사 논의에 따르면 57.1%에서 상승 [@scaling01, @llama_index]
- GDPval-AA: 1753 Elo [@scaling01, @ArtificialAnlys]
- ARC-AGI-1: 92%; ARC-AGI-2: 75.83% [@scaling01]
Artificial Analysis는 Opus 4.7이 GDPval-AA에서 새로운 1위로 출시되었으며, 해당 작업 세트에서 GPT-5.4 대비 약 60%의 일대일 승률을 암시한다고 말했습니다 [@ArtificialAnlys].
- Anthropic은 더 많은 토큰 사용량을 보상하기 위해 구독자 한도를 늘렸습니다 [@bcherny, @bcherny].
- Anthropic은 벤치마크 트레이드오프를 인정하고 "과학적 정직성"을 위해 시스템 카드에 MRCR을 유지하면서, Graphwalks를 선호하는 장문 컨텍스트 메트릭으로 전환할 것임을 시사했습니다 [@bcherny].
Vals AI는 Opus 4.7이 Vals Index에서 71.4%로 1위를 차지했으며, 이전 최고 기록인 67.7%에서 상승했고, Vibe Code Bench, Vals Multimodal, Finance Agent, Mortgage Tax, SAGE, SWE-Bench, Terminal Bench 2에서도 1위를 차지했다고 말했습니다 [@ValsAI].
그들은 별도로 Opus 4.7이 Vibe Code Benchmark에서 71%로 1위를 차지했으며, 4.5개월 전 벤치마크를 처음 출시했을 때는 25%를 넘는 모델이 없었다고 말했습니다 [@ValsAI].

### 파트너 및 고객의 제품/평가
- Cursor는 Opus 4.7으로 내부 벤치마크가 58%에서 70%로 상승했다고 말했습니다 [@cursor_ai, @scaling01].
- 별도의 Cursor 게시물에 따르면, 500개 팀에 걸쳐 개발자들이 올해 68% 더 많은 고난도 작업을 처리하고 있지만, 이는 Opus 4.7에만 국한된 것이 아니라 전반적으로 더 나은 모델에 대한 내용이었습니다 [@cursor_ai].
- Notion은 내부 평가에서 14% 향상을 보였고, 도구 오류는 3분의 1로 줄었다고 보고했습니다 [@mikeyk].
- GitHub도 비슷한 개선을 보였다고 보고했지만, 트윗 스레드에는 구체적인 수치가 포함되지 않았습니다 [@scaling01].

### 문서 이해: 진전은 있지만 경제성은 혼재
LlamaIndex와 Jerry Liu는 유용한 독립적인 뉘앙스를 제공했습니다:
- LlamaIndex의 ParseBench 방식 비교에 따르면 Opus 4.7은 차트에서 엄청난 개선(13.5% → 55.8%)을 보였지만, 포맷팅(64.2% → 69.4%), 콘텐츠(89.7% → 90.3%), 테이블(86.5% → 87.2%)은 약간만 개선되었고, 레이아웃(16.5% → 14.0%)은 퇴보했습니다 [@llama_index].
- Jerry Liu는 별도로 Opus 4.7이 "테이블에 상당히 능숙하고", 차트에서 더 좋으며, 콘텐츠 충실도에서 가장 강력하지만, OCR과 유사한 사용에는 페이지당 약 7센트로 비용이 많이 든다고 말했습니다. 반면 그들의 에이전틱 모드는 페이지당 약 1.25센트, 비용 효율적인 모드는 페이지당 약 0.4센트입니다 [@jerryjliu0].
이는 독립적인 평가가 출시 낙관론을 완화하는 가장 명확한 사례 중 하나입니다. 전반적인 기능은 향상되었지만, 특정 기업 문서 파이프라인은 비용/성능 측면에서 여전히 전문화된 스택을 선호할 수 있습니다.

### 의견 / 해석
- "이것은 Mythos의 디스틸레이션 버전입니다" [@eliebakouch].
- "토크나이저가 변경되었기 때문에 이것은 새로운 기반 모델입니다" [@natolambert].
- "Anthropic이 학습 중에 사이버 점수를 인위적으로 낮게 유지했습니다"는 사용자들이 시스템 카드에서 일부 기능을 차등적으로 줄였다는 문구를 인용하는 한 부분적으로 사실이지만, "너프된 Mythos"에 대한 더 광범위한 주장은 해석에 불과합니다 [@scaling01, @Yuchenj_UW].
- "벤치마크만으로는 그 진가를 알 수 없습니다"와 "실제 사용 경험은 엄청나게 개선되었습니다"는 주관적이지만 실제 사용자들에 의해 널리 반복되고 있습니다 [@mweinbach, @jeremyphoward].
- "시스템 프롬프트가 모델을 로보토마이즈(둔화)시켰습니다"는 행동 변화에 대한 사용자 불만이지, 확립된 사실은 아닙니다 [@theo].

## 다양한 관점

### 지지적: 의미 있는 실제 사용 개선
상당수의 기술 사용자들이 특히 더 빈번한 출시 주기를 고려할 때, 이번 업데이트가 상당한 개선이라고 주장했습니다.
- Scaling01은 "중간 업데이트"라는 평가에 반복적으로 반박하며, SWE-bench Verified에서 약 80%에서 거의 90%로의 도약을 언급하고, 이전 출시 주기에서는 이것이 엄청나게 보였을 것이라고 강조했습니다 [@scaling01, @scaling01, @scaling01].
- Alex Albert는 더 나은 비동기 작업, 더 예측 가능한 노력 수준, 더 나은 이미지 처리, 그리고 UI/문서에서 더 강력한 품질을 강조했습니다 [@alexalbert__].
- Michael Weinbach는 단 두 번의 프롬프트 후 행동과 명령어 준수에서 "상당히 큰" 개선이 있었다고 말했습니다 [@mweinbach].
- Jeremy Howard는 자신이 무엇을 하는지 "이해하는" 첫 번째 모델이며, 무작정 밀어붙이기보다는 논의하려는 의지를 칭찬했습니다 [@jeremyphoward, @jeremyphoward].
- Cat Wu는 사용자들에게 마이크로매니징하는 페어 프로그래머가 아니라, 작업을 위임하는 엔지니어처럼 대하라고 명시적으로 조언하며, Anthropic이 이 모델을 자율 실행에서 더 강력하다고 본다는 점을 시사했습니다 [@_catwu].

### 중립적/분석적: 트레이드오프가 있는 강력한 업데이트
가장 좋은 논평 중 일부는 기술적이고 혼합적이었습니다.
- Kimmonismus는 이를 Anthropic의 핵심 구매자 우선순위인 에이전틱 코딩 신뢰성, 컴퓨터 사용 에이전트를 위한 비전, 그리고 지식 작업에 중점을 둔 "견고한 업그레이드"라고 불렀지만, "Mythos에 비해 분명히 부족하다"고 덧붙였습니다 [@kimmonismus].
- Artificial Analysis는 GDPval-AA 성능 향상과 1위 순위를 검증했지만, 전반적인 압승으로 평가하지는 않았습니다 [@ArtificialAnlys].
- LlamaIndex와 ParseBench 결과는 실제 가격 제약이 있는 상황에서 눈에 띄지만 고르지 않은 문서 처리 성능 향상을 시사했습니다 [@llama_index, @jerryjliu0].

### 회의적/비판적: 퇴보, 토큰 인플레이션, UX 문제
상당한 반발도 있었습니다.
- 여러 사용자는 장문 컨텍스트 성능이 더 나빠 보였으며, 특히 MRCR / 건초 더미 속 바늘 찾기 방식의 메트릭에서 그러했다고 말했습니다 [@scaling01, @nrehiew_, @eliebakouch, @kimmonismus].
- Anthropic의 Boris Cherny는 MRCR이 방해 요소 쌓기 트릭에 과도한 가중치를 부여하기 때문에 단계적으로 폐지되고 있으며, Graphwalks가 더 나은 응용 추론 신호라고 답했습니다. 그는 4.6에서 4.7로 Graphwalks가 38.7%에서 58.6%로 상승했음을 보여주는 수치를 제시했습니다 [@bcherny, @scaling01].
- 토크나이저 변경은 Opus가 "토큰 먹는 하마"가 되어 정가는 유지되었음에도 불구하고 실질적인 비용을 증가시킬 수 있다는 불만을 야기했습니다 [@dejavucoder, @madiator].
- Yuchen은 Claude 웹이 "Adaptive" 또는 비사고 모드만 노출했으며, 명시적인 강제 사고 토글이 없었기 때문에 일부 사용자에게는 비코딩 작업이 실제로 더 나쁘게 느껴지게 했다고 말했습니다 [@Yuchenj_UW].
- Mikhail Parakhin도 비슷하게 비코딩 답변에 대한 첫인상이 "더 멍청했다"고 말했는데, 이는 그가 추론을 강제할 수 없었기 때문입니다 [@MParakhin].
- Theo는 새로운 시스템 프롬프트를 "로보토마이즈(둔화)되었다"고 날카롭게 비판했으며, 나중에 T3 Chat에서 "로보토마이즈된 시스템 프롬프트 없이" 모델을 시도해 볼 것을 제안했습니다 [@theo, @theo].

### 안전성 / 거버넌스 관점
- Scaling01은 Anthropic이 학습 중에 사이버 기능을 차등적으로 줄이려는 노력을 실험했다는 시스템 카드 문구를 강조했습니다 [@scaling01].
- 동시에 사용자들은 Opus 4.7이 Firefox 셸 익스플로잇과 같은 일부 익스플로잇 관련 평가에서 4.6보다 여전히 더 높은 점수를 기록하며, Mythos에 가까운 프롬프트 인젝션 견고성을 가지고 있다고 언급했습니다 [@scaling01, @scaling01].
- 한 사용자는 과장하여 "이 속도라면 Opus는 생물학 무기 위험이 될 것입니다"라고 말하며, 일반적인 기능 향상을 최악의 오용 시나리오와 혼동하는 지속적인 경향을 반영했습니다 [@scaling01].

### Anthropic의 Claude Code 워크플로우 가이드
Cat Wu의 스레드는 엔지니어들에게 유용한 운영 신호입니다:
1. 위임하고, 마이크로매니징하지 마십시오 [@_catwu]
2. 전체 목표 + 제약 조건 + 승인 기준을 미리 제시하십시오 [@_catwu]
3. 모델에게 변경 사항을 검증하는 방법을 알려주고; claude.md 또는 스킬에 테스트 워크플로우를 인코딩하십시오 [@_catwu]
이는 Anthropic이 명시적인 검증이 핵심인 자율 작업 루프에 최적화되었음을 강력히 시사합니다.

## 실제 적용 사례

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-anthropic-claude-opus-47-literally&utm_source=paywall-free-trial&utm_medium=web&utm_content=194468374&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-anthropic-claude-opus-47-literally&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
