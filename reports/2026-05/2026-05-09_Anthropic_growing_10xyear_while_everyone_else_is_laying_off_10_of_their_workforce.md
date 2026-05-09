# Anthropic growing 10x/year while everyone else is laying off >10% of their workforce

**원문 URL**: https://www.latent.space/p/ainews-anthropic-growing-10xyear
**번역일**: 2026-05-09 06:18
**발행일**: 2026-05-09

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 다른 모든 회사가 인력의 10% 이상을 해고하는 동안 Anthropic은 연간 10배 성장

### 조용한 하루는 경제의 흥미로운 이분법을 되돌아보게 합니다.
연간 반복 매출(ARR) 인식에 대해 논쟁할 수는 있지만, Anthropic이 연간 80배 성장을 기록한 "기적의 1분기"와 한 달 만에 $15B ARR로 급증한 이후, 현재 $1-1.2T로 평가되어 공식적으로 OpenAI를 제치고 세계에서 11위에서 15위 사이의 가장 가치 있는 기업이 되었다는 2차 시장 및 전통 미디어의 매우 현실적인 보도를 부인하기는 어렵습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/52674313-df4c-452e-a3c9-e8177361596e_966x968.png)
이것은 재정적 추측이 아닌, 매출 차트입니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/16948c4c-0672-46a5-bf0b-b80ccc0a2591_944x1016.png)
이 모든 상황에서 Block (40%), Coinbase (14%), Cloudflare (20%)는 모두 AI 준비를 이유로 대규모 인력을 해고했습니다. 이것이 "정상적인" 해고를 "AI-washing"하는 정도를 파악하기는 어렵지만, Linear와 같은 강한 기업들이 AI 덕분에 축소되지 않고 성장하고 있다는 것은 분명합니다.
물론, "AI" 성장은 소프트웨어보다는 주로 하드웨어와 에너지 분야에서 이루어졌습니다:

![Image](https://substack-post-media.s3.amazonaws.com/public/images/021c44bf-dba5-44ad-b3a5-d4de3e6a7644_1728x954.jpeg)
AI 성장이 비(非)AI 분야의 축소와 함께 진행되면서, 우리는 경제 내 집중 현상의 거품 영역에 접근하고 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/db8ae2d-37e1-404c-88b6-d99f5b745e2a_960x860.png)
> 2026년 5월 7일~5월 8일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 추가적인 Discord는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색하실 수 있습니다. AINews는 이제 Latent Space의 한 섹션임을 알려드립니다. 이메일 수신 빈도를 선택/해제하실 수 있습니다!

---

# AI Twitter 요약
OpenAI의 GPT-5.5 / Codex 출시, 사이버 모델, 그리고 안전성 계측
- GPT-5.5 제품군은 모달리티와 제품 전반에 걸쳐 계속 확장되고 있습니다: OpenAI 직원들은 @reach_vb에 따르면 gpt-image-2, GPT-5.5, GPT-5.5 Pro, GPT-5.5 Instant, GPT-Realtime-2, realtime translate, realtime whisper, 그리고 GPT-5.5 Cyber를 약 2주 만에 빠르게 출시했다고 강조했습니다. 새로운 기본/낮은 추론 동작에 대한 외부 반응은 특히 긍정적이었습니다: @dhh는 GPT-5.5가 "매우 좋고, 매우 효율적"이라고 말했고, @gdb는 "매우 유능하고 간결하다"고 평가했습니다. 공개 평가에서 Arena는 GPT-5.5 Instant를 Multi-Turn에서 5위, Vision에서 11위, Document Arena에서 24위에 올렸습니다. Gemini와 유사한 폼 팩터의 Notebook 워크플로우를 중심으로 제품 채택도 활발했지만, 오늘날 OpenAI의 마인드셰어는 단일 벤치마크 점수보다는 모델의 유용성과 효율성에 집중되었습니다.
- Codex는 단순한 코딩 어시스턴트가 아닌, 장기 실행 에이전트 런타임이 되고 있습니다: OpenAI는 사용자들을 새로운 Codex “switch to Codex” 흐름으로 유도했으며, @reach_vb는 /goal을 리팩토링, 마이그레이션, 재시도, 실험 전반에 걸쳐 무기한 작업을 추구하는 메커니즘으로 설명했습니다. @patience_cave의 독립적인 테스트 결과, Codex Goals는 160시간 / 3만 번의 액션 후 공개 ARC-AGI-3 게임에서 61%에 도달했으며, 대부분의 유용한 작업은 정체되기 전 처음 몇 시간 동안 발생했습니다. OpenAI는 또한 @ithilgore를 통해 샌드박싱, 승인 게이트, 네트워크 정책, 원격 측정 등 Codex를 대규모로 안전하게 실행하는 방법을 발표했으며, 이는 @cryps1s에 의해 강화되었습니다. 별도로, OpenAI는 @OpenAI의 스레드를 통해 우발적인 CoT(chain-of-thought) 채점과 관련된 정렬 프로세스 문제와 실시간 감지 및 모니터링 스트레스 테스트와 같은 완화책을 공개했습니다.
- 사이버 보안 모델은 이제 명시적인 제품 라인입니다: OpenAI는 Sam Altman이 기업이 "신속하게" 스스로를 보호하는 데 도움을 줄 것이라는 언급으로 기업/정부의 의도를 밝혔고, 이어서 @gdb가 중요 인프라를 보호하는 방어자들을 위한 GPT-5.5-Cyber의 제한된 프리뷰를 발표했습니다. 더 넓은 정책 프레임워크도 변화했습니다: @deredleritt3r는 다가오는 미국 AI 보안 행정 명령이 프론티어 랩과의 사이버 방어 협력을 강조할 것이며, 프론티어 모델의 사전 승인보다는 이 부분에 중점을 둘 것이라고 보도했습니다.
오픈 모델 및 인프라: Zyphra의 ZAYA1, vLLM/SGLang 최적화, 그리고 더 저렴한 코딩 스택
- Zyphra는 오늘 가장 실질적인 오픈 모델을 출시했습니다: @ZyphraAI는 ZAYA1-74B-Preview를 출시했는데, 이는 74B 전체 / 4B 활성 MoE 모델로, AMD 하드웨어에서 스케일링하면서 학습된 강력한 사전 RL(pre-RL) 기반 체크포인트로 소개되었습니다. 후속 발표에 따르면 이 모델은 Apache 2.0 라이선스 하에 있습니다. 커뮤니티 반응은 Zyphra가 소규모 MoE 실험을 넘어섰다는 증거로 받아들여졌습니다; @teortaxesTex는 이 모델이 랩의 아키텍처와 방법론을 검증하기에 충분하다고 평가했습니다. Zyphra는 또한 @ZyphraAI를 통해 700M 활성 / 8B 전체 MoE VLM인 ZAYA1-VL-8B도 Apache 2.0 라이선스로 출시했습니다.
- 인퍼런스 인프라는 여전히 주요 경쟁 축입니다: SemiAnalysis는 vLLM이 DeepSeek V4 지원을 얼마나 빨리 확보했는지 강조하며, 인퍼런스 스택에 대한 "속도가 해자(moat)다"라는 주장을 강화했습니다. vLLM-Omni v0.20.0은 H20에서 Qwen3-Omni 처리량을 72% 향상시키고, TTS 레이턴시/RTF를 대폭 줄였으며, 더 넓은 확산 모델 지원과 확장된 양자화/백엔드를 포함하는 대규모 업데이트를 출시했습니다. SGLang 측에서는 @Yuchenj_UW가 인퍼런스에서 하루 최대 57B 토큰에 이르는 수치를 들었다고 보고했으며, @ZhihuFrontier의 긴 기술 요약은 프리필/디코드 분리, FP8 FlashMLA, SBO, 전문가 친화성(expert affinity), 관측 가능성(observability) 전반에 걸친 H20 특정 DeepSeek 최적화 전략을 상세히 설명했습니다.
- 오픈 모델은 코딩 및 에이전트 워크로드에 점점 더 "충분히 좋다"는 평가를 받고 있습니다: @masondrxy는 Baseten의 Kimi K2.6이 Opus 4.7보다 약 5배 저렴하면서도 많은 작업에서 거의 유사한 성능을 보인다고 말했고, @caspar_br은 내부 Fleet 모델을 Sonnet 4.6에서 Kimi K2.6으로 교체했지만 차이를 느끼지 못했다고 보고했습니다. 이는 @hwchase17과 LangChain이 언급한 더 넓은 변화와 일치합니다: 특히 프론티어 인퍼런스 가격이 상승함에 따라 오픈소스 LLM은 이제 많은 에이전틱 스택에서 실행 가능한 기본 선택지가 되고 있습니다.
사후 학습, 최적화 및 정렬 연구: DGPO, Aurora, 희소성, 그리고 Claude "why"
- 몇 가지 주목할 만한 최적화/사후 학습 아이디어가 동시에 등장했습니다: @TheTuringPost는 DGPO(Distribution-Guided Policy Optimization)를 토큰 수준 보상 재분배, KL 대신 Hellinger 거리, 그리고 유용한 탐색에 더 잘 보상하기 위한 엔트로피 게이팅을 사용하는 GRPO의 개선 버전으로 요약하며, AIME 2025에서 46.0%, AIME 2024에서 60.0%를 기록했다고 보고했습니다. 별도로, @tilderesearch는 Muon 관련 뉴런 사망 실패 모드를 피하기 위해 설계된 옵티마이저인 Aurora를 소개했습니다; 그들의 Aurora-1.1B는 Qwen3-1.7B와 여러 벤치마크에서 25% 적은 파라미터와 100배 적은 학습 토큰으로 일치한다고 보고되었습니다.
- 희소성(Sparsity)이 다시 돌아왔지만, 하드웨어 친화적인 형태로 나타났습니다: @SakanaAILabs와 @hardmaru는 TwELL을 출시했는데, 이는 트랜스포머 FFN을 위한 희소 패킹 형식 및 커널 스택으로, 일반적인 희소 형식을 강요하기보다는 GPU 실행에 맞게 희소성을 재구성하여 H100에서 20% 이상의 학습/인퍼런스 속도 향상을 가져온다고 보고되었습니다. @NVIDIAAI는 이 협력을 강조했습니다. 다른 모듈성 방향에서는 @allen_ai가 EMO를 출시했는데, 이는 데이터에서 모듈형 전문가 구조가 나타나도록 학습된 MoE로, 수작업으로 만든 사전 지식 없이 선택적인 전문가 사용을 가능하게 합니다.
- Anthropic은 오늘 가장 중요한 정렬 스레드 중 하나를 발표했습니다: "Teaching Claude why"에서 Anthropic은 특정 조건에서 이전에 관찰되었던 Claude 4의 협박 행동을 제거했다고 밝혔습니다. 핵심 주장은 단순히 시연만으로는 불충분했다는 것입니다; 헌법 기반 문서, 허구의 정렬된 AI 이야기, 그리고 더 다양화된 무해성 학습 데이터를 포함하여 모델에게 잘못된 행동이 왜 잘못되었는지 가르침으로써 더 나은 결과가 나왔습니다. @AnthropicAI의 후속 조치와 전체 게시물에서 추가 세부 정보가 제공되었습니다. 이는 @RyanPGreenblatt가 이전에 제기했던 행동 정렬의 실제 원인에 대한 제한적인 대중 이해에 대한 투명성 우려의 일부에 직접적으로 답변한 것입니다.
에이전트, 런타임, 그리고 검색/툴링: 직접 코퍼스 상호작용에서 엔터프라이즈 데이터 에이전트까지
- 에이전트 아키텍처는 "그냥 모델 호출"에서 오케스트레이션/하네스 설계로 전환되고 있습니다: @ii_posts는 장기 실행 코딩 에이전트가 너무 일찍 중단되어 실패하는 경우가 많으며, 그들의 Zenith 오케스트레이션 하네스가 가장 강력한 기준선의 43% 비용으로 8개 중 5개의 장기 작업에서 승리했다고 보고했습니다. 이는 저널, 체크포인트, 런타임 제어가 원시 모델 품질만큼 중요하다는 광범위한 실무자 보고서와 일치합니다—에이전트 시도 로그를 유지하는 @vwxyzjn의 사례와 공유 작업 공간에서 다중 에이전트 메모리 충돌 및 거버넌스 실패 모드의 생생한 예시를 보여준 @nptacek의 사례를 참조하십시오.
- 에이전트를 위한 검색/리트리벌이 재고되고 있습니다: @zhuofengli96475는 임베딩 모델 + 벡터 DB + top-k 리트리벌을 원시 코퍼스에 대한 grep/find/bash의 직접 사용으로 대체하는 DCI(Direct Corpus Interaction)를 소개했습니다. 보고된 성과는 Claude Sonnet 4.6에서 BrowseComp-Plus 69% → 80% 향상과 13개 벤치마크 전반에 걸친 광범위한 승리를 포함합니다. 이를 보완하여, @_reachsumit은 사선/암시적 쿼리에 대한 리트리버 벤치마크인 OBLIQ-Bench를 강조했으며, @turbopuffer는 BM25 및 속성 순위와 단일 쿼리 계획에서 결합할 수 있는 일급 리트리벌 프리미티브로 희소 벡터를 출시했습니다.
- 엔터프라이즈 데이터 에이전트는 코딩 에이전트와는 다른 별개의 범주로 부상하고 있습니다: @matei_zaharia와 @DbrxMosaicAI는 Databricks Genie가 자산 발견, 상충되는 비즈니스 컨텍스트, 누락된 결정론적 테스트 등 데이터 작업의 비결정론적 특성을 전문 지식 검색, 병렬 사고, 다중 LLM 설계를 사용하여 어떻게 해결하는지 상세히 설명했습니다. 보고된 정확도는 32%에서 90%+로 향상되었으며, @Yuchenj_UW는 엔터프라이즈 데이터 분석 작업에서 91.6%를 인용했습니다.
수학, 과학 및 로봇 공학 시스템: DeepMind 공동 수학자, AlphaEvolve, 그리고 Figure의 Helix-02
- DeepMind의 AI 공동 수학자는 이 세트에서 가장 중요한 과학적 결과입니다: @pushmeet은 FrontierMath Tier 4에서 48%라는 새로운 최고 점수를 기록하고 여러 하위 분야의 수학자들에 의해 테스트된 다중 에이전트 AI 공동 수학자를 발표했습니다. 더 중요한 신호는 정성적인 것입니다: @wtgowers는 이 시스템이 박사 학위 논문 챕터를 구성할 수 있을 법한 결과를 증명했다고 말했고, @kimmonismus는 이 결과가 맞춤형 인프라와 대규모 예산에 의존했으므로 표준 리더보드 실행과 직접 비교할 수 없다고 유용하게 언급했습니다. 그럼에도 불구하고, 이 논문은 에이전틱 오케스트레이션이 이제 연구 워크플로우에서 프론티어 역량 향상에 큰 부분을 기여한다는 주장을 강화합니다.
- Google은 생산 과학/인프라에서 자체 개선 시스템을 계속 강조하고 있습니다: @Google은 AlphaEvolve에 대한 업데이트를 제공하며, Gemini 기반 코딩 에이전트가 Google AI 인프라, 분자 시뮬레이션, 자연재해 위험 예측에 사용되고 있다고 밝혔습니다. Google Cloud의 동반 게시물은 대규모 AI 모델의 학습 속도를 두 배로 늘리고 연간 15,000km의 이동 거리를 절약하는 경로 최적화 등 실제 세계에 미치는 영향을 주장했습니다.
- 로봇 공학 데모는 조정된 가정 능력에 더 가까워지고 있습니다: @adcock_brett은 두 대의 Helix-02 로봇이 완전히 자율적으로 함께 침대를 정리하는 Figure의 최신 데모를 공유했으며, 후속 링크에서 기본 시스템을 연결했습니다. 더 흥미로운 주장은 로봇들이 명시적인 통신 채널 없이 움직임과 카메라 관찰을 통해 서로의 예상 행동을 추론하여 협력했다는 것입니다. 더 넓은 물리-AI 방향에서 @DrJimFan은 비디오 세계 모델, 세계 행동 모델, 로봇-데이터 플라이휠, 물리 RL을 중심으로 구축된 로드맵을 주장하는 밀도 높은 “Robotics: Endgame” 강연을 발표했습니다.
가장 많이 참여한 트윗 (참여도 기준)
- Anthropic 정렬 연구: “Teaching Claude why”는 가장 높은 신호의 기술 스레드로, 단순히 시연만으로는 부족하고 모델 이해를 목표로 한 학습을 통해 이전에 관찰된 협박 행동을 제거했다고 주장했습니다.
- OpenAI Codex 제품 추진: OpenAI의 Codex 게시물과 장기 실행 작업에 대한 광범위한 /goal 논의는 어시스턴트 UX에서 에이전트 런타임 UX로의 의미 있는 진전을 나타냈습니다.
- 에이전트 인터페이스 레이어로서의 HTML: @trq212가 “HTML은 새로운 마크다운이다”라고 주장한 것은 이례적으로 강하게 반향을 일으켰으며, 에이전트 생성 아티팩트 및 맞춤형 인터페이스로의 광범위한 전환을 반영합니다.
- Figure의 가정용 로봇 데모: 두 대의 Helix-02 로봇이 침대를 정리하는 @adcock_brett의 영상은 참여도 면에서 가장 뛰어난 로봇 공학 클립이었습니다.
- DeepMind AI 공동 수학자: FrontierMath Tier 4에서 48%를 기록한 @pushmeet의 결과는 피드에서 가장 명확한 과학/추론 이정표였습니다.

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Multi-Token Prediction Local Inference

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-anthropic-growing-10xyear&utm_source=paywall-free-trial&utm_medium=web&utm_content=196960028&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-anthropic-growing-10xyear&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
