# NVIDIA Cosmos 3, Nemotron 3 Ultra, and RTX Spark

**원문 URL**: https://www.latent.space/p/ainews-nvidia-cosmos-3-nemotron-3
**번역일**: 2026-06-02 06:19
**발행일**: 2026-06-02

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] NVIDIA Cosmos 3, Nemotron 3 Ultra, and RTX Spark

### 젠슨이 엄청난 승리를 거두었습니다.
Share오늘 팟캐스트 게스트는 1년여 전 NVIDIA Cosmos의 리더였으며, 비디오 생성(videogen) 및 월드 모델 학습에 대해 논의했습니다. 이에 걸맞게, Cosmos 3가 오늘 출시되었으며, 언어, 이미지, 비디오, 오디오 및 액션을 Mixture-of-Transformers 아키텍처로 통합했습니다. 이 아키텍처는 오토리그레시브 추론 모델(reasoner)과 확산 생성 모델(diffusion generator)을 다음과 같이 결합합니다:
- base Nano (16B: 8B 추론 모델 타워 + 8B 생성 모델 타워)
- Super (64B: 32B 추론 모델 타워 + 32B 생성 모델 타워) 모델, 그리고
- Text2Image 및 Image2Video를 위한 Super 파인튜닝 모델은 이제 Nano Banana 2 바로 아래의 새로운 SOTA 오픈 웨이트 이미지 생성(imagegen) 및 비디오 생성(videogen) 모델입니다.

![X avatar for @liu_mingyu](https://pbs.substack.com/profile_images/2002841783735042048/07JFOmTh.jpg)
대만 Computex에서 젠슨은 Nemotron 3 Ultra를 통해 열기를 더했습니다. 이 모델은 550B-A55B 규모의 놀랍도록 효율적이고 빠른 오픈 웨이트 LLM으로, 새로운 미국 SOTA를 달성했습니다:

![Image](https://substack-post-media.s3.amazonaws.com/public/images/f6685277-4569-4135-92cb-e7a4645246125_4096x2732.jpeg)
마지막으로, RTX Spark 개인용 컴퓨터 1 페타플롭 슈퍼칩이 Microsoft, OpenClaw, Hermes Agent를 론칭 파트너로 하여 미리 공개되었습니다 (여기에서 좋은 분석을 볼 수 있습니다).

![X avatar for @NVIDIARTXSpark](https://pbs.substack.com/profile_images/2061303426479431680/BDJQPK6Q.jpg)
> 2026년 5월 30일~6월 1일 AI 뉴스입니다. 저희는 12개의 subreddits, 544개의 Twitters 계정을 확인했으며, 더 이상의 Discords 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
NVIDIA Cosmos 3, Nemotron 3 Ultra, 그리고 오픈 물리 AI(Physical AI)를 향한 추진
- NVIDIA의 오픈소스 주간: NVIDIA는 Cosmos 3(물리 AI를 위한 옴니모달 월드 모델의 오픈 패밀리)와 Nemotron 3 Ultra(일부 포스터들이 현재까지 가장 강력한 미국 오픈 모델이라고 칭한 550B 오픈 웨이트 모델) 발표로 오픈 모델 논의를 주도했습니다. Cosmos 3는 가중치, 코드, 데이터셋, 파인튜닝 레시피를 포함하는 풀스택 릴리스로 구성되었으며, NVIDIA는 Runway를 포함한 파트너들과 함께 Cosmos Coalition을 출범하여 월드 모델을 위한 오픈 생태계를 구축했습니다. @NVIDIAAI ecosystem context, @runwayml coalition announcement, @kimmonismus Cosmos thread, @ClementDelangue on NVIDIA’s HF footprint.
- Cosmos 3가 기술적으로 중요했던 이유: 로봇 공학적 수사(rhetoric)를 넘어, 더 구체적인 내용은 Cosmos 3가 오토리그레시브 추론 모델과 확산 생성 모델을 결합하는 단일 Mixture-of-Transformers 디자인으로 언어, 이미지, 비디오, 오디오 및 액션을 통합한다는 것이었습니다. Artificial Analysis는 Cosmos 3가 Text-to-Image 및 Image-to-Video 리더보드 모두에서 오픈 웨이트 모델 중 1위를 차지했다고 밝혔으며, 생성 모델이 구조화된 JSON 프롬프트를 사용하고 외부 프롬프트 업샘플링 하네스 또는 자체 추론 모델 브랜치에 의해 구동될 수 있다고 언급했습니다. 별도로, NVIDIA의 하드웨어 + 소프트웨어 추진은 OpenMDW 프레임워크 채택 및 fal과 같은 플랫폼에서의 파트너 생태계 통합으로 확장되었습니다. @ArtificialAnlys, @fal.
- Nemotron 3 Ultra에 대한 반응: Nemotron 3 Ultra에 대한 커뮤니티 반응은 새로운 오픈 릴리스치고는 이례적으로 강력했습니다. 포스터들은 Nemotron 3 Ultra의 기능과 서빙 특성을 모두 강조했으며, 일부 오픈 평가에서 이미 최고 성능을 보이고 있으며, 특정 설정에서는 300+ tok/s로 서빙될 수 있다고 주장했습니다. 이는 대규모 DeepSeek/Kimi 클래스 모델보다 훨씬 빠른 속도입니다. @scaling01, @ctnzr, @caspar_br. 또한 Nemotron이 Kimi K2 / DeepSeek V4와 같은 다른 모델들보다 희소성(sparse)이 낮은 것으로 보인다는 기술적 논의도 있었습니다. 대략 활성 파라미터가 ~10% 대 ~3%로, 이는 경제성과 동작 방식 모두에 영향을 미칠 수 있습니다. @eliebakouch.
MiniMax M3, Qwen3.7-Plus, JetBrains Mellum2가 오픈 에이전트 모델 분야를 확장합니다
- MiniMax M3의 출시가 그날의 가장 큰 모델 릴리스였습니다: M3는 1M 컨텍스트, 네이티브 멀티모달리티, 그리고 경쟁력 있는 에이전트 벤치마크를 갖춘 오픈 웨이트 멀티모달 에이전트/코딩 모델로 소개되었습니다. 론칭 파트너들 사이에서 반복된 주요 수치는 SWE-Bench Pro 59.0%, Terminal Bench 2.1 66.0%, MCP Atlas 74.2%였습니다. @MiniMax_AI, @PBDTokenRouter, @kimmonismus. 여러 인프라 벤더들이 출시 당일(day-0) 지원을 제공했습니다 — Novita, Vercel AI Gateway, Cloudflare AI Gateway, OpenClaude, Flowith 등 — 이는 이례적으로 빠른 생태계 채택을 시사합니다. @MiniMax_AI on Novita, @rauchg, @gitlawb.
- 벤치마크와 실제 경험은 엇갈렸습니다: M3는 프론트엔드 생성, 시각/게임 작업, 그리고 가격 대비 성능 면에서 찬사를 받았습니다. 나란히 진행된 데모에서는 강력한 원샷 UI/게임 결과물과 Next.js 에이전트 평가에서 주목할 만한 벤치마크 순위를 보여주었습니다. @notjazii, @lostinlatencyX, @rauchg. 그러나 여러 평가자들은 높은 토큰 소비량, 장황한 자체 검사 루프, 그리고 긴 작업에서 가끔 발생하는 요구사항 이탈을 보고했으며, 이는 M3가 "품질 우선, 효율성 나중" 모델에 가깝다는 인상을 주었습니다. @ZhihuFrontier review, @teortaxesTex skepticism.
- Qwen3.7-Plus: Alibaba는 GUI 및 CLI 작업, 시각적 추론, 코딩, 검색 증강 QA를 통합하는 멀티모달 인터랙티브 하이브리드 에이전트인 Qwen3.7-Plus를 출시했습니다. 이 모델은 Alibaba Cloud Model Studio를 통해 API로 이용 가능하며, Cline과 같은 도구에 빠르게 추가되었습니다. @Alibaba_Qwen launch, @cline. 이번 출시는 아시아의 오픈 지향(open-ish) 연구소들이 더 이상 "단순한 챗 모델"이 아닌, 완전한 에이전트 기능을 갖춘 멀티모달 시스템을 출시하고 있다는 추세를 강화합니다.
- JetBrains Mellum2: JetBrains는 약 11T 토큰으로 학습되고 RLVR로 사후 학습된, 2.5B 활성 파라미터를 가진 12B MoE 모델인 Mellum2를 출시했습니다. 이 모델은 base / SFT / RL 체크포인트와 기술 보고서와 함께 제공됩니다. @nv_pavlichenko, @jetbrains. 이 모델의 의도된 틈새시장은 특히 흥미롭습니다: 라우팅, RAG, 서브 에이전트, IDE 사용을 위한 초저 레이턴시 인퍼런스이며, vLLM에 즉시 통합되었습니다. @vllm_project. 이는 벤치마크를 쫓는 프론티어 릴리스라기보다는 "개발자 워크플로우를 위한 작고 빠른 오픈 모델"이라는 진지한 시도로 보입니다.
에이전트, 샌드박스, 메모리, 검색이 실제 제품 표면이 되고 있습니다
- 스택이 모델 호출에서 에이전트 런타임으로 전환되고 있습니다: 여러 출시 모델들은 이제 주요 엔지니어링 레버리지가 모델 자체보다는 하네스에 있다는 생각에 수렴했습니다. Perplexity의 "Search as Code"가 가장 명확한 예시입니다. 반복적인 검색 도구 호출 대신, 모델이 검색 SDK에 대해 Python 코드를 작성하여 사용자 지정 랭킹 파이프라인, 인덱스에 대한 맵리듀스, 배치 처리, 집계, 그리고 낮은 토큰 오버헤드를 가능하게 합니다. Perplexity는 이 아키텍처를 통해 내부 WANDR 벤치마크에서 0.152에서 0.386으로 점프했다고 보고했습니다. @perplexity_ai, @AravSrinivas.
- 관리형 에이전트 + 샌드박스가 표준이 되고 있습니다: Google은 Gemini API에서 관리형 에이전트(Managed Agents)를 상세히 설명했습니다. 여기서는 단일 API 호출로 추론하고, 코드를 작성/실행하며, 파일을 관리하고, 호스팅된 Linux 샌드박스 내에서 작동하는 에이전트를 실행할 수 있습니다. @_philschmid, @GoogleAIStudio. LangChain은 Deep Agents, Context Hub, LangSmith Sandboxes/Engine과 관련하여 유사한 아이디어를 추진하며, 영구적인 컨텍스트, 에이전트 라이프사이클 툴링, 자동화된 실패 분류를 강조했습니다. @LangChain, @hwchase17.
- 메모리는 여전히 부족한 기본 요소입니다: 반복적으로 제기된 불만 중 하나는 방대한 컨텍스트 윈도우가 여전히 세션 간 메모리 문제를 해결하지 못한다는 것이었습니다. HydraDB에 대한 한 스레드에서는 "RAG + 수동 컨텍스트 주입"이 메모리로 잘못 불리고 있으며, 실제 영구적인 세션 지식은 여전히 제대로 제공되지 않고 있다고 주장했습니다. @kimmonismus. 관련 연구 스레드들은 AdaCoM과 같은 재사용 가능한 컨텍스트 관리 정책을 지적했습니다. AdaCoM은 RL을 통해 별도의 LLM을 학습시켜 고정된 에이전트의 컨텍스트를 가지치기/보존합니다. @dair_ai.
- 보안은 엔터프라이즈 에이전트의 핵심 문제입니다: Microsoft Security Intelligence는 90개 이상의 redhat-cloud-services 패키지에 영향을 미치는 주요 npm 공급망 침해에 대한 주목할 만한 경고를 발표했습니다. 여기에는 npm/GitHub/AWS/SSH 자격 증명을 훔치는 자가 증식 웜이 포함됩니다. @MsftSecIntel. 동시에 엔터프라이즈 에이전트 벤더들은 NVIDIA OpenShell 및 LangChain의 샌드박스 기조연설 논의를 포함하여, 샌드박싱, 런타임 격리, 보안 스택 통합을 배포를 위한 전제 조건으로 강조했습니다. @shannholmberg, @LangChain.
Codex, Claude Code, 그리고 경쟁적인 코딩 에이전트 경쟁
- OpenAI가 Codex를 더 많은 곳으로 확장했습니다: OpenAI는 프론티어 모델과 Codex가 이제 AWS / Amazon Bedrock에서 일반적으로 사용 가능하며, 기존 AWS 보안/규정 준수 워크플로우 내에서 OpenAI 기능을 원하는 기업들을 직접적으로 겨냥한다고 발표했습니다. @OpenAI, @OpenAIDevs. OpenAI는 또한 스레드, 턴, 스트리밍, 재개, 이미지, 샌드박스 제어를 지원하는 Codex Python SDK를 출시했으며, Bedrock 기반 Codex 워크플로우에 대한 지원도 추가했습니다. @reach_vb, plus support for Bedrock-backed Codex workflows @reach_vb on Bedrock config.
- Claude Code에서 실제 운영(ops) 사고가 발생했습니다: Anthropic은 일부 Opus 4.8 세션이 너무 많은 병렬 서브 에이전트/도구 호출을 생성하여 예기치 않게 사용량을 소모하는 버그를 수정한 후, Pro 및 Max 사용자의 5시간 및 주간 속도 제한을 재설정했습니다. @ClaudeDevs, follow-up. 이는 코딩 에이전트 제품 품질이 단순히 원시 모델 IQ뿐만 아니라 오케스트레이션 동작에 의해 점점 더 많이 결정된다는 점을 상기시켜 줍니다.
- 코딩 모델 간의 행동 차이는 여전히 중요합니다: 개발자들은 ProgramBench 및 WeirdML과 같은 벤치마크에서 GPT, Claude 및 기타 모델 간의 큰 질적 차이를 강조했습니다. Opus는 때때로 점수 극대화보다 탐색을 선호하거나 벤치마크별 특이점을 보였습니다. @OfirPress, @htihle. 별도의 긴 스레드에서는 최신 Claude Opus 4.6–4.8 변형 모델이 코딩 외 도메인에서 그럴듯하지만 허구적인 개념을 조작할 수 있으며, 이는 일반적인 환각보다는 진실성/정렬(alignment) 퇴행 가능성을 시사한다고 주장했습니다. @distributionat.
인프라, 하드웨어, 로컬 AI 시스템
- NVIDIA가 PC 시장을 노리고 있습니다: 가장 많이 논의된 하드웨어 출시는 NVIDIA/Microsoft의 "개인 AI 컴퓨터"인 RTX Spark였습니다. 이 컴퓨터는 Grace + Blackwell을 기반으로 구축되었으며, 최대 128GB의 통합 메모리와 1 PFLOP FP4 성능을 주장합니다. 핵심 전략적 해석은 다음과 같습니다: NVIDIA는 더 이상 가속기만 판매하는 것이 아니라, Apple Silicon, x86 PC, Qualcomm과 동시에 경쟁하는 엔드투엔드 로컬 AI 시스템을 제공하고 있다는 것입니다. @kimmonismus, @swyx.
- 클러스터/네트워킹 업데이트: 데이터센터 측면에서는 Lambda가 NVIDIA Quantum-X InfiniBand Photonics Q3450-LD 스위치를 최초로 채택하여, 대규모 AI 클러스터에서 네트워크 전력 및 장애를 줄이기 위해 코패키지드 옵틱스(co-packaged optics)를 추진하고 있다고 밝혔습니다. @LambdaAPI. OpenAI는 또한 폐쇄 루프 냉각을 사용하고 인력/교육 약속과 결합된, 계획된 1GW 데이터센터인 Stargate Michigan을 발표했습니다. @OpenAINewsroom.
- 로컬 오픈 모델 툴링이 빠르게 개선되고 있습니다: MLX-VLM v0.6.0 릴리스는 투기적 디코딩(speculative decoding), Anthropic 스타일 및 응답 스타일 API, 도구 호출, 많은 새로운 멀티모달 모델 지원, 그리고 Apple 기기를 "진정한 로컬 에이전트 머신"으로 전환하겠다는 명확한 목표를 가진 이미지/오디오 기능을 추가하는 등, 더욱 실질적인 로컬 인퍼런스/툴링 업데이트 중 하나였습니다. @Prince_Canuma. 이는 로컬 NVFP4 MoE 서빙을 위한 DGX Spark + vLLM 실험 증가와 잘 어울립니다. @vllm_project.
인기 트윗 (참여도 기준, 기술적 관련성 필터링)
- Anthropic의 IPO 경로: Anthropic은 SEC에 S-1 초안을 기밀리에 제출했으며, 검토 후 IPO 가능성을 열었습니다. @AnthropicAI.
- Claude Code 사용량 사고: Opus 4.8 병렬 서브 에이전트/도구 호출 버그로 인해 과도한 할당량 소모가 발생한 후, Anthropic은 사용자 속도 제한을 재설정했습니다. @ClaudeDevs.
- Qwen3.7-Plus: Alibaba는 GUI/CLI 작업, 코딩, 시각적 작업을 아우르는 멀티모달 에이전트 모델을 출시했습니다. @Alibaba_Qwen.
- Bedrock의 OpenAI: OpenAI 모델과 Codex는 이제 엔터프라이즈 워크플로우를 위해 Amazon Bedrock을 통해 이용 가능합니다. @OpenAI.
- ARC-AGI-3 움직임: Claude Opus 4.8은 ARC-AGI-3에서 1.5%로 새로운 SOTA를 기록했습니다. 이는 절대적인 수치로는 여전히 작지만, 해당 벤치마크에서는 의미 있는 도약입니다. @arcprize.

---

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-nvidia-cosmos-3-nemotron-3&utm_source=paywall-free-trial&utm_medium=web&utm_content=200231944&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-nvidia-cosmos-3-nemotron-3&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
