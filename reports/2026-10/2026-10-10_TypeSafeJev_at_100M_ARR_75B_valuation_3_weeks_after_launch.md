# TypeSafe/Jev at >$100M ARR, $7.5B valuation 3 weeks after launch

**원문 URL**: https://www.latent.space/p/ainews-typesafejev-at-100m-arr-75b
**번역일**: 2026-10-10 12:28
**발행일**: 2026-10-10

---

[AINews] TypeSafe/Jev, 출시 3주 만에 >$100M ARR, $7.5B 가치 달성

### 와우.
Oct 10, 2026Share 아래 AINews X 요약 섹션에서 보시듯이, 전 세계 모든 사람이 Jev API를 클론했지만, 오직 한 회사만이 이 카테고리를 만들 수 있습니다. TypeSafe는 "Series AI"를 발표했으며, Sequoia는 그들이 첫 주에 100M ARR을 돌파했다고 "유출했습니다".

![X avatar for @CompleteSkeptic](https://pbs.substack.com/profile_images/1650708125685800960/7k6r0UZg.jpg)
회의론과 여론 조작(astroturfing)에 대한 비난이 있지만, 저희 Jev 팟이 100% 진정성이 있었다는 점이 분명하기를 바랍니다.
> 2026년 10월 8일-10월 9일 AI 뉴스입니다. 저희는 12개의 subreddit, 544개의 Twitter를 확인했으며, 더 이상의 Discord는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter 요약
결정 모델이 제품 카테고리로 부상하다
- 패턴: 여러 벤더들이 같은 날 "결정" 모델을 출시했습니다. 이 모델들은 자유 텍스트 대신 단일 포워드 패스(forward pass)로 타입이 지정된 답변(확률, 목록에서 선택, 점수)을 반환합니다. Jev는 모두가 벤치마크하는 기준점이며, @scaling01은 이 포맷이 얼마나 빠르게 확산되었는지 언급했습니다.
OpenAI Decisions API: 세 가지 요청 타입: 조건이 참일 확률, 목록에서 선택, 또는 레벨에 대한 점수입니다. 텍스트와 이미지를 모두 받으며, GPT-6 Luna에서 실행됩니다. 출력 요금 없이 M 입력 토큰당 $0.10의 비용이 들고, OpenAI 자체 수치에 따르면 "최대 10배 더 빠릅니다" (@LearnOpenCV).
Microsoft-Decision-1: LLM 심사관 및 과학적 가설 스크리닝을 위해 포지셔닝되었습니다. 초기 평가자는 결정 모델이 여전히 일관성과 복잡한 결정에서 어려움을 겪는다고 말합니다 (@omarsar0).
Perplexity pplx-decider-v1.1-27b: 1,071개 사례에서 Decision Bench 최고 정확도 94.5%를 달성했다고 주장하며, 1K 결정당 $0.017의 비용이 듭니다 (@perplexitydevs).
Cloudflare clef: 새로운 clef-omni는 오디오, 비디오, 이미지 및 텍스트를 받습니다. clef-flash는 이제 Jev보다 저렴하며, clef 전체적으로 약 2배 더 빠릅니다 (@michellechen). 가중치는 Hugging Face에 있습니다.
Liquid d1: 이제 Vercel AI Gateway에서 사용할 수 있으며, 분류(classify), 라우팅(route) 및 점수 매기기(score) 작업에 대한 비전 지원을 제공합니다 (@vercel_dev).
- 서빙 및 라우팅: vLLM Semantic Router의 Decision 2.0은 단일 입력에 대한 여러 질문에 대해 한 번의 패스로 옵션별 확률과 함께 답변합니다 (@vllm_project). LangSmith는 Jev를 모든 트레이스(trace)에서 난이도와 정확성에 대한 별도의 타입이 지정된 답변을 반환하는 심사관으로 사용합니다 (@hwchase17).
- 직접 학습시키기: Unsloth는 8GB VRAM에서 Qwen3.5-4B를 결정 모델로 전환하는 무료 노트북을 출시했습니다 (@UnslothAI). Qwen3.5-0.8B에 대한 워크스루(walkthrough)는 60단계에서 정확도가 37%에서 65%로 상승했으며, 4GB에서 약 10분 소요되었다고 보고합니다 (@akshay_pachaar).
- 하네스(harness)가 이를 원하는 이유: 많은 에이전트 단계는 생성(generation)보다는 예/아니오 호출입니다. LangChain은 각 작업을 가장 저렴하고 적절한 모델로 라우팅함으로써 작업당 Open SWE 중앙값 비용을 64% 절감했다고 말합니다 (@hwchase17).
- 관련 연구: Apple/CMU의 "Selection-based Structured Reasoning (SSR)"은 에이전트 내부에 동일한 아이디어를 적용합니다 (@ZhihuFrontier).
방법: KV-cache를 공유하는 하나의 배치 포워드 패스(batched forward pass)에서 6가지 자연어 전략이 길이 정규화된 로그-우도(log-likelihood)로 점수 매겨집니다.
결과: 턴당 추론 레이턴시(latency)는 90% 이상 감소하지만, 질문당 엔드투엔드 레이턴시는 28–54%만 감소합니다. GRPO가 적용된 Qwen3-VL-4B에서 평균 성공률은 61.37%이며, TAPO+GSPO 기준선은 61.25%입니다.
멀티 에이전트 오케스트레이션 및 코딩 도구
- Claude Managed Agents 동적 워크플로우 (공개 베타): 리드 에이전트가 단계별 계획을 작성하고, 실행당 최대 1,000개의 에이전트에 분산시킨 다음, 결과를 병합합니다. multiagent_20261001로 활성화됩니다 (@ClaudeDevs, config).
비용 경고: Anthropic은 토큰 사용량이 높을 수 있으므로 범위가 지정된 작업부터 시작할 것을 권고합니다 (guidance).
Claude Code Projects: 대기자 명단에 있던 모든 Pro 및 Max 사용자가 승인되었습니다. 각 프로젝트는 병렬 스레드로 작업을 실행하며 (@ClaudeDevs), 세션은 이제 로컬에서 실행될 수 있습니다 (@gem_ray).
Opus 5.5 fast mode: 출시되었지만, 사용 크레딧에 따라 요금이 부과되며 구독에는 포함되지 않습니다 (@theo).
- 에이전트 팀이 효과가 있을까요?: Vals AI는 Vibe Code Bench에서 GPT-6 Sol과 Opus 5.5를 단독으로 또는 팀으로 실행했습니다 (@ValsAI).
결과: 팀은 1.8–5.1배 더 많은 비용이 들었습니다. 중간 노력(medium effort)의 Sol만이 7.3점 향상되어 크게 개선되었습니다.
행동: Sol은 아키텍처 라인을 따라 병렬로 위임했습니다. Opus는 순차적인 웨이브(sequential waves)를 실행하여 최대 노력(max effort) 시 앱당 약 6.8개의 서브 에이전트와 약 1,140개의 서브 에이전트 도구 호출에 도달했지만, 유의미한 이득은 없었습니다 (details).
- Prime Agent가 Rust로 자체 재작성: 2주 동안 2,000개 이상의 에이전트 무리가 10K개 이상의 샌드박스와 200B개 이상의 GLM-5.3 토큰을 사용했습니다. 그 결과, 사용 가능한 입력에 약 13배 더 빠르게 도달하고 시작 메모리를 83% 덜 사용합니다 (@PrimeIntellect). 함께 제공된 에세이는 컨텍스트 제한이 필연적으로 무리(swarms)로 이어진다고 주장합니다 (essay).
- Codex 업데이트:
Windows 샌드박스: Microsoft Execution Containers (MXC)를 기반으로 구축된 새로운 모드는 더 빠른 설정, 네트워크 적용 및 세분화된 파일 제어를 제공합니다 (@OpenAIDevs).
Composer 예측: Codex는 이제 다음 메시지를 제안하며, Pro 사용자에게만 베타로 제공됩니다 (announcement). 일부 사용자는 Pro 전용 제한을 비판합니다 (@Angaisb_).
신뢰성: 하루 종일 지속되는 서비스 중단에 대한 불만이 있었습니다 (@dzhng).
여론: DHH는 GPT-6.1 Sol이 Claude보다 Codex를 자신의 주요 도구로 만들었다고 말합니다 (@dhh).
- Devin과 Grok Bot: Devin은 이제 관리되는 Devin들의 트리를 생성할 수 있으므로, 실제 소요 시간(wall time)은 합계가 아닌 가장 느린 브랜치를 추적합니다 (@devindevelopers). Devin은 또한 GPT 사용을 위한 개인 ChatGPT 플랜을 받습니다 (@cognition). 별도로, Grok Bot은 가입 및 스케줄링을 위한 자체 이메일 주소를 얻습니다 (@bot).
모델 출시 및 독립 평가
- Qwen-Image-2.1-Turbo (오픈 웨이트): 7B Qwen-Image-2.1의 가속화된 체크포인트입니다. 8단계 2K 생성 및 자연어 편집을 수행하며, Diffusers QwenImage21Pipeline을 통해 로드되고, Pro 및 Turbo API와 함께 출시됩니다 (@Alibaba_Qwen).
- StepFun Step 5 Preview: 총 600B, 활성 27B의 희소 MoE 모델로, 1M 컨텍스트와 비전을 지원합니다 (@omarsar0).
결과: Hermes Index에서 33.89점을 기록하여 GPT-6 Luna와 일치하며, Nous Portal에서 일주일 동안 무료로 제공됩니다 (@NousResearch).
가용성: 사용량을 측정하는 OpenRouter Trending에서 1위를 차지했습니다 (품질이 아님) (@kimmonismus). 오픈 웨이트는 10월 15일에 출시될 예정입니다. 최대 출력은 64K 토큰으로 수정되었습니다 (correction).
- Upstage Solar Mini 4: 3B 활성, 524K 컨텍스트 및 208 tok/s를 가진 35B MoE입니다. AAII 점수 24점은 3B 활성 모델 중 최고이며, Nemotron 3 Ultra와 1점 차이입니다. Cline에서 무료로 제공됩니다 (@cline).
- Gemini 4 Argon: DeepSWE v1.1에서 77.9%를 기록하여 Opus 5.5의 74.2%와 비교됩니다. Fairwind Program 방어자 650명 이상에게 M 토큰당 $2/$10의 가격으로 먼저 출시됩니다 (@dl_weekly).
신호: Antigravity에서 추론 노력 선택기(reasoning-effort selectors)가 나타났으며 (@testingcatalog), Logan Kilpatrick은 "Argon이 오고 있다"고 말합니다 (@OfficialLoganK).
미확인: Business Insider는 내부 "Carbon" 체크포인트가 코딩에서 Opus 5.5에 근접한다고 보도합니다.
- 음성 모델: HeyGen Voice는 Artificial Analysis Controlled Voice TTS 아레나에서 ELO 1,201로 1위를 차지했으며, 1M 문자당 $30, 초당 40문자의 속도를 제공합니다 (@ArtificialAnlys). Whistle은 Whisper base에 필적한다고 알려진 16.9MB 온디바이스 STT 모델입니다 (@victormustar).
- 멀티턴 이미지 편집: Artificial Analysis는 30개의 연속적인 편집을 연결했습니다 (@ArtificialAnlys).
결과: Ideogram 4.5와 FLUX 3는 로컬에서 편집하며, 작은 편집에서는 이미지의 95% 이상을 그대로 둡니다. GPT Image 2.5 Sunburst는 매 턴마다 프레임의 대부분을 다시 렌더링하여 약 20%만 변경되지 않은 채로 유지하므로, 드리프트(drift) 현상이 발생합니다. Nano Banana 2.1은 점차 어두워집니다.
- OCR 벤치마크: Roboflow의 새로운 벤치마크는 48개 모델을 다루며, GPT-6 Astra가 텍스트 로컬라이제이션(text localization)을 선도합니다 (@skalskip92). Datalab의 OmniParseBench는 90개 언어에 걸쳐 16K개의 테스트를 포함하며, 자체 모델은 1위를 차지하지 못했습니다 (@VikParuchuri).
- 아레나 요약: Claude Haiku 5.5는 WebDev에서 $0.10/$0.50로 30위를 기록했으며, GPT-6 Luna와 가격이 같으면서도 6점 더 높은 점수를 받았습니다. Mistral Large 4는 Agent Arena에서 43위에 있습니다 (@arena). ARC-AGI-3에서는 59.17%의 새로운 최고 점수가 기록되었습니다 (@arcprize).
연구, 학습 및 인퍼런스 시스템
- vLLM과 SGLang on Vera Rubin: vLLM은 AgentX에서 동일한 상호작용성으로 MiniMax M3에서 GB200 처리량(throughput)이 7.8배 이상 증가했다고 보고합니다. 이는 초기 결과입니다 (@vllm_project).
기술: Locality-aware MoE는 CUDA 13.4 로컬리티 도메인(locality domains)을 사용하여 각 SM이 로컬 HBM만 읽도록 하며, 이는 MoE 디코드를 최대 1.2배 더 빠르게 만듭니다 (details).
SGLang: 128K 컨텍스트에서 FP8 MLA를 최대 20% 더 빠르게 하며, 디코드 단계당 276개의 론치(launch)를 제거하는 MoE 테일 퓨전(tail fusion)을 통해 5.9%의 엔드투엔드 이득을 얻습니다 (@sgl_project).
SemiAnalysis 주장: 미리 보기 InferenceX 제출은 GB300 대비 기가와트당 3.2배의 이익과 달러당 최대 10배의 성능을 보여줍니다 (@SemiAnalysis_).
- TRL v1.15: 이제 퓨즈드 LM 헤드(fused LM head)가 기본적으로 활성화되어 전체 로짓 텐서(logits tensor)를 구체화하는 것을 방지합니다 (@LysandreJik).
결과: Gemma 3 1B에서 GRPO 시퀀스 길이는 28K에서 114K로, DPO는 10K에서 59K로 증가합니다. 8K에서의 피크 메모리는 52–82% 감소하며, 학습은 약 11% 더 빨라집니다.
- 데이터 및 사후 학습 서비스:
Datology Curation Studio: 30B MoE를 위해 39개의 오픈 데이터셋에서 6배의 컴퓨팅 승수(compute multiplier)를 주장합니다 (@pratyushmaini). 또한 $450K로 학습된 Thomson-1이 GPT-5.6 Sol을 정면 대결에서 이겼다고 인용합니다 (@arimorcos).
Tinker: 최대 70%의 가격 인하, 긴 컨텍스트가 짧은 컨텍스트와 동일하게 가격이 책정되며, GLM-5.3-Flash 및 DeepSeek-v4.1-Flash가 추가되었습니다 (@tinkerapi).
- DeepSeek 주기적 약점: ByteDance Seed는 리트리벌(retrieval)이 토큰이 압축 스트라이드(compression stride)에 상대적으로 어디에 위치하는지에 따라 달라진다는 것을 발견했습니다 (@ZhihuFrontier).
증거: 이 패턴은 RoPE 또는 학습된 게이트(learned gates) 없이도 지속되며, 스트라이드 길이(stride length)를 추적합니다.
해석: V4.1의 스트라이드 2는 이 효과를 줄이지만 제거하지는 못합니다.
- 에이전트 연구:
에이전트 가소성(Agent plasticity) (Meta): 학습 비용당 보유 이득(held-out gain)을 측정합니다. 최고의 성능을 보이는 에이전트가 가장 효율적인 학습자는 아닙니다 (@omarsar0).
MIMESIS: 행동 충실도(behavioral fidelity)에서 Opus 5를 13.4점 앞서는 9B 사용자 시뮬레이터입니다 (@dair_ai).
기반 모델 선택 (NVIDIA): 기반 모델이 "결정적인 편집(decisive edit)"을 재현할 수 있는지 여부에 따라 체크포인트를 순위 매깁니다. 이는 사후 학습된 SWE-bench Verified 점수를 추적하는 신호입니다 (@dair_ai).

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 동안 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-typesafejev-at-100m-arr-75b&utm_source=paywall-free-trial&utm_medium=web&utm_content=219685324&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-typesafejev-at-100m-arr-75b&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
