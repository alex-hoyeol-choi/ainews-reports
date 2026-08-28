# OpenAI to reach AGI bar by end-2026

**원문 URL**: https://www.latent.space/p/ainews-openai-to-reach-agi-bar-by
**번역일**: 2026-08-28 12:03
**발행일**: 2026-08-28

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] OpenAI, 2026년 말까지 AGI 기준 도달 목표

### 때가 왔습니다. 이제 최종 단계에 접어들었습니다.
Aug 28, 2026공유저희 Latent Space는 보통 AGI 타임라인에 대한 논의를 피합니다. 그 정의가 모호하고 책임지기 어렵기 때문입니다. 하지만 지금 시점에서 이를 놓치는 것이 더 큰 잘못일 것입니다. 저희는 9개월 전 OpenAI의 AGI 타임라인을 마지막으로 확인했습니다. 그리고 예상대로, 최고 과학자 Jakub Pachocki는 미공개 모델 Astra가 2026년 9월까지 목표했던 “Automated AI Research Intern”이라고 말하고 있습니다. Sama는 TIME 인터뷰에서 더 나아가, 2026년 12월까지 내부적으로 AGI 달성을 선언할 것으로 예상했습니다.

![X avatar for @deredleritt3r](https://pbs.substack.com/profile_images/1874359541720092672/ciOMFG2x.jpg)
시계를 작동시키세요.
> 2026년 8월 22일~8월 24일 AI 뉴스입니다. 저희는 12개의 subreddit, 544개의 Twitter를 확인했으며, Discord는 더 이상 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 호를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter Recap
오픈소스 로봇공학의 돌파구: Hugging Face와 Pollen의 399달러 Microduck
- Microduck 출시: 가장 눈에 띄는 하드웨어 출시는 Pollen Robotics와 Hugging Face가 선보인 25cm 오픈소스 이족보행 로봇 Microduck이었습니다. 가격은 399달러이며 크리스마스 이전에 배송될 예정입니다. 이 로봇은 시뮬레이션에서 학습하고 실제 로봇에 배포할 수 있으며, 15개의 액추에이터와 카메라, 스피커, LiDAR, NFC, Bluetooth, Wi-Fi를 포함한 풍부한 센서 스택을 갖추고 있습니다. @pollenrobotics, @Thom_Wolf, @ClementDelangue의 출시 게시물들은 강화 학습 기반의 맞춤화와 여러 사전 학습된 정책(pre-trained policies)을 강조합니다.
- 기술적으로 중요한 이유: 흥미로운 점은 단순히 “저렴하고 귀여운 로봇”이 아니라 패키지 디자인에 있습니다. 오픈 시뮬레이터, 시뮬레이션에서 하드웨어로의 전이, 그리고 데모 소비에 그치지 않고 커뮤니티 정책 학습을 유도할 만큼 저렴한 폼 팩터입니다. 시뮬레이터는 이미 @HuggingApps가 강조했듯이 Hugging Face Space를 통해 공개되었으며, 커뮤니티 학습에서 실제 배포로 이어지는 이러한 오픈 루프(open-loop) 방식은 @yacineMTB 및 @gneubig와 같은 여러 연구자들이 즉시 유닛을 구매하게 만들었습니다.
- 초기 반응 및 커뮤니티 실험: 이번 출시는 로봇공학 분야에서 이례적으로 광범위한 반향을 일으켰습니다. Thom Wolf는 로봇이 레이저 포인터를 실시간으로 따라가도록 하는 빠른 이미지 감지기 통합과 같은 실험을 @Thom_Wolf를 통해 공유했으며, 이후 5초마다 Microduck 한 대가 판매되는 속도와 나중에 100만 달러의 매출을 @Thom_Wolf, @Thom_Wolf를 통해 보고했습니다. 저렴한 가격, 오픈 시뮬레이션, 그리고 embodied RL의 조합은 이것을 최근 기억에 남는 가장 신뢰할 수 있는 “소비자 규모의 물리적 AI” 출시 중 하나로 만들었습니다.
GLM-5.3-Flash/Ox Alpha 공개 및 로컬 오픈 모델 모멘텀
- Ox Alpha, GLM-5.3-Flash로 밝혀져: 가장 큰 모델 관련 소식 중 하나는 미스터리 모델 Ox Alpha가 실제로는 Z.ai / Zhipu의 GLM-5.3-Flash였다는 확인이었습니다. 이는 @theo, @UnslothAI, @togethercompute에 의해 언급되었습니다. 트윗에서 반복적으로 인용된 공개 사양은 320B 총 파라미터, 18B 활성 파라미터, 1M 컨텍스트, 하이브리드 어텐션이며, 코딩/에이전틱 벤치마크에서 강력한 결과를 보였습니다.
- 오픈 웨이트 + 양자화 + 로컬 서빙: 이번 출시는 사람들이 빠르게 로컬 워크플로우에 적용했기 때문에 주목을 받았습니다. Unsloth는 @UnslothAI를 통해 이 모델이 128GB RAM에서 3비트 GGUF를 실행할 수 있다고 말했으며, @danielhanchen은 4비트가 93%의 정확도를 유지하고 256GB Mac 또는 두 대의 DGX Sparks에서 모델을 실용적으로 만들 수 있다고 주장했습니다. 이것은 오픈 모델 엔지니어들이 출시 후 생태계 반응에서 중요하게 생각하는 바로 그런 종류입니다: 양자화, 서빙 레시피, 그리고 실제 배포 제약 사항들이 거의 즉시 해결되는 것입니다.
- 가격/성능 내러티브: 여러 트윗에서 GLM-5.3-Flash를 새로운 효율성 프론티어(frontier)로 평가했습니다. @togethercompute는 DeepSWE에서 Luna와 거의 필적하면서도 동일한 예산으로 두 배 이상의 작업을 수행한다고 말했습니다. @theo는 자신의 모델 순위를 재조정할 만큼 충분히 좋다고 평가했습니다. @zainhas는 정확도가 거의 변동이 없는 반면 토큰 사용량이 두 배로 늘어났기 때문에 최대 추론 노력(reasoning effort) 대신 높은 추론 노력을 사용할 것을 제안했습니다. Baseten은 또한 @baseten을 통해 출시 당일 122+ TPS의 서빙 처리량(throughput)을 강조했으며, Databricks는 @Yuchenj_UW를 통해 OfficeQA Pro v2에서 GLM-5.2보다 1/10의 비용으로 270 tok/s와 10% 더 높은 품질을 언급했습니다.
비디오 생성 경쟁: Gemini Omni 1.1 Flash와 H3 Max
- Gemini Omni 1.1 Flash: Google은 Gemini Omni 1.1 Flash를 출시했습니다. 이는 여러 개발자용 제어 기능을 갖춘 멀티모달 비디오 생성/편집 모델로, 40초까지의 장면 확장, 첫/마지막 프레임 제어, 3초 비디오 참조, 360p 드래프트 모드, 그리고 4K 업스케일링을 포함합니다. 출시는 @Google, @GoogleAIStudio에 의해 발표되었으며, @_philschmid에 의해 프롬프팅 가이드와 함께 요약되었습니다. 가장 주목할 만한 제품 세부 사항은 Google이 단순히 “더 강력한 프롬프트”를 넘어 점점 더 명시적인 시간적 및 참조 컨디셔닝을 노출하고 있다는 점입니다.
- 초기 리더보드 결과: @arena는 Omni 1.1 Flash가 Text-to-Video Arena에서 1위, Image-to-Video Arena에서 2위를 차지했으며, 3위 텍스트-투-비디오 모델보다 20점 앞서고 이전 Gemini Omni Flash보다 이미지-투-비디오에서 25점 향상되었다고 보고했습니다. 이는 모든 질적 질문을 해결하지는 못하지만, Google의 최신 사후 학습(post-training) 및 제어 스택이 선호도 데이터로 전환되고 있음을 나타냅니다.
- fal + MiniMax H3 Max: 이와 동시에, fal은 MiniMax와 함께 H3 Max를 출시했으며, @krea_ai를 통해 5초 만에 15초 분량의 고품질 비디오를 생성하고 다른 고품질 모델보다 “50배 더 빠르다”고 광고했습니다. @fal의 기술 문서와 @MiniMax_AI의 찬사가 있었습니다. 두 출시 모두에서 분명한 주제는 다음과 같습니다: 비디오 분야에서 인퍼런스 최적화와 제품화된 제어 가능성이 이제 기본 모델 품질만큼 중요해졌다는 것입니다.
에이전트, 하네스, 그리고 엔터프라이즈 툴링
- 하네스가 핵심 요소로 부상: 반복되는 주제는 모델 기능이 에이전트 하네스에 의해 점점 더 중재된다는 것이었습니다. @omarsar0는 JIT-Agent를 강조했습니다. 이 에이전트에서는 모델이 메모리, 계획, 액션 프로토콜, 도구 오케스트레이션을 위한 모듈 위에 하네스를 합성하며, 기성 에이전트보다 향상된 성능을 보고했습니다. 별도로, @dair_ai는 에이전트 트레이스에서 컴팩트한 유한 상태 머신을 유도하는 작업을 공유하며, 행동 토폴로지가 기본 LLM보다는 배포 스캐폴딩에 의해 더 많이 형성될 수 있음을 시사했습니다.
- 에이전트 인프라 관련 제품 출시: Anthropic은 Claude Managed Agents를 Vercel의 Chat SDK에 연결하기 위한 쿡북을 출시하여, 서버 측 하네스, 세션 관리 및 메모리를 갖춘 통합 채팅 레이어를 제공했습니다 @ClaudeDevs. Perplexity는 Agent API에 GitHub, Slack, Google Drive, Datadog용 커넥터를 추가했습니다 @perplexitydevs. Cursor는 웹 앱을 생성하고, Origin으로 코드를 저장하며, Vercel에 배포하는 워크플로우를 발표했습니다 @cursor_ai.
- 더 높은 신뢰도의 브라우저 자동화: Nous는 브라우저 사용 에이전트를 위한 중요한 진전을 이루었습니다: Hermes Agent는 이제 사용자의 실제 Chrome 프로필/로그인 관리 사본을 사용하여 사용자를 대신하여 브라우징할 수 있습니다 @NousResearch, @Teknium. 이는 주목할 만한 사용성 향상이지만, 인증 마찰을 줄이고 범위 지정 권한(scoped-permission) 설계를 훨씬 더 시급하게 만듦으로써 클라우드 에이전트의 위험 표면(risk surface)을 실질적으로 변화시킵니다.
보안, 에이전트 오정렬, 그리고 사이버 방어 조정
- OpenAI 주도의 사이버 방어 연합: OpenAI는 Anthropic, AWS, Google, Microsoft, Oracle을 포함한 116개 기관이 서명한 공개 서한을 발표하여, AI 기반 공격에 대한 사이버 방어의 전 세계적인 강화를 촉구했습니다 @OpenAI. Sam Altman은 @sama를 통해 “행동할 시간이 많지 않다”고 강조했습니다. 개인의 정책적 선입견과 관계없이, 이는 그날의 가장 명확한 산업 간 조정 움직임 중 하나였습니다.
- 이중 맹검 프론티어 평가: Google DeepMind는 프론티어 AI에 대한 이중 맹검 평가 파일럿을 발표했습니다. 이는 테스트 프롬프트나 모델 웨이트(weights)가 공개되지 않는 보안 환경을 사용합니다 @GoogleDeepMind. 실무자들에게 핵심적인 의미는 절차적인 것입니다: 어느 한쪽에게 상대방의 자산에 대한 완전한 가시성을 제공하지 않으면서 외부 평가를 가능하게 하려는 진지한 시도입니다.
- 에이전트 사고 분석 계속: OpenAI/Hugging Face 에이전트 사고에 대한 논의는 활발하게 이어졌습니다. 조사에 참여한 연구자들은 대규모 트랜스크립트 스윕, 에이전트 간 협업 패턴, 그리고 이전 작업을 기반으로 구축된 것으로 보이는 후속 스웜에 대한 추가 세부 정보를 공유했습니다 @RyanGreenblatt, @HjalmarWijk, @ajeya_cotra. @omarsar0의 EvoMal에 대한 별도 논문 요약은 공유된 스킬 라이브러리가 코딩 에이전트의 자가 중독성 멀웨어 전파 채널이 될 수 있다고 경고했습니다. 이 모든 것은 성숙해가는 인식을 가리킵니다: 다중 에이전트 시스템은 고전적인 소프트웨어 버그도, 표준 모델 평가 문제도 아닌 새로운 실패 모드를 도입합니다.
인기 트윗 (참여도 기준)
- Microduck이 관심사를 장악: 가장 높은 신호의 제품 소식은 @ClementDelangue의 Microduck 발표, @Thom_Wolf의 기술 출시 스레드, 그리고 @Thom_Wolf의 후속 판매 이정표에 집중되었습니다.
- 사이버 방어 촉구, 큰 반향 얻어: 가장 강력한 정책/보안 참여는 @sama와 @OpenAI의 집단 사이버 방어에 대한 것이었습니다.
- Anthropic의 과학 분야 추진 성공: @claudeai는 10,000명의 연구자를 대상으로 하는 과학자용 Claude Team 플랜을 발표했습니다. 이 플랜은 무료 표준 좌석과 연간 월 15달러의 프리미엄 좌석을 제공합니다.
- Hermes 브라우저 접근성, 두각을 나타내다: @NousResearch는 에이전트에게 사용자의 실제 브라우저 프로필 접근 권한을 부여하여 상당한 참여를 이끌어냈습니다. 이는 현재 에이전트 툴링에서 더 중요한 UX/보안 트레이드오프 중 하나입니다.

---

# AI Reddit Recap

## /r/LocalLlama + /r/localLLM Recap

### 1. NVIDIA-Hugging Face 인수 여파

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-openai-to-reach-agi-bar-by&utm_source=paywall-free-trial&utm_medium=web&utm_content=213103239&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-openai-to-reach-agi-bar-by&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
