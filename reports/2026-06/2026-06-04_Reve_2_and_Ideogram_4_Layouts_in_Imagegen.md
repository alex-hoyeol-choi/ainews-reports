# Reve 2 and Ideogram 4: Layouts in Imagegen

**원문 URL**: https://www.latent.space/p/ainews-reve-2-and-ideogram-4-layouts
**번역일**: 2026-06-04 06:21
**발행일**: 2026-06-04

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Reve 2와 Ideogram 4: 이미지 생성의 레이아웃

### 조용한 하루.
4년 전 우리는 이미지 구성이 부분적으로 AGI-Hard라고 주장했습니다. 그 문턱이 올해 무너졌습니다. Reve와 Ideogram이 오늘 동시에 출시되었고, 둘 다 강력한 레이블링과 레이아웃 코드를 통해 어떻게 발전을 이루었는지 크게 강조했다는 것은 단순한 우연일 수 없습니다.

![X avatar for @reve](https://pbs.substack.com/profile_images/1965505496083038217/10qkW0k9.jpg)
그리고 여기 Ideogram 4.0이 있습니다. 이제 최고의 오픈 이미지 모델입니다.

![X avatar for @ideogram_ai](https://pbs.substack.com/profile_images/2062202352526831616/9CslGhhc.jpg)
이것들은 훌륭한 성과이며, 모두 미국 모델들의 훌륭한 성과입니다. 하지만 Arena 랭킹은 GPT-Image-2가 얼마나 앞서 있는지 보여줍니다…

![X avatar for @Taesung](https://pbs.substack.com/profile_images/1902838668097925120/aihe-9_C.jpg)
> 2026년 6월 2일~6월 3일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터(X)를 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터(X) 요약
Microsoft의 MAI-Thinking-1 기술 보고서, 학습 스택, 그리고 프론티어 파인튜닝 추진
- MAI-Thinking-1은 오늘 가장 밀도 높은 기술 발표였습니다. Microsoft는 타사 디스틸레이션 없이 학습된 범용/추론 모델인 MAI-Thinking-1을 소개했으며, AIME 2025에서 97%, SWE-Bench Pro에서 53%를 기록했고, 블라인드 비교에서 Sonnet 4.6보다 인간 선호도에서 우위를 차지했다고 보고했습니다. 109페이지 분량의 이 보고서는 @eliebakouch, @nrehiew_, @mustafasuleyman으로부터 이례적인 투명성으로 널리 칭찬받았습니다. 주요 기술 주제는 Microsoft가 "맨바닥부터 언덕을 올랐다(hillclimbed from scratch)"는 것으로 보이며, @MinjiYoon90은 이러한 노력을 명시적으로 그렇게 표현했습니다.
- 연구자들이 이 보고서에 주목한 이유: 가장 많이 언급된 세부 사항은 벤치마크 품질뿐만 아니라 공개된 시스템/학습 정보의 양이었습니다. @eliebakouch는 합성 데이터와 이전 모델 디스틸레이션이 전혀 없었다는 점을 강조했는데, 이는 추론, 도구 사용, 에이전틱 행동이 합성 "콜드 스타트" 없이 사후 학습에서 학습되었다는 것을 의미합니다. 해당 스레드에서는 스케일링 래더 레시피, 정확한 MFU 수치, 타겟 손실 구성의 공개도 언급했습니다. 후속 글에서 @eliebakouch는 비공개 NLL 혼합이 코드 50%, STEM 17.5%, 수학 17.5%, 일반 지식 10%, 다국어 5%로 가중되었으며, 내부 모델에 대한 정규화가 이루어졌다고 언급했습니다. 그는 또한 MoE 설정에서 100–200 TPP 주변의 어블레이션도 지적했습니다. 커뮤니티 요약에서 드러난 다른 주목할 만한 구현 세부 사항으로는 Microsoft가 스택의 일부에 SGLang을 사용했으며(@eliebakouch), 사전 학습 데이터 큐레이션에는 dspy.GEPA를 사용했다는 점(@lateinteraction 및 @harold_matmul)이 있습니다.
- Microsoft의 제품화 방향은 단일 모델을 넘어섭니다. 보고서와 함께 Microsoft는 더 광범위한 "자신만의 모델 소유(own your model)" 스토리를 추진했습니다. @mustafasuleyman은 워크플로우별 적응을 위한 강화 학습 환경에 중점을 둔 Frontier Tuning을 설명하며, 내부 Excel 지향 MAI-튜닝 모델이 관련 작업에서 GPT-5.4 수준의 품질에 도달하면서도 최대 10배 더 효율적일 수 있다고 주장했습니다. Build 출시에는 Microsoft가 텍스트-투-이미지에서 3위, 이미지-투-이미지 Arena 리더보드에서 2위라고 밝힌 MAI-Image-2.5와 MAI-Code-1-Flash, 그리고 OneDrive Photos와 같은 제품으로의 배포도 포함되었습니다. 메타적인 관점에서 볼 때, 이는 올해 한 연구소가 프론티어 스타일 보고서를 발표하면서 동시에 해당 스택을 기업 맞춤형 인프라로 전환하려는 가장 명확한 사례 중 하나입니다.
오픈 모델 출시: Gemma 4 12B, Ideogram 4.0, Miso One, 그리고 로컬 우선 모멘텀
- Gemma 4 12B는 단연 돋보이는 오픈 모델 출시였습니다. Google은 약 16GB VRAM으로 온디바이스에서 실행되도록 설계된 Apache 2.0 멀티모달 모델인 Gemma 4 12B를 출시했습니다. 아키텍처의 참신함은 인코더 없는 디자인입니다. 즉, 별도의 비전 또는 오디오 타워가 없습니다. Google이 설명했듯이, 이미지는 경량 임베딩 모듈을 통해 처리되고, 원시 오디오는 텍스트-토큰 공간으로 직접 투영됩니다. 커뮤니티 반응은 모달리티 인코더를 LLM 백본으로 통합하는 우아함에 집중되었으며, @googlegemma, @googleaidevs, @mtschannen, @armandjoulin 모두 같은 점을 강조했습니다. vLLM, Ollama, llama.cpp/MLX(@osanseviero를 통해), 그리고 양자화된 형태로 8GB RAM만으로도 로컬 실행이 가능하다고 알려진 Unsloth GGUF에 걸쳐 즉시 툴링 지원이 이루어졌습니다.
- Ideogram의 오픈 웨이트 전환은 모델 자체만큼이나 중요했습니다. Ideogram 4.0은 "세계 최고의 오픈 이미지 모델"로 발표되었으며, 오픈 웨이트와 함께 fal 및 Hugging Face를 통해 즉시 배포되었습니다. Arena는 Ideogram-4.0-Quality를 전체 8위, 오픈 모델 중 1위로 빠르게 평가했으며, 텍스트 렌더링 및 브랜딩/상업 디자인에서 특히 강력한 성능 향상을 보였습니다. 이 오픈 릴리스는 Ideogram이 이전에 매우 디자인 중심적이지만 클로즈드 소스로 간주되었기 때문에 큰 주목을 받았으며, 이러한 전환은 @multimodalart와 @cloneofsimo에 의해 언급되었습니다.
- 오픈 오디오 분야도 강세를 보였습니다. Miso One은 원샷 보이스 클로닝과 110ms의 레이턴시를 주장하는 8B 오픈 웨이트 TTS 모델로 출시되었으며, 더 표현력이 풍부한 보이스오버를 목표로 합니다. Alibaba의 Fun-Realtime-TTS 또한 Artificial Analysis의 Speech Arena에서 1219 ELO로 1위를 차지했으며, Gemini 3.1 Flash TTS와 Inworld를 제치고 100만 글자당 $27.59의 비용을 보였습니다. 별도로, Google의 Magenta RealTime 2는 온디바이스 사용을 위한 오픈 웨이트, 저 레이턴시 연속 음악 생성기로 강조되었습니다.
- 더 큰 흐름은 로컬 AI가 주류 배포 타겟이 되고 있다는 점입니다. @ggerganov는 Computex를 로컬 AI 워크로드의 강력한 신호로 언급했으며, @rasbt 또한 성장하는 오픈 웨이트, 소비자 하드웨어 생태계를 지적했습니다. Microsoft의 Surface Laptop Ultra 홍보(최대 1 PFLOP AI 컴퓨팅, 128GB 통합 메모리, RTX GPU)는 하드웨어 측면에서 같은 트렌드에 부합합니다.
에이전트, 하네스, 그리고 프레임워크에서 실행 레이어로의 전환
- 중심축이 "프레임워크"에서 에이전트 하네스 및 실행 환경으로 이동하고 있습니다. 여러 게시물이 같은 아이디어로 수렴했습니다. @gakonst는 미래의 IDE 스택이 코드 에디터보다는 파일을 스레드로 대체하고 계획/설계/빌드/배포/모니터링 루프를 묶는 것에 더 가깝다고 주장하며, 협업/동기화 엔진이 핵심 미해결 문제로 남아있다고 했습니다. 보완적인 인터뷰 요약에서 @ConorBronsdon은 Jerry Liu의 견해를 전했는데, "프레임워크 시대"가 끝나고 있으며, 추상화가 Python 래퍼보다는 스킬, 도구, 컨텍스트 품질로 상향 이동하고 있다는 것입니다.
- 다중 에이전트 및 에이전트 최적화 작업이 더욱 구체화되고 있습니다. CMU/LTI의 MACU와 @kohjingyu의 스레드는 컴퓨터 사용 에이전트가 관리자가 작업을 분해하고 병렬 서브 에이전트를 파견하는 다중 에이전트 DAG 기반 시스템으로 설계되어야 한다고 주장합니다. 보고된 성능 향상은 벤치마크 전반에서 4.7–25.5%였으며, Odysseys에서는 1.5배 더 빠른 완료를 보였습니다. 최적화 측면에서 Microsoft의 SkillOpt는 @omarsar0로부터 실질적인 검증을 받았는데, 그는 이를 오케스트레이터에 연결하자 하나의 멀티모달 추출 스킬이 0.73에서 0.93으로 향상되었다고 말했습니다.
- 에이전트 UX 및 배포 툴링이 그 자체로 제품이 되고 있습니다. Nous의 Hermes Agent 업데이트는 강력한 참여를 이끌어냈는데, 여기에는 원격 연결 수정, 업데이트된 원격 가이드, 그리고 더 큰 대시보드 전면 개편이 포함됩니다. Perplexity는 Windows용 Personal Computer를 출시했는데, 이는 앱/파일을 위한 온디바이스 오케스트레이터입니다. 한편 Cloudflare Browser Run 원격 탭은 더 에이전트 네이티브적인 브라우저 제어 경로를 보여주었습니다. LangChain/LangSmith는 Gateway 지출 추적, Sandbox/Gateway/Observability 문서, 그리고 Deep Agents 및 LangSmith 관련 사례 연구를 통해 관측 가능성 및 비용 제어 레이어를 강화했습니다.
라우팅, 비용 제어, 그리고 오픈 대 프론티어 배포 전략
- 모델 라우팅은 이제 슬로건이 아닌 실제 논쟁입니다. @levie는 토큰 예산이 의미 있는 운영 비용(opex) 범주가 되면서 모델 라우팅이 불가피하며, 도메인별 평가가 차별화 요소가 될 것이라고 주장했습니다. 그러나 @scottastevenson은 대부분의 라우팅 제품을 지금까지 "사기(snake oil)"라고 부르며 강력히 반박했습니다. 프론티어 모델은 재시도를 피하면 전체적으로 더 좋고/빠르고/저렴할 수 있으며, 라우팅은 긴밀하게 결합된 시스템을 불안정하게 만들 수 있고, API 벤더는 종종 명백한 차익 거래를 내부화할 수 있다는 것입니다. @fabianstelzer는 캐시 쓰기 및 하네스-모델-프롬프트 적합성이 예상되는 절감 효과를 없앨 수 있다고 덧붙였습니다.
- 기업 사용자들은 엄격한 비용 상한선을 시행하기 시작했습니다. @simonw는 Uber가 코딩 에이전트 지출을 직원당 도구당 월 $1,500로 제한한다는 보고서를 강조했습니다. LangChain은 즉시 이를 LangSmith Gateway의 사용 사례로 제시했습니다. 더 넓은 분위기는 @Yuchenj_UW에 의해 포착되었습니다. 일부 조직은 곧 모든 사람이 "토큰을 최대한 사용하도록(tokenmaxx)" 허용하거나, 예산을 제한하거나, 인력을 줄이고 가장 생산적인 AI 지원 작업자에게 지출을 재할당하는 세 가지 선택에 직면할 수 있습니다.
- 하이브리드/오픈 전략에 대한 실제 데이터 포인트가 나타나기 시작했습니다. Harvey의 벤치마크 결과가 가장 명확한 예시였습니다. 한 연구에서 Harvey는 GLM 5.1을 주요 작업자로, Opus 4.7을 어드바이저로 사용하는 하이브리드 법률 에이전트가 순수 Opus보다 전체 통과율(18% 대 14%)에서 우수했으며, 100개 작업에 걸쳐 $368 대 $954의 비용이 들었다는 것을 발견했습니다. Harvey는 또한 SFT가 Kimi 2.6의 성능을 11%에서 15%로 향상시켜, Opus를 약 11배 낮은 비용으로 능가할 수 있다고 보고했습니다. 다른 한편으로, @ClementDelangue는 라우팅과 사후 학습된 오픈 모델이 비용/속도/제어 측면에서 종종 우위를 점할 것이라고 주장했으며, @ypatil125는 오픈 모델과 오픈 모델 클라우드를 중요한 워크로드의 궁극적인 기본값에 대한 선행 지표로 보았습니다.
인기 트윗(참여도 기준)
- Gemma 4 12B 출시: @googlegemma와 @Google은 인코더 없는 멀티모달 릴리스로 가장 큰 기술적 참여를 이끌어냈습니다.
- Ideogram 4.0 오픈 웨이트: @ideogram_ai는 강력한 클로즈드 이미지 모델에서 오픈 웨이트로의 주목할 만한 전환을 발표했습니다.
- MAI-Thinking-1 투명성: @eliebakouch의 스레드는 MAI 보고서에 대한 가장 영향력 있는 기술 독해 가이드였습니다.
- 생명 과학을 위한 Rosalind: OpenAI의 GPT-Rosalind 업데이트는 프론티어 모델이 도메인별 과학 연구로 더욱 수직화되고 있음을 시사했습니다.
- 오픈 오디오/TTS 모멘텀: Alibaba의 Fun-Realtime-TTS와 Miso One은 단순한 연구 데모가 아닌 실용적인 출시로 돋보였습니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Gemma 4 멀티모달 오픈 모델

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-reve-2-and-ideogram-4-layouts&utm_source=paywall-free-trial&utm_medium=web&utm_content=200554331&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-reve-2-and-ideogram-4-layouts&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
