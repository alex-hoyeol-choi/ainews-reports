# GPT-Realtime-2, -Translate, and -Whisper: new SOTA realtime voice APIs

**원문 URL**: https://www.latent.space/p/ainews-gpt-realtime-2-translate-and
**번역일**: 2026-05-08 12:18
**발행일**: 2026-05-08

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] GPT-Realtime-2, -Translate, and -Whisper: 새로운 SOTA 실시간 음성 API

### OpenAI, GPT-5를 모든 곳에 계속 배포하고 있습니다
OpenAI는 3개월 전 realtime-1.5를 출시했지만, 여전히 4o 기반 인텔리전스였기 때문에(Big Bench Audio에서 5% 향상) 상대적으로 미미한 수준이었습니다. 하지만 오늘 출시된 realtime-2(BBA에서 15.2% 향상)에서는 엄청난 자신감을 엿볼 수 있었고, 이에 걸맞게 좋은 반응을 얻었습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/9c9ffc6c-f36-4f23-a2c3-34d5e64955aa_1014x918.png)
블로그 게시물에서 설명하듯이, 3가지 모델이 출시되며, 이를 “음성 입력, 음성 출력, 음성 대 음성”으로 단순화할 수 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/81d9ff0f-63ea-4b44-85a9-7fcc0d69f75_1716x772.png)
초점은 “음성 품질”보다는 유용성에 있습니다. 요약하자면:
- 프리앰블: 개발자는 “확인해 보겠습니다” 또는 “잠시만요, 찾아보겠습니다”와 같이 주요 응답 전에 짧은 문구를 활성화할 수 있습니다.
- 병렬 툴 호출 및 툴 투명성: 모델은 여러 툴을 동시에 호출할 수 있으며, “캘린더를 확인 중입니다” 또는 “지금 찾아보고 있습니다”와 같은 문구로 해당 동작을 소리로 들리게 하여 에이전트가 작업을 완료하는 동안 응답성을 유지하도록 돕습니다.
- 더 강력한 복구 동작: 모델은 실패하거나 중단되는 대신 “지금 문제가 발생했습니다”와 같이 말함으로써 더 우아하게 복구할 수 있습니다.
- 더 긴 컨텍스트: 32K → 128K
- 더 강력한 도메인 이해: 모델은 전문 용어, 고유 명사, 의료 용어 및 기타 어휘를 더 잘 유지합니다.
- 더 제어 가능한 톤 및 전달: 모델은 컨텍스트에 따라 차분하게, 공감하며, 또는 활기차게 말하는 등 자신의 톤을 더 잘 조절할 수 있습니다.
- 조정 가능한 추론 노력: 개발자는 이제 최소, 낮음, 중간, 높음, 최고 추론 레벨 중에서 선택할 수 있으며, 낮음이 기본값입니다.
데모 비디오는 주요 화자가 다른 사람과 대화할 때 오디오 모델이 더 잘 튜닝되어 방해를 훨씬 덜 하는 모습을 보여주었습니다:
> 2026년 5월 6일-5월 7일 AI 뉴스. 저희는 12개의 서브레딧, 544개의 트위터(X)를 확인했으며 더 이상 디스코드 채널은 없습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
주요 소식: GPT-Realtime-2 및 OpenAI 음성 AI 논평

## 무슨 일이 있었나요
OpenAI는 Realtime API에 3가지 새로운 스트리밍 오디오 모델인 GPT-Realtime-2, GPT-Realtime-Translate, GPT-Realtime-Whisper를 출시했습니다. OpenAI는 GPT-Realtime-2를 “현재까지 가장 지능적인 음성 모델”로 포지셔닝하며, 듣고, 추론하고, 방해를 처리하고, 툴을 사용하며, 대화가 진행됨에 따라 더 긴 대화를 유지할 수 있는 실시간 음성 에이전트에 “GPT-5급 추론”을 제공합니다 @OpenAI. 동반 모델들은 실시간 음성 번역 및 전사를 목표로 합니다: GPT-Realtime-Translate는 70개 이상의 입력 언어에서 13개 출력 언어로의 스트리밍 번역을 지원하며, GPT-Realtime-Whisper는 음성이 생성될 때 전사/캡션을 스트리밍합니다 @OpenAI, @OpenAIDevs. OpenAI는 현재 Realtime API에서 모델을 사용할 수 있지만, ChatGPT 음성 업그레이드는 아직 보류 중이라고 밝혔습니다: “계속 지켜봐 주세요, 저희는 작업 중입니다” @OpenAI. Sam Altman은 이번 출시를 행동 변화를 중심으로 설명했습니다: 사용자들이 많은 컨텍스트를 “쏟아내야” 할 때 AI와 음성을 점점 더 많이 사용하며, OpenAI는 ChatGPT 음성 개선 작업도 진행 중입니다 @sama.

## 사실 대 의견
사실 / OpenAI 및 평가자들이 직접 주장한 내용
- 모델 제품군: GPT-Realtime-2, GPT-Realtime-Translate, GPT-Realtime-Whisper는 오늘 Realtime API에서 사용할 수 있습니다 @OpenAIDevs.
- GPT-Realtime-2 기능: 프로덕션 음성 에이전트를 위한 추론 지향적인 네이티브 음성-대-음성 모델; 툴 사용/액션, 방해 복구, 더 긴 대화, 그리고 OpenAI의 표현에 따르면 “GPT-5급 추론”을 지원합니다 @OpenAI, @reach_vb.
- 컨텍스트 윈도우: 커뮤니티/OpenAI 개발자 논평에 따르면 GPT-Realtime-2 음성 에이전트의 컨텍스트는 128K입니다 @reach_vb; Artificial Analysis는 컨텍스트 윈도우가 32K에서 128K로 증가했으며, 최대 출력 토큰은 32K라고 독립적으로 보고했습니다 @ArtificialAnlys.
- 번역: GPT-Realtime-Translate는 70개 이상의 입력 언어에서 13개 출력 언어로의 실시간 음성 번역을 지원합니다 @OpenAI, @reach_vb.
- 전사: GPT-Realtime-Whisper는 Realtime API에서 캡션, 메모 및 연속적인 음성 이해를 위해 낮은 레이턴시의 스트리밍 전사를 제공합니다 @OpenAIDevs.
- 프롬프팅/제어: OpenAI는 추론 노력, 프리앰블, 툴 동작, 불분명한 오디오 처리, 정확한 엔티티 캡처, 긴 세션에서의 상태 유지 등을 다루는 음성 프롬프팅 가이드를 게시했습니다 @OpenAIDevs.
- 독립 벤치마크: Scale AI는 GPT-Realtime-2가 Audio MultiChallenge S2S 리더보드에서 1위를 차지했다고 보고했으며, GPT-Realtime-1.5 대비 지시 유지율이 36.7%에서 70.8% APR로 상승했고 음성 편집/실시간 복구에서 강력한 성능을 보였습니다 @ScaleAILabs.
- 독립 벤치마크: Artificial Analysis는 Big Bench Audio 음성-대-음성 추론에서 96.6%를 기록했으며, Conversational Dynamics 벤치마크에서 96.1%를 기록했고, 높은 추론 시 평균 첫 오디오 응답 시간은 2.33초, 최소 추론 시 1.12초였다고 보고했습니다. 오디오 가격은 입력 시간당 $1.15, 출력 시간당 $4.61로 이전 모델과 동일하다고 밝혔습니다 @ArtificialAnlys, @ArtificialAnlys.
- 추론 노력 제어: Artificial Analysis는 조정 가능한 추론 레벨(최소, 낮음, 중간, 높음, 최고)을 보고했으며, 낮음이 기본값입니다 @ArtificialAnlys.
- 기업/제품 평가: Glean은 GPT-Realtime-2가 실시간 조직 음성 상호작용을 위한 내부 평가에서 이전 버전 대비 42.9%의 상대적 유용성 증가를 보였다고 밝혔습니다 @glean. Genspark는 자사의 Call for Me Agent가 GPT-Realtime-2로 전환되어 유효 대화율이 26% 증가하고 통화 끊김이 줄었다고 말했습니다 @genspark_ai.
의견 / 해석 / 논평
- 지지자들은 이번 출시를 음성 에이전트의 “큰 진전” @sama, “완전한 실시간 승리” @reach_vb, 그리고 복잡한 음성 에이전트에서 “실제 작업”에 충분한 최초의 음성-대-음성 모델이라고 평가했습니다 @kwindla.
- 더 신중한 견해: Simon Willison은 이번 발표가 ChatGPT 음성 모드 자체가 아직 업그레이드되었다는 의미는 아니라고 지적했습니다; ChatGPT 업그레이드는 “곧 출시될 것 같다”고 말했습니다 @simonw, @simonw.
- 인터페이스 회의론: Will Depue는 오디오를 VR에 비유하며—자주 흥미롭지만, 역사적으로 인터페이스로서 잘 정착하지 못했다—실시간 툴 사용, 말하면서 추론하기, 실시간 번역과 같은 기능들이 오디오 인터페이스를 마침내 성공시킬 수 있는 종류의 기능이라고 주장했습니다 @willdepue.
- 더 넓은 UX 낙관론: 여러 논평자들은 음성을 인간에게 더 자연스럽고 대역폭 효율적인 것으로 보았으며 @BorisMPower, Jarvis와 같은 항상 사용 가능한 컴퓨터 에이전트로 가는 길 @willdepue, 궁극적으로는 훨씬 더 높은 대역폭의 BCI로 대체될 것이라고 보았습니다 @iScienceLuvr.
- 경쟁 상황: Elon Musk는 고객 지원을 위해 Grok Voice를 추진했으며 @elonmusk, 이는 실시간 음성 지원/고객 서비스 자동화가 이제 여러 연구소에서 경쟁의 장이 되었음을 강조합니다.

## 기술 세부 사항 및 벤치마크 데이터
GPT-Realtime-2
- 네이티브 음성-대-음성 / 실시간 음성 모델로, OpenAI의 Realtime API를 통해 출시되었습니다 @OpenAI.
- 음성 에이전트를 위한 “GPT-5급 추론”으로 평가됩니다 @OpenAI.
- 다음 기능을 수행할 수 있는 에이전트를 위해 설계되었습니다:
    - 대화 중 추론
    - 툴 사용/액션 수행
    - 방해 처리
    - 사용자가 음성을 수정하거나 복구할 때 복구
    - 확장된 컨텍스트로 더 긴 세션 유지
    @OpenAI, @reach_vb.
- 보고된 컨텍스트: 32K에서 증가한 128K 토큰 @ArtificialAnlys.
- 보고된 최대 출력: 32K 토큰 @ArtificialAnlys.
- Artificial Analysis가 보고한 입력: 텍스트, 오디오, 이미지 @ArtificialAnlys.
- 추론 노력 레벨: 최소, 낮음, 중간, 높음, 최고; 기본값 낮음 @ArtificialAnlys.
- 첫 오디오 응답 시간:
    - 최소 추론 시 1.12초
    - 높은 추론 시 2.33초
    @ArtificialAnlys.
- 가격: 오디오 입력 시간당 $1.15, 오디오 출력 시간당 $4.61로, Artificial Analysis에 따르면 이전 모델과 동일합니다 @ArtificialAnlys.
- 대화 기능: 주요 응답 전에 짧은 프리앰블을 지원하며—예: “확인해 보겠습니다”—툴 호출 중 음성 투명성을 제공합니다—예: “캘린더를 확인 중입니다” @ArtificialAnlys.

벤치마크
- Scale AI Audio MultiChallenge S2S: GPT-Realtime-2가 1위를 차지했습니다; GPT-Realtime-1.5 대비 지시 유지율이 36.7%에서 70.8% APR로 향상되었으며; 사용자가 실시간으로 음성을 복구/수정할 때 강력한 음성 편집 기능을 제공합니다 @ScaleAILabs.
- Artificial Analysis Big Bench Audio: GPT-Realtime-2 높음 변형이 96.6%를 기록했으며, Gemini 3.1 Flash Live Preview High와 동등하며 이전 최고 결과보다 약 13% 높은 것으로 보고되었습니다 @ArtificialAnlys.
- Justin Uberti는 Big Bench Audio에서 GPT-Realtime-1.5 대비 15% 포인트 향상으로, 거의 포화 상태에 도달했다고 별도로 요약했습니다 @juberti.
- Conversational Dynamics / Full Duplex Bench 서브셋: GPT-Realtime-2 최소 변형이 96.1%를 기록했으며, 일시 정지 처리 및 차례 주고받기에서 강점을 보였습니다 @ArtificialAnlys.

GPT-Realtime-Translate
- 70개 이상의 입력 언어에서 13개 출력 언어로의 실시간 스트리밍 음성 번역 @OpenAI.
- OpenAI 공동 창립자 Greg Brockman은 실시간 음성-대-음성 번역이 회사 초기부터 예상했던 OpenAI 애플리케이션이었으며, 이제 누구나 이를 활용하여 개발할 수 있다고 말했습니다 @gdb.
- Vimeo는 미리 로드된 캡션 없이 실시간 더빙을 시연하며, 번역이 완전히 실시간으로 생성되는 것을 보여주었습니다 @Vimeo.
- Junling Zhang은 새로운 실시간 번역 모델을 강조하고 API 사용을 장려했습니다 @jxnlco.
- Boris Power는 실시간 번역이 “실제로 놀랍도록 잘 작동한다”고 말하며 정기적으로 사용할 계획이라고 밝혔습니다 @BorisMPower.

GPT-Realtime-Whisper
- 사람들이 말할 때 스트리밍 전사로, 실시간 캡션, 메모 및 음성 이해를 위해 사용됩니다 @OpenAI.
- Justin Uberti는 이를 “Whisper이지만 이제 실시간 스트리밍이 가능해졌다”고 설명하며 새 모델을 사용하도록 데모를 업데이트했습니다 @juberti.
- Uberti는 또한 실시간 타이핑 데모에서 레이턴시/정확도 트레이드오프를 보여주기 위해 딜레이 셀렉터를 만들었습니다 @juberti.

## 제품 통합 및 데모
- Glean: 조직 컨텍스트에 기반한 GPT-Realtime-2 기반의 실시간 음성 기능을 출시했습니다; 내부 평가에서 이전 버전 대비 42.9%의 상대적 유용성 증가를 보였습니다 @glean.
- Vimeo: GPT-Realtime-Translate를 사용하여 실시간 더빙을 시연했으며, 번역이 실시간으로 생성되고 미리 로드된 캡션은 없었습니다 @Vimeo.
- Genspark: 자사의 Call for Me Agent를 GPT-Realtime-2로 업그레이드했습니다; 다음은 Genspark Realtime Voice입니다; 더 날카로운 추론, 더 엄격한 지시 따르기, 26% 증가한 유효 대화율, 그리고 줄어든 통화 끊김을 주장했습니다 @genspark_ai.
- Gradient Bang / 게임 에이전트 데모: Kyle Windland는 GPT-Realtime-2가 “실제 작업”을 수행하는 자신의 음성 에이전트에 충분한 최초의 OpenAI 음성-대-음성 모델이라고 말하며, 툴 호출 및 서브 에이전트가 있는 복잡한 에이전트에서 이를 선박 AI로 보여주었습니다 @kwindla.
- 음성 제어 시장 대시보드: Levin Stanley는 GPT-Realtime-2가 의도에 따라 인터페이스를 제어하는 것을 시연했습니다— “Apple에 집중해줘”, “지난 30일 동안 어땠어?”, “뒤로 가”—실시간 방해 및 추론이 UI 루프를 탐색에서 지시로 바꾼다고 주장했습니다 @levinstanley.
- 실시간 데모: Justin Uberti는 GPT-Realtime-2용 hello-realtime을 업데이트하고 전화 데모 번호를 제공했습니다 @juberti; Diego Cabezas는 GPT-Realtime-2의 빠른 데모를 게시했습니다 @diegocabezas01; Ray Fernando는 “실시간 번역기 구축” 방송을 진행했습니다 @RayFernando1337.
- Reachy Mini / 로봇 음성 인터페이스 관심: Clement Delangue는 누가 Reachy Mini에 새로운 음성 기능을 추가할 것인지 물었으며 @ClementDelangue, 이전에 Gradium, Kyutai, ElevenLabs와 같은 음성 AI 연구소에 로봇 음성 사용 사례에 도움을 줄 수 있는 곳이 있는지 물어본 후였습니다 @ClementDelangue.

## 이것이 중요한 이유
이번 출시는 음성 에이전트를 “챗봇을 감싸는 음성 I/O 래퍼”에서 전이중(full-duplex), 툴 사용, 긴 컨텍스트, 추론 에이전트로 발전시킵니다. 기술적 변화는 단순히 더 나은 ASR 또는 TTS가 아닙니다; 이는 낮은 레이턴시의 차례 주고받기, 방해 처리, 더 긴 컨텍스트, 툴 호출 투명성, 그리고 조정 가능한 추론 노력이 단일 실시간 루프에서 결합된 것입니다. 이는 고객 지원, 회의, 접근성, 실시간 번역, 로봇 공학, 브라우저/컴퓨터 제어, 그리고 텍스트 채팅이 너무 느리거나 어색한 핸즈프리 워크플로우에 중요합니다.

가장 중요한 엔지니어링 시사점은 음성 앱이 이제 프롬프트-응답 엔드포인트가 아닌 상태 저장(stateful) 실시간 시스템으로 설계되어야 한다는 것입니다. OpenAI의 프롬프팅 가이드는 개발자들에게 추론 노력 튜닝, 프리앰블, 툴 동작, 불분명한 오디오 복구, 엔티티 캡처, 긴 세션 상태 관리를 명시적으로 안내합니다 @OpenAIDevs. 이는 음성 에이전트의 품질이 점점 더 하네스(harness) 설계에 달려 있음을 시사합니다: 레이턴시 예산, 방해 의미론, 툴 호출 UX, 대화 메모리, 실패 복구 등—단순한 원시 모델 선택이 아닙니다.

남아있는 불확실성은 배포입니다. API 모델은 현재 사용 가능하지만, Simon Willison의 관찰에 따르면 ChatGPT 음성 모드는 아직 업그레이드를 받지 못했습니다 @simonw. 만약 ChatGPT Voice가 동일한 기능을 갖추게 된다면, 소비자 영향은 훨씬 더 커질 수 있습니다. 그때까지는 이번 출시가 주로 전문화된 실시간 에이전트를 구축하는 개발자와 플랫폼에 이점을 제공합니다.

---

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-gpt-realtime-2-translate-and&utm_source=paywall-free-trial&utm_medium=web&utm_content=196871624&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-gpt-realtime-2-translate-and&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
