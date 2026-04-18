# The Two Sides of OpenClaw

**원문 URL**: https://www.latent.space/p/ainews-the-two-sides-of-openclaw
**번역일**: 2026-04-18 12:36
**발행일**: 2026-04-18

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] OpenClaw의 두 가지 측면

### 조용한 하루, 이번 주 OpenClaw를 되돌아봅니다.
Share오늘, 세 개의 주요 컨퍼런스가 동시에 열리는 절묘한 시점에 Peter Steinberger의 TED talk과 AIE talk이 공개되었습니다. 일반 대중에게는 OpenClaw의 감동적인 이야기가 무대 위에서 즐겁게 전달되었고, 이는 모든 성공적인 순간들을 요약합니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/d938eb29-488f-4a91-9b9d-7ba5dabf55af_1416x1022.png)
엔지니어링 청중에게는 더 진지한 내용으로, 역사상 가장 빠르게 성장하는 오픈소스 프로젝트를 유지하는 데 따른 전례 없는 수준의 보안 사고(curl보다 60배 많은 보고, 스킬 기여의 최소 20%가 악성)와 스케일링 문제에 대해 이야기했습니다.
제 진행으로 AMA가 마지막에 포함되어 있습니다.
두 가지 관점을 비교해 보시고, 의견을 환영합니다.
> 2026년 4월 16일-4월 17일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 추가 Discord는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Anthropic의 Claude Opus 4.7 및 Claude Design 출시
- Claude Design이 Anthropic의 첫 디자인/프로토타이핑 표면으로 출시되었습니다: @claudeai는 Claude Opus 4.7 기반의 자연어 지시를 통해 프로토타입, 슬라이드, 원페이저를 생성하는 연구 프리뷰 도구인 Claude Design을 발표했습니다. 이 출시는 Anthropic이 챗/코딩을 넘어 디자인 툴링으로 나아가고 있음을 즉시 보여주었으며, @Yuchenj_UW, @kimmonismus, @skirano를 포함한 여러 관찰자들은 이를 Figma/Lovable/Bolt/v0에 대한 직접적인 공격으로 평가했습니다. 시장 반응 자체도 이야기의 일부가 되었는데, @Yuchenj_UW 등은 발표 후 Figma의 급격한 하락을 언급했습니다. @TheRundownAI를 통해 제품 세부 정보가 공개되었습니다: 인라인 리파인먼트, 슬라이더, Canva/PPTX/PDF/HTML로 내보내기, 그리고 Claude Code로의 핸드오프를 통한 구현이 가능합니다.
- Opus 4.7은 전반적으로 더 강력해 보이지만, 출시 과정은 시끄러웠습니다: 서드파티 벤치마크 게시물들은 대체로 긍정적이었습니다. @arena는 Opus 4.7을 Code Arena에서 1위로 선정했으며, Opus 4.6보다 37점 높고 Anthropic 외 경쟁 모델보다 앞섰습니다. 같은 계정은 Opus 4.7을 Text Arena에서도 코딩 및 과학 분야에서 카테고리 우승을 차지하며 전체 1위로 평가했습니다. @ArtificialAnlys는 Intelligence Index 상위권에서 Opus 4.7 57.3, Gemini 3.1 Pro 57.2, GPT-5.4 56.8로 거의 3파전 무승부를 보고했으며, GDPval-AA(이들의 에이전틱 벤치마크)에서도 Opus 4.7을 1위로 선정했습니다. 또한 Opus 4.6보다 약 35% 적은 출력 토큰으로 더 높은 점수를 기록했으며, 태스크 예산 도입과 적응형 추론을 선호하는 확장된 사고의 완전한 제거를 언급했습니다. 그러나 출시 후 첫 24시간 동안 사용자 경험은 엇갈렸습니다: @VictorTaelin은 회귀 및 컨텍스트 오류를 보고했고, @emollick은 Anthropic이 다음 날까지 적응형 사고 행동을 이미 개선했다고 말했으며, @alexalbert__는 많은 초기 버그가 수정되었음을 확인했습니다. @theo는 Design 자체의 제품 안정성에 대한 불만과 같은 계정에서 계정 수준 안전성 문제에 대한 불만도 있었습니다.
- 비용/효율성 논의가 순수 품질만큼이나 중요해졌습니다: @scaling01은 일부 ML 문제 실행에서 이전 하이엔드 모델 대비 약 10배 적은 토큰으로 유사한 성능을 유지했다고 주장했으며, @ArtificialAnlys는 Opus 4.7을 텍스트와 코드 모두에서 가격/성능 파레토 프론티어에 위치시켰습니다. 모든 벤치마크가 절대적인 리더십에 동의한 것은 아닙니다(예: @scaling01은 LiveBench에서 여전히 Gemini 3.1 Pro 및 GPT-5.4에 뒤처진다고 언급했습니다). 그러나 이러한 게시물들의 공통된 의견은 Anthropic이 모델의 에이전틱 유틸리티와 효율성을 실질적으로 개선했다는 것입니다.
컴퓨터 사용, 코딩 에이전트, 하네스 디자인
- 컴퓨터 사용 UX가 주류 제품 카테고리가 되고 있습니다: OpenAI의 Codex 데스크톱/컴퓨터 사용 업데이트는 실무자들로부터 이례적으로 강력한 반응을 이끌어냈습니다. @reach_vb는 서브에이전트 + 컴퓨터 사용이 실질적인 느낌에서 AGI에 "매우 가깝다"고 말했으며, @kr0der, @HamelHusain, @mattrickard, @matvelloso는 모두 Codex Computer Use가 화려할 뿐만 아니라 빠르며, Slack, 브라우저 플로우, 임의의 데스크톱 앱을 구동할 수 있고, 엔터프라이즈 레거시 소프트웨어에 대한 최초의 진정으로 사용 가능한 컴퓨터 사용 플랫폼이 될 수 있다고 강조했습니다. @gdb는 Codex가 완전한 에이전틱 IDE가 되고 있다고 명시적으로 평가했습니다.
- 이 분야는 "간단한 하네스, 강력한 평가, 모델 불가지론적 스캐폴딩"으로 수렴하고 있습니다: 여러 고신호 게시물들은 이제 신뢰성 향상이 가장 큰 모델을 쫓는 것보다 하네스에서 더 많이 온다고 주장했습니다. @AsfiShaheen은 라우터 / 레인 / 분석가로 구성된 3단계 금융 분석가 파이프라인을 설명했는데, 각 단계에 엄격한 컨텍스트 경계와 골드 세트를 두어 많은 버그가 실제로는 지시/인터페이스 버그였다고 주장했습니다. @AymericRoucher는 유출된 Claude Code 하네스에서 동일한 교훈을 얻었습니다: 간단한 계획 제약과 더 깔끔한 표현 레이어가 "화려한 AI 스캐폴드"보다 더 나은 성능을 보입니다. @raw_works는 훨씬 더 명확한 예를 보여주었습니다: Qwen3-8B는 dspy.RLM을 사용하여 LongCoT-Mini에서 33/507점을 기록했지만, 바닐라 버전은 0/507점을 기록하여 스캐폴드가 파인튜닝이 아닌 "100%의 역할을 했다"고 주장했습니다. LangChain은 이러한 패턴을 제품에 더 많이 적용했습니다: @sydneyrunkle은 deepagents 배포에 서브에이전트 지원을 추가했으며, @whoiskatrin은 Agents SDK에 메모리 프리미티브를 발표했습니다.
- 오픈소스 에이전트 스택이 계속 확산되고 있습니다: Hermes Agent는 여전히 중심점이었습니다. @GitTrend0x의 커뮤니티 생태계 개요는 Hermes Atlas, Hermes-Wiki, HUDs, 제어 대시보드와 같은 파생 모델들을 강조했습니다. @ollama는 ollama launch hermes를 통해 네이티브 Hermes 지원을 출시했으며, @NousResearch가 이를 확산시켰습니다. Nous와 Kimi는 또한 2만 5천 달러 규모의 Hermes Agent Creative Hackathon을 @NousResearch에서 시작하여 코딩/생산성에서 창의적인 에이전트 워크플로우로의 전환을 알렸습니다.
에이전트 연구: 자기 개선, 모니터링, 웹 스킬, 평가
- 일련의 논문들이 에이전트 견고성과 지속적인 개선을 추진했습니다: @omarsar0은 LLM 심사자 또는 히든 스테이트 프로브를 사용하여 추론 성능 저하를 모니터링하는 Cognitive Companion을 요약했습니다. 주요 결과는 주목할 만합니다: 레이어 28 히든 스테이트에 대한 로지스틱 회귀 프로브는 측정된 인퍼런스 오버헤드 없이 AUROC 0.840으로 성능 저하를 감지할 수 있으며, LLM 모니터 버전은 약 11%의 오버헤드로 반복을 52~62% 줄입니다. @dair_ai의 웹 에이전트에 대한 별도의 연구인 WebXSkill은 에이전트가 궤적에서 재사용 가능한 스킬을 추출하여 WebArena에서 최대 +9.8점, WebVoyager에서 그라운디드 모드로 86.1%를 달성했다고 설명했습니다. 그리고 @omarsar0은 또한 에이전트가 역량 격차를 식별하고, 개선 사항을 제안하고, 이를 검증하고, 재학습 없이 작동하는 변경 사항을 통합하는 프로토콜인 Autogenesis를 강조했습니다.
- 오픈 월드 평가가 중요한 주제가 되고 있습니다: 여러 게시물들은 현재 벤치마크가 너무 좁다고 주장했습니다. @CUdudec은 장기적이고 개방형 환경에 대한 오픈 월드 평가를 지지했으며, @ghadfield는 이를 규제 및 "에이전트 경제" 문제와 연결했습니다. @PKirgis는 복잡한 실제 환경에서 AI 에이전트의 정기적인 오픈 월드 평가를 위한 프로젝트인 CRUX에 대해 논의했습니다. 측정 측면에서는 @NandoDF가 2500개 토픽 버킷에 걸쳐 학습 도메인 외부의 책/기사에 대한 광범위한 NLL/perplexity 기반 평가 스위트를 제안했지만, 이는 RLHF/후속 학습 후에도 perplexity가 여전히 유용한지에 대한 @eliebakouch, @teortaxesTex 등의 논쟁을 촉발했습니다.
- 문서/OCR 및 리트리벌 평가도 에이전트 중심적으로 변화했습니다: @llama_index는 누락, 환각, 읽기 순서 위반에 대한 16만 7천 개 이상의 규칙 기반 테스트를 통해 콘텐츠 충실도에 중점을 둔 OCR 벤치마크인 ParseBench에 대해 자세히 설명했습니다. 이는 기준을 "사람이 읽을 수 있는" 것에서 "에이전트가 작동하기에 충분히 신뢰할 수 있는" 것으로 명시적으로 재정의한 것입니다. 리트리벌 분야에서는 @Julian_a42f9a가 후기 상호작용 리트리벌 표현이 RAG에서 원본 문서 텍스트를 대체할 수 있음을 보여주는 새로운 연구를 언급하며, 일부 RAG 파이프라인이 전체 텍스트 재구성을 우회할 수 있음을 시사했습니다.
오픈 모델, 로컬 인퍼런스, 인퍼런스 시스템
- Qwen3.6 로컬/양자화 워크플로우는 실용적인 밝은 부분이었습니다: @victormustar는 Qwen3.6-35B-A3B를 로컬 에이전트 스택으로 사용하는 구체적인 llama.cpp + Pi 설정을 공유하며, 로컬 에이전틱 시스템이 얼마나 실현 가능해졌는지 강조했습니다. Red Hat은 NVFP4 양자화된 Qwen3.6-35B-A3B 체크포인트를 @RedHat_AI를 통해 빠르게 출시했으며, 예비 GSM8K Platinum 100.69% 복구율을 보고했습니다. @danielhanchen은 동적 양자화를 벤치마크하며, 많은 Unsloth 양자화가 KLD 대 디스크 공간의 파레토 프론티어에 위치한다고 주장했습니다.
- 소비자 하드웨어 인퍼런스가 계속 개선되고 있습니다: @RisingSayak은 PyTorch/TorchAO와 함께 FP8 및 NVFP4 양자화를 사용하여 주요 레이턴시 페널티 없이 오프로딩을 가능하게 하는 작업을 발표했으며, 메모리 제약이 있는 소비자 GPU 사용자를 명시적으로 대상으로 했습니다. Apple 측 로컬 인퍼런스도 @googlegemma를 통해 선보였는데, Gemma 4가 긴 컨텍스트로 iPhone에서 완전히 오프라인으로 실행되는 것을 시연했습니다.
- 주목할 만한 인퍼런스 인프라 업데이트: @vllm_project는 AMD/EmbeddedLLM과 함께 MORI-IO KV Connector를 강조하며, PD-분리형 커넥터를 통해 단일 노드에서 2.5배 더 높은 굿풋을 달성했다고 주장했습니다. Cloudflare는 @Cloudflare의 isitagentready.com, @fayazara의 Flagship 기능 플래그, 그리고 한 예시에서 92KB를 159바이트로 줄이는 등 극적인 페이로드 감소를 가져오는 공유 압축 사전을 통해 에이전트/AI 플랫폼 추진을 이어갔습니다.
과학, 의학, 인프라를 위한 AI
- 과학적 발견과 개인 맞춤형 건강은 주요 응용 테마였습니다: @JoyHeYueya와 @Anikait_Singh_는 모델이 "부모" 논문으로부터 후속 논문의 핵심 기여를 생성하는 통찰력 예측에 대해 게시했습니다. 후자는 이 태스크에서 프론티어 모델을 능가한다고 보고된 RL 학습 모델인 GIANTS-4B를 소개했습니다. 건강 측면에서는 @SRSchmidgall이 웨어러블 데이터 기반의 바이오마커 발견 시스템을 공유했는데, 첫 번째 발견은 "심야 둠스크롤링"이 우울증 심각도를 ρ=0.177, p<0.001, n=7,497로 예측한다는 것이었습니다. 이는 모델 자체가 기능을 명명했다는 점에서 주목할 만합니다. 별도로 @patrickc는 현재 코딩 에이전트가 개인 맞춤형 유전체 해석에 이미 매우 유용하다고 주장하며, 약 30배 높은 흑색종 소인과 후속 개입을 밝혀낸 100달러 미만의 분석 실행을 설명했습니다.
- 대규모 컴퓨팅 구축은 핵심 메타 스토리로 남아있습니다: @EpochAIResearch는 7개 미국 Stargate 사이트 전체를 조사한 결과, 이 프로젝트가 2029년까지 9+ GW를 달성할 것으로 보이며, 이는 뉴욕시의 최대 전력 수요와 맞먹는 수준이라고 결론지었습니다. @gdb는 Stargate를 "컴퓨팅 기반 경제"를 위한 인프라로 평가했으며, @kimmonismus는 오늘날 연간 글로벌 데이터센터 CAPEX가 인플레이션 조정 기준으로 연간 약 5~7개의 맨해튼 프로젝트에 해당한다고 언급했습니다.
참여도 높은 인기 트윗
- Claude Design / Anthropic 제품 확장: @claudeai가 Claude Design을 출시했으며, 이는 단연코 그날의 가장 큰 순수 AI 제품 출시 신호입니다.
- 모델 벤치마킹 / 순위: @ArtificialAnlys의 Opus 4.7이 전체 1위를 차지하고 GDPval-AA에서 선두를 달리고 있다는 내용.
- 코딩 에이전트 / 컴퓨터 사용: @cursor_ai가 새로운 에이전트 창에서 Composer 2 제한을 두 배로 늘렸다는 내용과 @HamelHusain의 Codex Computer Use 관련 내용.
- 오픈소스 에이전트: @ollama가 네이티브 Hermes Agent 지원을 출시했습니다.
- 의학 분야 응용 AI: @patrickc의 유전체 분석 및 개인 맞춤형 예방을 위한 코딩 에이전트 관련 내용.
- 인프라 / 전력 스케일링: @EpochAIResearch의 Stargate 9+ GW 궤적 관련 내용.

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Qwen3.6 모델 출시 및 기능

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-the-two-sides-of-openclaw&utm_source=paywall-free-trial&utm_medium=web&utm_content=194589475&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-the-two-sides-of-openclaw&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
