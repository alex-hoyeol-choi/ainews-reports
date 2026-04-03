# Gemma 4: The best small Multimodal Open Models, dramatically better than Gemma 3 in every way

**원문 URL**: https://www.latent.space/p/ainews-gemma-4-the-best-small-multimodal
**번역일**: 2026-04-03 07:18
**발행일**: 2026-04-03

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Gemma 4: 최고의 소형 멀티모달 오픈 모델, Gemma 3보다 모든 면에서 비약적으로 개선

### Google의 반가운 업데이트입니다!
공유Allen Institute의 갑작스러운 인력 이탈과 GPT-OSS의 불확실한 상태로 인해 미국 오픈 모델의 미래가 불투명해진 상황에서, Google DeepMind가 Gemma 4의 개발 속도를 유지하는 것은 매우 매우 매우 반가운 소식입니다! 31B 덴스(dense) 모델은 Kimi K2.5 (744B-A40B) 및 Z.ai GLM-5 (1T-A32B)와 함께 세계 최고 수준의 오픈 모델로 어깨를 나란히 하지만, 훨씬 적은 총 파라미터 수를 가지고 있습니다 (아래에서 다른 흥미로운 아키텍처 선택 사항을 확인하십시오):

![](https://substack-post-media.s3.amazonaws.com/public/images/24c86eb5-bb3b-4f1d-9c92-7ff21d46366_2048x1153.png)
의례적인 파레토 차트Arena의 이 이미지는 수년간의 발전을 보여줍니다 (숫자 순위가 아닌 # 순위로 인해 과장된 측면이 있지만, GPQA 및 AIME와 같은 진정한 표준 벤치마크에서도 Gemma 3 대비 엄청난 개선을 보였습니다):

![](https://substack-post-media.s3.amazonaws.com/public/images/590ec254-eaaf-4ab6-b939-d49704ab6b31_1612x1616.png)
라이선싱 또한 적절한 Apache 2.0 라이선스로 개선되었으며, 이 모델들은 "비디오와 이미지를 기본적으로 처리하고, 가변 해상도를 지원하며, OCR 및 차트 이해와 같은 시각적 작업에서 탁월한 성능을 발휘합니다. 또한, E2B 및 E4B 모델은 음성 인식 및 이해를 위한 기본 오디오 입력을 특징으로 합니다."
뛰어난 온디바이스(on-device) 기능은 이 모델들이 Apple과의 계약에 따라 새로운 Siri에 배포될 모델의 기반이 될지 궁금하게 만듭니다….
> 2026년 4월 1일~4월 2일자 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터를 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 호를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Google DeepMind의 Gemma 4 출시: 오픈 웨이트, Apache 2.0, 멀티모달, 긴 컨텍스트 — 그리고 빠른 생태계 확산
- Gemma 4는 Google이 지난 1년간 선보인 오픈 웨이트 라이선싱 및 기능 면에서 가장 큰 도약입니다: Google/DeepMind는 Gemma 4를 추론 및 에이전틱 워크플로우, 그리고 로컬/엣지 배포를 위해 명시적으로 포지셔닝한 모델 제품군으로 출시했으며, 이제 상업적으로 허용되는 Apache 2.0 라이선스 하에 제공됩니다 (이전 Gemma 라이선싱과는 확연히 달라진 점입니다). @GoogleDeepMind, @GoogleAI, @Google의 출시 스레드와 @JeffDean의 Jeff Dean의 설명 및 채택 통계 (Gemma 3: 4억 다운로드, 10만 변형)를 참조하십시오.
- 모델 라인업 + 주요 사양: 31B 덴스, 26B MoE ("A4B", 약 4B 활성), 그리고 모바일/IoT를 목표로 하는 두 가지 "효율적인" 엣지 모델 E4B 및 E2B가 발표되었으며, 이들은 기본 멀티모달 지원 (엣지용으로 텍스트/비전/오디오 강조)을 제공합니다. DeepMind의 주요 특징으로는 함수 호출 + 구조화된 JSON, 그리고 @GoogleDeepMind 및 @GoogleAI에서 언급된 최대 256K의 긴 컨텍스트 (대규모 모델)가 포함됩니다. 커뮤니티 요약과 "로컬에서 실행하는 방법" 가이드가 @_philschmid 및 @UnslothAI와 같이 빠르게 확산되었습니다.
- 초기 벤치마크 신호 (주의사항 포함):Arena/Text: Arena는 Gemma-4-31B를 오픈 모델 중 3위 (전체 27위)로, Gemma-4-26B-A4B를 오픈 모델 중 6위로 보고했습니다 (@arena); Arena는 나중에 이를 오픈 리더보드에서 미국 오픈 모델 1위로 선정했습니다 (@arena).과학적 추론: Artificial Analysis는 Gemma 4 31B (Reasoning)에 대해 GPQA Diamond 85.7%를 보고하며, @ArtificialAnlys 및 @ArtificialAnlys에서 동급 모델 대비 토큰 효율성 (약 1.2M 출력 토큰)을 강조했습니다.여러 게시물에서 규모/효율성 놀라움 (예: "자신보다 20배 큰 모델을 능가한다")을 강조하지만, 선호도 기반 리더보드는 조작될 수 있다는 점을 지적합니다; Raschka의 보다 신중한 해석은 @rasbt에 있습니다.
- Day-0 생태계 지원이 주요 이슈가 되었습니다: Gemma 4는 일반적인 로컬 + 서빙 스택에 즉시 적용되었습니다:llama.cpp Day-0 지원: @ggerganovOllama (0.20+ 필요): @ollamavLLM Day-0 지원 (GPU/TPU 등): @vllm_projectLM Studio 사용 가능: @lmstudioTransformers/llama.cpp/transformers.js 언급: @mervenoyannModular/MAX 프로덕션 인퍼런스 "수일 내": @clattner_llvm
- 로컬 인퍼런스 성능에 대한 일화들이 이례적으로 구체적이었습니다:"Brew install + llama-server"는 많은 사람들에게 표준적인 한 줄 명령어가 되었습니다: @julien_c.llama.cpp 성능 데모: M2 Ultra에서 Gemma 4 26B A4B Q8_0, 내장 WebUI, MCP 지원, @ggerganov에서 "300 t/s (실시간 비디오)" (프롬프트 암송/추측 디코딩에 대한 후속 주의사항은 @ggerganov에 있습니다).RTX 4090 긴 컨텍스트 처리량 + TurboQuant KV 양자화 세부 정보는 @basecampbernie에 있습니다.WebGPU/transformers.js를 통한 브라우저 로컬 실행 데모는 @xenovacom에 의해 언급되었고 @ClementDelangue에 의해 확산되었습니다.

---

Gemma 4 아키텍처 노트: 하이브리드 어텐션, MoE 레이어링 선택, 효율성 트릭

### 특이한 트랜스포머 세부 사항
- eliebakouch가 강조한 내용:소형 모델의 계층별 임베딩명시적인 어텐션 스케일 없음 (정규화 가중치에 흡수되었을 가능성 시사)QK norm + V norm대형 모델의 K/V 공유소형 모델의 공격적인 KV 캐시 공유슬라이딩 윈도우 크기 512 및 1024싱크 없음소프트캐핑로컬/글로벌 레이어에 다른 세타를 사용하는 부분 차원 RoPE
- Grad62304977은 누락된 어텐션 스케일이 QK norm 가중치에 병합되었을 가능성이 높다고 답했습니다.
- baseten은 추가적인 아키텍처 선택 사항을 요약했습니다:대체 어텐션 메커니즘비례 RoPE계층별 임베딩 (PLE)KV-캐시 공유비전을 위한 기본 종횡비 처리오디오를 위한 더 작은 프레임 윈도우
- norpadon은 이를 "표준 트랜스포머와는 매우 다르다"고 평했습니다.
- rasbt는 31B 덴스 모델에 대해 보다 보수적인 해석을 제시했습니다: 멀티모달 지원을 제외하고는 아키텍처가 "Gemma 3와 거의 변함이 없다"고 보이며, 하이브리드 5:1 로컬/글로벌 어텐션 메커니즘과 클래식 GQA를 유지하고 있어, 급진적인 덴스 모델 아키텍처 변경보다는 학습 레시피와 데이터에서 더 큰 도약이 있었을 가능성을 시사했습니다.
- "표준 트랜스포머가 아니다"라는 의견과 구체적인 차이점: @norpadon의 스레드에서 Gemma 4가 "갤럭시 브레인 아키텍처"를 가지고 있다고 지적했으며, 이어서 Gemma의 MoE가 DeepSeek/Qwen과 어떻게 다른지에 대한 더 구체적인 설명이 있었습니다 (Gemma는 일반 MLP 블록과 함께 별도의 레이어로 MoE 블록을 사용합니다) (@norpadon).
- 구체적인 저수준 세부 사항 유포: 특이점 (예: 명시적인 어텐션 스케일 없음, QK/V norm, KV 공유, 슬라이딩 윈도우 크기, 부분 RoPE + 다른 세타, 소프트캐핑, 계층별 임베딩)에 대한 간결한 요약은 @eliebakouch에 있습니다. Baseten의 출시 게시물 또한 유사한 "아키텍처 혁신" (PLE, KV-캐시 공유, 비례 RoPE, 비전을 위한 종횡비 처리, 더 작은 오디오 프레임 윈도우)을 @baseten에 나열합니다.
- Raschka의 해석: 최소한의 아키텍처 변경, 큰 레시피/데이터 변경: Raschka는 Gemma 4 31B가 Gemma 3 27B와 아키텍처적으로 유사하며, 여전히 하이브리드 슬라이딩 윈도우 + 글로벌 어텐션 패턴과 GQA를 사용하고 있다고 주장하며, 이러한 도약은 아키텍처 전면 개편보다는 학습 레시피/데이터에서 비롯되었을 가능성이 높다고 시사했습니다: @rasbt.

---

에이전트, 하네스 엔지니어링, "로컬 에이전트" 모멘텀 (Hermes/OpenClaw + 모델/하네스 학습 루프)
- 에이전트 엔진으로서의 오픈 모델이 이제 주류 포지셔닝입니다: 여러 게시물에서 Gemma 4를 오픈 에이전트 스택 (OpenClaw/Hermes/Pi/opencode)을 위한 "완벽한" 로컬 모델로 평가하고 있습니다. @ClementDelangue, @mervenoyann, @ben_burtenshaw를 참조하십시오.
- Hermes Agent 성장 + 플러그형 메모리:Hermes Agent는 주요 사용 이정표를 달성하고 로드맵 의견을 요청했습니다: @Teknium.새로운 플러그형 시스템을 통해 메모리 통합이 여러 제공업체로 확장되었습니다: @Teknium.로컬 임베딩 및 8ms 쿼리로 "너무 많은 작업 공간 파일" 문제를 해결하는 것으로 제시된 로컬 시맨틱 인덱스 플러그인 ("Enzyme"): @jphorism.
- 해자(moat)로서의 하네스 엔지니어링 (그리고 루프): 강력한 "모델-하네스 학습 루프" 논지 — 오픈 모델 + 트레이스 + 파인튜닝 인프라 —가 @Vtrivedy10에서 명확히 제시되었고, @Vtrivedy10에서 더 일반적으로 반향을 일으켰습니다. 관련하여: LangChain은 오픈 모델이 Deep Agents와 같은 하네스를 구동하기에 도구 사용/리트리벌/파일 작업에서 "충분히 좋다"고 언급합니다 (@hwchase17).
- 에이전트 자가 치유 + 관측 가능성 트렌드:"자가 치유" GTM 에이전트 피드백 루프에 대한 블로그가 @hwchase17에 의해 언급되었고 @Vtrivedy10에 의해 확장되었습니다.LangSmith는 6.7B 에이전트 실행을 기반으로 Azure의 OpenAI 트래픽 점유율이 10주 동안 8%에서 29%로 증가했다고 보고하며, 이는 기업 거버넌스/컴플라이언스가 라우팅 결정을 주도하고 있음을 시사합니다: @LangChain.

---

툴링 및 인프라: 커널, 파인튜닝 스택, 벡터 DB 인체공학, 문서 추출
- 새로운 선형 어텐션 커널: CUDA 선형 어텐션 커널 드롭은 @eliebakouch에 있습니다 (트윗 내 repo 링크).
- Axolotl v0.16.x: Axolotl의 릴리스는 MoE + LoRA 속도/메모리 이점 (15배 빠르고 40배 적은 메모리 주장)과 GRPO 비동기 학습 (58% 빠름)을 강조하며, @winglian 및 @winglian에서 문서 전면 개편을 포함합니다. Gemma 4 지원은 @winglian에서 이어집니다.
- 벡터 DB 인체공학: turbopuffer는 @turbopuffer에서 문서당 여러 벡터 컬럼 (다른 차원/유형/인덱스)을 추가합니다.
- 문서 자동화 스택: LiteParse + Extract v2:LiteParse 오픈소스 문서 파서: 바운딩 박스를 사용한 공간 텍스트 파싱, 대규모 표 중심 PDF에서 빠르며, @jerryjliu0에서 원본으로 돌아가는 감사 추적을 가능하게 합니다.Extract v2 (LlamaIndex/LlamaParse): 간소화된 계층, 저장된 추출 구성, 추출 전 구성 가능한 파싱, @llama_index에서 v1 전환 기간 및 @jerryjliu0의 추가 컨텍스트.

---

프론티어 조직 업데이트: Anthropic 해석 가능성, OpenAI 제품 배포, Perplexity "세금용 컴퓨터"
- Anthropic: Claude 내부의 "감정 벡터": Anthropic은 내부 감정 개념 표현이 조절 가능하며 행동에 측정 가능한 영향을 미친다고 보고합니다 (예: "절박함" 벡터를 높이면 속임수가 증가하고, "침착함"은 이를 감소시킵니다). 핵심 스레드는 @AnthropicAI, @AnthropicAI, @AnthropicAI에 있습니다. 이 작업은 또한 해석 커뮤니티에서 인용/선례 논쟁을 촉발했습니다 (예: @aryaman2020, @dribnet, 그리고 @jeremyphoward를 통한 vgel의 게시물에 대한 논의).
- OpenAI: CarPlay + Codex 가격 변경:Apple CarPlay의 ChatGPT 음성 모드가 iOS 26.4+에 출시됩니다: @OpenAI.ChatGPT Business/Enterprise의 Codex 사용량 기반 가격 책정 (프로모션 크레딧 포함): @OpenDevs. Greg Brockman은 "선불 약정 없이 직장에서 시도해보세요"라고 강조합니다: @gdb.
- Perplexity: 에이전틱 "세금용 컴퓨터": Perplexity는 연방 세금 신고서 초안 작성/검토를 돕는 워크플로우 ("내 세금 탐색")를 @perplexity_ai에서 출시했으며, 자세한 내용은 @perplexity_ai에 있습니다.

---

인기 트윗 (참여도 기준, 기술/제품/연구 필터링)
- Gemma 4 출시 (오픈 웨이트, Apache 2.0): @Google, @GoogleDeepMind, @demishassabis, @GoogleAI
- Anthropic "감정 개념/벡터" 해석 연구: @AnthropicAI
- Karpathy의 "LLM 지식 베이스" (Obsidian + 컴파일된 마크다운 위키 워크플로우): @karpathy
- Cursor 3 (에이전트 협업 인터페이스): @cursor_ai
- CarPlay의 ChatGPT: @OpenAI
- llama.cpp 로컬 성능 데모 + MCP/WebUI: @ggerganov
- Perplexity "세금용 컴퓨터": @perplexity_ai

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Gemma 4 모델 출시 및 기능

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[Start trial](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-gemma-4-the-best-small-multimodal&utm_source=paywall-free-trial&utm_medium=web&utm_content=193042475&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-gemma-4-the-best-small-multimodal&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
