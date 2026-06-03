# Microsoft Build: MAI-Thinking-1 and MAI Family models

**원문 URL**: https://www.latent.space/p/ainews-microsoft-build-mai-thinking
**번역일**: 2026-06-03 06:19
**발행일**: 2026-06-03

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Microsoft Build: MAI-Thinking-1 및 MAI Family 모델

### Microsoft Build 요약 및 새로운 MAI 모델 기술 세부 정보
공유오늘은 GitHub 대 Agents의 현황을 파악하고 No Priors 및 Satya Nadella와 함께 특별 팟캐스트를 녹음했기 때문에 중요한 날이었습니다. MS Build에서 Satya와 Mustafa는 7개의 새로운 MAI 모델을 발표했습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/1e8ca90a-629c-44d5-af2f-0b0cd2a60aa2_1510x886.png)
이것은 인상적인 라인업입니다. 특히 MAI를 설립한 Microsoft-Inflection 딜이 불과 2년 전에 이루어졌고, 이 모든 모델이 처음부터 사전 학습되었다는 점을 고려하면 더욱 그렇습니다. 오늘날의 MAI는 결코 검증되지 않은 프론티어 랩은 아니지만, 도메인 특화 파인튜닝을 지원하는 분명한 동기를 가진 훌륭한 2티어 신생 랩입니다(파인튜닝을 거의 모두 중단한 프론티어 랩들과는 대조적으로).
이 쇼의 스타는 연구 커뮤니티에서 극찬을 받고 있는 100페이지가 넘는 MAI 기술 보고서였습니다.

![X avatar for @eliebakouch](https://pbs.substack.com/profile_images/1745893660099592193/MmYemsw6.jpg)
나머지 모든 발표 내용은 훌륭한 Verge 요약과 아래 트윗 요약에서 확인하실 수 있습니다.
> AI News for 06/1/2026-6/2/2026. We checked 12 subreddits, 544 Twitters and no further Discords. AINews’ website lets you search all past issues. As a reminder, AINews is now a section of Latent Space. You can opt in/out of email frequencies!

---

# AI Twitter 요약
주요 소식: Microsoft Build 요약 및 새로운 MAI 모델 기술 세부 정보

## 무슨 일이 있었나
Microsoft는 Build를 통해 자신을 AI 플랫폼 회사이자 프론티어 모델 랩으로 포지셔닝하며, 광범위한 제품 출시와 함께 새로운 MAI 모델 제품군에 대한 이례적으로 상세한 공개를 진행했습니다.
- @MicrosoftAI 및 @mustafasuleyman에 따르면 Microsoft AI는 MAI-Thinking-1, MAI-Code-1-Flash, MAI-Image-2.5, MAI-Transcribe-1.5, MAI-Voice-2를 필두로 추론, 코드, 이미지, 음성 전사 및 음성을 아우르는 7개의 새로운 MAI 모델을 발표했습니다.
- 주력 추론 모델인 MAI-Thinking-1은 @mustafasuleyman, @baseten, @tuhinone, @HannaHajishirzi의 게시물에서 깨끗한 데이터 계보와 타사 모델로부터의 디스틸레이션 없이 구축된 Microsoft의 첫 번째 추론 모델로 소개되었습니다.
- Microsoft는 MAI-Thinking-1에 대한 109페이지 분량의 기술 보고서를 발표했으며, @eliebakouch, @ethanCaballero, @nrehiew_, @yacinelearning, @stochasticchasm을 포함한 기술 지향적인 독자들로부터 높은 투명성 수준에 대해 강력한 긍정적 반응을 얻었습니다.
- Microsoft는 또한 온디바이스 AI 및 에이전트 네이티브 Windows를 강조했습니다. Build 메시징은 에이전트를 위한 보안 실행 계층, 새로운 Surface RTX Spark Dev Box, 더 넓은 Windows GPU 설치 기반에 대한 Windows AI 액세스, Project Solara/Scout와 같은 콘셉트 하드웨어를 강조했으며, 이는 @yusuf_i_mehdi, @TheTuringPost, @kimmonismus, @kimmonismus에 의해 요약되었습니다.
- Build에는 또한 @pierceboggan, @lukehoban의 발표와 @techgirl1908의 반응에 따라 캔버스, 기기 간 연속성, 더 긴밀한 GitHub 에이전트 워크플로우를 포함하여 "에이전트 네이티브 소프트웨어 개발을 위한 데스크톱 허브"로서의 주요 GitHub Copilot 앱 추진이 포함되었습니다.
- Microsoft는 AI 에이전트를 위한 새로운 그라운딩/검색 API 스택인 Web IQ를 소개했으며, @JordiRib1을 통해 이 API가 이미 "오늘날 업계의 거의 모든 AI 에이전트 및 챗봇(Copilot 및 ChatGPT 포함)"에 사용되고 있다고 주장했습니다.
- Satya Nadella는 Build를 단일 제품 출시가 아닌 생태계의 중요한 순간으로, Mustafa Suleyman은 Microsoft의 내부 "언덕 오르기 기계"의 결과물로 설명했으며, 이는 @satyanadella, @mustafasuleyman의 게시물과 @nrehiew_의 반응에서 나타났습니다.

## MAI 모델 제품군: 공개된 사실 및 기술 세부 정보

### MAI-Thinking-1
- Microsoft는 @mustafasuleyman에서 MAI-Thinking-1을 256K 컨텍스트 윈도우를 가진 35B 활성 파라미터 MoE로 설명했습니다.
- @scaling01의 별도 요약에 따르면 이 모델은 1T@35B 파라미터 모델로, 30T 토큰으로 사전 학습되었으며, 8192개의 GB200 GPU를 사용하여 학습되었습니다. 이는 Microsoft 마케팅 자료가 아닌 기술 보고서를 읽은 것으로 보입니다.
- @kimmonismus도 유사하게 45B 활성 파라미터를 가진 중간 크기 MoE로 요약했지만, 이는 Mustafa의 35B 활성 수치와 상충됩니다. 트윗 세트에서 더 권위 있는 수치는 공식 35B 활성 수치입니다.
- Microsoft는 AIME 2025에서 97%, SWE-Bench Pro에서 53%를 달성했으며, Surge의 블라인드 인간 평가자들은 전반적으로 Sonnet 4.6보다 이 모델을 선호한다고 @mustafasuleyman 및 @asadovsky를 통해 주장했습니다.
- Microsoft는 이 모델이 MAIA 200에 최적화되어 있으며, MAI 모델을 엔드투엔드로 실행할 때 GB200 대비 달러당 성능이 30% 향상되고 와트당 성능이 1.4배 향상되었다고 @mustafasuleyman을 통해 밝혔습니다.
- Microsoft와 파트너들은 @baseten, @tuhinone, @MicrosoftAI에서 Baseten을 통해 타사 디스틸레이션 없음, "깨끗한 데이터 계보", "100% 비공개" 사후 학습 데이터를 통한 기업 제어 파인튜닝을 반복적으로 강조했습니다.

### MAI-Code-1-Flash
- Microsoft는 VS Code 및 GitHub Copilot CLI를 위한 빠른 코딩 모델인 MAI-Code-1-Flash를 소개했으며, @pierceboggan이 처음 발표하고 나중에 @mariorod1이 강조했습니다.
- @mustafasuleyman을 통한 공식 Microsoft 메시징에 따르면 Code-1-Flash는 5B 파라미터에 불과함에도 불구하고 SWE-Bench Pro에서 51%를 달성하여 Haiku급 크기/비용에 근접한 위치를 차지합니다.
- @scaling01의 경쟁 요약은 이 모델을 137B 파라미터 MoE, 256K 컨텍스트, 10T+ 토큰으로 학습되었으며, "Claude 4.5 Haiku보다 강력하고 효율적"이라고 설명합니다. 이는 총 파라미터가 아닌 5B 활성 파라미터를 의미할 가능성이 높습니다. 트윗은 이 구분을 완전히 해소하지 못하지만, 함께 볼 때 훨씬 더 큰 MoE 내의 작은 활성 풋프린트를 암시합니다.
- @scaling01 및 @mariorod1에 따르면 출시 시점의 가용성은 GitHub Copilot / VS Code 우선으로 강조되었습니다.

### MAI-Image-2.5
- Microsoft는 MAI-Image-2.5와 Flash 변형을 출시했으며, 둘 다 리더보드에서 2위를 차지했다고 주장하며, @mustafasuleyman은 이미지 편집에서 Nano Banana 2를 능가한다고 밝혔습니다.
- 독립적인 리더보드 계정은 높은 순위를 지지했습니다. @arena는 Image Edit Arena에서 1401점으로 2위를 기록했으며, Nano Banana 2, Grok Imagine, ChatGPT Image Latest HF보다 10점 높았습니다.
- @arena는 또한 MAI-Image-2.5가 "파레토 프론티어를 발전시킨다"고 말했는데, 이는 해당 가격대에서 이 벤치마크에서 더 높은 점수를 받는 모델이 없다는 의미입니다.
- @OpenRouter 및 @fal을 포함한 유통 파트너들이 빠르게 뒤를 이었습니다.

### MAI-Transcribe-1.5
- @ArtificialAnlys는 MAI-Transcribe-1.5가 STT 프론티어에서 이례적으로 강력한 속도/정확도 지점(실시간 대비 약 276배, 2.4% AA-WER, 리더보드 전체 3위)을 기록했다고 보고했습니다.
- @ArtificialAnlys에 따르면 이 모델은 영어, 프랑스어, 아랍어, 일본어, 중국어를 포함한 43개 언어를 지원하며, 이름이나 의학 용어와 같은 희귀 용어에 대한 키워드 바이어싱을 지원합니다.
- @ArtificialAnlys에 따르면 가격은 Microsoft Foundry를 통해 오디오 1,000분당 6달러로 보고되었습니다.
- @OpenRouter에서 OpenRouter도 같은 날 출시한 세 가지 MAI 모델 중 이 모델을 나열했습니다.

### MAI-Voice-2
- MAI-Voice-2는 Microsoft의 "7개 모델" 범주와 @OpenRouter의 OpenRouter 가용성 게시물에 나타납니다.
- 트윗 세트에는 Voice-2 자체에 대한 출시/가용성 외의 기술적 세부 정보는 거의 없습니다.

## 연구자들에게 중요했던 기술 보고서 세부 사항

### 보고서가 돋보인 이유
- 지배적인 기술적 반응은 Microsoft가 이례적으로 상세한 프론티어 모델 보고서를 발표했다는 것이었습니다. @eliebakouch는 이를 "이 규모의 모델에 대해 가장 투명한 보고서 중 하나"라고 불렀고, @nrehiew_는 "오늘날 LLM 학습을 위한 최신 교과서 역할을 할 수 있을 것"이라고 말했으며, @stochasticchasm은 이를 "금광"이라고 불렀습니다.
- 여러 독자들은 보고서가 파이프라인 세부 사항, 스케일링 래더 방법론, 데이터 큐레이션, 인프라 지표, MFU 수치를 공개했다고 강조했습니다. 이러한 구체성 수준이 @ethanCaballero, @eliebakouch, @nrehiew_로부터 칭찬을 이끌어냈습니다.

### 사전 학습 및 데이터
- MAI-Thinking-1이 사후 학습뿐만 아니라 공개된 파이프라인 전체에서 합성 데이터와 디스틸레이션을 사용하지 않았다는 것이 반복적으로 언급된 주요 기술적 주장이며, 이는 @eliebakouch, @stochasticchasm, @HannaHajishirzi의 게시물에서 나타났습니다.
- @eliebakouch는 보고서가 Common Crawl과 비공개 소스의 데이터를 명시적으로 언급하며, 다양한 도메인을 위한 타겟팅된 서브 파이프라인, 대규모 추출/중복 제거 작업, 합성 데이터를 사용하지 않기로 한 의도적인 선택을 포함한다고 말합니다.
- 스케일링 결정에 사용된 보고서의 내부 비공개 NLL 세트는 @eliebakouch에 의해 다음과 같이 요약되었습니다.
    *   50% 코드
    *   17.5% STEM
    *   17.5% 수학
    *   10% 일반 지식
    *   5% 다국어
- @eliebakouch는 스케일링 래더에서의 아키텍처 승격이 효율성 이득(EG) 지표, 즉 후보 모델의 손실과 일치시키기 위해 기준 모델이 필요로 하는 추가 컴퓨팅 양을 기반으로 했다고 말합니다.
- 같은 스레드에서 파라미터당 약 100/200 토큰에서 어블레이션이 언급되었는데, 이는 설정에 대한 "Chinchilla 최적" 수준으로 설명되었으며, @eliebakouch는 MoE 구조로 인해 밀집 모델 휴리스틱과 다르다는 점도 언급했습니다.

### 사후 학습 / RL
- 가장 많이 논의된 기술적 선택은 Microsoft가 이전 추론 노출이 없는 체크포인트에서 RL을 시작한 것으로 보인다는 점이었고, 여러 독자들은 이를 주목할 만하다고 생각했습니다. @stochasticchasm은 이를 "매우 흥미로운 결정"이라고 불렀고, @stochasticchasm은 AIME25에서 20% 미만에서 95% 이상으로 급증하는 그래프에 반응했습니다.
- @HannaHajishirzi는 "맨바닥부터 오르기" 레시피를 간단한 레시피, 엄격한 과학, 자기 디스틸레이션, 인내, 훌륭한 인프라로 설명했습니다.
- @soldni는 이 과정을 "거물들이 하는 것처럼 디스틸레이션 없이 오르기"로 특징지었습니다.
- 일부 독립적인 독자들은 보고서에서 Microsoft가 의도적으로 피했음에도 불구하고 합성 데이터가 더 넓은 분야에서 에이전틱 성능에 여전히 매우 중요하다는 것을 추론했습니다. @stochasticchasm을 참조하십시오.

### 데이터 큐레이션 / 심사관 / DSPy GEPA
- DSPy/후기 상호작용 커뮤니티로부터 상당한 주목을 받은 세부 사항: Microsoft는 사전 학습 데이터 큐레이션 및 품질 평가에 GEPA / DSPy 최적화 LLM 심사관을 사용한 것으로 알려졌습니다.
- 이는 @bj2rn, @LakshyAAAgrawal, @lateinteraction에 의해 강조되었습니다.

### 인프라 / 활용 / 하드웨어 공동 설계
- Microsoft는 반복에 걸친 정확한 MFU를 공개한 것으로 알려졌으며, 여러 독자들은 이 규모에서는 거의 공유되지 않는다고 @eliebakouch를 통해 말했습니다.
- @scaling01은 이 실행이 8192개의 GB200 GPU를 사용했다고 요약했습니다.
- @eliebakouch는 보고된 와트당 처리량 수치가 약 40% 더 높다는 점을 "매우 인상적이며 마이크로소프트 칩에 대해 낙관적"이라고 지적했지만, 이는 랙 수준 예산 또는 서빙 구성을 의미할 수 있으며 트윗에서 완전히 설명되지는 않았습니다.
- Microsoft의 공식 프레이밍은 모델 설계를 MAIA 200 맞춤형 실리콘과 연결하고 @mustafasuleyman에서 NVIDIA GB200 대비 더 나은 달러당 성능 및 와트당 성능을 강조했습니다.
- Build의 더 넓은 Windows/온디바이스 AI 내러티브 또한 다음과 같은 하드웨어 세부 사항에 중점을 두었습니다.
    *   DGX Station에서 로컬로 실행되는 1조 파라미터
    *   128GB 통합 메모리
    *   110 TOPS AI 성능
    *   20 CPU 코어
    *   70개 이상의 PowerToys 유틸리티 (from @TheTuringPost)
- 반응은 또한 대규모 모델의 로컬 실행을 지적했습니다. 예를 들어, @kimmonismus는 RTX Spark에서 120B 파라미터 모델을 로컬로 실행하는 것을 언급했습니다.

## 모델 외 Build 제품/플랫폼 요약

### GitHub Copilot 앱 및 에이전트 네이티브 개발
- GitHub는 @pierceboggan에 의해 에이전트 네이티브 소프트웨어 개발을 위한 데스크톱 표면으로 제시된 GitHub Copilot 앱을 공개했습니다.
- 주요 테마는 다음과 같습니다.
    *   사용자와 에이전트 간의 양방향 작업을 위한 캔버스 (@Techmeme)
    *   CLI, 모바일, 웹, 로컬, 클라우드 전반의 연속성 (@lukehoban)
    *   GitHub가 에이전트 워크플로우의 중심으로서 역할이 커지고 있음 (@techgirl1908 및 @OrenMe)
- Copilot CLI는 또한 탭, 내장 피드백/러버 덕, 프롬프트 스케줄링, 음성 입력을 갖춘 실험적인 터미널 UI를 얻었습니다 (@GHchangelog).

### 에이전트 런타임으로서의 Windows
- Microsoft의 Windows 조직은 @yusuf_i_mehdi에 따라 "더 빠른 개발자 실행, 에이전트를 위한 보안 실행 계층, 기기에서 로컬로 실행되는 무제한 인텔리전스"를 중심으로 Build를 구성했습니다.
- 여러 게시물은 Microsoft가 Azure뿐만 아니라 Windows가 에이전트를 위한 신뢰할 수 있는 실행 플랫폼이 되기를 원한다고 강조했습니다.
- @TheTuringPost는 Project Solara를 에이전트 우선 기기를 위한 플랫폼으로 설명했으며, 다음과 같은 개념을 포함합니다.
    *   데스크톱 AI 동반자
    *   카메라, 마이크, 센서, 보안 인증 기능을 갖춘 웨어러블 배지
- @kimmonismus는 이를 에이전트 제어를 위한 휴대용/데스크톱 기기로 보았고, 사람들이 독립형 OpenAI 하드웨어에 대해 가졌던 기대와 비교했습니다.
- @kimmonismus는 별도로 Microsoft Scout를 "항상 켜져 있는 업무용 개인 에이전트"로 강조했습니다.

### Web IQ 및 에이전트용 검색
- @JordiRib1은 웹 페이지, 뉴스, 이미지, 비디오를 위한 AI 네이티브 그라운딩 API 스위트인 Microsoft Web IQ를 발표했습니다.
- 그의 프레이밍은 중요한 맥락을 제공합니다. 고전적인 검색 엔진은 인간을 위해 만들어졌지만, Microsoft는 미래의 검색 수요가 에이전트로부터 올 것이며, 이는 인간 검색 트래픽보다 잠재적으로 1000배 더 많은 쿼리가 될 수 있다고 믿습니다.
- 그는 Web IQ가 품질, 레이턴시, 토큰 효율성을 위해 Bing의 스택에서 재설계되었으며, Copilot 및 ChatGPT를 포함한 주요 챗봇에 이미 사용되고 있다고 주장했습니다.

### Foundry 및 오픈 모델 배포
- @jeffboudier는 Satya가 Microsoft Foundry에서 11,000개 이상의 모델을 사용할 수 있다고 언급했으며, 그 중 10,928개가 Hugging Face에서 온 것이라고 말했습니다.
- 이는 Build에서 Microsoft의 병렬적인 정체성을 지지합니다. 즉, 자사 모델 빌더이자 대규모 멀티 모델 호스팅/배포 플랫폼이라는 것입니다.

### 데이터센터 및 컴퓨팅에 대한 Build 메시징
- 여러 관찰자들은 데이터센터 확장, 커뮤니티 반발, 그리고 AI 인프라가 지역 사회의 전기료를 올리지 않고도 확장될 수 있다는 Microsoft의 주장에 대한 Build 논의를 언급했습니다. @kimmonismus 및 @kimmonismus를 참조하십시오.
- @scaling01은 Mustafa가 AI 컴퓨팅이 향후 3년 내 1000배 성장하여 현재 약 5e27 FLOPs의 프론티어 규모가 2029년까지 5e30 FLOPs로 증가할 것이라고 말한 점을 강조했습니다.
- @mustafasuleyman은 회사의 철학적 주제를 "인본주의적 초지능"으로 요약했습니다.

## 사실 대 의견

### 트윗 세트의 사실적 주장
- Microsoft는 Build에서 7개의 새로운 MAI 모델을 출시했습니다: @MicrosoftAI
- MAI-Thinking-1의 공식 지표: 35B 활성 MoE, 256K 컨텍스트, AIME 2025에서 97%, SWE-Bench Pro에서 53%, Sonnet 4.6보다 블라인드 인간 선호도 우위: @mustafasuleyman
- MAI-Code-1-Flash의 공식 지표: SWE-Bench Pro에서 51%, 트윗 내용에 명시된 5B 파라미터: @mustafasuleyman
- MAI-Image-2.5 순위 주장은 @arena에 의해 독립적으로 확인되었습니다.
- MAI-Transcribe-1.5의 속도/정확도 세부 정보는 독립적인 벤치마크 계정 @ArtificialAnlys에서 나왔습니다.
- Microsoft는 109페이지 분량의 기술 보고서를 발표했습니다: @eliebakouch

### 의견 / 해석
- "@teortaxesTex의 'Microsoft가 이제 진지한 모델을 학습시키고 있나?'는 모델/보고서 품질에 대한 해석적 반응이지 독립적인 사실이 아닙니다."
- 보고서가 "가장 투명한 보고서 중 하나" 또는 "최신 교과서"라는 주장은 @eliebakouch 및 @nrehiew_의 의견이며, 많은 독자들이 공유하는 견해입니다.
- @kimmonismus 및 @TheTuringPost는 Build를 클라우드 전용 AI에서 로컬 추론/에이전트 중심의 전략적 전환으로 보았습니다. 이는 공식 문구라기보다는 분석입니다.
- @swyx 및 @scaling01을 포함하여 Microsoft가 Anthropic Mythos FLOPs를 "유출했다"는 주장은 슬라이드에 대한 추측성 해석이며, 나중에 동일한 댓글 그룹에 의해 이의 제기되었습니다.

## 다른 의견 및 관점

### 지지하는 견해
- 기술 독자들은 보고서의 투명성과 Microsoft가 이 규모에서 일반적으로 공개되지 않는 세부 사항을 발표하려는 의지에 전반적으로 깊은 인상을 받았습니다: @eliebakouch, @nrehiew_, @ethanCaballero, @stochasticchasm
- 일부는 MAI-Thinking-1을 Microsoft가 단순한 모델 리셀러나 애플리케이션 계층이 아닌 진정한 프론티어 랩이 되고 있다는 증거로 보았습니다. 예를 들어 @teortaxesTex, @echen, @NandoDF
- 기업/플랫폼 지지자들은 깨끗한 데이터 계보, 파인튜닝 가능, 비공개 사후 학습 데이터 스토리를 좋아했으며, 특히 Baseten/Microsoft의 소유권 및 제어권에 대한 포지셔닝을 높이 평가했습니다: @baseten, @tuhinone

### 중립적 / 분석적 견해
- 여러 게시물은 출시를 환영하기보다는 보고서를 읽고 분석하는 데 중점을 두었습니다. 특히 @stochasticchasm, @nrehiew_, @eliebakouch
- 일부 평론가들은 벤치마크 해석에 신중했습니다. @kimmonismus는 Microsoft가 일반적으로 Sonnet 4.6과 비교하는 것처럼 보였고, Opus 수준의 비교 가능성은 SWE Pro에서만 나타났다고 언급했습니다.
- @iScienceLuvr는 코딩/수학뿐만 아니라 HealthBench Professional 및 MedXpertQA와 같은 건강 벤치마크에 대한 보고를 특히 높이 평가했습니다.

### 회의적 / 반대 견해
- 일부에서는 모든 수치와 비교가 정확하게 해석되었는지, 특히 활성 파라미터 및 외부 모델 비교에 대해 의문을 제기했습니다.
- 가장 눈에 띄는 회의론은 명백한 Mythos FLOP "유출"에 관한 것이었습니다. @iScienceLuvr는 그것이 아마도 추정치일 뿐 유출이 아닐 것이라고 제안했습니다. @scaling01은 나중에 원래의 6.1e27 FLOP 수치가 비현실적이라고 주장하고 더 낮은 대체 추정치를 제시한 후 @scaling01에서 정정 게시물을 올렸습니다.
- 또한 합성 데이터 없음 / 디스틸레이션 없음이 최고의 에이전틱 성능을 위한 올바른 장기적 레시피인지에 대한 분야 내 암묵적인 회의론도 있었습니다. 예를 들어, 다른 곳의 합성 데이터 차이를 강조하는 독자들(@stochasticchasm)이 언급했습니다.

## 맥락: 왜 이것이 중요한가
- Build의 발표는 Microsoft가 더 이상 다음 역할에만 만족하지 않는다는 것을 시사하기 때문에 중요합니다.
    *   Azure/OpenAI의 클라우드 호스트
    *   GitHub의 개발자 표면
    *   Copilot의 애플리케이션 셸
    Microsoft는 또한 자체 모델 제품군, 실리콘 스택, 사후 학습 플랫폼을 갖춘 자사 프론티어 모델 개발자가 되려고 노력하고 있습니다.
- 깨끗한 계보 / 디스틸레이션 없음 강조는 전략적으로 중요합니다. 이는 IP 출처, 미래 제어 가능성, 외부 랩에 대한 의존도에 대한 기업의 우려를 해소합니다.
- 온디바이스 AI 강조는 Microsoft가 AI 전략을 Azure뿐만 아니라 Windows 및 기기 배포와 연결하고 있기 때문에 중요합니다. Build 메시징은 추론 모델, 플래너, 에이전트가 클라우드뿐만 아니라 기기에서도 점점 더 많이 실행될 수 있다는 아이디어를 반복적으로 강조했습니다: @TheTuringPost, @yusuf_i_mehdi
- 109페이지 분량의 보고서는 프론티어 모델 투명성이 일반적으로 줄어들고 있으며, 특히 데이터, 인프라, 학습 방법론에 대한 투명성이 줄어들고 있기 때문에 중요합니다. 여러 연구자들은 이 규모에서 공개 수준이 이례적이라고 명시적으로 언급했습니다: @eliebakouch, @nrehiew_
- Build 요약은 또한 Microsoft가 스택의 모든 계층을 통합하려고 노력하고 있음을 보여주었습니다.
    *   모델: MAI 제품군
    *   칩: MAIA 200
    *   클라우드: Azure + Foundry
    *   OS: Windows 에이전트 런타임
    *   개발자 UX: Copilot 앱 / VS Code / CLI
    *   리트리벌/그라운딩: Web IQ
    *   하드웨어 폼 팩터: Solara / Scout 개념
- 이러한 조합 때문에 여러 관찰자들은 이 이벤트를 일반적인 개발자 컨퍼런스라기보다는 클라우드, 엣지, OS, 맞춤형 모델을 아우르는 에이전트 플랫폼을 향한 조직적인 움직임으로 묘사했습니다. 예를 들어 @satyanadella, @mustafasuleyman, @TheTuringPost.

## “Mythos FLOPs 유출” 미니 스토리
- Build 기간 중/이후, 일부 사용자들은 Microsoft 슬라이드가 Anthropic의 소문난 Claude Mythos의 훈련 컴퓨팅을 의도치 않게 공개했다고 주장했으며, @swyx는 Mustafa가 FLOPs 수를 유출했는지 물었습니다.
- @scaling01은 해당 슬라이드가 픽셀 측정 기반의 신뢰 구간과 함께 6.1e27 FLOPs를 암시한다고 추정했으며, @kimmonismus는 이는 Gemini 3.1 Pro 규모의 컴퓨팅과 비슷할 것이라고 언급했습니다.
- 이러한 해석은 이후 @iScienceLuvr에 의해 이의가 제기되었는데, 그는 그것이 아마도 추정치일 것이라고 주장했습니다. 그리고 @scaling01은 3.37e26에서 1.46e27 FLOPs에 이르는 더 낮은 범위의 모델 기반 추정치를 게시했으며, 이후 @scaling01에서 원래 수치는 가짜라고 말했습니다.
- 이 에피소드는 주로 맥락상 유용합니다. Build의 컴퓨팅/스케일링 메시징은 사람들이 발표 자료에서 경쟁사의 훈련 예산을 추론하기 시작할 만큼 충분히 상세했습니다.

## 개발자 도구, 에이전트, 그리고 코딩 워크플로우
- OpenAI는 Codex에 Sites를 출시했습니다. 이는 팀이 아이디어/문서/계획을 인증 및 동적 데이터를 갖춘 배포된 내부 웹사이트/앱으로 전환할 수 있도록 하며, 우선 비즈니스/엔터프라이즈 사용자를 대상으로 합니다. (@OpenAI, @TheRohanVarma, @gdb)
- OpenAI는 또한 영업, 데이터 분석, 크리에이티브 프로덕션, 제품 디자인 및 공공 주식 워크플로우 전반에 걸쳐 역할별 Codex 플러그인을 확장했으며, 62개의 앱과 110개의 스킬에 접근할 수 있습니다. (@OpenAI, @OpenAIDevs)
- GitHub의 Copilot 앱과 Microsoft의 Build에서 에이전트 네이티브 소프트웨어 개발에 대한 강조는 그날의 툴링 뉴스에서 핵심이었습니다. (@pierceboggan, @lukehoban, @GHchangelog)
- Anthropic은 Claude Platform용 CLI를 출시하고 Claude Code의 /fork를 업그레이드하여 정확한 컨텍스트 + 프롬프트 캐시를 가진 백그라운드 에이전트를 실행하도록 했습니다. (@ClaudeDevs, @ClaudeDevs)
- Nous는 Hermes 에이전트를 위한 로컬/네이티브 데스크톱 인터페이스인 Hermes Desktop을 출시했습니다. (@NousResearch, @Teknium) 이후 @Teknium과 @ollama에서 Tailscale/Ollama 통합 관련 소식이 있었습니다.
- Cognition은 Devin Desktop을 출시했습니다. 이는 로컬/클라우드 에이전트 관리를 위한 에이전트 중립 데스크톱이자 로컬 계획과 클라우드 실행 간의 핸드오프를 위한 것으로 포지셔닝되었습니다. (@cognition, @ScottWu46, @russelljkaplan)

## 모델, 로컬 인퍼런스, 그리고 라우팅
- H Company는 Qwen 스타일 아키텍처 기반의 로컬 컴퓨터 사용 모델 제품군인 Holo 3.1을 출시했습니다. 0.8B에서 35B까지의 체크포인트와 NVFP4, FP8, Q4 GGUF를 포함한 형식을 지원합니다. 인기 있는 요약본에 따르면 35B 모델은 AndroidWorld에서 79.3%를 기록했습니다. (@TeksEdge, @hcompany_ai의 출시 트윗)
- Perplexity는 Perplexity Computer를 위한 하이브리드 에이전틱 인퍼런스를 발표했습니다. 이는 온디바이스 로컬 모델과 프론티어 클라우드 모델 간에 작업을 분할하여 프라이버시와 토큰 효율성을 높입니다. (@perplexity_ai, @AravSrinivas)
- @ttunguz가 공유한 OpenRouter 데이터에 따르면 오픈 웨이트 모델이 토큰 볼륨의 69.1%를 차지했으며, 클로즈드 모델은 30.9%였습니다.
- 모델 라우팅이 미래의 핵심 추상화가 될 것이라는 의견이 @ClementDelangue, @garrytan, @matanSF로부터 나왔으며, @glennko는 기업의 프로덕션 신뢰성 때문에 일반적인 라우팅이 열성적인 사람들이 제안하는 것보다 더 어렵다고 주장하며 반대 의견을 제시했습니다.
- 로컬 AI UX 개선 사항은 Hugging Face의 하드웨어 호환성 검사와 @m_newhaus 및 @jundotkim의 oMLX 네이티브 macOS 앱 출시에서도 나타났습니다.

## 연구 및 평가
- Google DeepMind는 과학을 위한 Gemini 기반의 다중 에이전트 가설 생성 시스템인 Co-Scientist를 발표했습니다. 이는 간 섬유증 표적, ALS 접근법, 노화 관련 유전적 단서를 식별하는 데 도움이 된 협업을 주장합니다. (@GoogleDeepMind, @GoogleDeepMind, @GoogleDeepMind)
- 편집 가능한 과학 그림 생성에 대한 새로운 Crafter / CraftEditor 작업은 그림을 생성하고 개선하며 래스터-SVG 변환을 위한 5개 에이전트 워크플로우로서 주목을 받았습니다. (@HuggingPapers, @_akhaliq, @TheTuringPost)
- Tilde Research는 대각선 망각 게이트를 가진 RoPE-free 어텐션 방법인 Wall Attention을 소개했습니다. 이는 4k에서 훈련하고 200k+ 토큰으로 일반화하며 Triton 커널과 강력한 디코드 처리량을 제공한다고 주장합니다. (@tilderesearch)
- @jbhuang0604는 정적 이미지 사전 학습에 의존하기보다 동적 인식을 인코딩하여 실제 OOD 성공률을 22.5% 높였다고 주장하는 로봇 비전 인코더를 게시했습니다.
- 주목할 만한 새로운 평가/벤치마크:
    - 정확한 이미지 편집을 위한 PaintBench (최고 모델은 17.1%에 불과했습니다.) (@itskaixu)
    - 비디오 상태 추적을 위한 VSTAT (프론티어 MLLM이 진화하는 세계 상태를 추적하는 데 여전히 약하다고 주장합니다.) (@PinzhiHuang, @sainingxie)
    - 엔터프라이즈 데이터 워크플로우를 위한 Data Agent Benchmark (@sh_reya)

## 인퍼런스, 인프라, 그리고 에이전트 시스템
- Harvey + LangChain은 법률 에이전트를 위한 저렴한 검증기에 대한 작업을 공유했습니다. 이는 DeepSeek V4 Flash가 Opus 4.7과 94–96%의 일치율을 유지하면서 기준별 모드에서 비용을 18배, 배치 모드에서 약 1000배 절감할 수 있음을 보여주었습니다. 3,200회의 RL 롤아웃에 대해 검증 비용이 18,000달러에서 18달러로 감소했습니다. (@harvey, @hwchase17, @nikogrupen)
- W&B는 Weave를 에이전트 우선 관측성으로 재출시했습니다. 이는 일반적인 하네스 전반의 통합과 실패 모드의 자동 감지 기능을 갖추고 있습니다. (@wandb, @neutralino1)
- Prime-RL은 크로스 노드 프리픽스 / KV 캐시 재사용을 위해 Mooncake Store를 vLLM과 통합했습니다. 이는 에이전틱 롤아웃의 핵심으로 제시되었습니다. (@m_sirovatka)
- Together는 MiniMax-M3를 위한 서빙 최적화를 상세히 설명했습니다. KV-블록 메이저 희소 어텐션, 페이지드 디코드, 최적화된 인덱스 스코어링, 멀티모달 전처리 등을 통해 81–125%의 처리량 개선을 언급했습니다. (@togethercompute)
- MiniMax 자체는 1M 컨텍스트, 네이티브 멀티모달리티, 데스크톱 컴퓨터 작동, 그리고 MSA가 디코드 시간에서 어텐션의 비중을 약 30%에서 약 5%로 줄인다는 점을 강조했습니다. (@MiniMax_AI)

## 생태계, 하드웨어, 그리고 산업 역량
- Westmag는 미국 로봇 액추에이터 및 드론 모터 개발을 위해 스텔스를 해제했습니다. a16z가 주도하고 Founders Fund, Lux, NFDG, Menlo 등이 참여하여 1,100만 달러를 유치했습니다. (@boxcardavid, @packyM, @oyhsu)
- PyTorch는 NVIDIA가 4개의 오픈 모델 제품군에 걸쳐 개방형 AI 모델 라이선스 프레임워크인 OpenMDW-1.1을 채택했다고 언급했습니다. (@PyTorch)
- Martin Scorsese는 Black Forest Labs와 함께 스토리보딩을 위한 FLUX의 제한적이고 사전 제작 단계의 사용을 공개적으로 시연했습니다. 이는 생성적 대체가 아닌 손으로 그린 작업에 대한 탐색적이고 보완적인 것으로 설명되었습니다. (@robrombach, @TheRundownAI)

---

# AI Reddit Recap

## /r/LocalLlama + /r/localLLM Recap

### 1. NVIDIA Nemotron 3 Ultra and RTX Spark Specs

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-microsoft-build-mai-thinking&utm_source=paywall-free-trial&utm_medium=web&utm_content=200399328&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-microsoft-build-mai-thinking&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
