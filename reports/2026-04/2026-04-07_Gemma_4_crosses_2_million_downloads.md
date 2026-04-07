# Gemma 4 crosses 2 million downloads

**원문 URL**: https://www.latent.space/p/ainews-gemma-4-crosses-2-million
**번역일**: 2026-04-07 01:17
**발행일**: 2026-04-07

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Gemma 4, 2백만 다운로드 돌파

### 조용한 하루 속에서 엄청난 성공을 거둔 Gemma 4 출시에 경의를 표합니다.
Share지난 목요일에도 언급했지만, 주말 동안 Gemma 4의 지속적인 배포와 긍정적인 평가 덕분에 출시 첫 주에 약 2백만 다운로드를 기록했습니다!
(참고로, Gemma 3는 지난 한 해 동안 총 670만 다운로드를 기록했으며, Gemma 2는 2024년 6월 출시 이후 140만 다운로드를 기록했습니다. 반면 Qwen 3.5는 397B-A17B 플래그십 모델 출시 이후 1.5개월 동안 약 2,700만 다운로드를 기록했습니다.)
Gemma 4 키노트는 런던에서 3일 후에 생중계될 예정이며, 지금 바로 북마크할 수 있습니다:
별도로, Hermes Agent에 대한 뜨거운 관심도 강조하고 싶습니다. Turing Post의 친구들이 Hermes와 OpenClaw의 차이점에 대한 좋은 글을 작성했습니다.
> 2026년 4월 4일-4월 6일 AI 뉴스입니다. 12개의 서브레딧, 544개의 트위터를 확인했으며, 추가 디스코드는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Gemma 4의 빠른 로컬 도입과 온디바이스 오픈 모델의 순간
- Gemma 4는 급격한 "로컬 우선(local-first)" 물결을 주도하고 있습니다. 여러 게시물에서 Gemma 4가 Hugging Face에서 가장 인기 있는/1위 모델이 되었으며, 단순히 리더보드 성능보다는 실용적인 유용성에 대한 강한 열정을 보여주었다고 지적했습니다. @ClementDelangue, @GlennCameronjr, @Yampeleg의 게시물을 참조하십시오. 가장 강력한 신호는 사람들이 소비자용 Apple 하드웨어에서 얼마나 빠르게 Gemma 4를 실행하고 있었는지였습니다. @adrgrondin은 MLX를 사용하여 iPhone 17 Pro에서 Gemma 4 E2B를 약 40 tok/s로 실행하는 것을 시연했습니다. @enjojoyy는 유사한 iPhone 배포를 보고했습니다. @_philschmid는 AI Edge Gallery에서 Gemma 4 E2B가 Wikipedia 쿼리용 스킬을 사용하는 것을 강조했습니다. Red Hat은 또한 @RedHat_AI를 통해 NVFP4 및 FP8-block 형식의 양자화된 Gemma 4 31B 모델 카드를 출시했으며, 명령어 추종 평가가 라이브로 진행 중이고 추론/비전 평가는 보류 중입니다. 이러한 게시물들은 Gemma 4가 단순히 또 다른 오픈 릴리스가 아니라, 엣지 인퍼런스, Apple Silicon 툴링, 그리고 마찰 없는 로컬 배포의 기준점이 되고 있음을 시사합니다.
- 상업적 함의는 유료 채팅 구독 및 클라우드 의존성에 대한 압력입니다. 일부 바이럴 코멘트는 환원적이었지만, 실제 변화를 포착하고 있습니다. @AlexEngineerAI는 Gemma 4가 로컬에서 실행되면서 일부 사용자에게는 Claude 구독의 매력을 떨어뜨릴 만큼 충분한 격차를 좁혔다고 주장했으며, @ben_burtenshaw는 Hugging Face에서 호스팅되는 모델은 무료로 사용할 수 있으며 에이전트 워크플로우의 일부를 대체할 수 있음을 상기시켰습니다. 인프라 측면에서는 @ollama가 NVIDIA Blackwell GPU를 기반으로 Ollama Cloud에 Gemma 4를 출시하여, OpenClaw 및 Claude 스타일 워크플로우와 같은 도구에서 자체 호스팅 없이 사용할 수 있도록 했습니다. @osanseviero의 주목할 만한 생태계 게시물은 출시 조정이 얼마나 광범위했는지(Hugging Face, vLLM, llama.cpp, Ollama, NVIDIA, Unsloth, SGLang, Docker, Cloudflare 등)를 강조했으며, 이는 "오픈 모델의 성공"이 단순히 가중치뿐만 아니라 동시적인 다운스트림 시스템 지원에 점점 더 의존하고 있음을 상기시켜 줍니다.
Hermes Agent의 자체 개선 에이전트 루프, OpenClaw의 마찰, 그리고 오픈 트레이스 데이터 추진
- Hermes Agent는 이번 배치에서 지배적인 에이전트 프레임워크 스토리였습니다. 핵심 서사는 Nous의 시스템이 영구 메모리, 자체 생성/정제된 스킬, 그리고 더 확고한 자체 개선 루프를 결합하여 주목을 받고 있다는 것입니다. @NousResearch의 Manim 스킬 출시는 특히 반향을 일으켰는데, 이는 또 다른 PDF 요약기가 아니라 기술 애니메이션 및 설명과 같이 즉시 이해할 수 있는 결과물을 생성하는 에이전트 스킬을 시연했기 때문입니다. 이는 @ErickSky, @lucatac0, @Sentdex, @casper_hansen_, @noctus91의 데모와 반응으로 증폭되었습니다. @Teknium의 제품 업데이트는 Discord/Telegram 봇을 위한 슬래시 커맨드 스킬 로딩을 추가했으며, Hermes HUD와 같은 커뮤니티 도구는 라이브 프로세스를 tmux 창에 매핑하고 @aijoey를 통해 승인을 표시했으며, @Teknium, @nesquena, @magiknono로부터 여러 WebUI 통합이 등장했습니다.
- OpenClaw와의 대비는 아키텍처와 비즈니스 모델의 취약성에 초점을 맞췄습니다. 여러 게시물에서 두 가지를 직접 비교했습니다. @TheTuringPost는 그 차이를 인간이 작성한 스킬 대 자체 형성 스킬, Markdown 메모리 대 영구/검색 가능한 메모리 스택, 그리고 게이트웨이 제어 플레인 대 자체 개선 루프라고 요약했습니다. 이러한 프레이밍은 @SnuuzyP, @DoctaDG, @spideystreet와 같은 실무자들에 의해 반복되었으며, 이들 중 다수는 더 쉬운 온보딩과 수동 스킬 조작의 감소를 언급했습니다. 이러한 배경에는 Claude 구독 게이팅 및 가동 시간에 대한 불만이 커지고 있었습니다. @theo는 Claude Code가 자체 소스를 분석할 때 오류를 보고했습니다. @Yuchenj_UW와 @ratlimit은 서비스 중단을 강조했습니다. @Yuchenj_UW는 20달러/200달러 구독 모델이 24/7 에이전트 워크로드와 구조적으로 맞지 않는다고 주장했습니다. 이러한 경제적 비판은 @NousResearch의 "오픈소스는 필연적이다(Open Source is inevitable)"라는 수사적 추진력을 설명하는 데 도움이 됩니다.
- 더 중요한 장기적 흐름은 오픈 에이전트 데이터였습니다. @badlogicgames는 PII 방어 기능을 갖춘 코딩 에이전트 세션을 Hugging Face 데이터셋으로 게시하기 위한 pi-share-hf를 출시한 다음, @badlogicgames를 통해 자신의 세션을 게시했습니다. @ClementDelangue는 이를 오픈소스 프론티어 에이전트에 필요한 누락된 요소로 명시적으로 규정했습니다. 커뮤니티는 이미 트레이스를 생성하고 있으므로 데이터셋을 크라우드소싱해야 한다는 것입니다. 이는 에이전틱 상호작용을 위한 궤적 샘플링/분류에 대한 @salman_paracha의 Signals 논문과, 자체 개선 모델이 깨끗한 샌드박스를 요구하는 대신 기록된 프로덕션 트레이스에서 직접 학습해야 한다는 @baseten을 통한 Baseten의 주장과 깔끔하게 연결되었습니다. 이는 아마도 여기에서 가장 기술적으로 실질적인 "에이전트" 트렌드일 것입니다. 단순히 더 나은 하네스가 아니라, 실제 사용에서 트레이스 캡처, 큐레이션 및 학습을 둘러싼 새로운 스택이 등장하고 있습니다.
새로운 연구 신호: RL, 라우팅, 에이전트 평가 및 소형 특화 모델
- 후속 학습 및 RL 효율성은 여전히 중요한 연구 분야로 남아있습니다. @TheTuringPost는 미래 단계에 강하게 영향을 미치는 토큰에 더 많은 크레딧을 할당하는 Alibaba Qwen의 FIPO(Future-KL Influenced Policy Optimization)를 강조했습니다. 보고된 결과에는 약 4K에서 10K+ 토큰으로 확장되는 추론 트레이스와 약 50%에서 ~56–58%로 증가한 AIME 이득이 포함되었으며, 이는 DeepSeekR1-Zero-Math보다 앞서고 설정에 따라 o1-mini와 비슷하거나 능가하는 수준입니다. @finbarrtimbers는 OLMo 3가 동기식 RL에서 비동기식 RL로 전환하여 토큰/초당 4배의 처리량 향상을 달성한 방법을 작성했습니다. 다른 주목할 만한 논문으로는 @_akhaliq와 @HuggingPapers를 통한 Self-Distilled RLVR / RLSD, 그리고 @TheAITimeline을 통한 Path-Constrained MoE가 있습니다. Path-Constrained MoE는 통계적 효율성을 개선하고 보조 로드 밸런싱 손실을 제거하기 위해 레이어 간 라우팅 경로를 제한합니다.
- 에이전트 및 벤치마크 연구는 장난감 같은 작업에서 벗어나고 있습니다. @GeZhang86038849는 포화된 시험 스타일 벤치마크 대신 전문가 수준의 개방형 워크플로우 평가를 명시적으로 목표로 하는 XpertBench를 소개했습니다. @TheTuringPost는 단일 함수 호출에서 장기 오케스트레이션, 재계획, 피드백 루프, 그리고 레이턴시/비용 예산과 같은 효율성 문제에 이르는 도구 사용의 진행 상황을 다루는 설문조사를 공유했습니다. 데이터/엔터프라이즈 워크플로우에서 @CShorten30는 이기종 DB 시스템 전반에 걸친 다단계 쿼리를 위한 Shreya Shankar의 Data Agent Benchmark를 지적했습니다. 이 모든 것은 평가 설계가 프로덕션 에이전트 빌더들이 중요하게 생각하는 것, 즉 워크플로우 완료, 모호성 처리, 오케스트레이션 품질 및 비용을 따라잡고 있다는 신호입니다.
- 소형 특화 모델은 강력한 사례 연구 주장을 계속하고 있습니다. @DavidGFar는 31K 인간 플레이 프레임으로 학습된 1.3M 파라미터 ModernBERT-Hash 모델인 SauerkrautLM-Doom-MultiVec-1.3M을 출시했습니다. 이 모델은 VizDoom 작업에서 훨씬 더 큰 API 액세스 LLM을 능가했으며, CPU에서 31ms 만에 실행되었습니다. 이 결과는 좁지만, 요점은 중요합니다. 적절하게 범위가 지정된 모델은 광범위한 세상 지식보다 레이턴시와 아키텍처가 더 중요한 실시간 제어 작업에서 지배적일 수 있습니다. 이와 관련하여 @MaziyarPanahi는 Falcon Perception을 추진했습니다. 이는 0.6B 세그멘테이션 지향 비전-언어 모델로, 그의 비교에서 SAM 3를 능가하고 MLX를 사용하여 MacBook에서 실행된다고 보고되었습니다. 이는 @Prince_Canuma와 @ivanfioravanti에 의해 반복되었습니다. 반복되는 주제는 특화 + 더 나은 시스템 적합성이 일반적인 스케일을 이길 수 있다는 것입니다.
OpenAI 및 Anthropic: 정책 신호, 거버넌스 조사 및 컴퓨팅 경제학
- OpenAI의 가장 큰 공개 움직임은 제품이 아닌 정치적인 것이었습니다. 회사와 그 동맹들은 @kimmonismus, @OpenAINewsroom, @AdrienLE가 요약한 새로운 "지능 시대 산업 정책" 프레이밍을 추진했습니다. 주요 아이디어에는 공공 부(Public Wealth) 기금, 휴대 가능한 혜택, 32시간 근무 주 시범 운영, AI에 대한 권리, 더 강력한 출처/감사 인프라, 그리고 위험하게 출시된 모델에 대한 봉쇄 플레이북이 포함되었습니다. 주목할 만한 전략적 메시지는 OpenAI가 이제 초지능으로의 전환을 먼 가설이 아닌 적극적인 정책 문제로 공개적으로 주장하고 있다는 것입니다. 반응은 엇갈렸습니다. 일부는 혼란에 대해 이례적으로 솔직하다고 보았고, 다른 일부는 시기상조이거나 정치적으로 편리하다고 보았습니다(예: @Dan_Jeffries1 및 @jeremyslevin). OpenAI는 또한 @OpenAI와 @markchen90를 통해 Safety Fellowship을 시작했습니다.
- 동시에, Sam Altman과 OpenAI 거버넌스에 대한 조사가 급격히 강화되었습니다. New Yorker의 주요 조사는 @RonanFarrow, @NewYorker, 그리고 @ohryansbelt와 같은 긴 커뮤니티 요약에 의해 증폭되었습니다. 이 보고서는 2023년 해고/복직 사가를 내부 메모, 기만 주장, 이사회 조작, 안전 프로세스 우려, 그리고 슈퍼 정렬(superalignment)의 자원 부족 주장을 통해 재조명했습니다. OpenAI 측의 반박은 @tszzl을 통해 이루어졌는데, 그는 정렬 팀이 회사에서 가장 크고 컴퓨팅 자원이 풍부한 프로그램 중 하나로 남아 있다고 말했습니다. 별도로, @anissagardizy8와 @kimmonismus는 Altman과 CFO Sarah Friar 사이에 특히 컴퓨팅 지출 및 IPO 준비를 둘러싼 긴장이 있다고 보고했습니다.
- Anthropic의 반박은 컴퓨팅 및 수익 규모였습니다. @AnthropicAI는 Google 및 Broadcom과 2027년부터 가동될 차세대 TPU 용량 수 기가와트(gigawatts)에 대한 계약을 발표하여 프론티어 Claude 모델을 학습시키고 서비스할 예정입니다. Anthropic은 또한 @AnthropicAI를 통해 2025년 말 90억 달러에서 300억 달러를 넘어섰다고 밝혔습니다. 이는 프론티어 연구소의 경제적 긴장에 대한 보고와 일치합니다. @kimmonismus는 WSJ 보고서를 인용하여 수익이 폭발적으로 증가하고 있지만, 학습 및 인퍼런스 비용은 여전히 엄청나며, OpenAI는 2028년까지 1,210억 달러의 컴퓨팅 지출을 예상하고 있다고 언급했습니다. 엔지니어들에게 실질적인 시사점은 간단합니다. 프론티어 경쟁은 더 이상 모델 아이디어만으로는 병목 현상이 발생하지 않으며, 자본 구조, 장기 컴퓨팅 계약 및 서비스 경제학에 의해 점점 더 제약을 받고 있습니다.
시스템 및 인프라: 더 빠른 RL, 더 빠른 MoE 디코딩, 더 나은 GPU/엣지 툴링
- 여러 게시물에서 시스템 개선 사항에 대해 이례적으로 구체적으로 언급했습니다. @cursor_ai는 "warp decode"를 통해 Blackwell GPU에서 MoE 토큰 생성이 1.84배 빨라지고 출력 품질이 향상되었다고 보고했으며, 이는 Composer 모델 업데이트 빈도 증가와 직접적으로 관련이 있습니다. @tri_dao는 빠른 Muon 옵티마이저 경로가 소비자용 Blackwell 카드에 적용될 예정이라고 언급했는데, 이는 구현이 matmul + epilogue로 표현되어 메인 루프 작업을 재사용할 수 있기 때문입니다. RL 측면에서는 @finbarrtimbers가 OLMo 3의 RL 스택을 비동기식으로 만들어 처리량을 4배 향상시킨 드문 엔지니어링 사후 분석을 제공했습니다.
- Apple/로컬 스택 및 학습/인퍼런스 교육 생태계도 계속 개선되었습니다. @josephjojoe는 Apple Silicon에서 단백질 모델링을 위한 ESM-2의 MLX 포트를 오픈소스화하여 로컬 바이오-LLM 실험을 확대했습니다. @rasbt는 LLM Architecture Gallery에 RSS 피드를 추가했는데, 이는 모델 디자인을 따라잡는 데 작지만 유용한 삶의 질 향상입니다. @UnslothAI는 자사의 무료 노트북이 이제 500개 이상의 모델을 학습/실행할 수 있다고 밝혔습니다. 더 깊은 시스템 이해를 위해 @levidiamode는 Hugging Face의 Ultra-Scale Playbook이 DP/TP/PP/EP/컨텍스트 병렬 처리를 최대 512개 GPU에 걸친 경험적 스케일링 증거와 통합한 것을 칭찬했습니다.
최고 인기 트윗 (참여도 기준)
- Gemma 4 온디바이스 데모: @adrgrondin이 MLX를 사용하여 iPhone 17 Pro에서 Gemma 4 E2B를 약 40 tok/s로 시연한 것이 가장 뛰어난 기술 바이럴 게시물이었습니다.
- Claude 구독 및 로컬 오픈 모델 대체: @AlexEngineerAI는 로컬 오픈 모델이 이제 많은 워크플로우에 "충분히 좋다"는 분위기를 포착했습니다.
- 오픈소스 입장: @NousResearch는 "오픈소스는 필연적이다(Open Source is inevitable)"라는 문구로 더 넓은 움직임을 요약했습니다.
- Claude 서비스 중단 및 게이팅 반발: @ratlimit, @theo, @Yuchenj_UW는 가동 시간과 구독 경제학을 주류 엔지니어링 불만으로 만들었습니다.
- OpenAI 거버넌스 조사: @RonanFarrow와 @ohryansbelt는 그날의 가장 큰 기술 관련 기업 거버넌스 스토리를 주도했습니다.
- Anthropic 컴퓨팅 규모: @AnthropicAI가 수 기가와트 TPU 용량을 발표하고 @AnthropicAI가 300억 달러의 연간 매출을 언급한 것은 프론티어 연구소 규모의 가장 명확한 신호 중 하나였습니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Gemma 4 모델 출시 및 벤치마크

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-gemma-4-crosses-2-million&utm_source=paywall-free-trial&utm_medium=web&utm_content=193410041&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-gemma-4-crosses-2-million&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
