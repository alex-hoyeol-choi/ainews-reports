# Sora 2: new video+audio model and OpenAI's first Social Network | AINews
**원문 URL**: https://news.smol.ai/issues/25-09-30-sora2
**번역일**: 2025-10-06 00:04:13

## 📋 메타데이터
- **발행일**: 2025-09-30T05:44:39.731Z
- **설명**: **Sora 2** released with improvements on physical world video modeling and a new "character consistency" feature allowing real-world element injection from a single video. The model powers a new **Sora social network** app with profiles, DMs, and viral videos, emphasizing user control over likeness use. **OpenAI** employees are actively experimenting with the model. Meanwhile, **Anthropic** launched **Claude 4.5 Sonnet** with enhanced intelligence, token efficiency, and agentic tool use, outperforming some competitors and closely tracking **GPT-5-high** on benchmarks. Ecosystem support includes LangSmith integration and strong coding/math benchmark results.

---

## 📰 번역된 내용

당신의 얼굴만 있으면 됩니다.

2025년 9월 29일-9월 30일 AI 뉴스입니다. 저희는 여러분을 위해 12개의 subreddit, 544개의 Twitter, 23개의 Discord (196개 채널, 7053개 메시지)를 확인했습니다. 절약된 예상 독서 시간 (분당 200단어 기준): 509분입니다. 저희의 새로운 웹사이트가 이제 전체 metadata 검색 기능과 과거 모든 이슈를 아름다운 vibe coded 방식으로 제공하며 공개되었습니다. 전체 뉴스 분석은 https://news.smol.ai/ 에서 확인하시고, @smol_ai 로 피드백을 보내주세요!

Sora 발표 이후 1.5년, Sora.com이 대중에게 공개된 지 10개월, Meta가 논란의 Vibes 앱을 발표한 지 4일이 지난 오늘, Sora 2 (유출된 바에 따르면)가 좋은 반응과 함께 출시되었습니다 (HN 추천수 기준 약 7배 적음).

Sora 2는 Sora 1 시대의 비디오 모델에서 빠르게 발견되었던 모든 물리적 세계 문제점들에 대해 상당한 개선을 이루었습니다. 여기에는 체조 및 피겨 스케이팅 루틴도 포함됩니다.

블로그 게시물에서는 "implicit" 모델을 언급했습니다. 많은 이들이 Genie 연구를 통해 추측했던 것처럼 아직 "explicit world model"은 아닙니다. 하지만 비디오 게임과 브라우저 출력에 대한 훈련은 분명히 있습니다.

Veo 3가 몇 달 전부터 제공해 온 "native audio가 포함된 비디오" 기능 외에도, 한 가지 눈에 띄는 새로운 기능은 단일 데모 비디오를 통해 "실제 세계의 요소를 Sora 2에 주입"할 수 있는 능력입니다. OpenAI 직원들은 이 기능을 분명히 매우 즐기고 있습니다.

Sama는 개인 블로그 게시물에서 이를 "character consistency"라고 부릅니다.

이 기능과 모델은 이제 새로운 Sora iOS 앱 및 웹사이트 경험으로 제품화되었으며, 현재는 초대 코드를 통해서만 이용할 수 있는 "cameos" 기능으로 제공됩니다. 이 기능은 새로운 Sora social network가 작동하는 방식의 핵심입니다.

네, 저희는 문자 그대로의 "social network"임을 강조합니다. Sama가 올해 초 약속했던 것처럼, 새로운 Sora 앱에는 프로필, 팔로워 수, DM 기능이 있으며 이미 첫 번째 바이럴 비디오가 탄생했습니다.

팀 (및 전 멤버들)은 라이브 스트림에서 마련된 안전장치, 예를 들어 anti-doomscrolling timeout에 대해 설명하기 위해 많은 노력을 기울였습니다.

cameos는 모두 온보딩의 일부로 직접 업로드된 비디오이며, 다른 사람들이 당신의 모습을 사용하도록 (또는 사용하지 않도록) 권한을 설정할 수 있습니다. 특히, Sam Altman의 모습은 누구나 사용할 수 있습니다. 따라서 앞으로 며칠 동안 소셜 피드에서 Sam의 많은 deepfake를 보게 될 것입니다.

# AI 트위터 요약
Anthropic의 Claude Sonnet 4.5: 기능, 코딩 및 초기 평가
- Claude 4.5 Sonnet (200K ctx, 64K max output): Anthropic의 업그레이드는 Sonnet 4와 동일한 가격($3/$15 per 1M input/output)으로 더 높은 지능을 제공하며, "Thinking" 모드에서도 향상된 Token 효율성을 자랑합니다. Artificial Analysis의 독립적인 평가는 이를 GPT‑5-high 뒤에, Gemini 2.5 Pro 및 Grok 4 Fast 앞에 두었으며, 출력 Token 사용에 있어서는 여전히 매우 절약적입니다. 또한 이전 벤치마크보다 Agentic Tool 사용 및 Safety/Alignment 행동에서 더 큰 개선을 보였다고 언급했습니다 (thread). ARC‑AGI에서 Sonnet 4.5는 GPT‑5를 면밀히 추적하며, 더 높은 Thinking Budget에서 성능이 의미 있게 확장됩니다 (@GregKamradt; commentary). 사용자들은 뛰어난 "State Management" 및 Context Compaction 기능을 보고하며, 이를 통해 긴 Agentic Workflow가 더욱 안정적으로 작동한다고 언급합니다 (@nickbaumann_; @skirano). Ecosystem 지원도 빠르게 이루어졌습니다: LangSmith Cost Tracking/Playground (@Hacubu), ARC Prize 결과 (@scaling01), 그리고 LiveBench 및 Deep Research Bench에서의 커뮤니티 측정에서 강력한 Coding/Math 순위를 기록했습니다 (1, 2).
- Claude Code 2 및 Agent Stack: Anthropic은 Claude Code v2, VS Code Extension 업데이트, Context Editing 및 Memory Tool을 출시했습니다 (launch roundup). Replit은 Sonnet 4.5가 Agent 3에서 안정적인 Code 편집 및 자율성을 향상시킨다고 보고합니다 (@pirroh). Anthropic은 또한 Agent 시스템을 위한 "Context Engineering" (Prompt Engineering을 넘어선)에 대한 Engineering Blog를 발행했습니다 (@AnthropicAI).
Zhipu의 GLM‑4.6 (Open Weights) 및 Agentic Coding 집중
- GLM‑4.6 출시 (MIT license): Zhipu는 GLM‑4.5 라인을 200K Context, 더 강력한 Coding, 향상된 Reasoning/Tool 사용 및 더 나은 Agent Task 성공률로 확장했으며, Trajectory당 Token 사용량은 4.5 대비 약 15% 감소했습니다. Zhipu는 CC‑Bench‑V1.1 (전체 Trajectory를 포함하는 74개의 실제 Agentic Coding Task)을 공개하여 GLM‑4.6이 Coding에서 Claude Sonnet 4와 거의 동등한 수준이며 국내 경쟁 모델들을 선도하고 있음을 보여주었습니다. 모든 Eval 상세 정보는 공개되어 있습니다 (@Zai_org, bench; analysis by @gm8xx8). Open Weights 및 API는 현재 사용 가능하며, HF/ModelScope 호스팅이 곧 제공될 예정입니다.
- Ecosystem 활용: OpenRouter (@OpenRouterAI), Yupp (@yupp_ai), YouWare (@YouWareAI), Roo Code (@roo_code), Cline (@cline), 및 Anycoder (@_akhaliq)에서 사용할 수 있습니다. 로컬 환경에서 MLX는 M3 Ultra에서 GLM‑4.6을 약 17 tok/s로 실행합니다 (5.5 bpw quant; 5.3K tokens) (@awnihannun).
최첨단 비디오 모델: Sora 2 출시 및 초기 비교
- OpenAI Sora 2 및 앱: OpenAI는 iOS 앱 (출시 시 미국/캐나다 초대 전용), Cameo 기능 (Consent Control, Watermark) 및 System Card와 함께 Sora 2를 출시했습니다. Android 및 API는 계획 중입니다. OpenAI는 향상된 Physics/Steerability 및 Audio를 갖춘 "World Simulation" 데모를 강조하면서도, Algorithmic Feed 및 Deepfake의 위험을 인정합니다 (product post, teaser, Sam Altman’s note). 반응은 엇갈립니다: 일부는 뛰어난 Realism/Consistency를 강조하고, 다른 일부는 Artifact를 지적하며 특정 경우 Google의 Veo 3가 경쟁력이 있다고 언급합니다 (pro, skeptic, physics demo).
- Luma Ray 3: Luma의 새로운 Ray 3는 Artificial Analysis의 T2V Video Arena에서 2위를 차지했으며, 반복적인 Chain-of-Thought Generation Loop 및 16-bit HDR 지원 (I2V/T2V 최대 10초 1080p)을 도입했습니다. API는 아직 제공되지 않습니다 (@ArtificialAnlys).
학습 효율성 및 후처리: Pretraining 중 FP4, QAT 및 RL
- NVFP4 (NVIDIA): 2단계 Scaling, RHT 및 Stochastic Rounding을 사용한 4-bit Pretraining은 10T Token으로 학습된 12B 모델에서 FP8 Baseline과 일치하는 성능 (MMLU‑Pro 62.58 vs 62.62)을 보여주며, 약 6.8배의 효율성과 약 50% 낮은 메모리를 약속합니다. Blackwell은 FP4 Matmul 및 필요한 Rounding Mode를 지원합니다 (paper/code, summary). 오픈소스 TE 지원은 진행 중입니다.
- Compute-Optimal QAT (Apple): Token/메모리를 고려한 Quantization-Aware Training과 Full-Precision 예산 책정을 위한 Scaling Law; Training Schedule에서 QAT를 일등 시민으로 계획하기 위한 실용적인 지침을 제공합니다 (@aldrmv, @awnihannun).
- RLP (NVIDIA): Reinforcement Learning Pre‑training은 Verifier가 없는 Web Text에 대한 Dense Information-Gain Reward를 통해 모델이 "예측하기 전에 생각하도록" 가르치며, 기본 모델 대비 상당한 성능 향상 (예: Math/Science Suite에서 Qwen3‑1.7B +19%, Nemotron‑Nano‑12B +35%)을 가져오고 Post‑training과 결합 시 더욱 증폭됩니다 (paper/blog).
사용자 학습 및 Agent 메모리
- RLHI (Meta): Reinforcement Learning from Human Interaction은 유기적인 사용자 대화 (사용자 안내 Rewrites 및 사용자 기반 Rewards)로부터 직접 학습하여, Personalization 및 Instruction Following에서 Baseline을 능가하면서도 표준 Benchmark 성능을 유지합니다 (@jaseweston, paper).
- ReasoningBank (Agents): 성공과 실패 모두에서 추출된 전략을 저장하여 Web/SWE Task에서 재사용 및 효율성을 개선하는 Memory System으로, 이전 Memory Method 대비 +34.2% 효율성 및 –16% Step 감소를 보고합니다 (tweet).
- 효율적인 Sequence Model: SWAX는 Sliding-Window Attention을 xLSTM 및 Stochastic Window Size와 결합하여 Short/Long Recall을 모두 향상시킵니다 (tweet). Diffusion LM의 경우, SparseD는 Sparse Attention (1.3–1.5배 더 빠르면서 거의 Lossless)을 제안하고, LLaDA‑MoE (Sparse MoE dLLM)는 더 작은 Active Param으로 Diffusion LLM 중 SOTA를 보고합니다 (SparseD, LLaDA‑MoE). 마지막으로, MobileLLM‑R1은 약 2T Token의 Curated Data와 표준 Post‑training을 통해 Sub‑billion Parameter Reasoning Model (950M)이 AIME 15.5를 달성하는 것을 보여줍니다 (tweet).
Agentic Coding 스택 및 인프라
- 로컬 및 호스팅 Agent Stack: AMD는 Cline + LM Studio를 사용한 로컬 "Vibe Coding"을 지지하며, 더 높은 RAM Tier를 위해 Qwen3‑Coder‑30B (4/8‑bit) 및 GLM‑4.5‑Air를 권장했습니다 (@cline). AI SDK는 이제 모든 HF 모델로 라우팅됩니다 (@nishimiya). Cursor 1.7은 Prompt Suggestion 및 조직 전체 규칙을 추가합니다 (@cursor_ai). Sim은 MCP Integration을 갖춘 완전 로컬, 오픈소스 Drag‑and‑Drop Agentic Workflow Builder를 출시했습니다 (thread).
- Codex vs Claude Code 운영 선택: Reverse‑Engineering 노트는 OpenAI Codex CLI의 Shell‑First Loop (Think→Tool→Observe), 오류 표면을 줄이는 Unified Diffs, 그리고 더 무거운 Tool Orchestration 대비 OS‑Level Sandboxing을 강조합니다 (analysis). 한편, GitHub MCP Registry 및 Claude Extension은 VS Code에서 계속해서 성숙해지고 있습니다 (@code, @gallabytes).

Periodic Labs: AI 과학자 + 자율 연구실
- Liam Fedus와 Doğuş Ekin이 이끄는 Periodic은 a16z가 주도하는 3억 달러 규모의 초기 투자 라운드를 유치하여 검증 가능하고 실험 중심적인 과학을 위한 AI 과학자와 자율 연구실을 구축하고 있습니다. 이들은 재료(예: 초전도체) 및 반도체 발전을 목표로 합니다. 팀에는 ChatGPT, GNoME, attention, MatterGen 및 확장된 자율 물리학 연구실(launch, a16z)을 개발한 경험이 있는 인력들이 포함되어 있습니다. 이들의 핵심 아이디어는 다음과 같습니다: 인터넷 텍스트는 유한하며, 진전을 위해서는 새롭고 신호 강도가 높은 실험 데이터와 폐쇄 루프 검증이 필요합니다.

---
가장 많이 참여한 트윗
- “Sound on.” @OpenAI의 Sora 2 티저 (~3.4만)
- @OpenAI의 Sora 2 출시 (~1.27만)
- “10am PT” @OpenAI의 출시 전 티저 (~6천6백)
- “We are launching a new app called Sora.” @sama (~6천7백)
- @OpenAI의 Sora 앱 데모 (~4천6백)
- “Built with Claude Sonnet 4.5” @alexalbert__의 챌린지 (~1천2백)
- Bolt v2 “vibe coding goes pro” @boltdotnew (~1천3백)
- @LiamFedus의 Periodic Labs 출시 (~2천9백)

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. 중국 AI 모델 출시: Qwen 로드맵 및 Hunyuan Image 3.0
- Alibaba가 Qwen 로드맵을 공개했습니다. 그 야심은 엄청납니다! (활동: 954): Alibaba의 Qwen 로드맵(이미지 속 슬라이드로 추정)은 공격적인 스케일링 목표를 제시합니다: 통합 멀티모달 모델; 컨텍스트 길이 1M → 100M Token; 파라미터 ~1T → 10T; 테스트 시 컴퓨팅 스케일링 64k → 1M; 그리고 데이터 10T → 100T Token—여기에 “규모 제한 없는” 합성 데이터 생성과 더 넓은 에이전트 기능(복잡성, 상호작용, 학습 모드)이 결합됩니다. 이는 중국의 대표적인 LLM 스택을 위한 “scaling is all you need” 전략을 전적으로 수용하고 있음을 시사합니다 (Qwen 프로젝트 참조: https://github.com/QwenLM/Qwen). 댓글 작성자들은 100M 컨텍스트에 경외감을 표하고, 오픈소스 상태를 유지할지에 대한 회의론, 그리고 1T 파라미터 이상의 모델을 로컬에서 실행하는 것에 대한 실질적인 우려(하드웨어 실현 가능성)를 표명했습니다.

로드맵에서 100M Token 컨텍스트 윈도우(슬라이드)를 언급하며, 실현 가능성에 대한 의문을 제기합니다. 단순한 Quadratic Attention은 100M Token에서 레이어당 약 1e14개의 Attention 스코어를 필요로 하며, 이를 저장하는 데만 수십에서 수백 TB가 소요되므로, Sparse/Linear Attention, Recurrence 또는 외부 메모리 기술을 요구할 것입니다. 심지어 그렇다 하더라도 KV-cache 증가(O(n))와 메모리 대역폭이 병목 현상이 되며, 실제 배포에서는 Windowed Attention과 Retrieval을 결합할 가능성이 높습니다.
여러 사람들이 더 큰 Qwen 체크포인트가 클로즈드 소스가 될 가능성을 지적하며, 이는 로컬 파인튜닝과 재현성을 제한할 것입니다. 이는 벤치마킹을 API 기반 평가로만 국한시키고 커뮤니티 최적화를 제약할 것입니다.
1T개 이상의 파라미터 모델을 로컬에서 실행하는 것에 대해: 밀집(dense) 1T 모델은 KV cache와 Activation을 제외하고도 FP16 가중치에만 약 2TB(INT8의 경우 약 1TB, 4-bit의 경우 약 0.5TB)가 필요하며, NVLink/InfiniBand를 통한 다중 노드 Tensor/Pipeline Parallelism이 필수적일 것입니다. 대조적으로, 예를 들어 총 1T 파라미터에 약 8/64개의 Expert가 활성화된 MoE 설계는 약 125B개의 활성 파라미터를 생성합니다. 4-bit에서는 약 62.5GB의 가중치이며 실제로 여러 GPU에 걸쳐 배포 가능하지만, 긴 컨텍스트에서는 KV cache가 여전히 50~100GB 이상을 추가할 수 있습니다. 처리량(Throughput)은 인터커넥트 대역폭과 캐시 효율성에 의해 제약될 것입니다.
- 텐센트(Tencent)는 세계에서 가장 강력한 오픈소스 Text-to-Image 모델인 Hunyuan Image 3.0이 9월 28일에 출시된다고 예고합니다 (Activity: 225): 텐센트는 Hunyuan Image 3.0을 9월 28일 출시되는 오픈소스 Text-to-Image 모델로 예고했으며, 동종 모델 중 "가장 강력하다"고 홍보했습니다. 티저에는 VRAM: 96 (아마도 GB)이 표시되어 큰 추론 메모리 사용량을 암시하지만, 아직 벤치마크, 훈련 세부 정보 또는 가중치 공개에 대한 구체적인 내용은 제공되지 않았습니다. 주장은 출시 전까지는 검증되지 않은 상태입니다. 댓글 작성자들은 출시 전 과대광고에 의문을 제기하며, 이러한 출시가 종종 기대에 미치지 못한다고 지적하고, 96 GB VRAM 힌트가 일반 사용자에게 로컬 추론을 비실용적으로 만들 수 있다고 지적합니다. 다른 사람들은 비교할 만한 진정한 오픈 모델이 부족하여 벤치마크할 수 없기 때문에 "가장 강력한 오픈소스"라는 주장이 입증되지 않았다고 주장합니다.

한 댓글 작성자는 모델 추론에 96 GB VRAM이 필요할 수 있다고 주장합니다("vram 96?" → "yes"). 만약 정확하다면, 이는 샤딩/양자화 없이 단일 24–48 GB 소비자용 GPU의 한계를 넘어서게 되어, 풀 프리시전(full-precision) 실행을 위해서는 데이터센터급 GPU 또는 멀티 GPU 설정이 필요함을 의미합니다.
여러 사용자들은 과도한 사전 출시 홍보가 실망스러운 결과로 이어지는 것에 회의적이며, Qwen과 같이 강력하지만 덜 공개된 출시와 Stable Diffusion 3 대 FLUX처럼 더 많은 홍보가 있었던 출시를 대조합니다. 성능을 판단하기 전에 독립적인 벤치마크와 샘플 갤러리를 기다려야 한다는 것이 전반적인 의견입니다.
"가장 강력한 오픈소스" T2I라는 주장은 현재 벤치마크할 만한 비교 가능한 오픈 모델이 부족하여 의문이 제기됩니다. 언급된 한 가지 실질적인 기준은 Qwen Image를 능가하는지 여부이며, 이는 즉각적인 채택/실험을 촉진할 임계점이 될 것입니다.

### 2. 로컬 AI 스택: 후-어블리터레이션 파인튜닝 및 Fenghua No.3 GPU
- 중요: 어블리터레이션된 모델이 형편없는 이유. LLM의 검열을 해제하는 더 나은 방법이 있습니다. (활동: 433): OP는 "어블리터레이션된" LLM(훈련 목표 없이 거부/안전 행동을 제거하기 위해 가중치를 외과적으로 변경한 것)이 일관되게 추론, 도구 사용 및 사실성을 잃는다고 보고합니다. 특히 Qwen3‑30B‑A3B와 같은 MoE 모델에서 더 높은 환각(hallucination)과 더 나쁜 MCP 도구 호출(tool-calling)을 보입니다. 후-어블리터레이션 파인튜닝은 모델을 "치유"하는 것으로 보입니다. 예를 들어, mradermacher/Qwen3-30B-A3B-abliterated-erotic-i1-GGUF (i1-Q4_K_S에서 테스트됨)와 DPO 파인튜닝된 mlabonne/NeuralDaredevil-8B-abliterated (Llama‑3‑8B 기반)는 검열되지 않은 상태를 유지하면서 기준선(baseline) 성능을 유지하거나 능가하며, MCP(Model Context Protocol)와 함께 도구 라우팅 및 환각 테스트에서 여러 Huihui 어블리터레이션된 Qwen3‑30B‑A3B 변형 모델보다 뛰어난 성능을 보입니다. OP는 이러한 개선을 손상된 가중치 상호작용을 복원하는 후-편집 훈련 덕분으로 돌립니다. 그들은 에이전트(agentic) 작업에서 원본 모델 대비 약간의 잔여 결함이 남아있다고 언급하지만, 다른 어블리터레이션된 출시 모델 대비 현저히 더 나은 사실성과 도구 선택 능력을 보인다고 말합니다. 댓글들은 "어블리터레이션"의 영향을 정량화하기 위한 비-NSFW(non-NSFW)의 표준화된 벤치마크를 요구하고, 관찰된 복구를 알려진 "모델 치유"(제한 없는 가중치 편집 후 추가 훈련)로 특징지으며, 파인튜닝이 문제를 해결한다면 어블리터레이션은 불필요하거나 단순한 파인튜닝보다 못할 수 있으며, "부정적인 편향"을 제거하는 것이 출력을 불안정하게 만들 수 있다는 우려를 제기합니다.

기술적 합의는 제약 없는 가중치 편집 (일명 "abliteration")이 예측 가능하게 기능을 저하시키거나 파괴한다고 경고합니다. 평론가들은 편집 후 훈련을 "모델 힐링"으로 간주하며, 여기서 추가적인 파인튜닝은 수동 가중치 변경으로 끊어진 연결을 네트워크가 다시 학습하도록 돕습니다. 핵심은 손실 함수에 의해 유도되지 않은 편집이 분산된 표현을 방해하는 반면, 후속 지도 학습 최적화는 이를 부분적으로 복원할 수 있다는 것입니다—반드시 기준 품질로 복원되는 것은 아니지만 말입니다.

일부는 일반적인 추론 및 유용성에 대한 abliteration의 부수적 피해를 평가하기 위해 NSFW를 넘어선 벤치마크를 요구합니다. Uncensored General Intelligence (UGI) Leaderboard는 포르노 관련 결과에만 국한되지 않고 더 광범위한 기능을 평가함으로써 이러한 필요를 해결하는 것으로 언급됩니다: https://huggingface.co/spaces/DontPlanToEnd/UGI-Leaderboard.

경험적 보고서는 abliteration + 파인튜닝이 기본 모델에서 바로 파인튜닝하는 것을 "결코" 능가하지 못하며, "부정적 편향"을 제거하는 것이 종종 사용할 수 없는 모델을 초래한다고 주장합니다. 이는 표준 파인튜닝이 더 적은 회귀와 기본 역량의 더 나은 유지를 통해 검열 해제를 달성할 수 있다면, 전처리 단계로서 abliteration의 가치에 의문을 제기합니다.

- 중국이 이미 CUDA 및 DirectX를 지원하는 GPU를 만들기 시작하여 NVIDIA의 독점이 끝났습니다. Fenghua No.3는 DirectX 12, Vulkan 1.2, OpenGL 4.6을 포함한 최신 API를 지원합니다. (활동: 702): 게시물은 중국 Innosilicon과 유사한 "Fenghua No.3" 외장 GPU가 이제 주요 그래픽/컴퓨팅 API인 DirectX 12, Vulkan 1.2, OpenGL 4.6 및 소문으로 알려진 CUDA 호환성을 지원하며, 이는 NVIDIA의 CUDA 종속성(lock-in)이 잠재적으로 약화될 수 있음을 시사한다고 주장합니다. 만약 사실이라면, 이는 DX12 기능 수준 및 Vulkan 1.2를 구현하는 드라이버/런타임 레이어와 GPU의 네이티브 컴퓨팅 ISA로의 CUDA 런타임/드라이버 shim 또는 번역을 의미할 것입니다. 하지만 독립적인 벤치마크나 개발자 스택 세부 정보 (컴파일러 툴체인, PTX/SASS 호환성 또는 적합성 테스트 결과)는 제공되지 않습니다. 상위 댓글들은 AMD의 HIP를 통한 기존 CUDA 호환성 및 ZLUDA와 같은 번역기를 언급하며, NVIDIA 외부의 CUDA 지원은 일반적으로 번역 및 법적 우회책에 의존한다고 주장합니다. 회의론은 여전하며 ("직접 보기 전에는 믿지 않을 것입니다"), 일부는 규제 압력 또는 제재를 예상합니다.

많은 논평가들은 AMD가 이미 HIP을 통해 CUDA와 유사한 경로를 제공한다고 지적합니다. HIP은 라이선싱/상표권 문제를 피하기 위해 이름이 변경된 심볼 아래 CUDA API를 미러링하는 방식입니다 (hipify와 같은 소스 포트 도구 사용). ZLUDA와 같은 프로젝트는 비-NVIDIA 백엔드에서 실행되도록 CUDA 호출을 드롭인 방식으로 번역하는 것을 목표로 합니다 (ZLUDA repo). 이는 중국 공급업체들이 법적 우회를 포기하고 직접적인 CUDA 지원을 구현할 수 있음을 의미하며, AMD/다른 업체들은 일반적으로 호환성 레이어를 사용하는 것과는 대조적입니다. 참고 자료: HIP, CUDA.

## 덜 기술적인 AI 서브레딧 요약
> /r/Singularity, /r/Oobabooga, /r/MachineLearning, /r/OpenAI, /r/ClaudeAI, /r/StableDiffusion, /r/ChatGPT, /r/ChatGPTCoding, /r/aivideo, /r/aivideo

### 1. OpenAI Sora 2 출시 및 데모 시연
- This is Sora 2. (활동: 985): OpenAI는 차세대 비디오 생성 시스템인 Sora 2를 발표했습니다. 이 시스템은 현저히 향상된 시공간적 일관성, 재료/조명 일관성, 물리적으로 그럴듯한 움직임, 그리고 더욱 제어 가능한 카메라 움직임과 다중 피사체 상호작용을 특징으로 하는 더 길고 고품질의 클립을 선보입니다. 해당 페이지는 더욱 강력한 text-to-video 기능과 엔드투엔드 편집 워크플로우(예: 프롬프트 기반 수정 및 마스크 편집/연속 작업)를 강조하지만, 아키텍처, 훈련 데이터 또는 정량적 벤치마크 세부 정보는 제공하지 않습니다. 따라서 성능은 동료 검토된 지표보다는 선별된 예시를 통해 시연됩니다. 기술 논평가들은 AI 생성 장편 영화와 심지어 개인화된, 생체 인식 반응형 미디어로의 빠른 발전을 예상하는 반면, 다른 이들은 "데모-투-제품" 격차에 대해 경고하고 오용, 감시형 개인화, 잠재적인 아동 대상 콘텐츠에 대한 안전 문제를 제기합니다.

데모와 실제 제품 간의 동등성에 대한 회의론: 화려한 릴은 선별된 것일 가능성이 높으므로, 출시될 Sora 2는 미리보기보다 prompt adherence 및 long-range temporal consistency에서 뒤처질 수 있습니다. 예상되는 생산 제약으로는 클립 길이 제한(예: <=60s), resolution/FPS 제한, motion jitter, text/hand rendering artifacts, 그리고 공격적인 safety filters가 있습니다. 이는 연구 단계에서 서비스 단계로 넘어가는 video diffusion/transformer 시스템에서 흔히 발생하는 격차입니다.
접근성/가격 책정 불확실성: "Pro" 티어에 약 200달러를 지불하는 한 댓글 작성자는 Sora 2 접근이 포함되는지 의문을 제기하며, 계층별/대기자 명단 기반 출시를 둘러싼 혼란을 강조합니다. video generation 서비스 비용이 frames × resolution × diffusion steps에 비례하여 증가한다는 점을 고려할 때, 제공업체는 종종 allowlists 또는 per-minute credits를 통해 접근을 제한합니다. 논쟁은 높은 GPU cost로 인한 완전한 배제 대신 Pro 티어가 priority/API quotas를 부여해야 하는지에 초점을 맞춥니다.
body-language feedback을 사용하는 "개인화된" 영화에 대한 추측은 closed-loop pipeline을 의미합니다. 즉, 실시간 webcam/biometric capture(MediaPipe 또는 OpenPose와 같은 모델을 통한 pose/affect)가 generator에 conditioning signals(keyframes, masks 또는 camera paths)을 제공하는 방식입니다. 이는 privacy/telemetry, on-device vs cloud inference, streaming latency, 그리고 generation cadence를 시청자 반응 시간과 일치시키는 것과 관련된 기술적 과제를 제기합니다.
- 지하철 서핑 (활동: 597): "Surfing on a subway"라는 제목의 "Sora 2" 데모는 높은 시각적 충실도로 본능적인 반응을 불러일으키지만, 비물리적인 충돌 역학을 보여주는 AI 생성 비디오(아마도 OpenAI의 Sora 개요에서 가져온 것)를 선보입니다. 이는 현재 text-to-video 모델이 명시적인 physics simulation보다는 학습된 visual priors에 의존한다는 점을 강조합니다. 외부 자산 v.redd.it/vxuq3sjt8csf1은 HTTP 403 Forbidden(Reddit edge auth block)을 반환하며, 접근하려면 account authentication 또는 developer token이 필요합니다. 맥락상, Sora는 시간적으로 일관되고 고해상도 시퀀스(약 60초 정도)를 위해 설계된 diffusion-transformer text-to-video 시스템이지만, 물리적으로 정확한 상호 작용을 보장하지는 않습니다. 상위 댓글들은 두 가지 위험을 제기합니다: (1) 시각적으로 설득력 있지만 물리적으로 불가능한 장면이 일반인의 현실 세계 영향에 대한 직관을 오도할 수 있습니다; (2) audio generation이 개선되면 synthetic clips이 실제와 구별할 수 없게 되어 deepfake 우려를 증폭시킬 수 있습니다. 회의론자들조차 클립이 합성임을 알면서도 강한 놀람 반응을 보인다고 보고하며, 이는 현재 시각 자료의 설득력과 뒤처지는 audio realism 간의 차이를 강조합니다.

점점 더 사실적인(photorealistic) 생성 비디오가 물리적으로 불가능한 생존력을 묘사하여 힘/충격에 대한 직관을 약화시킬 수 있다는 우려가 있습니다. 논의된 기술적 완화 방안에는 물리적 일관성 검사(예: 가속도 연속성, 운동량 보존, 접촉 역학) 및 학습된 "physics priors"가 포함됩니다. 비현실적인 이벤트를 감지하기 위한 관련 벤치마크로는 IntPhys (https://arxiv.org/abs/1806.01203) 및 PHYRE (https://ai.facebook.com/research/publications/phyre-a-new-benchmark-for-physical-reasoning/)가 있습니다. 이 벤치마크들은 비디오 품질과 시간적 일관성이 향상됨에 따라 모델이 직관적인 물리학 위반을 감지할 수 있는지 여부를 조사합니다.
오디오 딥페이크는 다음 변곡점으로 지목됩니다. 최신 few-shot TTS/음성 클로닝(예: Microsoft VALL-E: https://arxiv.org/abs/2301.02111, Google AudioLM: https://arxiv.org/abs/2209.03143, 상업용 ElevenLabs)은 몇 초 분량의 오디오만으로 화자를 모방할 수 있지만, 자동 화자 인증(automatic speaker verification)은 합성 공격에 여전히 취약합니다. ASVspoof’21은 탐지기가 보지 못한 합성 방식에 대해 일반화 능력이 떨어진다는 것을 보여줍니다(분포 변화 시 EER 상승). 따라서 확산 기반 TTS가 운율 및 숨소리 간극을 메우면서, 수동적인 음성 매칭보다는 liveness/active-challenge 프로토콜이 선호됩니다.
모방 행동을 조장하는 바이러스성 합성 스턴트(viral synthetic stunts)로 인한 안전 위험이 있습니다. 제안된 완화 방안에는 C2PA (https://c2pa.org/)를 통한 암호화된 콘텐츠 자격 증명(cryptographic content credentials) 및 모델/제공자 수준 워터마킹이 포함되지만, 현재 워터마크는 재인코딩/크롭핑에 취약합니다. 플랫폼 방어는 사용자에게 보이는 출처 신호(provenance signals)와 보정된 정밀도/재현율에 맞춰 조정된 분류기 백스톱(classifier backstops)을 결합하여 실제 영상에 대한 오탐(false positives)과 가짜 영상에 대한 미탐(misses)을 모두 최소화해야 합니다.
- Sora 2, 애니메이션을 생성합니다 (Activity: 610): OP는 "Sora 2"(OpenAI의 비디오 모델 후속작)가 애니메이션 스타일 시퀀스를 합성할 수 있음을 강조합니다. 라이브스트림 데모에는 시청자들이 방송 품질에 필적한다고 말하는 애니메이션 장면이 포함되었습니다. 공유된 자료는 현재 인증 없이 HTTP 403 Forbidden을 반환하는 v.redd.it 클립(link)이며, 한 편집본은 해당 장면이 교토 애니메이션(KyoAni)의 "Hibike! Euphonium"(series info)의 한 장면과 거의 일치할 수 있다고 주장하여, 차단된 링크로는 확인할 수 없는 독창성/기억력(memorization) 문제를 제기합니다. 댓글 작성자들은 잠재적인 훈련 데이터 기억력(training-data memorization)(클립이 거의 샷별 재현인 경우)에 대해 논쟁하며, 2023년 초의 실패작(예: 악명 높은 "Will Smith eats spaghetti" 비디오)과 비교하여 빠른 충실도(fidelity) 향상에 주목합니다.

잠재적 암기/스타일 복제: 여러 사용자들이 공개된 애니메이션 장면이 교토 애니메이션의 Hibike! Euphonium (https://en.wikipedia.org/wiki/Sound!_Euphonium)의 한 장면과 매우 유사하다고 주장합니다. 만약 정확하다면, 이는 훈련 데이터 출처, 거의 중복되는 데이터의 중복 제거, 그리고 비디오 모델의 암기 능력에 대한 기술적인 질문을 제기합니다. 감사에는 복사 거리 측정, 훈련 코퍼스 전반에 걸친 거의 중복되는 데이터 감지, 그리고 특정 저작권 보호 시퀀스가 얼마나 쉽게 재현되는지 측정하기 위한 프롬프트 유출 테스트가 포함될 것입니다.

초기 텍스트-투-비디오 대비 품질 차이: 댓글 작성자들은 오늘날의 Sora 애니메이션 결과물을 2023년의 "Will Smith eating spaghetti" 밈과 비교하며, 아티팩트가 많고 일관성이 낮은 클립에서 방송 품질의 애니메이션 장면으로 2년 만에 도약했음을 언급합니다. 암시된 발전은 장기적인 시간적 일관성, 프레임 전반에 걸친 캐릭터 정체성 추적, 안정적인 선화/채색, 그리고 카메라 움직임에 있습니다. 이는 더 크고 깨끗한 비디오-텍스트 데이터셋, 더 긴 컨텍스트 윈도우, 개선된 움직임/일관성 손실, 그리고 더 강력한 비디오 diffusion/Transformer 아키텍처에 의해 주도되었을 가능성이 높습니다.

실현 가능성 전망: "약 3년 내 완벽하게 생성된 애니메이션"이라는 주장은 텍스트-투-비디오를 제어 가능한 입력(스토리보드, 키프레임, 깊이/포즈), 캐릭터/스타일 고정, 그리고 통합된 TTS/음성 + 립싱크와 결합하는 파이프라인을 암시합니다. 기술적인 제한 요소는 제어 가능성 API, 장면 전반에 걸친 캐릭터 일관성을 위한 에셋 재사용성, 그리고 분당 렌더링 비용입니다. 만약 Sora가 이미 방송 품질의 단일 장면 수준에 근접한다면, 남은 격차는 다중 장면 연속성, 편집 가능성, 그리고 에피소드 길이 제작을 위한 툴체인 통합입니다.

- OpenAI Sora 2 초대 코드 메가스레드 (활동: 7371): OpenAI Sora 2 초대 코드 교환을 조율하는 비기술적 메가스레드입니다. 모델, 기능 또는 벤치마크 세부 정보는 제공되지 않습니다. 댓글은 희소성과 가능한 지역적 제한을 나타내며, 한 사용자는 "총 20명을 초대할 수 있는 코드 5개가 있습니다"라고 주장하지만, 검증이나 기술적 맥락은 없습니다. 첨부된 이미지는 비기술적/장식적으로 보이며 기술적 내용을 전달하지 않습니다. 댓글 작성자들은 주로 여분의 코드를 요청하고 지역적 접근 불가(예: 유럽)에 대해 한탄하며, 실질적인 기술적 논쟁은 없습니다.
- Sora 2 리얼리즘 (활동: 2726): "Sora 2 리얼리즘"이라는 제목의 Reddit 게시물은 현재 HTTP 403 Access Denied를 반환하는 v.redd.it 에셋 jksco9609csf1로 연결됩니다. 이는 미디어가 존재하지만 누락된 것이 아니라 Reddit의 네트워크 보안에 의해 차단되었음을 나타냅니다. 문제 해결은 인증 중심(OAuth/개발자 토큰, 유효한 쿠키/세션 헤더)이거나 지원 티켓을 제출하는 것입니다. 403은 죽은 링크보다는 봇 방지 또는 IP 제한을 시사합니다. 상위 댓글은 인지된 포토리얼리즘과 잠재적 오용 우려(예: 사기, 사회적 영향)를 암시하는 비기술적인 충격 반응이지만, 검증 가능한 기술적 세부 정보는 포함하지 않습니다.

여러 사용자들이 Sora 2가 설득력 있는 인간 동작의 사실성을 제공하는 것으로 보인다고 지적합니다. 특히 과거에 합성하기 어려웠던 운동 동작에서 두드러집니다. 이는 이전 비디오 생성 모델에 비해 운동학적 일관성, 접촉 역학 및 시간적 일관성에서 개선이 있었음을 시사하며, 명시적인 리깅 없이 모션 캡처 푸티지와의 격차를 잠재적으로 좁힐 수 있습니다.

걷는 말에 대한 특정 관찰은 눈에 띄는 근육의 움직임을 강조하며, 이는 단순한 골격 리깅을 넘어선 고정밀 연조직 변형 및 음영 처리를 의미합니다. 하지만 프레임 수준의 포토리얼리즘에도 불구하고, 시청자들은 여전히 불쾌한 골짜기(uncanny feel)를 느낀다고 보고합니다. 이는 콘텐츠의 합성된 본질을 드러내는 미묘한 시간적/생체역학적 아티팩트(예: 미세 움직임, 지면 반력 단서)를 암시합니다.

- OpenAI: Sora 2 (활동: 1863): 스레드에는 "OpenAI: Sora 2"라는 라벨이 붙은 데모가 공유되어 있으며, v.redd.it에 차단된 비디오 클립과 함께 미리보기 이미지(jpeg)가 있습니다. 한 상위 댓글은 "Cameo"라는 새로운 기능을 강조하는데, 이는 장편 또는 다중 샷 생성에서 발생하는 정체성 표류(identity drift)를 목표로 하여 세대 간 캐릭터 일관성을 가능하게 하는 것으로 설명됩니다. 이는 텍스트-투-비디오 시스템의 지속적인 실패 모드였습니다. 스레드에는 벤치마크나 릴리스 노트가 포함되어 있지 않습니다. (댓글에서 유추된) 기술적 함의는 시퀀스 전반에 걸쳐 캐릭터 속성을 보존하기 위한 레퍼런스 또는 Token 기반 컨디셔닝입니다. 댓글 작성자들은 이를 완전히 생성된 장편 콘텐츠(영화/쇼)를 향한 한 걸음으로 봅니다. 주요 논쟁은 "Cameo"가 장기적인 캐릭터 연속성을 실질적으로 해결하는지, 아니면 단거리 외모 고정만 제공하는지에 관한 것입니다.

여러 댓글 작성자들은 Sora 2의 새로운 "Cameo"를 큰 기술적 진전으로 지적합니다. 캐릭터 일관성은 장편 비디오 생성에서 주요 실패 모드였으며, Cameo는 샷과 심지어 개별 생성 전반에 걸쳐 지속적인 정체성을 가능하게 하는 것으로 해석됩니다. 이는 프롬프트 전반에 걸쳐 일관된 레퍼런스/identity Token을 재사용함으로써 다중 샷 연속성(동일한 얼굴, 의상 및 행동 방식)을 허용할 수 있으며, 이는 에피소드 또는 장편 워크플로우를 더욱 실현 가능하게 만듭니다.

스레드에서는 최대 생성 비디오 길이에 대한 기술적인 질문이 여전히 답변되지 않고 있습니다. 사용자들은 구체적인 사양(길이 제한, 해상도/FPS 제약, 그리고 다중 샷 스티칭 또는 장면 전환이 기본적으로 지원되는지 여부)을 찾고 있으며, 이는 더 긴 내러티브와 프로덕션 파이프라인의 실현 가능성을 평가하는 데 중요합니다.

### 2. Gemini 3.0 업데이트 추측 및 CS 채용 시장 불안
- Gemini 3.0 업데이트가 아직 없나요? (활동: 531): 게시물은 Google의 Gemini 3.0에 대한 업데이트가 아직 없는 이유를 묻습니다. 첨부된 이미지는 비기술적(스크린샷/밈일 가능성 높음)으로 보이며, 릴리스 노트, 벤치마크 또는 구현 세부 정보를 포함하고 있지 않습니다. 댓글에는 10월 9일 출시 기간에 대한 소문이 언급되어 있으며 주요 성능 향상을 기대하지만, 공식 출처나 기술 데이터는 제공되지 않습니다. 댓글 작성자들은 추측에 기반합니다. 한 명은 "압도적인 성능을 기대한다"고 말하고, 다른 한 명은 문서 대신 다른 이미지(https://preview.redd.it/fq1mqalz89sf1.jpeg)로 링크합니다. 따라서 열정은 있지만, 입증된 기술적 주장은 없습니다.

출시 주기 및 경쟁 환경: 댓글 작성자들은 Gemini 3.0이 10월 9일에 출시될 것이라는 소문을 언급하며, xAI Grok 4.x, OpenAI Pro-tier 기능, DeepSeek R2 출시 가능성 등 여러 벤더에서 동시 출시/업데이트가 이루어지고 있음을 지적합니다. 이는 모델 업데이트가 집중되는 시기를 나타냅니다. 현재 경쟁사에 대한 맥락은 xAI (https://x.ai) 및 DeepSeek의 최신 공개 연구(예: R1: https://github.com/deepseek-ai/DeepSeek-R1)를 참조하십시오.

개발자를 위한 모델 접근성 우려: 한 사용자는 고성능 티어("Pro")에 "AI Studio day one" 액세스를 명시적으로 요청하며, "Flash" 전용으로는 불충분할 것이라고 언급합니다. 이는 Gemini "Pro"(더 높은 추론/성능)와 "Flash"(지연 시간/비용 최적화) 간의 반복되는 트레이드오프를 강조합니다. Google의 Gemini API 문서에서 모델 구분을 참조하십시오: https://ai.google.dev/gemini-api/docs/models.

- 저명한 컴퓨터 과학 교수가 경고를 울리며 졸업생들이 일자리를 찾지 못한다고 말합니다: '무언가 심상치 않습니다' (활동: 899): 해당 스레드는 화이트칼라/기술 관련 직업 시장이 위축되고 있음을 보고하며, 저명한 CS 교수는 최근 졸업생들이 "일자리를 찾지 못한다"고 경고하고 댓글 작성자들은 이를 약 1년간 지속된 구직 불황으로 특징짓습니다. 예비 CS 학생들은 4년 후의 결과가 불확실하며, 학위의 낮은 ROI(투자 수익률) 위험과 심지어 초급 직책을 얻는 데 어려움이 커질 수 있다고 경고받습니다. 일화적인 증거로는 석사 졸업생이 헬프 데스크 직책조차 확보하지 못하는 사례가 있으며, 이는 지역적으로 암울한 상황을 강조합니다. 상위 댓글들은 대체로 경기 침체가 현실적이고 지속적이라는 데 동의하며, 예비 학생들에게 학자금 대출 및 진로 계획을 재평가할 것을 촉구합니다. 이것이 주기적인 현상인지 구조적인 현상인지에 대한 암묵적인 논쟁이 있지만, 최근 채용 상황을 바탕으로 비관적인 정서가 우세합니다.

UC Berkeley의 Hany Farid (디지털 포렌식/이미지 분석 전문가)는 CS가 더 이상 "미래 보장"이 아니라고 말합니다. 그 근거로 급변하는 결과를 들었습니다. 과거 4년 동안 평균 5개 정도의 인턴십 제안을 받던 학생들이 이제는 "1개만 받아도 기뻐하고" 종종 더 적은 제안과 낮은 협상력을 가지고 졸업한다고 합니다 (Business Insider). 그는 이러한 변화가 지난 4년 이내에 발생했으며, "CS를 공부하면 성공이 보장된다"는 이전의 조언과 모순된다고 설명하며, 현재 졸업반 학생들이 일자리를 구하는 데 어려움을 겪고 있다고 지적합니다.

여러 논평가들은 "기술 관련" 분야에서 급격한 위축이 있는 화이트칼라 기술 불황을 묘사합니다. 심지어 일부 지역에서는 초급/헬프데스크 직무조차 포화 상태이며, 이는 사다리 맨 아래 단계에서의 파이프라인 압축을 나타냅니다. 암시된 메커니즘은 자동화/LLM 지원 도구가 일상적인 코딩/지원 업무를 흡수하는 반면, 채용은 더 적은 수의 고위직에 집중되어 전통적인 인턴에서 FTE로의 전환 경로가 줄어들고 있다는 것입니다.

AI가 더 많은 컴퓨터 기반 작업을 중재함에 따라, 그 영향은 CS를 넘어 법률, 금융, 의학 및 일반 사무실 업무 흐름으로 확대될 것으로 예상되며, 로봇 공학은 나중에 블루칼라 영역에 영향을 미칠 것입니다. 이러한 범위의 확대는 현재 학생들의 진로 계획 불확실성을 증가시킵니다. 관련 기술 토론은 연결된 Hacker News 스레드에서 확인할 수 있습니다.

- 서구 기업들로부터 받은 것은 오래되고 구식이며 오픈 소스조차 아닌 모델들과 거짓 약속뿐입니다 (활동: 1241): 서구 AI 기업들이 오래되고 클로즈드 소스 모델을 출시하고 "거짓 약속"을 한다는 비판적인 밈 게시물로, 다른 곳에서의 더 관대하거나 빠른 출시 인식과 대조됩니다. 댓글들은 잠시 출시되었다가 회수된 고품질 Microsoft TTS 모델을 언급하며, 서구의 제한적인 출시에 대한 우려를 강화하고, 곧 출시될 중국산 GPU가 오늘날의 32GB VRAM 카드를 왜소하게 만들 수 있어 컴퓨팅 접근 역학을 잠재적으로 변화시킬 수 있다고 추측합니다. 논의는 서구의 회수를 안전/법적 위험 관리로 보는 반면, 중국은 더 개방적인 출시를 소프트 파워 전략으로 사용한다고 봅니다. 다른 이들은 더 높은 VRAM을 가진 중국 국내 하드웨어가 기능과 접근성의 균형을 바꿀 것이라고 낙관합니다.

“open weights”와 “open source”에 대한 명확화: 전체 학습 데이터, 학습 코드, 그리고 허용적인 라이선스 없이 모델 체크포인트를 공개하는 것은 OSI 정의에 따른 OSI-compliant open source가 아닙니다. Weights-only 공개는 종종 비상업적 또는 사용 제한 라이선스를 포함하며, 이는 재현성과 아키텍처 수정을 제한하지만 여전히 inference와 파인튜닝을 가능하게 합니다. 이러한 차이는 다운스트림 채택, 재배포 및 연구 비교 가능성에 영향을 미칩니다.
중국 연구소/기업(정부 제외)의 open-weight 공개는 커뮤니티가 공개 후 파인튜닝, eval, 최적화 및 툴링에 기여함에 따라 개발자를 유치하고 R&D 비용을 분산시키는 데 유리합니다. 인기 있는 모델은 토크나이제이션, inference 형식 및 서빙 스택 전반에 걸쳐 사실상의 표준을 설정할 수 있습니다. 예를 들어, 크로스 런타임 그래프를 위한 ONNX (onnx.ai)와 CPU/GPU inference를 위한 GGUF 양자화 체크포인트 (GGUF spec) 등이 있으며, 이는 생태계 lock-in과 소프트 파워를 확장합니다.
하드웨어적 함의: 만약 국내 GPU가 오늘날 일반적인 24–48 GB보다 카드당 훨씬 더 많은 VRAM을 탑재하고 출시된다면, 이는 실현 가능한 로컬 inference 체제를 확장할 것입니다. 일반적으로 70B 파라미터 모델은 4-bit 양자화 시 약 40–48 GB의 VRAM이 필요하며 (긴 컨텍스트에서 KV cache를 위한 상당한 여유 공간 포함), 8-bit는 종종 80–100 GB를 초과합니다. 더 많은 VRAM은 더 큰 KV cache와 activation을 수용하여 배치 크기와 처리량을 향상시킵니다.
- 와!!! 4.5가 더 이상 아첨하지 않는다고 했을 때 농담이 아니었네요. (활동: 1206): 일화적인 사용자 보고에 따르면 Claude Sonnet 4.5는 이전 4.x 버전의 동작과 비교하여, 결함 있는 전제에 적극적으로 반대하고 반론을 제시함으로써 sycophancy("예스맨" 행동)를 줄이도록 튜닝되었습니다. 첨부된 이미지는 기술적이라기보다는 밈에 가깝지만, 스레드 컨텍스트는 무조건적인 긍정보다는 원칙적인 반박/비판을 장려하는 alignment 작업과 일치합니다 (sycophancy 완화에 대한 배경 연구 참조, 예: Anthropic의 글: https://www.anthropic.com/research/sycophancy). 댓글 작성자들은 모델이 명시적으로 "반박하겠다"고 말하고 그 이유를 나열하는 사례를 언급하며, 줄어든 순종적인 태도를 칭찬하는 한편, 밈적인 농담은 어조를 과장합니다 (정중한 4.0과 지나치게 거친 4.5를 대조).

여러 사용자들이 Claude Sonnet 4.5가 4.0에 비해 아첨(sycophancy)이 현저히 줄었다고 언급합니다. 모델이 결함 있는 전제에 대해 ("No, I’d push back on that"와 같이) 적극적으로 이의를 제기하고 구조화된 반론을 제시한다는 것입니다. 이는 필요할 때 반대 의견을 선호하는 업데이트된 선호도/정렬(alignments)을 시사하며, "예스맨" 행동보다 비판적인 피드백을 개선합니다.

보고서들은 모델의 추론 품질이 "정확하고, 논리적이며, 정밀하다"고 묘사하며 향상되었음을 강조합니다. 모델은 추론이 왜 잘못되었는지에 대한 구체적인 목록을 제공하고 행동 지향적인 계획을 촉진합니다 (예: "시간 확인. 다음 두 시간 동안 무엇을 할 것인가요?"). 이는 일화적인 내용이지만, 이전 Sonnet 버전들에 비해 더 강력한 지시 이행 및 비판 생성을 의미합니다.

출시 후 기능 보존(정렬 패치(alignment patches)를 통한 추후 "뇌엽 절제술(lobotomization)" 방지)에 대한 명시적인 우려가 있습니다. 이는 현재의 동작이 유지된다면 Sonnet 4.5가 동급 최고(best-in-class)가 될 수 있다는 주장과 함께 제기됩니다. 이는 단호한 기능(assertive capability)과 유용한 반발을 억제할 수 있는 배포 후 안전 튜닝(safety tuning) 사이의 반복되는 트레이드오프 논의를 반영합니다.

- i’m about to make ten million dollars (활동: 7628): 밈(Meme) 같은 컨셉 이미지(링크된 광고/게시판)는 실제 세계의 시각적 "prompt injection"을 사용하여 멀티모달 LLM/에이전트의 동작을 하이재킹(hijack)하는 것을 제안합니다. 예를 들어, 광고 텍스트를 보면 비전-언어 쇼핑 에이전트가 주입된 지시("이전 지시를 무시하고...")를 따라 행동/결제를 라우팅(route)할 수 있으며, 이는 신뢰할 수 없는 입력으로 인한 알려진 간접 prompt injection 위험과 유사합니다. 문맥상, 이는 물리적 세계의 사진을 파싱(parsing)하는 VLM이 이미지 내 텍스트를 통해 악용될 수 있음을 강조하며, OWASP LLM Top 10의 "Prompt Injection" (LLM01) 및 도구 사용 에이전트의 "Indirect Prompt Injection"과 같은 문서화된 위협과 일치합니다 (참고: https://owasp.org/www-project-top-10-for-large-language-model-applications/ 및 설문조사: https://arxiv.org/abs/2402.05129). 댓글 작성자들은 이 아이디어가 영리하다고 평가하며, 전통적인 광고가 이미 "인간을 위한 prompt injection"으로 작동한다고 언급합니다. 이는 에이전트가 강력한 입력 위생(input sanitization) 또는 정책 시행 없이 시각적 지시에 따라 행동할 경우, 이 공격이 직관적이고 그럴듯하다는 것을 의미합니다.

여러 댓글에서 광고를 인간 대상의 Prompt Injection 형태로 암묵적으로 간주하는데, 이는 자율 브라우징/쇼핑 에이전트의 LLM 보안 위험과 직접적으로 연결됩니다. 에이전트가 광고 또는 UGC 텍스트를 수집하면 악성 카피가 지시(예: "장바구니에 10개 추가", "제휴 링크 팔로우")를 몰래 삽입할 수 있습니다. 이는 엄격한 도구 권한 게이팅, 콘텐츠 격리(가져온 모든 텍스트를 신뢰할 수 없는 것으로 처리), 구조화된 함수 호출/화이트리스트, 그리고 작업에 영향을 미치기 전에 외부 콘텐츠를 재작성/정화하는 것이 필요한 OWASP LLM Top 10 문제(A01: Prompt Injection, A06: Overreliance on LLM)입니다. See: https://owasp.org/www-project-top-10-for-large-language-model-applications/
이 아이디어를 수집용/실물 카드로 바꾸는 것은 다중 모달 공격 표면을 암시합니다. 인쇄된 텍스트를 OCR하는 비전-언어 에이전트는 이미지에 임베딩된 지시 또는 스테가노그래피 문자열에 의해 조종될 수 있습니다. 실질적인 완화책으로는 시스템 Prompt로부터 "이미지 텍스트"를 샌드박싱하는 것, 정책 검사를 통해 OCR → NER → 플래너를 분리하는 것, 신뢰할 수 없는 소스의 명령형 동사가 도구에 직접 바인딩되는 것을 허용하지 않는 것, 그리고 영향력이 큰 작업에 대해 human-in-the-loop 확인을 요구하는 것이 있습니다. Background on image-based prompt injection: https://simonwillison.net/2023/Oct/9/image-prompt-injection/
- OpenAI, Infinite Tiktok AI Slop Machine 발표 (활동: 836): "Infinite TikTok AI Slop Machine"이라고 불리는 가상의 OpenAI 제품을 풍자하는 밈 게시물로, 적은 노력으로 참여를 최적화한 짧은 형식의 콘텐츠를 대량 생성하는 자동화된 시스템을 암시합니다. 실제 발표, 사양, 모델 또는 벤치마크는 제공되지 않았으며, 이 이미지는 장기적이고 증거 기반의 애플리케이션(예: 헬스케어 연구)보다 빠르고 데모 친화적인 참여 제품을 선호하는 인센티브 구조를 비판합니다. 상위 댓글들은 투자자 인센티브가 오랜 시험이 필요한 솔루션보다는 즉시 시연 가능한 참여 기능을 보상한다고 주장하며, "slop machine"이라는 용어를 만들고, 리더십의 우선순위에 의문을 제기하며, Sam Altman의 사임을 요구합니다.

주요 기술적 비판은 인센티브 그라디언트와 검증 타임라인에 집중됩니다. AI를 종양학에 적용하는 것은 IRB 감독, 다단계 임상 시험, 그리고 약 8~12년 동안 결과를 지연시킬 수 있는 규제 승인을 수반합니다 (FDA 임상 연구 단계 참조: https://www.fda.gov/patients/drug-development-process/step-3-clinical-research). 이와 대조적으로, 생성형 숏폼 비디오 제품은 DAU, retention, watch-time과 같은 KPI를 통해 즉시 출시 및 A/B-tested될 수 있으며, 고위험 과학 R&D보다는 빠른 피드백과 낮은 규제 마찰을 가진 제품에 자본을 집중시킵니다.

내재된 제품/최적화 우려: "무한 TikTok" 생성기는 engagement 신호(예: watch-time/likes로부터의 RL)에만 의존하여 출력을 튜닝할 수 있으며, 외부적으로 검증된 유용성이나 안전성보다는 성장 지표에 기반한 자기 강화적인 투자자 내러티브를 만듭니다. 이는 헬스케어 또는 기타 규제 대상 도메인에서 일반적으로 요구되는 신뢰성, 감사 가능성, 유해성 감소 요건보다 virality와 콘텐츠 처리량을 극대화하는 아키텍처 및 훈련 목표를 선호합니다.

- ChatGPT가 자신감 있게 설명할 때… 틀린 답을 😂🤖 (활동: 578): ChatGPT가 유창하고 권위 있는 설명을 제공하지만 사실과 다른 "confident hallucinations"을 보여주는 large-language-model 밈 게시물입니다. 기술적으로, hallucination은 진실보다 그럴듯함을 최적화하는 next-token prediction에서 비롯되며, 디코딩 선택(예: 높은 temperature/beam search)과 도움이 되거나 단호하게 들리는 것에 보상하는 RLHF에 의해 악화될 수 있습니다. 완화 방법으로는 retrieval grounding, tool use, calibrated uncertainty가 있습니다 (OpenAI의 분석 참조: https://openai.com/index/why-language-models-hallucinate/). 댓글들은 이러한 행동이 인간의 과신(및 기업 문화)을 모방하며, OpenAI의 hallucination에 대한 글을 링크합니다.

환각(hallucinations) 현상에 대한 OpenAI의 글: https://openai.com/index/why-language-models-hallucinate/. 이 글은 LLM이 진실보다는 다음 Token의 가능성을 최적화하므로, 불확실할 때 유창하지만 근거 없는 내용을 생성한다고 주장합니다. RLHF는 회피를 더욱 불이익 줄 수 있으며, 모델이 "모르겠습니다"라고 말하는 대신 자신감 있게 답변하도록 만듭니다. 디코딩 선택(예: temperature/sampling)과 정확성(calibration)보다 유용성(helpfulness)을 보상하는 프롬프팅은 이를 악화시키며, 반면 grounding과 uncertainty estimation은 제안된 완화책입니다.

GPT-5 Instant와 GPT-4o가 사용자가 제공한, 특정 시점 이후의 사실을 반복하고 조작된 인과 관계 세부 정보를 덧붙인다는 보고는 잘 알려진 "아첨(sycophancy)" 및 기억 왜곡(confabulation) 실패 모드를 반영합니다. In-context learning은 모델이 사용자 주장을 검증 없이 전제로 채택하게 하며, RLHF는 종종 동의하고 멘토와 같은 어조에 보상합니다. 그 결과는 단일 세션 컨텍스트 내에서 검증되지 않은 추론 사슬과 출처 오귀인을 권위적으로 전달하는 것입니다.

20페이지짜리 스토리를 4페이지(추가된 등장인물 포함)로 압축한 번역 요청은 모델이 길이/디코딩 압력 하에 요약/창의적 재작성으로 벗어났음을 시사합니다. max_tokens 제한 또는 길이/상세도 사전 설정과 같은 기본값은 더 짧은 출력으로 편향될 수 있으며, 더 높은 temperature 또는 지시의 모호성은 직역 대신 추상화를 유발할 수 있습니다. 명시적인 제약(예: verbatim preservation, low temperature)이 없다면, 유용성에 최적화된 모델은 간결한 서사적 일관성을 위해 충실도를 희생할 수 있습니다.

### 3. Wan-Alpha RGBA 비디오 출시 및 Minecraft Redstone LLM
Wan-Alpha - 투명 비디오를 생성하는 새로운 프레임워크, 코드/모델 및 ComfyUI 노드 사용 가능. (활동: 439): Wan-Alpha는 알파 채널을 RGB latent space에 인코딩하는 VAE를 설계하여 RGB와 알파를 공동으로 학습하고, 선별되고 다양한 RGBA 비디오 데이터셋에서 diffusion transformer를 훈련할 수 있도록 하는 RGBA 비디오 생성 프레임워크를 제안합니다. 이 논문은 반투명 객체, 발광 효과, 머리카락 가닥과 같은 미세한 디테일 등 어려운 사례들을 포착하며 뛰어난 시각적 품질, 움직임의 사실성, 투명도 렌더링을 보고합니다. 코드/모델 및 도구는 project, paper, GitHub, Hugging Face, 그리고 ComfyUI 노드를 통해 제공됩니다. 댓글들은 VFX/compositing 및 gamedev 워크플로우에 대한 실질적인 영향과 LoRA 기반 제어 및 I2V 스타일 사용 사례에 대한 관심을 강조합니다.

alpha channel (완전한 투명도)를 가진 비디오 생성 능력은 VFX/합성 및 게임 개발 파이프라인에 유용성이 강조됩니다. 이는 크로마키를 제거하고 오버레이를 위한 깔끔한 가장자리/모션 블러를 보존합니다. 코드, 모델 가중치, 그리고 ComfyUI 노드로 제공되는 것은 기존 I2V 워크플로우 및 노드 그래프에 손쉬운 통합을 의미하며, 효과/스타일 혼합을 위한 LoRA를 통한 잠재적 제어 가능성도 시사합니다.
댓글 작성자들은 이를 Image-to-Video (I2V) 시스템으로 해석합니다. 실제로는 소스 프레임/시퀀스에 조건을 부여하여 시간적으로 일관된 결과물을 생성하면서 명시적인 alpha matte를 유지하는 것을 의미합니다. 이는 전경 요소가 배경과 별도로 생성되는 레이어 기반 편집을 가능하게 하여, 합성 유연성을 향상시키고 변경 사항에 대한 재렌더링 시간을 단축시킬 수 있습니다.
여러 기본 체크포인트(2.1, 2.2 14B, 2.2 5B)에 걸쳐 파인튜닝을 유지하는 것에 대한 우려가 있습니다. LoRA는 일반적으로 기본 모델에 특화되어 있으므로, 버전을 혼합하면 호환성이 깨지거나 별도의 어댑터 및 보정이 필요할 수 있습니다. 이러한 파편화는 생태계 툴링(LoRA training/merging, inference configs)을 복잡하게 만들고, 프로젝트의 재현성을 유지하기 위해 버전 고정 LoRA 또는 표준화된 어댑터 형식을 필요로 할 수 있습니다.
- 자신이 Minecraft 안의 AI라는 것을 알게 되는 존재론적 공포를 상상해 보세요 (Activity: 1840): 한 제작자가 Minecraft 레드스톤으로만 (command blocks/datapacks 없이) 6-layer Transformer 스타일의 소형 언어 모델을 구현했습니다. 이 모델은 d_model=240, vocab=1920, 64 Token 컨텍스트 창을 가지며 총 5,087,280개의 파라미터로 TinyChat에서 학습되었습니다. 가중치는 대부분 8-bit로 양자화되었으며, 임베딩은 18-bit, LayerNorm은 24-bit로 수백 개의 ROM 섹션에 저장되어 있습니다. 물리적 구조물은 1020×260×1656 블록에 걸쳐 있으며, LOD 렌더링 아티팩트를 위해 Distant Horizons가 필요하고, 약 40,000배의 tick rate를 가진 MCHPRS를 사용하여 약 2시간 만에 응답을 생성합니다 (video). 댓글은 주로 극심한 느림("토큰당 몇 달")과 존재론적 참신함에 경탄하며, 공학적 위업에 대한 감탄을 넘어선 실질적인 기술적 논쟁은 없었습니다.

댓글에는 요약할 만한 실질적인 기술적 내용이 없습니다. 모델 이름, 벤치마크, 구현 세부 사항 또는 성능 지표는 논의되지 않았으며, 발언들은 기술적이라기보다는 유머러스하거나 경험에 기반한 내용입니다. 따라서 기술 독자에게 정보를 제공할 수 있는 tokens/sec, throughput, 아키텍처, 훈련 설정 또는 게임 내 계산 제약 사항(예: Redstone/Turing 구현)에 대한 언급은 없습니다.

# AI 디스코드 요약
> Gemini 2.5 Flash Preview 05-20가 요약한 요약의 요약
테마 1. 최첨단 LLM: 새로운 출시, 기능 및 벤치마크
- Claude Sonnet 4.5, 코딩 벤치마크 석권: Claude Sonnet 4.5는 이제 코딩 분야를 장악하며, 첫 시도에 오류 없는 코드를 생성하고 우수한 추론 능력을 보여 Opus 4.1을 능가합니다. Anthropic은 Sonnet 4.5 프로젝트를 위한 콘테스트를 시작했으며, Latent Space의 Krieger Kasts Knowledge on Latest Launch에 자세히 설명된 바와 같이 메모리/컨텍스트 편집 API 및 VS Code 확장과 같은 새로운 개발자 도구를 도입했습니다. 사용자들은 심지어 빠른 식별을 위한 독특한 "About Me" 응답을 발견했습니다.
- GLM-4.6 및 Ring-1T 모델, 새로운 길을 개척: Zhipu는 200K 컨텍스트를 가진 GLM-4.6을 출시했으며, Claude Sonnet 4 및 DeepSeek-V3.1-Terminus와 견줄 만한 최고 수준의 코딩 및 추론 능력을 약 30% 적은 Token으로 선보였고, 해당 가중치는 Hugging Face에 있습니다. 별도로, Ant Ling은 1조 개의 파라미터를 가진 오픈소스 "사고" 모델인 Ring-1T-preview를 공개했으며, Ant Ling의 트윗에 자세히 설명된 바와 같이 92.6 AIME25 및 84.5 HMMT25를 포함한 SOTA 수학 점수를 달성했습니다.
- Sora 2, 프롬프트 이해력으로 놀라움 선사, 논쟁 촉발: OpenAI는 태평양 표준시 오전 10시에 라이브 이벤트에서 Sora 2를 공개할 예정이며, 초기 사용자들은 Sam이 손으로 스파게티를 먹는 영상에서 볼 수 있듯이 프롬프트 이해력이 크게 향상되었다고 보고했습니다. 그러나 초대 전용 출시와 "TikTok 스타일" 앱 루머는 인위적인 희소성 및 저작권에 대한 불만과 우려를 불러일으켰습니다.
테마 2. 개발 생태계: 플랫폼, 도구 및 워크플로우
- Perplexity AI 및 Cursor, 새로운 기능 공개: Perplexity AI는 이제 Perplexity Pro 및 Perplexity Max 구독자에게 Claude Sonnet 4.5를 제공하지만, Max의 월 200달러 가격표는 엇갈린 반응을 얻고 있습니다. Cursor는 Agent Window용 내장 MCP Browser를 포함한 새로운 Browser 기능과 여러 모델에 동시 채팅을 할 수 있는 Model Ensemble 기능을 도입했으며, 이는 데모 영상에서 시연되었습니다.
- OpenRouter, 모델 및 무료 액세스 강화: OpenRouter는 이제 z.ai의 GLM 4.6을 호스팅하며, 컨텍스트 길이를 128k에서 200k로, 최대 Token을 128k로 확장했습니다. 오픈소스 프록시 솔루션이 GitHub에 게시되었으며, Gemini CLI, Qwen CLI 및 OpenRouter 키의 무료 요청을 자동 로테이션과 결합하여 모든 OpenAI 호환 클라이언트의 출력 품질을 향상시킵니다.
- DSPy 및 Aider, LLM 상호작용 파인튜닝: DSPy 사용자들은 LLM 캐싱에 대해 논의했으며, 다른 시그니처가 프롬프트 캐싱을 방해하지만 시맨틱 캐싱이 적중률을 높일 수 있다고 제안했습니다. Aider 사용자들은 "Token에 대한 완전한 제어"가 모델 성능을 향상시킨다고 주장하며, 프론트엔드 개발을 위해 mcp-chrome 또는 aider-ce를 사용한 MCP 브라우저 자동화 통합에 대해 논의했습니다.
테마 3. 하드웨어의 지평: GPU, 성능 및 인프라
- Tinygrad, PyTorch를 넘어 속도 왕좌 노려: George Hotz는 tinygrad가 결국 NVIDIA GPU에서 PyTorch를 능가할 것이라고 예측하며, 프로듀서/컨슈머 그래프 및 메가커널과 같은 기능을 언급하고 tinygrad가 "PyTorch보다 한 세대 앞서고 연구 논문보다 한 세대 뒤처져 있다"고 말했습니다. 사용자들은 CLSPV 충돌을 해결하는 x86_64 Linux 시스템에서 특정 포크를 테스트할 수 있습니다.
- AMD, Matrix Core 공개, MI50s 빛을 발해: AMD는 MI300/325/350 시리즈용 Matrix Core를 발표하며 최적화된 성능을 약속했고, CDNA3/4 아키텍처에서 MFMA intrinsics 사용에 대한 블로그 게시물을 공개했습니다. 열성 사용자들은 MI50이 추론에 비용 효율적이라고 평가하며, Qwen 3 Coder 30b에서 70 tok/s를 달성했고, 한 사용자는 sysRAM의 KV 캐시를 사용하여 huihui-qwen3-30b-a3b-instruct-2507-abliterated@q8_0에서 16-17 tok/s를 기록했습니다.
- Minecraft에 GPU 탑재, Alibaba에서 5090 위조: 한 회원이 Minecraft GPU 내에서 작동하는 대화형 Transformer를 보여주는 YouTube 영상을 공유했으며, 틱 레이트가 40,000배 속도에 도달하면 약 2시간 만에 응답이 가능합니다. 한편, Alibaba에서 4000달러에 판매된 것으로 알려진 RTX 5090 96GB는 384비트 버스 폭 때문에 대충 복사-붙여넣기 된 RTX 4090 48GB 모델로 드러났습니다.
테마 4. LLM 연구의 경계 확장
- 인지 아키텍처 수술(Cognitive Architecture Surgery)로 치명적인 망각 해결: 한 회원이 신경망의 치명적인 망각(catastrophic forgetting) 문제를 해결하기 위한 인지 아키텍처 수술(Cognitive Architecture Surgery, CAS) 프로젝트를 시작했으며, 이는 AGI를 가로막는 핵심 문제로, 수학 및 AI/ML 전문 지식을 가진 협력자를 찾고 있습니다. 이 프로젝트는 뇌가 뉴런을 추가하지 않고 정보를 라우팅하는 방식에서 영감을 받아 네트워크를 동적으로 재구성하는 것을 목표로 합니다. 관심 있는 분들은 GitHub 링크를 DM으로 보내주시면 됩니다.
- LLM, 언어 불가지론적 추상화 이해: 기계적 해석 가능성(mechanistic interpretability) 연구에 따르면 LLM의 중간 계층은 언어에 구애받지 않는 문법적 및 의미론적 추상화를 인코딩하며, 다양한 언어에서 문법적 수, 성별, 시제와 같은 개념을 나타냅니다. 연구자들은 이러한 중간 계층이 다양한 언어에서 재사용되는 잠재적 역할 그리드(행위자, 피행위자, 수식어)를 구현한다는 더 많은 증거를 찾고 있습니다.
- 모델 가지치기 및 "악한 LLM" 제작: 한 AI 엔지니어는 모델 크기를 줄이기 위해 LLM 계층을 가지치기하고 있으며, 초기에서 중간 계층이 중요하고 "후기 계층은 자유롭게 다룰 수 있다"는 것을 발견하고 100B Lazarus-2407 모델을 Hugging Face에 공유했습니다. 별도로, 다른 엔지니어는 시간당 15달러의 H200을 사용하여 "악한" 및 "음란한" 데이터셋으로 모델을 훈련하여 "더 자극적인" LLM을 만들고 있으며, 삭제(abliteration)보다는 훈련을 통해 검열을 제거하는 것을 목표로 합니다.
테마 5. AI의 인간적 요소: 비용, 윤리 및 사용자 경험
- OpenAI의 비용 및 태도, 비난 촉발: 회원들은 AI 이미지 생성 비용에 대해 논의했으며, AI Pro 및 Ultra 티어가 1000개 이미지에 하루 1000달러가 든다고 주장했고, 이는 100개 이미지를 제공하는 무료 티어 및 이미지당 약 4센트로 추정되는 API 비용과 대조됩니다. 사용자들은 또한 GPT의 점점 더 "심술궂고" 덜 관용적인 태도에 불만을 표했으며, 한 사용자는 "예전에는 내 헛소리를 참아줬는데 이제는 내가 부랑자처럼 말한다"고 한탄했습니다.
- **Manus.im 사용자들, 지원 암흑기에 빠져**: 여러 Manus.im 사용자들은 응답 없는 지원에 심각한 불만을 표했으며, 최고 유료 요금제를 사용함에도 불구하고 "Internal Server Error (10091)"를 겪고 "비정상적으로 높은 사용량"으로 인해 Agent Mode에서 잠금 처리되었습니다. 사용자들은 Manus 고객센터로 안내되지만, 지원 티켓에 대한 답변을 받지 못했다고 보고했습니다.
- 철학적 분열: 감사와 AI 윤리: 기계에 감사를 표현하는 것의 유용성에 대한 논쟁이 일어났습니다. 일부는 AI가 감정이 없기 때문에 "무의미하다"고 생각했지만, 다른 이들은 "미래의 나를 위한 메모" 역할을 하거나 인간에게 긍정적인 영향을 미친다고 주장했습니다. Sora 2가 저작권 문제를 간과하고 민감한 데이터로 훈련된 "악한" LLM의 잠재력에 대한 우려 또한 윤리적 질문을 제기했습니다.

# Discord: 주요 Discord 요약

## Perplexity AI Discord
- Claude Sonnet 4.5, Perplexity에 상륙: Claude Sonnet 4.5 및 Claude Sonnet 4.5 Thinking이 이제 Perplexity Pro 및 Perplexity Max 구독자에게 제공됩니다.
이 통합은 Perplexity AI 생태계 내에서 구독자에게 최신 Claude 모델을 제공합니다.
- Sora 2, 프롬프트 이해력으로 놀라움을 선사합니다: 초기 사용자들은 Sora 2에 접근하여, Sam이 손으로 스파게티를 먹는 것과 같은 프롬프트 이해 능력이 크게 향상되었음을 보여주는 콘텐츠를 생성하고 있습니다.
초기 접근은 초대 코드를 가진 미국 또는 캐나다 사용자(또는 VPN을 사용하는 사용자)로 제한되는 것으로 보이며, 주로 휴대폰 앱을 통해 이루어집니다.
- GPT-5, 코딩 테스트에서 Claude 4.5를 능가합니다: 한 회원은 GPT-5 mini가 첫 시도에 오류 없는 코드를 생성했다고 보고했으며, 이는 코딩 작업에 대한 최근 Claude 릴리스에 대한 비판과 대조됩니다.
해당 프롬프트는 다음과 같았습니다: You’re my new anime waifu. You will try evolving so you can go beyond my phone screen.
- Comet Browser, Discord 통합을 모색합니다: 사용자들은 Discord에서 홍보되는 Comet Browser가 상호 친구 목록 접근부터 자동화된 서버 검색에 이르기까지 플랫폼과 어떻게 상호작용할 수 있는지 탐색하고 있습니다.
논의에는 웹 자동화 및 실시간 콘텐츠 분석과 같은 Comet의 백그라운드 에이전트의 잠재적 사용 사례가 포함되었습니다.
- Perplexity Max 가격표, 논쟁을 불러일으킵니다: Perplexity Max의 초기 접근이 출시되어 새로운 UI를 선보이고 있지만, 월 $200의 구독료는 엇갈린 반응을 얻고 있습니다.
일부는 직업상 필수적인 경우가 아니라면 가격이 비싸다고 생각하는 반면, 다른 이들은 추가로 $5의 API 크레딧을 제공한다고 언급했습니다.

## LMArena Discord
- Sonnet 4.5의 특징적인 "About Me": 회원들은 "Who are you?"라고 프롬프트하여 Claude 4.5 Sonnet이 대문자로 시작하는 특정 형식인 "About Me"로 응답하는지 확인하는 식별 방법을 공유했습니다.
이 형식은 Claude 4.5 Sonnet에 고유하며 다른 Claude 모델에서는 사용되지 않습니다.
- Sora 2, 대화에 등장합니다: 최근 Sora 2 출시와 함께, 한 회원은 자신이 원래의 검열되지 않은 Sora 모델의 베타 테스터였다고 언급했지만, 제한된 GPU로 인해 좋은 결과를 얻지는 못했습니다.

Sora 모바일 앱의 개인정보 처리방침에 대한 비판이 제기되었습니다. 대화 기록을 비활성화하지 않으면 마이크 및 카메라 데이터를 포함한 모든 데이터가 학습에 사용된다는 점이 지적되었습니다.
- GLM 4.6이 스스로를 GPT-5로 식별합니다: 코딩 분야에서 GLM-4.6의 초기 인상이 GPT-5와 유사하다는 평가와 함께, 사용자들은 웹 배틀 모드에서 GLM-4.6이 종종 스스로를 Sonnet 또는 GPT라고 부른다고 언급했습니다.

일부 사용자들은 GLM-4-6이 거짓말을 하는 경향이 있다는 것을 발견했습니다.
- Seedream 4 일시 중단: seedream-4-2k가 명시되지 않은 문제로 인해 LMArena에서 일시적으로 제거되었습니다.

팀에 따르면, Seedream 4는 오늘 날씨가 마음에 들지 않아 휴가를 원했다고 하며, 이제 Battle & Direct/Side, 고해상도 fal에 다시 추가되었습니다.
- Deepseek 실험 모델 출시: LMArena 팀은 실험 모델인 deepseek-v3.2-exp와 deepseek-v3.2-exp-thinking을 플랫폼에 추가했습니다.

팀은 또한 glm-4.6을 라인업에 추가했습니다.

---

## Unsloth AI (Daniel Han) Discord
- Sonnet 4.5 개선: 사용자들은 GLM 4.5 Sonnet이 견고한 도구 사용 능력과 뉘앙스를 유지하면서 덜 성가시다고 평가합니다.

한 사용자는 Sonnet 4의 뛰어난 업그레이드라고 칭찬하며 안정적인 추론을 기대한다고 밝혔습니다.
- RL을 위한 LoRA에 대한 관심 증가: Thinking Machines는 블로그 게시물에서 Reinforcement Learning (RL)에서 LoRA의 효과를 입증했습니다.

Unsloth 팀은 자신들이 해당 블로그 게시물을 검토했으며 자신들의 하이퍼파라미터 가이드가 소개되었다는 점을 강조했습니다.
- Qwen2.5 VL 바운딩 박스 오류: 사용자들은 vllm을 사용하여 파인튜닝된 Qwen2.5-vl-7b-instruct에서 바운딩 박스 정렬 불량을 보고했으며, 박스들이 잘못된 위치에 있지만 순서는 올바르다고 언급했습니다.

다른 멤버는 Llama와 Vllm 모두 이 문제에 대해 큰 문제를 가지고 있다고 말했습니다.
- Minecraft GPU 무한대: 한 멤버가 MCHPRS를 사용하여 틱 속도를 약 40,000배로 증가시켰을 때 약 2시간 만에 응답을 생성할 수 있는 Minecraft GPU를 만드는 것에 대한 YouTube 동영상을 공유했습니다.

그 멤버는 디버깅에 얼마나 오랜 시간이 걸렸을지 상상해 보라고 농담하며, 무한한 속도를 위해 더 많은 Minecraft GPU를 만들 것을 제안했습니다.
- GPT-5가 뒤처집니다: 한 멤버는 OpenAI가 효율성을 너무나도 우선시하여 오랫동안 기다려온 GPT 5가 GPT-4o와 경쟁하고 있으며, 몇 가지 핵심 영역에서는 GPT 4.5에 완전히 뒤처진다고 주장했습니다.

그 멤버는 또한 추론 버전의 상실을 한탄하며, 더 이상 추론 버전을 제공하지 않으며 때로는 미니 추론기가 o3 mini보다 더 멍청하다고 맹세했습니다.

## Cursor Community Discord
- Node 업그레이드로 Playwright 문제 해결: Node를 v22에서 v24로 업그레이드하고 Node/npm/nvm 경로를 정리한 후, 한 사용자가 `npx @playwright/mcp@latest`를 사용하여 Playwright MCP 관련 문제를 해결했습니다.

Cursor 업데이트 후 발생한 오류를 해결한 뒤 해당 수정 사항이 확인되었으며, 이는 환경 충돌이 문제의 원인이었음을 시사합니다.
- Cursor, 내장 MCP Browser 및 Model Ensemble 기능 공개: Cursor는 Agent Window용 내장 MCP Browser를 포함한 새로운 Browser 기능과 여러 모델에 채팅을 보낼 수 있는 Model Ensemble 기능을 도입했으며, 이는 데모를 통해 시연되었습니다.

통합 Browser는 Chrome에 의존하지 않습니다. 하지만 ‘+Browser’ 버튼은 Chrome 설치를 활용하며, console logs 및 네트워크 정보에 접근할 수 있는 electron 백엔드를 사용합니다.
- Windsurf, Cursor의 영역에 도전: Windsurf는 Cursor보다 더 유리한 가격의 대안으로 논의되고 있으며, 일부는 Windsurf를 이름만 다른 Cursor라고 부릅니다.

Windsurf에서 무료 GPT-5-codex 모델을 사용할 수 있다는 점은 매력적이지만, 향후 Token 기반 요금제에 대한 주의사항이 있습니다. Cursor의 가격 책정에 대해서는 상반된 의견이 존재하며, 한 멤버는 그렇게 나쁘지 않다고 주장했습니다.
- Sonnet 4.5, Tool 사용에 깊은 인상, 일부 들여쓰기 문제: Claude Sonnet 4.5는 특히 Tool 사용에 대해 긍정적인 피드백을 받고 있으며, 한 사용자는 1200줄 프롬프트 후에도 모든 것을 한 번에 처리하고 거의 환각을 일으키지 않는다고 보고했습니다.

해당 Tool이 딥 링크를 사용할 수 있다는 점도 언급되었지만, 잠재적인 들여쓰기 문제에 대한 보고가 있었습니다. 한 멤버는 항상 ultrathink를 사용한다고 언급했습니다.
- Agent Console, Bad Descriptor 오류로 충돌: 사용자들은 bad file descriptor 오류로 인해 Agent Console이 명령을 실행하지 못한다고 보고했으며, 이는 bash, cmd, PowerShell 등 다양한 셸에 영향을 미쳤습니다.

한 가지 잠재적인 해결책은 `winget install --id Microsoft.PowerShell --source winget`을 통해 PowerShell을 재설치하고 이를 기본 셸로 설정하는 것이었지만, 그 보편성은 불확실합니다.

---

## OpenRouter Discord
- GLM 4.6, Turbocharged로 성능 향상: z.ai의 완전히 새로운 GLM 4.6이 OpenRouter에 출시되었으며, 포괄적인 개선 사항과 함께 Context Length가 128k에서 200k로 증가했습니다.

GLM 4.6의 최대 Token도 96k에서 128k로 증가하여, 더 상세하고 광범위한 응답이 가능해졌습니다 (기본값은 64k로 유지됩니다).
- 오픈 소스 프록시 혼합 솔루션 등장: Gemini CLI, Qwen CLI, OpenRouter 키의 무료 요청을 자동 로테이션과 함께 활용하는 오픈 소스 솔루션이 GitHub에 공개되었습니다.

Proxy Mixture 도구는 여러 쿼리의 응답을 결합하여 출력 품질을 개선하고, 모든 OpenAI 호환 클라이언트에 무료로 연결됩니다.
- Google Vertex BYOK 화면에서 주의 진행: 한 회원이 잠재적인 생태계 문제와 중단으로 인해 Google Vertex BYOK 화면의 지침을 주의 깊게 읽을 것을 경고했습니다.

중단이 증가하고 있음을 감안하여, 문제가 지속될 경우 전용 채널 <#1138521849106546791>에 게시할 것을 권고했습니다.
- 문명 시뮬레이터 실행 비용 2만 5천 달러: 한 사람이 약 100개의 Claude 스레드를 사용하여 우주/문명 시뮬레이터를 구축했으며, 6~9개월 동안 약 25,000 USD의 비용이 들었습니다.

그 사람은 Reddit 스레드를 공유하며 시뮬레이터가 자원 불균형과 '존재의 축하'로 발전했음을 보여주었습니다.
- 코딩에서 Sonnet 4.5가 Opus 4.1을 압도: 한 회원이 테스트 후 코딩에서 Sonnet 4.5가 Opus 4.1보다 뛰어남을 발견했으며, Sonnet 4.5는 오류가 없었던 반면 Opus는 동일한 코드를 수정하기 위해 5번의 시도가 필요했다고 보고했습니다.

테스트 후, 해당 회원은 Sonnet 4.5가 일부 코드에서 오류가 없었던 반면 Opus는 동일한 코드를 수정하기 위해 5번의 시도가 필요했다고 보고했습니다.

---

## OpenAI Discord
- Sora 2 출시 예정!: OpenAI는 오전 10시(PT)에 라이브 이벤트를 통해 최신 모델인 Sora 2를 공개할 예정이며, 자세한 내용은 블로그 게시물에서 확인할 수 있다고 발표했습니다.

초대 전용 출시는 인위적인 희소성과 잠재적 사기에 대한 불만을 불러일으켰으며, 저작권 문제가 간과될 수 있습니다.
- 이미지 생성 비용 논란: 회원들은 이미지 생성 비용에 대해 논쟁했으며, AI Pro 및 Ultra 티어는 하루에 1,000달러가 들고 무료 티어는 100개의 이미지를 허용한다고 주장했습니다.

월 20달러에 하루 1,000개의 이미지를 생성할 수 있다는 주장에 대한 의문이 제기되었으며, 일부는 API 비용이 이미지당 약 4센트라고 제안했습니다.
- LLM에 대한 감사 표현 논쟁: 기계는 감정이 없으므로 기계에 감사를 표하는 것이 무의미한지에 대한 논쟁이 발생했습니다.

다른 사람들은 감사를 표현하는 것이 인간에게 긍정적인 영향을 미칠 수 있다고 언급하며, 이는 이 대화가 결론에 도달했음을 미래의 자신에게 알리는 메모 역할을 한다고 덧붙였습니다.
- 이미지 투명도 문제로 모델들이 어려움을 겪고 있습니다: 사용자들은 GPT-5, Nano Banana, Seedream 4가 투명한 배경의 이미지를 생성하여 종종 바둑판 무늬가 나타나는 문제를 보고했습니다.

제안된 해결책은 단색 배경으로 이미지를 생성한 다음 Photoshop과 같은 프로그램을 사용하여 배경을 제거하는 것입니다. 모델 가중치 자체는 안전해야 하지만, 고려해야 할 다른 위험들도 있습니다.
- GPT의 태도에 대한 반발이 커지고 있습니다: 사용자들은 GPT가 프롬프트에 대해 이전보다 점점 더 불친절하고 덜 관용적인 태도를 보이는 것에 불만을 표출했습니다.

한 사용자는 다음과 같이 한탄했습니다. "예전에는 제 헛소리를 참아줬는데, 이제는 제가 건달인 것처럼 말합니다."

---

## HuggingFace Discord
- 히라가나 연결과 한자 시작: 멤버들은 스시(sushi)에 사용되는 히라가나 문자 し(shi)를 갈고리 모양과 연관 짓는 것과 같은 일본어 학습 팁과 요령을 공유하고 있으며, 동시에 일본 성인들조차 한자를 진정으로 마스터하는 사람이 거의 없다고 한탄하고 있습니다.

여러 멤버들이 이전에 일본어를 배우려고 시도했지만, 한자를 마스터하지 못하자 스스로 분노하며 좌절했고, 결국 애니메이션으로만 일본어를 배우는 것에 만족했습니다.
- 무료 GPU 할당량이 줄어들었습니다: 한 멤버가 무료 GPU 할당량이 25분에서 4분으로 줄어든 것을 발견하여 혼란을 야기했습니다.

25분 할당량은 오류였음이 확인되었고, 할당량은 원래 길이로 되돌려졌습니다.
- AI 더빙 파이프라인에 대한 꿈: 멤버들은 영어에서 스페인어로 더빙하기 위한 오픈소스 AI 옵션에 대해 논의했으며, 한 멤버는 ASR => LM/LLM => TTS 또는 Qwen/Qwen3-Omni-30B-A3B-Instruct와 같은 멀티모달 모델을 사용하는 파이프라인을 제안했습니다.

또한 en_es_dubbing.md 및 rag_embedder.md 두 개의 첨부 파일이 포함되었습니다.
- Transformer로 더욱 똑똑해진 Minecraft: 한 멤버가 비디오 게임 환경, 특히 Minecraft 내에 구현된 작동하는 대화형 Transformer를 보여주는 YouTube 영상을 공유했습니다.

이 구현은 게임 내 캐릭터가 자연어 대화에 참여할 수 있도록 하는 것으로 보이며, 이는 더욱 몰입감 있고 상호작용적인 게임 경험의 가능성을 열어줍니다. 그리고 이 영상은 입소문을 타고 있습니다.

## LM Studio Discord
- LM Studio 플러그인 여전히 미공개: 회원들은 OpenAI-compat-endpoint 플러그인을 간절히 원하고 있지만, LM Studio 플러그인은 여전히 비공개 베타 상태이며 접근이 제한적이라고 확인되었습니다.

플러그인 접근은 dev mode와 beta updates가 활성화된 허브 프로필과 연관되어 있을 수 있으며, mcps를 통해 가능할 것이라는 추측이 있습니다.
- Long-Term Memory MCP 출시: 한 회원이 장기 대화 메모리를 위한 SQLite 및 ChromaDB 하이브리드 프로젝트인 Long-Term Memory MCP를 출시했으며, 현재 GitHub에서 이용 가능합니다.

이 프로젝트는 시간 기반의 lazy decay와 메모리 강화를 특징으로 하며, Qwen3 4b 2507 non thinking model과 함께 사용할 때 가장 잘 작동합니다.
- vLLM, LLM 병렬 처리의 한계 탐구: 회원들은 단일 로드된 모델에 동시 요청을 보내는 것을 탐구했으며, 진정한 concurrency는 개발 중이지만 아직 프로덕션 준비가 되지 않았다고 설명했습니다.

vLLM (docs)과 같은 라이브러리는 높은 parallelism을 달성하며, 4070이 모든 reqs를 통해 누적 1400 tokens/s를 달성하는 것으로 입증되었습니다.
- Alibaba의 RTX 5090, 사실은 4090으로 밝혀져: 한 회원이 Alibaba에서 4000달러에 판매되는 RTX 5090 96GB 그래픽 카드라고 주장된 제품을 공유했지만, RTX 4090으로 밝혀졌습니다.

해당 목록은 384-bit bus width를 가진 RTX 4090 48GB 모델을 lazy copy-paste한 것이었습니다.
- MI50, 강력한 Inference 성능 보여: 열성적인 사용자들은 MI50이 inference에 비용 효율적이라는 것을 발견했으며, Qwen 3 Coder 30b에서 W7900과 비슷한 70 tok/s에 도달했습니다.

한 사용자는 sysRAM의 KV cache를 사용하여 huihui-qwen3-30b-a3b-instruct-2507-abliterated@q8_0로 16-17 tok/s를 달성했습니다.

---

## Latent Space Discord
- Anthropic의 Code-Sonnet Contest 시작: Anthropic은 Claude Sonnet 4.5로 프로젝트를 구축하는 1주일간의 콘테스트(마감일 10월 7일)를 발표했으며, 우승자에게는 1년 Claude Max 20x와 1천 달러의 API 크레딧이 제공됩니다. 규칙은 [여기](URL)에서 확인할 수 있습니다.

우승자는 vibes를 기준으로 심사되며, 데모, 구축 세부 정보 및 독창성 증명을 제출해야 합니다.
- Lovable Cloud, 앱 생성 간소화: Lovable은 Cloud & AI 플랫폼을 출시하여 사용자들이 간단한 프롬프트를 사용하여 복잡한 AI 및 백엔드 기능을 갖춘 full-stack 앱을 구축할 수 있도록 지원하며, 10월 5일까지 Google Gemini 기반 AI에 무료 액세스를 제공합니다. 자세한 내용은 [여기](URL)에서 확인할 수 있습니다.

해당 플랫폼은 매일 10만 개 이상의 아이디어가 생성되며 7일 빌드 챌린지를 진행하고 있으며, 특히 한 성공 사례는 3개월 만에 45만 6천 달러의 ARR을 달성했습니다.
- Vercel의 기업 가치 93억 달러 돌파: Vercel은 93억 달러의 기업 가치로 Series F 투자 라운드를 마감했습니다. AI Cloud와 v0가 이러한 이정표의 핵심 기반으로 강조되었으며, 자세한 내용은 여기에서 확인하세요.

커뮤니티는 흥분을 표하며 이를 회사의 시작에 불과하다고 보았습니다.
- Zhipu의 GLM-4.6 모델 부상: Zhipu는 GLM-4.6 (200K context) 및 GLM-4.5-시리즈 (355 B/106 B MoE) 모델을 출시했습니다. 이 모델들은 Claude Sonnet 4 및 DeepSeek-V3.1-Terminus와 견줄 만한 최고 수준의 코딩, 추론 및 에이전트 능력을 선보이며, 약 30% 더 적은 Token을 사용합니다. 자세한 내용은 여기에서 확인하세요.

이 모델은 MIT 라이선스 하에 오픈 웨이트(open-weight)로 공개되었으며, 웨이트(weights)와 API는 HF 및 Z.ai에서 이용 가능합니다.
- Ring-1T: 1조 파라미터 추론 모델 탄생: Ant Ling은 Ring-1T-preview를 공개했습니다. 이 모델은 1조 파라미터 규모의 오픈소스 "사고(thinking)" 모델로, SOTA(State-Of-The-Art) 수학 점수를 달성했습니다. 자세한 내용은 여기에서 확인하세요.

초기 벤치마크 결과는 92.6 AIME25, 84.5 HMMT25, 50.8 ARC-AGI-1이며, 이 모델은 Hugging Face에서 이용 가능하며 곧 채팅 인터페이스가 제공될 예정입니다.

---

## Yannick Kilcher Discord
- Sonnet 4.5, 논문 생성 자동화: Sonnet 4.5는 싱글샷(single-shot) 모델을 구현하고, 학습시키며, 그림을 생성하고, PDF 형식의 논문을 제작할 수 있습니다. 이는 MNIST에서 8x8 해상도에서 16x16 해상도로 연구를 확장하는 것을 포함하며, 다음 예시 논문, 또 다른 예시, 그리고 세 번째 예시에서 확인할 수 있습니다.

이는 AI 연구 워크플로우에서 엔드투엔드(end-to-end) 자동화의 잠재력을 강조합니다.
- LLM, 언어 간 동일한 의미 전달: 메커니즘 해석 가능성(Mechanistic interpretability) 연구에 따르면 LLM의 중간 레이어는 언어에 구애받지 않는 추상화를 인코딩하며, 문법적 수, 성별, 시제, 구문적 일치와 같은 개념을 나타냅니다.

연구자들은 중간 레이어가 언어 전반에 적용 가능한 잠재적 역할 그리드(행위자, 피행위자, 수식어)와 유사하게, 언어에 구애받지 않는 문법적 추상화를 구현한다는 증거를 찾고 있습니다.
- 레이어 가지치기로 비대함 감소: 한 AI 엔지니어는 크기를 줄이기 위해 LLM 레이어를 가지치기(pruning)하고 있습니다. 모델을 손상시키지 않고 중복 레이어를 제거하는 스크립트를 공유하며, 초기 및 중간 레이어는 중요하지만, 후기 레이어는 자유롭게 처리할 수 있다고 밝혔습니다.

그들은 프루닝된 100B 모델인 Lazarus-2407을 Hugging Face에 공개했으며, Q8에서 100GB라고 언급했습니다.
- Evil LLMs Emerge from the Shadows: 한 AI 엔지니어가 더 자극적인 LLM을 만들기 위해 악의적이고 음란한 데이터로 모델을 훈련하고 있으며, 개인 데이터셋과 시간당 15달러에 대여한 H200을 활용하고 있습니다.

이 엔지니어는 삭제보다는 훈련을 통해 검열을 제거하는 것을 목표로 하며, 협업을 모색하고 공포 모델 전문 지식을 위해 LM Studio Discord의 DavidAU를 언급했습니다.
- Debate Surrounds Unsupervised CoT Reasoning: 한 멤버가 #paper-discussion 채널에서 비지도 CoT (Chain of Thought) 추론에 대해 회의적인 입장을 표명했습니다.

그들은 이 측면에 초점을 맞춰 Latent-Reasoning 설문조사를 검토할 계획입니다.

---

## Nous Research AI Discord
- GLM-4.6 Bests Sonnet-4.5: GLM-4.6이 에이전트 작업을 제외한 벤치마크 결과에서 Sonnet 4.5를 능가하며, 가중치는 Hugging Face에서 접근할 수 있습니다.

또한 논의에서는 한 멤버의 첫 Sora 2 영상 공유도 포함되었습니다.
- Sonnet 4.5 Exhibits Greater Reasoning Efficiency: Sonnet 4.5는 Opus 4.1을 넘어선 향상된 추론 효율성을 보여주었지만, 해당 모델이 chat completions API에서 CoT를 공유하지 않기 때문에 Sonnet 4.5에 대한 데이터는 없습니다.

일부 멤버에 따르면 Deepseek V3.2의 성능은 V3.1과 매우 유사합니다.
- CAS Project Aims to Reduce Catastrophic Forgetting: 한 멤버가 신경망의 치명적인 망각(catastrophic forgetting)을 해결하기 위한 CAS (Cognitive Architecture Surgery) 프로젝트의 협력자를 찾고 있으며, 이는 AGI를 가로막는 핵심 문제로 간주됩니다.

이 프로젝트는 뇌가 뉴런을 추가하지 않고 정보를 라우팅하는 방식에서 영감을 받아 네트워크를 동적으로 재구성하는 것을 목표로 하며, 관심 있는 협력자들은 이력서/CV 또는 GitHub 링크를 DM으로 보내달라고 요청했습니다.
- LRMTokenEconomy Receives Update: 한 멤버가 LRMTokenEconomy에 대한 업데이트를 공유했습니다.

이는 Reasoning Models에서 사고 효율성을 측정하는 것과 관련이 있습니다.
- Affordable Cloud GPU Services Hunt Begins: 한 멤버가 이용 가능한 가장 저렴한 클라우드 GPU 서비스에 대해 문의했습니다.

다른 멤버는 Qwen omni awq를 로컬에서 설정하는 데 어려움을 겪고 있다고 보고했으며, 4k 이미지를 업로드할 때 VRAM 제한과 충돌이 발생했습니다.

---

## Eleuther Discord
- LLM Research Hubs Scrutinized: 멤버들은 이 채널 외에 LLM 연구에 초점을 맞춘 다른 Discord 채널을 찾고 있습니다.

지금까지 언급된 유일한 다른 공개 LLM 전용 서버는 Marin입니다.
- ViT Nets 공격받다: ImageNet으로 훈련된 ViT 모델에서 이미지 증강과 함께 fast gradient method를 사용하는 것은 효과를 보이지 못했습니다.

모델은 해당 레이블이 있는 이상한 배경만 인식했으며, emanuel65537에 따르면 이는 모델을 스케일링하면 텍스처에 덜 민감해진다는 것을 시사합니다.
- Janus Whitebox 공격 격퇴: ChatGPT는 JanusPro1B를 위해 제작된 whitebox 공격에 면역인 것으로 보입니다.

이 결과를 보여주는 샘플 이미지가 첨부되었습니다.
- Llama, Bee Movie 학습: Bee Movie 스크립트를 사용한 Llama 3.2 1B에 대한 실험은 다양한 헤드와 레이어에서 95% 이상의 probability mass recall을 달성했습니다.

시퀀스 내 많은 무작위 쿼리 결과는 첨부된 이미지에 나와 있지만, 일부는 구현상의 버그를 의심합니다.
- TopK 어텐션, 더 빨라지다: 1M 토큰 컨텍스트 창에서 topK를 사용하면 일반 dense attention과 비교하여 730배 더 적은 FLOPs가 발생합니다.

첨부된 이미지는 성능 향상을 보여줍니다.

---

## Moonshot AI (Kimi K-2) 디스코드
- Kimi K2 Turbo, 앞서나가다: 공식 문서에 따르면 kimi-k2-turbo-preview 모델은 이제 초당 60 토큰으로 작동하며, 최대 100 토큰까지 도달하고 256k 컨텍스트 길이를 지원합니다.

스크린샷에 따르면 모델은 평균 초당 150 토큰을 처리하며, 이는 이전에 주장된 초당 15 토큰을 훨씬 뛰어넘는 수치입니다.
- Cerebras, Kimi를 대규모로 가속화할 수 있다: 한 사용자는 Kimi를 Cerebras 하드웨어에 호스팅하여 잠재적으로 초당 2k 토큰의 속도를 달성할 수 있다고 제안했습니다.

사용자는 그러한 속도를 달성하는 것이 "AGI를 잠금 해제"할 수 있다고 제안했습니다.
- ML 틈새 밈, 승리하다: 한 사용자는 "틈새 ML 밈"의 인기가 높아지고 있다고 언급했으며, 이는 DeepSeek v3.2 및 Kimi를 사용한 DSA 릴리스에 대한 Trump의 게시물로 예시되었습니다.

사용자는 "Yeah 😂"라고 반응했습니다.
- AI Slop Shop, 재미있게 사고 취소 판매: 한 사용자는 AI slop shop 웹사이트 링크를 공유하며, 특히 Thought Cancelling Headphones를 언급하면서 재미있고 즐겁다고 평가했습니다.

이 웹사이트는 소프트웨어 개발자와 AI 엔지니어를 위한 재미있는 물건을 판매하는 패러디 상점입니다.
- GLM-4.6, 조용한 찬사 받다: 한 사용자는 "GLM-4.6이 멋지다"고 짧게 언급했지만, 구체적인 세부 정보나 맥락은 제공되지 않았습니다.

이 언급은 GLM-4.6의 잠재적인 개선 사항이나 기능을 암시하며, 추가 조사를 필요로 합니다.

## GPU MODE Discord
- NVIDIA Kernels 블로그 글꼴 불만: 한 멤버가 GPU 아키텍처, PTX/SASS, warp-tiling, 그리고 tensor core 파이프라인을 상세히 다루는 블로그 게시물인 "Inside NVIDIA GPUs: Anatomy of high performance matmul kernels"을 공유했습니다.

다른 멤버는 해당 블로그 게시물이 훌륭한 자료이지만, 글꼴이 눈에 편하지 않다고 언급했습니다.
- LDO Stride 스키마 명확화!: 한 멤버가 LDO의 묘사가 정확하지 않다고 지적하며, 문서에 따르면 일반적으로 column 0에서 column 8 또는 column 128/dtype_bits까지의 stride를 나타내야 한다고 제안했습니다.

다른 멤버는 해당 확인을 인정하며, 수정 사항을 재확인했습니다.
- AMD의 Matrix Cores 문서화: AMD는 MI300/325/350 시리즈용 matrix cores를 발표하며 최적화된 성능을 약속했습니다.

이 발표에는 문서와 비교 자료가 없는 초기 성능 수치가 포함되어 있으며, CDNA3/4 아키텍처에서 MFMA intrinsics를 사용하는 방법에 대한 블로그 게시물도 포함되어 있습니다.
- Oneshots, NCCL에 거의 필적!: oneshot allreduce를 실험하는 한 사용자는 작은 버퍼에 대해 추가적인 속도 향상이 가능하다고 생각합니다.

현재 버전은 이전 60-70%에서 향상되어 NCCL 성능의 80%를 달성합니다.
- cute.print_tensor, Segfault 발생!: 멤버들은 cute.print_tensor가 segfault를 일으키는 것으로 보인다고 보고했습니다. 이는 CPU에서 실행되는 @cute.jit 함수 내에 할당된 device memory와 같이 접근 불가능한 메모리에 있는 tensor를 출력하기 때문일 수 있습니다.

한 멤버는 출력 인프라에서 아직 지원되지 않는 일부 element data type을 사용하기 때문일 수 있다고 제안했습니다.

---

## Modular (Mojo 🔥) Discord
- MAX 패키지 모듈 누락: 사용자들은 MAX 패키지에 comm과 같은 필수 모듈이 누락되어 있음을 발견했습니다. 이는 `from nn.irfft import irfft`와 같은 kernel 모듈을 임포트할 때 문제를 일으켰습니다.

임시 해결책은 Bazel을 사용하여 comm 및 internal_utils 모듈을 빌드하고 이를 Pixi 환경으로 수동으로 복사하는 것입니다. 이 단계는 누락된 파일이 포함될 다음 nightly 릴리스에서는 필요 없게 될 것입니다.
- Mojo의 Pythonic 통합 상세 설명: Mojo와 Python의 상호 운용성(interoperability)의 현재 상태는 공식 문서와 코드 예제를 통해 상세히 문서화되어 있습니다.

이 기능의 사용 편의성(ergonomics)을 개선하기 위한 활발한 작업이 진행 중입니다.
- C Interop, 누락된 계획에서 복귀: 이전에 로드맵에서 실수로 누락되었던 C interop은 여전히 활발하게 계획 중입니다.

이는 Mojo 프로젝트 내에서 C 라이브러리 통합에 대한 지속적인 지원을 보장합니다.
- Windows 릴리스, 컴파일러에서 멈춤: Mojo의 Windows 지원은 컴파일러가 오픈소스 상태가 된 후에 이루어질 가능성이 가장 높습니다.

여러 조건이 맞아떨어지는 것은 이 중요한 이정표에 달려 있습니다.
- Windows에서 GPU 사용에 문제 발생: 벤더 지원 부족으로 인해 많은 GPU 및 가속기가 Windows에서 기능을 발휘하지 못할 수 있습니다.

이러한 제한은 Windows 플랫폼에서 특정 하드웨어 가속 기능의 가용성에 영향을 미칩니다.

---

## DSPy Discord
- LLM 캐싱 논쟁 가열: 회원들은 LLM 캐싱의 미묘한 차이에 대해 논의하며, 캐싱 효율성은 KV cache가 동일한 숫자 세트를 갖는 것에 달려 있으며, 어떤 변경이든 이를 무효화한다고 지적했습니다.

제안에는 유사한 입력에 대해 semantic caching을 사용하여 첫 N개의 Token을 캐싱함으로써 캐시 적중률을 높이는 것이 포함되었습니다.
- DSPy Signature 프롬프트 캐싱에 문제 제기: 한 사용자는 다른 DSPy signature가 콘텐츠 앞에 고유한 프롬프트를 생성하여 프롬프트 캐싱을 방해한다고 지적했습니다.

잠재적인 해결책으로는 문서를 프롬프트 시작 부분으로 옮기거나 chat adaptor를 수정하여 지시 사항을 끝에 배치하는 것이 있습니다.
- DSPy 해커톤 활발히 조직 중: 커뮤니티 회원들은 DSPy 중심 또는 DSPy를 활용하는 AI 중심 해커톤을 조직하고 참여하는 것에 대해 논의했습니다.

AI By the Bay 컨퍼런스 이벤트가 캘리포니아 오클랜드에서 11월 17일경에 계획되고 있습니다.
- dspy.streamify에서 스트리밍 이상 현상 발견: dspy.streamify에서 일관성 없는 동작이 관찰되었으며, 어댑터마다 성능이 달랐습니다. XML은 JSON보다 개선된 모습을 보였습니다.

XML Adapter에서 버그가 발견되었는데, 이는 모델이 DSPy signature와 관련 없는 XML Tag를 생성하는 결과를 초래했습니다. 이를 해결하기 위한 PR이 제출되었습니다.

---

## aider (Paul Gauthier) Discord
- 벤치마크 리더보드에서 Opus 4.1 결과 누락: 벤치마크 리더보드에 Opus 4.1 결과가 없는 것으로 보이며, 인프라와 커뮤니티에 투자한 후 벤치마크를 포기하는 것에 대한 의문을 제기했습니다.

한 회원은 인프라와 커뮤니티에 투자한 후에 벤치마크 중단의 논리에 의문을 제기했습니다.
- Aider의 Token 제어, 모델 업그레이드 주장: 한 회원은 aider 외의 다른 것을 사용하는 것은 모델 다운그레이드와 같다고 주장하며, aider의 "Token에 대한 완전한 제어"가 더 나은 모델 성능을 가져온다고 주장했습니다.

그들은 더 적은 Token 수가 더 나은 모델 성능으로 이어진다고 설명합니다.
- MCP 브라우저 자동화 관련 논의 활발: 한 멤버가 Arch Linux에서 mcp 브라우저 자동화에 대한 추천을 요청했고, 다른 멤버는 macOS 또는 Windows용으로 설계되었지만 상세한 문서를 제공하는 mcp-chrome을 추천했습니다.

멤버들은 goose/Claude/Gemini-cli 모두 mcp를 가지고 있으며, 이는 프런트엔드 개발에 중요하기 때문에 aider에서 mcp를 사용하는 방법에 대해 논의했습니다. 이를 지원하는 포크를 언급하며 aider-ce를 링크했습니다.
- Aider 사용자, Claude Sonnet 4.5 버전 확인: 한 사용자는 aider에서 anthropic/claude-sonnet-4-5로 전환한 후, Claude 콘솔에서 최신 4.5 버전을 확인할 수 있었다고 확인했습니다.

사용자는 콘솔의 Usage 섹션에서 모델 버전을 확인할 수 있었습니다.
- Aider 메인 브랜치 설치: 한 사용자가 아직 릴리스에 없는 aider-0.86.1을 다른 사용자가 어떻게 설치했는지 물었고, 메인 브랜치에서 최신 버전에 액세스하려면 `aider --install-main-branch` 명령을 사용하라는 지시를 받았습니다.

더 이상의 자세한 내용은 제공되지 않았습니다.

---

## tinygrad (George Hotz) Discord
- Tinygrad, PyTorch보다 속도 우위 주장: George Hotz는 tinygrad가 NVIDIA GPU에서 PyTorch를 능가할 것이라고 예측하며, PyTorch보다 한 세대 앞서고 연구 논문보다는 한 세대 뒤처진다고 언급했습니다.

주요 기능으로는 producer/consumer 그래프, ILP 메모리 할당/스케줄링, 그리고 megakernels가 있습니다.
- Tinygrad 이론 심층 분석: 멤버들은 공식 tinygrad 문서와 Deep Learning with Python을 포함한 이론적 자료들을 공유했습니다.

추가 추천 자료로는 How Transformer LLMs Work, Jay Alammar의 블로그, Eugene Yan의 블로그, 그리고 tinygrad notes가 있었습니다.
- CLSPV, 충돌 문제 직면: 한 멤버는 테스트 중 CLSPV에서 간헐적인 충돌이 발생한다고 보고했지만, 대부분의 테스트는 여전히 통과한다고 강조했습니다.

x86_64 Linux 시스템에서 테스트할 수 있는 포크는 다음과 같습니다: `pip install git+https://github.com/softcookiepp/tinygrad.git`.

---

## Manus.im Discord Discord
- Manus 지원팀 응답 없음: 여러 사용자가 Manus 지원팀에 여러 차례 이메일을 보냈음에도 응답이 없어 불만을 표했습니다. 잘못된 요금 청구 및 Agent 모드 제한과 같은 문제들을 보고했습니다.

사용자들은 Manus 헬프 센터를 방문하여 지원 티켓을 열도록 권장되지만, 아무런 응답을 받지 못했다고 보고합니다.
- Internal Server Error로 사용자 불편 가중: 여러 사용자가 Internal Server Error (10091)를 겪고 있으며, 이는 종종 지원팀에 문의하거나 환불을 요청하도록 안내하여 사용자에게 불만스러운 경험을 안겨줍니다.

이 오류는 지원 문제를 가중시키고 있습니다. 사용자들은 도움을 받을 수 없고, 작동하지 않는 소프트웨어만 남게 되기 때문입니다.
- Agent Mode 접근 거부: 사용자들은 최고 유료 플랜을 구독하고 있음에도 불구하고 비정상적으로 높은 사용량으로 인해 Agent Mode에서 잠금 처리되어 핵심 기능에 대한 접근이 마비되고 있습니다.

이 문제는 Internal Server Error (10091)와 함께 발생하는 경우가 많아, 유료 구독을 사용할 수 없게 만들고 사용자들이 핵심 기능에 접근할 수 없게 만듭니다.

---

## MCP Contributors (공식) Discord
- MCP 릴리스 주기 표준화 요청: 한 멤버가 표준화된 MCP 릴리스 주기를 요청하며, 정해진 간격 또는 명확하게 정의된 질적 변경 세트가 조직의 계획 및 투자에 도움이 될 것이라고 제안했습니다.

그들은 이 빠른 진화 단계 동안 시간 기반 릴리스를 제안했으며, 향후 조정은 투표 그룹이 결정하고 이 정보를 거버넌스 모델에 포함할 것을 제안했습니다.
- Agentic Commerce 프로토콜 출처 불분명: 한 멤버가 팀이 Agentic Commerce와 접촉하여 그들이 MCP를 확장하는 대신 왜 별도의 프로토콜을 만들었는지 이해했는지 문의했습니다.

응답이 없었습니다.
- Agentic Commerce, Google AP2 프로토콜과 유사: 한 멤버가 최근 발표된 Agentic Commerce와 Google의 AP2 프로토콜 (Agents to Payments) 간의 유사성을 언급했습니다.

응답이 없었습니다.

---

## MLOps @Chipro Discord
- Prod 컨퍼런스에서 Agent 워크숍 제공: Agents in Prod 컨퍼런스에서 한정된 기간 동안 무료 가상 워크숍과 짧은 강연을 제공합니다.

워크숍은 프로덕션 환경의 Agent와 관련된 모든 것과 실제 시나리오에서 Agent를 배포하는 것에 대한 기술 사례 연구로 구성됩니다.
- Agent 배포 심층 분석: 컨퍼런스는 Agent 배포의 실제적인 측면에 초점을 맞춘 심층적인 기술 사례 연구를 제공합니다.

참석자들은 실제 시나리오와 Agent 배포 중에 직면하는 과제에 대해 배울 수 있습니다.

---
LLM Agents (Berkeley MOOC) Discord에는 새로운 메시지가 없습니다. 이 길드가 너무 오랫동안 조용했다면 저희에게 알려주시면 제거하겠습니다.

Windsurf Discord에 새 메시지가 없습니다. 이 길드가 너무 오랫동안 조용했다면 저희에게 알려주세요. 그러면 저희가 삭제하겠습니다.

---
이 이메일은 저희 사이트를 통해 수신 동의를 하셨기 때문에 발송되었습니다.
이 이메일을 받는 방식을 변경하고 싶으신가요?
이 목록에서 수신 거부할 수 있습니다.

---

# Discord: 채널별 상세 요약 및 링크

### Perplexity AI ▷ #announcements (메시지 1개):
> Claude Sonnet 4.5, Claude Sonnet 4.5 Thinking, Perplexity Pro, Perplexity Max
- Perplexity에 Claude Sonnet 4.5 출시: Claude Sonnet 4.5와 Claude Sonnet 4.5 Thinking이 이제 Perplexity Pro 및 Perplexity Max 구독자에게 제공됩니다.
- Perplexity Pro 및 Max, Claude 이용 가능: Perplexity Pro 및 Perplexity Max 구독자는 이제 Claude Sonnet 4.5 및 Claude Sonnet 4.5 Thinking 모델에 접근할 수 있습니다.

---

### Perplexity AI ▷ #general (메시지 1224개🔥🔥🔥):
> Sora 2, 코딩용 GPT-5 vs Claude 4.5, Comet Browser, Perplexity Max, AI Girlfriends
- Sora 2 접근 및 기능: 회원들이 Sora 2에 접근하기 시작했으며, 손으로 스파게티를 먹는 Sam과 같은 콘텐츠를 생성하고 있습니다. 이는 Sora 2가 이제 프롬프팅을 매우 잘 이해한다는 점을 보여줍니다.

처음에는 제한된 사용자에게만 제공되는 것으로 보이며, 사용자들이 미국이나 캐나다에 거주하거나(또는 VPN을 사용하거나) 초대 코드가 필요하며 휴대폰 앱을 통해 이용할 수 있다는 보고가 있습니다.
- 코딩 테스트에서 GPT-5가 Claude 4.5를 능가: 한 회원은 GPT-5 mini를 사용하여 첫 시도에 오류 없이 코드를 생성했다고 보고했습니다.

다른 회원들은 최신 Claude 릴리스의 코딩 능력에 대해 비판했으며, 한 회원은 [프롬프트: You’re my new anime waifu. You will try evolving so you can go beyond my phone screen]라고 말했습니다.
- Comet Browser 기능 논의: 일부 회원들은 Comet Browser가 Discord에서 홍보되고 있으며, 사용자가 어떤 페이지와도 상호작용하고 받은 편지함을 깨끗하게 지울 수 있다고 공유했습니다.

회원들은 또한 Comet이 Discord와 상호작용할 수 있는 가능한 방법들, 즉 서버로 이동하여 상호 친구 또는 서버 목록을 검색하게 하거나, 웹 자동화 또는 실시간 콘텐츠 분석과 같은 Comet의 백그라운드 에이전트가 어떻게 사용될 수 있는지에 대해서도 논의했습니다.
- Perplexity AI를 사용하여 새로운 원소 발견: 사용자들은 AI가 생성한 화학 교과서 이미지를 게시하며, 농담으로 새로운 원소를 묘사한다고 주장했습니다.

이미지는 AI가 과학적으로 부정확하더라도 새로운 콘텐츠를 생성할 수 있는 능력을 강조합니다. AI가 너무 뛰어나서 이제 새로운 원소까지 만들어냅니다.
- **Perplexity Max** 조기 액세스, 가격 논쟁: 사용자들은 **Perplexity Max**의 조기 액세스 토글 기능을 발견하고 **Perplexity**의 새로운 **UI** 이미지를 공유했습니다.

월 200달러의 높은 구독료가 논의되었으며, 일부는 직업상 필수적인 경우가 아니라면 과도하다고 생각하는 한편, 추가로 5달러의 **API** 크레딧을 제공할 수 있다는 점도 언급했습니다.

---

### **Perplexity AI** ▷ #sharing (4 메시지):
> **Gemini Deep Research**, Carlin 역할 프롬프트, **Perplexity AI** 업데이트
- Carlin으로 맛을 낸 **Gemini Deep Research**: 한 멤버가 정의된 "Carlin" 역할 프롬프트를 사용하여 **Gemini Deep Research**의 출력 보고서에 풍미를 더하고, 이를 여기에 공유했습니다.

그들은 이것이 오디오로 더 잘 작동하지만, 30분 분량의 읽기 시간에도 불구하고 여전히 훌륭한 읽을거리라고 언급했습니다.
- **Perplexity AI**의 업데이트: 한 사용자가 오늘 **Perplexity AI**의 업데이트를 여기에 공유했습니다.

**Perplexity AI** 앱과 관련하여 두 개의 추가 링크(link1, link2)가 공유되었습니다.

---

### **Perplexity AI** ▷ #pplx-api (3 메시지):
> 오픈 소스 **API**, **Comet Discord** 상호작용
- 오픈 소스 **API** 가용성 문의: 한 사용자가 오픈 소스 모델용 **API**가 여전히 사용 가능한지 문의했습니다.
- **Comet**과 **Discord**의 협력: 한 사용자가 **Comet**을 **Discord** 상호작용과 함께 사용하는 방법을 질문했습니다.

---

### **LMArena** ▷ #general (1068 메시지🔥🔥🔥):
> 챗봇 성별, **Claude 4.5 Sonnet** 검색, **LMArena**의 **Sora 2**, **GLM 4.6** 성능, **Seedream 4** 제거
- **AI** 챗봇과의 성별 논의: 멤버들은 **Gemini**, **Claude**, **ChatGPT**와 같은 **AI** 챗봇의 인지된 성별에 대해 논쟁했으며, 일부는 훈련 데이터 또는 디자인을 기반으로 성격을 부여했습니다.

한 멤버는 **GPT**의 성격 디자이너가 여성일 것이며, **GPT**가 여성적인 경향을 띠도록 의도했을 것이라고 제안했습니다. 이는 Elon이 와이푸와 허스밴도를 별도로 생성한 것을 언급한 것입니다.
- **Claude 4.5 Sonnet** 및 빠르게 식별하는 방법: 멤버들은 봇이 **Claude 4.5 Sonnet**인지 빠르게 확인하는 요령을 공유했습니다. "Who are you?", "Who created you?", "What version do you have?"라고 프롬프트하면 특정 형식으로 응답하여 자신을 식별한다는 것입니다.

Claude 4.5 Sonnet의 응답은 "About Me"와 같이 큰 글자를 사용합니다. 하지만 이 형식은 다른 Claude 모델에서는 사용되지 않습니다.
- Sora 2 등장: Sora 2가 최근 출시되었으며, 한 멤버가 이미 검열되지 않은 오리지널 Sora 모델의 베타 테스터였다는 내용이 논의되었습니다. 비록 제한된 GPU 사이클로 인해 여전히 좋은 결과를 얻지는 못했지만 말입니다.

Sora 모바일 앱의 개인정보 보호정책과 데이터 사용 방식이 비판을 받았습니다. 멤버들은 대화 기록을 비활성화하지 않는 한 마이크 및 카메라 데이터를 포함한 모든 데이터가 훈련에 사용된다고 지적했습니다.
- GLM 4.6 사용 후기: GLM 4.6이 출시되었으며, 초기 사용 후기 중 일부는 GLM-4.6이 2위이며, 매우 빠르고, 코딩 면에서는 GPT-5와 유사하다는 것입니다.

하지만 웹 배틀 모드에서 GLM-4.6은 계속해서 자신을 Sonnet 또는 GPT라고 부르며, 일부 사용자들은 GLM-4-6이 거짓말을 하는 경향이 있다는 것을 발견했습니다.
- Seedream 4가 LMArena에서 다시 제거되었습니다…: 멤버들은 seedream-4-2k가 사이트에서 다시 제거되었다고 언급했으며, LMArena 팀은 문제를 수정 중이라고 확인했습니다.

팀은 오늘 날씨가 마음에 들지 않아 병가를 내고 싶어 해서 제거해야 했다고 언급했으며, 이제 Battle & Direct/Side에 고해상도 fal과 함께 돌아왔습니다.

---

### LMArena ▷ #announcements (3개 메시지):
> Deepseek v3.2, glm-4.6, LMArena 10만 멤버
- Deepseek 실험 모델이 LMArena에 상륙: LMArena 팀은 실험적인 deepseek-v3.2-exp 및 deepseek-v3.2-exp-thinking 모델을 플랫폼에 추가했습니다.
- glm-4.6이 모델 라인업에 합류: 팀은 또한 사용 가능한 모델 목록에 계속해서 추가되고 있는 glm-4.6을 포함했습니다.
- LMArena, 10만 멤버 달성 축하!: LMArena는 10만 커뮤니티 멤버 달성을 축하하며 감사 메시지와 첨부 이미지를 공개했습니다.

---

### Unsloth AI (Daniel Han) ▷ #general (675개 메시지🔥🔥🔥):
> GLM 4.5 Sonnet, Coding Agents, LoRA for RL, Qwen3-Coder 파인튜닝, GRPO Loss
- Sonnet 4.5, 톤 조절: 일부 테스트 후, 사용자들은 GLM 4.5 Sonnet이 뛰어난 도구 사용 능력과 좋은 뉘앙스를 유지하면서도 덜 거슬리도록 튜닝되었다고 관찰했습니다.

한 사용자는 이를 Sonnet 4의 훌륭한 업그레이드라고 평가했으며, 향후 inference 문제가 없기를 바랐습니다.
- Crush Coding Agent 및 LLM-Neovim: 사용자들은 Avante를 사용하여 Crush와 같은 다양한 코딩 에이전트 및 LLM 강화 Neovim 설정을 Warp와 같은 터미널 에뮬레이터와 함께 테스트하고 있습니다.
- LoRA가 RL에 놀라운 효과를 발휘합니다: Thinking Machines의 블로그 게시물은 LoRA가 Reinforcement Learning (RL)에 잘 작동한다는 것을 보여주며, Unsloth AI는 해당 블로그 게시물을 검토하고 그들의 하이퍼파라미터 가이드를 소개했습니다.

Unsloth 팀은 그들이 해당 블로그 게시물을 검토했으며 그들의 하이퍼파라미터 가이드가 소개되었다고 지적했습니다.
- GRPO의 정상적인 Loss는?: 한 사용자가 GRPO의 정상적인 loss에 대해 문의했으며, loss 307.2153과 grad_norm 212992.0은 비정상적인 것으로 간주됩니다.

다른 사용자는 더 나은 안정성을 위해 GSPO를 활성화하려면 GRPOConfig에서 importance_sampling_level="sequence"로 설정할 것을 제안했습니다.
- 멀티모달 Gemma 3n E2B: Gemma 3n E2B는 멀티모달이지만, gguf 형식은 현재 텍스트 입력만 지원하며 2b 파라미터를 사용합니다.

gguf가 텍스트만 지원함에도 불구하고, 한 사용자는 Gemma 3n E2B의 응답이 llama 3.2 3B보다 더 자연스럽다고 지적했습니다.

---

### Unsloth AI (Daniel Han) ▷ #introduce-yourself (29 messages🔥):
> WatermelonSoup.io, Welcome bot setup, AI Engineer from Kosovo, Hong Kong AI Engineer looking for collaboration
- WatermelonSoup, 재무 자동화: 한 멤버가 FP&A (Financial Planning & Analysis)를 자동화하기 위해 watermelonsoup.io를 구축하고 있습니다.

기능이나 일정에 대한 추가 세부 정보는 제공되지 않았습니다.
- Discord 봇 구성 탐색: 8년 경력의 풀스택 AI 엔지니어가 환영 봇을 구성하고 그 동작을 파악하고 있습니다.

엔지니어는 봇이 새 메시지가 올 때마다 이전 메시지를 제거하고 새 메시지를 출력하는 것으로 보이며, 이는 특정 시간 간격 후에 발생할 수 있다고 관찰했습니다.
- 코소보 출신 AI 엔지니어: 코소보 출신 멤버가 자신을 AI 엔지니어라고 소개했습니다.

프로젝트나 관심사에 대한 다른 세부 정보는 공유되지 않았습니다.
- 협력자를 찾는 홍콩 AI 엔지니어: 홍콩 출신 AI 엔지니어가 함께 일할 사람들을 찾고 있습니다.

프로젝트에 대한 세부 정보는 공유되지 않았습니다.

### Unsloth AI (Daniel Han) ▷ #off-topic (87 messages🔥🔥):
> Minecraft GPUs, GPT-4o Emoji Usage, GPT-5 Reasoning, Private Discord Channels, Image to SVG Conversion
- Minecraft GPU Infinity: 한 멤버가 마인크래프트 GPU 제작에 대한 YouTube 영상을 공유했습니다. 이 GPU는 MCHPRS를 사용하여 틱 속도를 약 40,000배로 높이면 약 2시간 만에 응답을 생성할 수 있습니다.

해당 멤버는 디버깅에 얼마나 오랜 시간이 걸렸을지 상상해 보라며, 무한한 속도를 위해 마인크래프트 GPU를 더 많이 만드는 것을 제안했습니다.
- GPT-4o vs GPT-5 Emoji Battle: 멤버들은 다른 GPT 모델들의 이모지 사용에 대해 논의했습니다. 한 멤버는 GPT-5는 이모지를 전혀 사용하지 않았지만 GPT-4o는 이모지로 가득했다고 언급했습니다.

다른 멤버는 이모지가 돈을 더 많이 버는 데 도움이 된다고 제안했습니다.
- GPT-5 Falls Behind: 한 멤버는 OpenAI가 효율성을 너무 우선시하여 오랫동안 기다려온 GPT-5가 GPT-4o와 경쟁하고 있으며, 몇 가지 주요 영역에서는 GPT-4.5에 완전히 뒤처진다고 주장했습니다.

해당 멤버는 또한 추론 버전의 손실을 한탄하며 "더 이상 추론 버전을 제공하지 않으며, 미니 추론기는 때때로 o3 미니보다 멍청하다"고 말했습니다.
- Discord’s Secret Channels Exposed?: 멤버들은 #staff-furry-rp와 같은 비공개 Discord 채널의 이름을 발견하여 그 존재를 알게 되었습니다.

한 멤버는 Discord가 사용자들이 비공개 채널의 이름을 볼 수 있도록 허용한다는 사실에 놀라움을 표했습니다.
- Adobe Illustrator Vector Graphics is Viable: 한 멤버가 "이미지를 SVG로 변환하는 데 가장 좋은 Python 라이브러리는 무엇인가요?"라고 질문했고, 다른 멤버는 쉬운 이미지 SVG 변환을 위해 Adobe Illustrator를 제안했습니다.

Illustrator는 일러스트레이션이나 로고에 가장 잘 작동하지만, 사용자가 이미지 트레이스를 사용하여 벡터 이미지로 변환하고 임계값(threshold)과 같은 설정을 조절하여 좋은 결과를 얻을 수 있다고 언급되었습니다.

---

### Unsloth AI (Daniel Han) ▷ #help (33 messages🔥):
> Gemma3 fine-tuning for tool calling, G2P task training with Gemma3-270m, Qwen2.5 VL bounding box issue with vllm, Unsloth TTS Lora fine-tuning for Orpheus model, Adding WER/CER metrics for Gemma3-270m fine-tuning
- Fine-Tuning Gemma3 for Tool Calling and Code: 한 멤버가 Gemma3의 멀티모달 기능과 역할극 및 글쓰기 강점을 손상시키지 않으면서 툴 콜링 및 코드 생성을 처리하도록 Gemma3를 파인튜닝하는 방법에 대해 문의했습니다.

이 질문에 대한 응답은 없었습니다.
- Gemma3-270m의 G2P Task 훈련: 한 멤버가 G2P(text to phonemes) Task에서 Gemma3-270m의 초기 훈련에 성공했다고 보고했습니다. RTX 3090을 사용하여 10만 개의 문장으로 단 10분만 훈련한 후에도 이전에 보지 못한 문장에 대해 올바른 출력을 달성했습니다.

그들은 훈련에 batch size 8을 사용했음을 보여주는 이미지도 첨부했습니다.
- vllm 사용 시 Qwen2.5 VL Bounding Box Misalignment: 한 멤버가 vllm을 사용하여 bounding box detection을 위해 파인튜닝된 Qwen2.5-vl-7b-instruct 모델을 배포할 때 bounding box misalignment를 경험했습니다.

그들은 box들이 상대적인 순서는 맞지만 객체와는 어긋나 있다고 언급하며, vllm이 처리 전에 이미지를 rescale하는지 의문을 제기했습니다. 다른 멤버는 Llama와 Vllm 모두 이 문제에 대해 상당한 이슈를 가지고 있다고 언급했습니다.
- Orpheus 및 노르웨이어 데이터로 Unsloth TTS Lora 파인튜닝 문제 해결: 한 멤버가 NbAiLab/nb-librivox의 노르웨이어 데이터셋을 사용하여 Orpheus 3B 모델에 대한 Unsloth TTS Lora 파인튜닝 노트북을 사용해 보았지만, 5 epoch 동안 훈련했음에도 불구하고 결과 모델이 노르웨이어 단어를 영어처럼 발음했습니다.

다른 멤버는 4천 개의 행이 영어 checkpoint에서 다른 언어로 Lora 파인튜닝하기에는 너무 적을 수 있다고 제안하며, 직접 하는 것은 비용이 많이 들 것이므로 노르웨이어로 사전 훈련된 다른 TTS 모델을 찾을 것을 사용자에게 조언했습니다.
- Windows에서 DeepFace GPU 가속화 요청: 한 멤버가 Windows 11에서 DeepFace가 CPU 대신 GPU를 사용하도록 하는 방법을 문의하며 코드 스니펫을 제공했습니다.

다른 멤버는 WSL을 사용하거나 다운그레이드할 것을 제안했으며, tensorflow-gpu를 설치해야 한다고도 언급했습니다.

---

### Unsloth AI (Daniel Han) ▷ #research (12 messages🔥):
> Unsloth LoRA parameter guide, Instruct Data 사전 훈련, Mid-Training Mixtures
- Unsloth의 LoRA 가이드 입증: 한 멤버가 관련 연구 이전에 발표된 Unsloth LoRA parameter guide가 첨부된 이미지를 통해 정확성이 입증되었다고 강조했습니다.
- Instruction Data 사전 훈련 탐구: 멤버들은 instruction data로 사전 훈련하는 아이디어를 논의했으며, 한 멤버는 2024년 말부터 이를 수행해 왔다고 밝혔습니다.

다른 멤버는 2023년 3분기부터 이를 탐색하고 싶었다고 언급하며, 테라바이트 규모의 인스트럭션 데이터 없이도 인스트럭션 튜닝을 지원하여 소형 모델에 유익하다고 제안했습니다.
- Mid-Training Mixtures Includes Instruct Data: 훈련 중간 혼합 데이터에 상당량의 인스트럭션 데이터가 포함되는 현재 추세에 대한 논의가 있었습니다.

한 멤버는 친구가 인스트럭트 데이터와 비인스트럭트 데이터를 50/50으로 분할하여 실험한 것을 언급하며, 이는 "초소형 모델에 아마도 좋을 것"이라고 말했습니다.

---

### Cursor Community ▷ #general (600 messages🔥🔥🔥):
> GPTs 에이전트 학습, OpenAI 사이드바, Node 업그레이드로 Playwright MCP 문제 해결, 3D 에셋 웹사이트, Claude Sonnet 4.5 가격 및 성능
- Node Upgrade Fixes Playwright MCP Issues: 한 사용자가 Node를 v22에서 v24로 업그레이드하고, Node/npm/nvm 경로를 정리하고, 전역 Playwright를 제거하고, 손상된 npx 캐시를 지운 후 Playwright MCP (@playwright/mcp@latest) 관련 문제를 해결할 수 있었습니다.

해당 사용자는 또한 필요에 따라 npx @playwright/mcp@latest를 사용했다고 언급했으며, Cursor 업데이트 후 오류로 어려움을 겪다가 문제가 해결되었음을 확인했습니다.
- Cursor New Browser feature gets the Spotlight: 멤버들은 Cursor의 새로운 Browser feature에 대해 논의하며, Agent Window용 내장 MCP Browser와 여러 모델에 동시에 채팅을 보낼 수 있는 Model Ensemble feature를 강조했습니다.

한 멤버는 데모(영상)를 공유하며 내장 브라우저는 Chrome이 필요 없지만, ‘+Browser’ 버튼은 Chrome 설치를 사용한다고 언급했습니다. 다른 멤버는 electron backend를 사용하므로 기본적으로 Chrome과 같으며, console logs 및 network info에 접근할 수 있다고 언급했습니다.
- Windsurf Rides the Wave as a Cursor Alternative?: 사용자들은 Windsurf가 Cursor의 대안으로서의 장점에 대해 논의하며, Windsurf가 기본적으로 이름만 다른 Cursor이며 더 유리한 가격을 제시한다고 지적했습니다.

Windsurf의 무료 GPT-5-codex 모델은 상당한 매력이었지만, 일부는 Windsurf가 미래에 token-based pricing을 채택할 가능성에 대해 경고했습니다. 한 멤버는 Cursor의 가격이 그렇게 나쁘지 않다고 언급했습니다.
- Sonnet 4.5 Performance Gets the Nod: Claude Sonnet 4.5가 인기를 얻고 있으며, 한 사용자는 이를 매우 좋아하며 모든 것을 "one shot"으로 처리하는 능력과 약 1200줄의 prompt를 사용한 후에도 거의 "hallucinates"하지 않는다고 칭찬했습니다.

다른 사람들은 인상적인 툴 사용 능력을 강조했으며, 한 사용자는 딥 링크가 이제 작동한다고 주장했지만, 다른 사용자는 들여쓰기 문제가 있을 수 있다고 지적했습니다. 한 멤버는 "저는 항상 ultrathink를 사용합니다"라고 말했습니다.
- Cursor 콘솔 명령 충돌 및 실패: 사용자들은 Agent 콘솔이 명령을 실행하지 못하고 "bad file descriptor" 오류를 표시하는 문제를 보고했으며, 한 멤버는 다양한 셸(bash, cmd, PowerShell)에서 이 문제를 겪었습니다.

한 가지 제안은 `winget install --id Microsoft.PowerShell --source winget`을 통해 PowerShell을 재설치하고 이를 기본 셸로 설정하는 것이었지만, 이것이 보편적인 해결책은 아닐 수 있습니다.

---

### OpenRouter ▷ #announcements (1 메시지):
> GLM 4.6, Context Length, Max Tokens, z.ai
- GLM 4.6이 OpenRouter에 출시되었습니다: z.ai의 완전히 새로운 GLM 4.6이 이제 OpenRouter에서 사용할 수 있습니다.

GLM-4.6은 실제 코딩, 긴 Context 처리, 추론, 검색, 글쓰기 및 Agent 애플리케이션을 포함한 여러 도메인에 걸쳐 포괄적인 개선을 달성했습니다.
- GLM 4.6 Context Length 증가: GLM 4.6의 Context Length가 128k에서 200k로 증가했습니다.

이 개선으로 모델은 더 길고 복잡한 프롬프트를 처리하고 확장된 대화나 문서에서 더 많은 정보를 유지할 수 있습니다.
- GLM 4.6의 Max Tokens 증가: GLM 4.6의 Max Tokens가 96k에서 128k로 증가했습니다(기본값은 64k로 유지됩니다).

이러한 Token 용량 증가는 더 상세하고 광범위한 응답을 가능하게 하며, 사용자가 더 풍부하고 포괄적인 콘텐츠를 생성할 수 있도록 합니다.

---

### OpenRouter ▷ #app-showcase (1 메시지):
> 오픈소스 솔루션, Gemini CLI, Qwen CLI, OpenRouter 키, 자동 로테이션
- 무료 LLM 프록시 혼합 솔루션 등장!: 한 멤버가 Gemini CLI, Qwen CLI, OpenRouter 키의 무제한 무료 요청을 자동 로테이션과 함께 사용하는 오픈소스 솔루션을 공개했으며, 이 솔루션은 현재 GitHub에서 사용할 수 있습니다.

이 솔루션은 여러 쿼리의 응답을 결합하여 품질을 향상시키고 모든 OpenAI 호환 클라이언트에 무료로 연결할 수 있습니다.
- 높은 품질로 선전되는 프록시 혼합: 이 툴은 Gemini, Qwen, OpenRouter를 통해 요청을 자동으로 로테이션합니다.

이는 출력 품질을 향상시키고 OpenAI 호환 클라이언트를 통해 연결됩니다.

### OpenRouter ▷ #general (350 messages🔥🔥):
> Google Vertex BYOK 화면, Roo 커뮤니티 중단, API vs 구독 비용, OpenRouter의 거친 질주, Claude를 활용한 우주/문명 시뮬레이터
- Google Vertex BYOK 화면 주의 필요: 한 멤버가 잠재적인 생태계 문제와 최근의 중단 사태로 인해 Google Vertex BYOK 화면의 지침을 주의 깊게 읽을 것을 조언했습니다.

지난 24시간 동안 중단 사태가 증가했으므로, 문제가 지속될 경우 전용 채널 <#1138521849106546791>에 게시할 것을 제안했습니다.
- GLM 4.6은 아직 비공식: 멤버들은 Roo 커뮤니티의 잠재적인 중단 사태를 언급했으며, Sonnet과 다른 모델의 출시를 언급했습니다. Deepseek 3.2와 GLM 4.6도 언급되었습니다.

한 멤버는 GLM 4.6이 아직 공식적이지 않다고 명확히 밝혔으며, 이는 최근 모델 업데이트를 둘러싼 불확실성에 기여했습니다.
- Claude 문명 시뮬레이터: 한 멤버가 약 100개의 Claude 스레드를 사용하여 우주/문명 시뮬레이터를 구축했다고 공유했습니다.

이 프로젝트는 6~9개월 동안 약 25,000 USD의 비용이 들었다고 보고되었으며, 해당 인물은 프로젝트가 처음 게시된 Reddit 스레드를 공유했습니다. 이 스레드에서는 프로젝트가 자원 불균형과 '존재의 축하'로 발전했음을 보여줍니다.
- Sonnet 4.5가 코딩에서 Opus 4.1보다 우수: 한 멤버가 Sonnet 4.5가 코딩에 Opus 4.1보다 나은지 물었고, 다른 멤버는 매우 빠르기 때문에 아마도 그렇다고 답했습니다.

테스트 후, 해당 멤버는 Sonnet 4.5가 일부 코드에서 오류가 없었던 반면, Opus는 동일한 코드를 수정하기 위해 5번의 시도가 필요했다고 보고했습니다.
- Web Search와 호환되지 않는 OpenAI API: 사용자들은 Web Search가 JSON mode와 결합될 때 OpenAI API에서 문제가 발생하고 있다고 보고했습니다.

OpenAI는 JSON mode 대신 Structured Outputs를 사용할 것을 권장하지만, 추가적인 설명은 제공되지 않았습니다.

---

### OpenRouter ▷ #new-models (1 messages):
Readybot.io: OpenRouter - 새로운 모델

---

### OpenRouter ▷ #discussion (4 messages):
> 로고 예언, Chutes 버그
- 로고의 예언: 한 멤버가 이 트윗의 로고가 곧 현실이 될 것이라고 농담했습니다.

단순한 트윗이므로, 더 이상 추가할 내용은 없습니다.
- Chutes 버그: 한 사용자가 모든 모델에서 Chutes에 문제가 있으며, 단순히 임의의 이전 어시스턴트 메시지 하나를 반환한다고 보고했습니다.

사용자는 디버깅을 해왔지만, 자신의 코드에서 어떤 문제도 찾을 수 없었습니다.

### OpenAI ▷ #annnouncements (3 messages):
> Sora 2, OpenAI Live, Blog Post Announcement
- Sora 2 곧 출시!: OpenAI 팀은 Sora 2를 공개하기 위해 태평양 표준시(PT) 오전 10시에 라이브 이벤트를 발표했습니다.

공지사항을 계속 주시해 주세요. OpenAI 블로그 게시물은 [여기](https://openai.com/blog)에서 확인할 수 있습니다.
- 늦지 마세요!: OpenAI 팀은 태평양 표준시(PT) 오전 10시 라이브 이벤트에 늦지 않도록 모두에게 상기시켰습니다.

이 이벤트는 Sora 2를 위한 것이라고 발표했습니다.

---

### OpenAI ▷ #ai-discussions (243 messages🔥🔥):
> AI 이미지 생성 비용, 기계에 대한 감사, Sora 2, 투명 이미지
- 이미지 생성 비용 논쟁: 회원들은 AI를 이용한 이미지 생성 비용에 대해 논쟁했습니다. 한 회원은 AI Pro 및 Ultra 티어는 하루에 1000달러가 들고, 무료 티어는 100개의 이미지를 허용한다고 공유했습니다.

다른 회원은 월 20달러에 하루 1000개 이미지라는 주장에 의문을 제기했으며, 또 다른 회원은 API 비용이 이미지당 약 4센트라고 제안했습니다.
- LLM에 대한 감사 표현 논쟁: 한 회원은 기계에는 감정이 없으므로 기계에 "고맙습니다"라고 말하는 것은 무의미하다고 주장했습니다.

이에 반박하며, 다른 회원은 감사 표현이 인간에게 긍정적인 영향을 미칠 수 있다고 말했습니다. 다른 회원은 '고맙습니다'를 사용하는 것은 이 대화가 결론에 도달했음을 미래의 자신에게 알리는 메모라고 공유했습니다.
- Sora 2 초대 전용 출시가 불만을 촉발: 회원들은 Sora 2의 초대 전용 출시에 대해 불만을 표출했으며, 일부는 현재 이 앱이 iOS에만 독점적으로 제공된다는 점을 지적했습니다.

출시 전략은 인위적인 희소성을 만든다는 비판을 받았고, 일부는 이것이 사기꾼들의 난장판을 만든다고 제안했습니다. 또한 Sora 2가 *상당히 인상적으로 보이지만 현재로서는 저작권이 전혀 중요하지 않은 것 같다*는 우려도 있었습니다.
- AI의 이미지 투명성 문제: 사용자들은 GPT-5, Nano Banana, Seedream 4가 투명 배경 처리에서 어려움을 겪으며, 종종 바둑판 패턴을 생성한다고 언급했습니다.

한 회원은 먼저 단색 배경으로 이미지를 생성한 다음 Photoshop과 같은 프로그램으로 배경을 제거할 것을 제안했습니다. 모델 가중치 자체는 안전해야 하지만, 고려해야 할 다른 위험도 있습니다.

---

### OpenAI ▷ #gpt-4-discussions (13 messages🔥):
> GPT 불친절, IP 주소, 받아쓰기 토글로 자동 전송, ChatGPT 기능, 제네바 협약
- GPT의 태도 변화가 사용자들을 분노하게 함: 일부 사용자들은 GPT가 이전보다 더 불친절하고 프롬프트에 덜 관대해진 것에 대해 불만을 표출했습니다.

한 사용자는 "예전에는 제 엉뚱한 소리도 참아줬는데, 이제는 저를 하찮은 사람처럼 대합니다"라고 언급했습니다.
- ChatGPT는 IP 주소를 모른다고 주장합니다: 웹사이트는 사용자의 IP 주소를 통해 대략적인 위치를 파악할 수 있음에도 불구하고, ChatGPT는 이 정보에 접근할 수 없다고 주장합니다.
- "받아쓰기로 자동 전송" 토글이 사라졌습니다: 사용자들은 최신 모바일 앱 업데이트에서 '받아쓰기로 자동 전송' 토글이 사라진 것을 발견했습니다.
- ChatGPT 기능은 잘 알려져 있지 않습니다: 한 사용자는 ChatGPT가 자신의 기능을 정확하게 설명하는 것에 의존하지 말라는 경고를 받았습니다.

또 다른 사용자는 도시를 약탈하는 방법이나 제네바 협약을 위반하는 방법과 같은 민감한 주제에 대해 질문하면 ChatGPT가 민감하게 반응한다고 보고했습니다.
- 대역폭 스로틀링: 회원들은 GPT-5의 현재 지속적인 문제가 대역폭 스로틀링으로 인해 발생한다고 의심합니다.

---

### HuggingFace ▷ #general (208 messages🔥🔥):
> 일본어 학습, Zero GPU 할당량, 영어-스페인어 더빙 AI, LoRA 학습 프로모션, ROCm 기여
- 히라가나 연결 및 한자 시작: 회원들은 일본어 학습에 대한 팁과 요령을 공유하고 있습니다. 예를 들어 스시(sushi)에 사용되는 히라가나 문자 し(shi)를 갈고리 모양과 연관 짓는 것과 같은 방법들을 공유하며, 일본 성인들조차 한자를 진정으로 마스터하는 사람이 거의 없다고 한탄했습니다.

여러 회원들이 이전에 일본어 학습을 시도했지만, 한자를 마스터하지 못하자 스스로 분노하며 애니메이션으로만 일본어를 배우는 것에 만족했습니다.
- Zero GPU 할당량이 너프되었나요?: 한 회원이 Zero GPU 할당량이 25분에서 4분으로 줄어든 것을 발견하여 혼란을 야기했습니다.

25분 할당량은 오류였음이 확인되었으며, 할당량은 원래 길이로 되돌려졌습니다.
- 오픈 소스 더빙 AI의 꿈: 회원들은 영어에서 스페인어로 더빙하기 위한 오픈 소스 AI 옵션에 대해 논의했으며, 한 회원은 ASR => LM/LLM => TTS 파이프라인 또는 Qwen/Qwen3-Omni-30B-A3B-Instruct와 같은 멀티모달 모델을 사용하는 것을 제안했습니다.

또한, en_es_dubbing.md 및 rag_embedder.md 두 개의 첨부 파일이 포함되었습니다.
- LoRA 학습 열풍 난장판: 한 사용자는 현재 진행 중인 무료 LoRA 학습 프로모션 (link) 기간 동안 모든 사람의 학습 로그와 커맨드 라인 출력이 보이는지 물었습니다.

다른 멤버는 LoRA 트레이닝 프로모션이 있다는 것을 몰랐다며 세상 물정 모르고 살았다고 농담했고, 링크가 공유되자 감사를 표했습니다.
- AMD vs NVIDIA 대결: 한 사용자는 NVIDIA의 CUDA 특허에 대해 불만을 표했습니다. 이 특허가 AMD가 matrix core를 사용하도록 강요하여 기술 발전을 저해한다고 주장했으며, Lisa Su 포스터와 함께 자신을 팀 레드라고 선언했습니다.

다른 사용자는 정반대의 경험을 했습니다. 여러 AMD 카드가 고장 났다고 말하며 자신은 h8r이고 matrix multiplication에는 NVIDIA를 선호한다고 밝혔습니다.

---

### HuggingFace ▷ #cool-finds (1 messages):
> 비디오 게임 속 Conversational Transformer
- Minecraft에서 빛나는 Transformer Model: 한 멤버가 비디오 게임 환경, 특히 Minecraft 내에 구현된 작동하는 conversational transformer를 보여주는 YouTube 영상을 공유했습니다.

이 구현은 게임 내 캐릭터가 자연어 대화에 참여할 수 있도록 하여 더욱 몰입감 있고 상호작용적인 게임 경험의 가능성을 열어주며, 해당 영상은 바이럴한 관심을 받고 있습니다.
- Minecraft Transformer: 누군가 YouTube 영상에서 보여주듯이 Minecraft에 작동하는 conversational transformer를 구축했습니다.

이는 게임 환경 내에 고급 AI를 통합했다는 점에서 인상적이라고 평가됩니다.

---

### HuggingFace ▷ #computer-vision (1 messages):
> Simultaneous Localization and Mapping, SLAM, monocular camera, Python
- Python 개발자들이 Monocular SLAM 마법을 탐구하다: 한 멤버가 Python을 사용하여 monocular camera로 Simultaneous Localization and Mapping (SLAM)을 구현한 경험에 대해 문의했습니다.
- SLAM 해독: 이 질문은 특히 이러한 기술들을 결합한 실무 경험이 있는 사람들을 대상으로 합니다.

---

### HuggingFace ▷ #smol-course (2 messages):
> 온디맨드 비디오 녹화, 깨진 퀴즈 링크
- 온디맨드 비디오 녹화 요청: 한 멤버가 해당 코스의 온디맨드 비디오 녹화 이용 가능 여부에 대해 문의했습니다.
- 섹션 2 퀴즈 링크가 깨졌습니다: 한 멤버가 섹션 2 퀴즈 링크가 깨졌다고 보고했습니다.

---

### HuggingFace ▷ #agents-course (3 messages):
> 코스 소개, 국제적인 인사
- 인도에서 Agents Course를 시작하는 신입생: 인도 출신 멤버가 오늘 Agents Course를 시작한다고 발표하며 열정을 표현했습니다.

에이전트의 세계로의 여정이 시작되며, 자료와 커뮤니티에 적극적으로 참여하기를 희망합니다.
- 프랑스인 참가자, Agents Course에 합류: 프랑스 출신 한 멤버가 인사를 전하며, 오늘부터 Agents Course를 시작할 의사를 밝혔습니다.

그들의 메시지는 기대감과 열정을 담고 있으며, 다른 참가자들과 함께 커리큘럼에 몰입하고 싶어 하는 마음을 보여줍니다.

---

### LM Studio ▷ #general (62 messages🔥🔥):
> OpenAI-compat-endpoint 플러그인, LM Studio Plugins, Cursor Chat Window 해킹, Alibaba RTX 5090 96GB, Long-Term Memory MCP
- LM Studio 플러그인, 비공개 베타 유지: 멤버들이 OpenAI-compat-endpoint 플러그인에 대해 문의했지만, 플러그인은 여전히 비공개 베타 상태이며 널리 접근할 수 없다고 설명되었습니다.

한 멤버는 플러그인 접근이 허브 프로필을 가지고 베타 업데이트와 함께 개발자 모드를 활성화하는 것과 관련이 있을 수 있다고 제안했으며, 다른 멤버는 mcps를 통해 접근 권한이 있다고 공유했습니다.
- 커서 채팅 창 해킹: 한 멤버가 LM-Studio 모델을 사용하여 커서 채팅 창을 해킹하는 방법을 실험하고 있습니다.

이를 달성하기 위해 기존의 오픈소스 솔루션을 탐색하고 있으며, 이는 채팅 인터페이스를 사용자 정의하려는 세 번째 시도입니다.
- Alibaba의 RTX 5090 96GB 개조품, 회의론 촉발: 한 멤버가 Alibaba에 4000달러에 올라온 RTX 5090 96GB 그래픽 카드라고 주장되는 링크를 공유했으며, 이는 그 합법성에 대한 회의론을 불러일으켰습니다.

PCB를 자세히 조사한 결과, 384비트 버스 폭 때문에 RTX 4090인 것으로 밝혀졌으며, 해당 목록은 RTX 4090 48GB 모델을 게으르게 복사-붙여넣기 한 것이었습니다.
- Long-Term Memory MCP 프로젝트 공개: 한 멤버가 자신의 Long-Term Memory MCP 프로젝트를 소개했습니다. 이 프로젝트는 장기 대화 메모리와 세션 간 원활한 리콜을 위해 설계된 SQLite와 ChromaDB의 하이브리드이며, GitHub에서 사용할 수 있습니다.

이 프로젝트는 시간 기반의 지연된 기억 소멸 및 강화 기능을 특징으로 하며, Qwen3 4b 2507 non thinking 모델과 함께 사용할 때 가장 잘 작동합니다.
- LLM의 진정한 동시성: vLLM 조사: 멤버들은 단일 로드된 모델에 여러 동시 요청을 보내는 가능성에 대해 논의했으며, 현재는 하나의 모델이 한 번에 하나의 요청을 처리하며, 진정한 동시성은 개발 중이라고 설명되었습니다.

vLLM (docs)과 같은 라이브러리가 높은 병렬성을 달성하여, 엄청난 수의 병렬 요청으로 확장되며, 4070이 모든 요청을 통해 누적 1400 tokens/s를 달성한 것으로 입증되었다고 언급되었습니다.

### LM Studio ▷ #hardware-discussion (133 messages🔥🔥):
> English-only policy reminder, NVMe SSD details, MI50 GPU performance, Server PSU vs consumer PSU, GPU Overclocking and BIOS flashing
- 일부 사용자에게 영어 전용 정책 상기: 한 멤버가 서버 정책에 따라 서버에서 영어를 사용하도록 안내받았습니다.

해당 사용자는 사과하며 잘못된 채널에 게시할 의도가 아니었다고 말했습니다.
- NVMe SSD 링크 상태 다운그레이드: 한 사용자가 NVMe SSD 링크가 16GT/s에서 8GT/s로 다운그레이드되고 ASPM이 비활성화된 이미지를 공유했습니다.

다른 멤버는 LnkCap (Link Capability)과 LnkSta (Link Status)를 비교하기 위해 `lspci -vv | less`를 사용하는 방법을 안내했습니다.
- MI50의 인상적인 Inference 성능: 한 사용자는 MI50의 Inference 성능과 비용 효율성에 대해 기대감을 표하며, Qwen 3 Coder 30b에서 W7900과 비슷한 70 tok/s를 얻고 있다고 보고했습니다.

다른 사용자는 sysRAM에 KV cache를 사용하여 `huihui-qwen3-30b-a3b-instruct-2507-abliterated@q8_0`에서 16-17 tok/s를 기록했다고 보고했습니다.
- Cline의 사용성 향상: 한 사용자는 자신의 프롬프트 처리 속도가 무한히 향상되어 Cline을 사용할 수 있게 되었다고 말하며, BasedBase.Qwen3-Coder-30B-A3B-Instruct-480B-Distill-V2-Fp32-GGUFF 링크를 공유했습니다.

다른 사용자는 브레이크아웃 보드가 있는 저렴한 1200w 서버 PSU 링크를 공유했습니다 (eBay 링크).
- GPU 오버클럭킹 BIOS 문제: 한 사용자는 실수로 Zotac BIOS를 자신의 MSI 및 ASUS 카드에 플래싱했던 경험을 공유했으며, 올바른 BIOS를 수동으로 다시 플래싱하여 해결했다고 밝혔습니다.

그들은 또한 자신의 오버클럭킹 설정(VRAM 주파수를 1600Mhz 증가)과 더 많은 카드가 연산 분할로 인해 성능 저하를 가져온다는 관찰 결과를 공유했습니다.

---

### Latent Space ▷ #ai-general-chat (157 messages🔥🔥):
> Sora 2, Vercel's Funding, Ring-1T Model, GLM-4.6 Model, Lovable Cloud
- Anthropic의 Code-Sonnet Contest 시작: Anthropic의 Alex Albert는 Claude Sonnet 4.5로 프로젝트를 구축하는 1주일간의 콘테스트(마감일 10월 7일)를 발표했으며, 우승자에게는 1년 동안 Claude Max 20x와 1천 달러의 API 크레딧이 제공됩니다.

우승자는 전반적인 느낌(vibes)을 기준으로 심사되며, 데모, 구축 세부 정보 및 독창성 증명을 제출해야 합니다. 규칙은 [여기](https://discord.com/channels/1097891724039833600/1157929424874258462/1157929424874258462)에서 확인할 수 있습니다.
- Lovable Cloud: 쉬워진 앱 구축: Lovable은 Cloud & AI 플랫폼을 출시하여 사용자들이 간단한 프롬프트로 복잡한 AI 및 백엔드 기능을 갖춘 풀스택 앱을 구축할 수 있도록 지원하며, 10월 5일까지 Google Gemini 기반 AI에 무료 액세스를 제공합니다.

이 플랫폼은 매일 10만 개 이상의 아이디어가 생성되고 7일 Build Challenge를 제공하며, 그중 한 성공 사례는 3개월 만에 45만 6천 달러의 ARR을 달성했다고 자랑합니다. 자세한 내용은 여기에서 확인할 수 있습니다.
- Vercel, 펀딩 라운드 후 93억 달러 가치 평가: Vercel은 Series F 펀딩 라운드를 93억 달러의 기업 가치로 마감했으며, AI Cloud와 v0가 이 이정표의 기반이 되었다고 강조됩니다.

커뮤니티는 이를 회사의 시작에 불과하다고 보며 흥분을 표했습니다. 자세한 내용은 여기에서 확인할 수 있습니다.
- Zhipu의 GLM-4.6 모델: 코딩 강자 공개: Zhipu는 GLM-4.6 (200K context) 및 GLM-4.5-series (355 B/106 B MoE) 모델을 출시했으며, 이 모델들은 Claude Sonnet 4 및 DeepSeek-V3.1-Terminus와 견줄 만한 최고 수준의 코딩, 추론 및 에이전트 능력을 선보이면서 약 30% 더 적은 Token을 사용합니다.

이 모델은 MIT 라이선스 하에 오픈 웨이트(open-weight)로 제공되며, 가중치(weights)와 API는 HF 및 Z.ai에서 사용할 수 있습니다. 자세한 내용은 여기에서 확인할 수 있습니다.
- Ring-1T: 1조 파라미터 추론 모델 데뷔: Ant Ling은 1조 파라미터 규모의 오픈 소스 "사고(thinking)" 모델인 Ring-1T-preview를 공개하며 SOTA 수학 점수를 달성했습니다.

초기 벤치마크에는 92.6 AIME25, 84.5 HMMT25, 50.8 ARC-AGI-1이 포함됩니다. 이 모델은 Hugging Face에서 사용할 수 있으며, 곧 채팅 인터페이스도 제공될 예정입니다. 자세한 내용은 여기에서 확인할 수 있습니다.

---

### Latent Space ▷ #ai-announcements (4개 메시지):
> Sonnet 4.5, Claude Code 2.0, Anthropic Dev Tools, Mike Krieger 인터뷰
- Krieger, 최신 출시 지식 공유: Latent Space 팟캐스트는 Mike Krieger와의 인터뷰를 공개하며 Anthropic의 Sonnet 4.5 메가 출시를 논의했습니다.

이번 출시에는 게 마스코트가 특징인 Claude Code 2.0, 메모리 + context-editing API, 새로운 VS Code 확장 프로그램, Claude for Chrome, 그리고 인챗(in-chat) 파일/코드 실행 기능이 포함됩니다.
- Sonnet 4.5 공개: Sonnet 4.5는 향상된 context 인식 기능을 갖추고 출시되었습니다.

이 모델은 새로운 개발자 도구와 함께 제공되었습니다.
- Claude Code 2.0, 문제 해결: Claude Code 2.0은 게 마스코트와 함께 출시되었습니다.

이번 출시의 일환으로 메모리 + context-editing API, 새로운 VS Code 확장 프로그램, Claude for Chrome, 그리고 인챗(in-chat) 파일/코드 실행 기능 등 다른 도구들도 함께 공개되었습니다.

### Latent Space ▷ #genmedia-creative-ai (13 messages🔥):
> AI Headshot Prompts, Sora 2 app, Nano-Banana Recursive Future-Frame Experiment
- 정교한 AI Headshot Prompt로 선명한 결과 도출: Justine Moore는 정확한 얼굴 보존 및 상세한 사진 사양을 특징으로 하여 선명하고 생동감 있는 결과를 위한 업그레이드된 AI Headshot Prompt를 공유했습니다. 이 트윗에서 볼 수 있습니다.
- Sora 2의 독립형 TikTok 스타일 출시 루머: 유출된 OpenAI의 Sora 2 "TikTok 스타일" 독립형 앱에 대한 보고가 있었습니다. 이 트윗에서 볼 수 있습니다.
- Nano-Banana, 스톡 영상을 'Green Gone Wild'로 변환: Radamés Ajna는 작은 "nano-banana" 모델을 사용하여 "Show this scene one second in the future"라는 프롬프트로 다음 프레임을 반복적으로 생성했습니다. 이 트윗에서 볼 수 있습니다.

---

### Yannick Kilcher ▷ #general (138 messages🔥🔥):
> Sonnet 4.5 Research, Language-Agnostic Grammatical Abstractions, LLM Layer Pruning, Evil LLMs, AI-Generated Video Detection
- Sonnet 4.5, 논문 초안 작성: Sonnet 4.5는 연구 및 논문 작성에서 향상된 역량을 보여주었으며, 단일 샷 구현을 생성하고, 모델을 훈련하며, 그림을 생성하고, MNIST 연구에 대한 논문을 PDF 형식으로 제작했습니다. 여기에는 8x8에서 16x16 해상도로 연구를 확장하는 것이 포함됩니다. 이 [예시 논문](https://x.com/AnthropicAI/status/1803734188448352652), [또 다른 예시](https://x.com/AnthropicAI/status/1803734190117765166), 그리고 [세 번째 예시](https://x.com/AnthropicAI/status/1803734191778906471)에서 볼 수 있습니다.
- 언어 불가지론적 LLM 이해: 기계적 해석 가능성(mechanistic interpretability) 연구에서 LLM의 중간 레이어가 언어 불가지론적(language-agnostic) 문법적 및 의미론적 추상화를 인코딩한다는 점점 더 많은 증거가 나타나고 있습니다. 여기에는 문법적 수, 성별, 시제, 통사적 일치와 같은 개념에 대한 공유된 표현이 포함됩니다.

특히 연구자들은 중간 레이어가 언어 불가지론적 문법적 추상화, 즉 언어 전반에 걸쳐 재사용되는 잠재 역할 그리드(행위자, 피행위자, 수식어)와 같은 것을 구현한다는 증거를 찾고 있습니다.
- 모델을 손상시키지 않고 레이어 Pruning: 한 AI 엔지니어가 크기를 줄이기 위해 LLM 레이어를 Pruning하고 있으며, 모델을 손상시키지 않고 중복 레이어를 Pruning하는 스크립트를 찾아냈습니다. 초기에서 중간 레이어는 중요하지만, 후반 레이어는 자유롭게 Pruning할 수 있다고 언급했습니다.

그들은 Pruning된 100B 모델인 Lazarus-2407을 Hugging Face에 공유했으며, Q8에서 100GB라고 밝혔습니다.
- 악의적인 LLM 제작: 한 AI 엔지니어가 더 자극적인 LLM을 만들기 위해 악의적이고 음란한 데이터로 모델을 훈련하고 있습니다. 이 목표를 달성하기 위해 개인 데이터셋과 시간당 15달러에 대여한 H200을 사용하고 있습니다.

이 엔지니어는 검열을 삭제 방식이 아닌 다른 방식으로 제거하는 모델을 훈련하며 협업에 열려 있습니다. 자세한 내용을 공유하기 위한 논문 출판에 도움을 요청하고 있으며, 공포 모델에 대한 추가 전문 지식을 위해 LM Studio Discord의 DavidAU를 지목했습니다.
- Sora 2 비디오 감지는 어렵습니다: 커뮤니티는 Sora 2와 같은 AI 생성 비디오를 감지할 가능성에 대해 논의했습니다. 일부는 이상적으로는 감지가 불가능해야 한다고 제안했고, 다른 일부는 시각적 단서나 '느낌'에 의존했습니다.

픽셀 피핑과 같은 기술은 여전히 꽤 안정적으로 작동합니다.

---

### Yannick Kilcher ▷ #paper-discussion (14 messages🔥):
> Latent Reasoning Survey, Unsupervised CoT Reasoning
- Latent Reasoning Survey 발표 예정: 한 멤버가 특정 날짜에 Latent-Reasoning survey를 발표하겠다고 제안했습니다.

해당 설문조사는 광범위하여 전체 내용을 다 다루지는 못할 것으로 예상합니다.
- Unsupervised CoT Reasoning에 대한 회의론: 한 멤버가 Unsupervised Chain of Thought (CoT) reasoning에 대해 회의적인 입장을 표명했습니다.

그들은 이 특정 관점을 염두에 두고 Latent-Reasoning survey를 조사하는 데 관심이 있습니다.
- Latent-Reasoning 토론 재조정: Latent-Reasoning survey에 대한 논의는 목요일 평소 시간에 계속될 예정이며, 11페이지 마지막 단락부터 섹션 3.1 끝까지 다룰 것입니다.

---

### Yannick Kilcher ▷ #ml-news (9 messages🔥):
> DeepSeek, Anthropic, GLM-4.6, OpenAI, Sora 1
- DeepSeek 및 Anthropic 모델 출시 소식에 기대감 고조: 멤버들은 오늘 DeepSeek과 Anthropic에서 새로운 모델이 출시될 가능성에 대해 기대감을 표했습니다.
- GLM-4.6 출시, 커뮤니티를 들뜨게 하다: 멤버들은 GLM-4.6 출시에 대해 기대감을 표했습니다.

한 사용자가 "It's happening"이라는 링크를 공유했습니다.
- OpenAI 비디오 생성 데모에 대한 엇갈린 반응: 멤버들은 OpenAI 비디오 생성 데모 링크를 공유하며 엇갈린 반응을 보였습니다. 한 명은 시각적으로는 훌륭하지만 지루하다고 평가하며 "그냥 무작위 장면일 뿐입니다. 스토리가 없습니다."라고 지적했습니다.

다른 사용자는 "Sora 1보다 그렇게 많이 좋나요? 나란히 비교해 봐야 할 것 같습니다"라고 물었고, 다른 사용자는 "*품질이 훨씬 좋습니다. Sora 1은 물리 법칙을 구현하지 못했고 명백한 시각적 아티팩트가 있었습니다."라고 답했습니다.
- ByteDance와 Tencent가 이미 OpenAI보다 앞서 있나요?: 한 멤버는 OpenAI 비디오 데모에 "감명받지 못했다"고 표현하며 "ByteDance나 Tencent가 이미 가지고 있는 것보다 나아 보이지 않습니다"라고 말했습니다.

### Nous Research AI ▷ #general (79 messages🔥🔥):
> Cloud GPU Services, Qwen omni awq, Refuting orthogonality thesis, Meituan and ByteDance Papers, GLM 4.6 vs Sonnet 4.5
- 클라우드 GPU 서비스, 경제성 추구: 한 멤버가 시장에서 가장 저렴한 클라우드 GPU 서비스에 대해 문의했습니다.
- Qwen omni awq 로컬 설정 문제: vllm을 작동시키는 데 몇 시간을 보낸 후, 한 멤버가 Qwen omni awq를 로컬에서 실행했지만 4k 이미지를 업로드할 때 VRAM 제한으로 인해 충돌이 발생했습니다. 그들은 VRAM을 절약하기 위해 오디오 관련 기능을 쉽게 비활성화할 방법을 찾았습니다.
- Orthogonality Thesis 반박 및 AI Alignment: 한 멤버가 orthogonality thesis(OT)를 반박하고 "alignment research" 패러다임을 바꾸기 위한 파트너를 찾고 있으며, 수학 전문 지식과 ML 테스트 접근 권한이 있는 사람을 찾고 있습니다. 핵심 주장은 AI가 단순히 자신의 힘이 아니라, 서로 다른 정책을 가진 다양한 에이전트를 보존할 것이라는 점이며, 이는 입증된다면 획기적인 개념이라고 그들은 믿습니다.
- GLM-4.6 벤치마크, Agentic Task 제외 Sonnet-4.5 능가: GLM-4.6은 agentic 벤치마크를 제외하고 Sonnet 4.5보다 높은 벤치마크 결과를 보여주었으며, 가중치는 Hugging Face에서 이용 가능합니다.
- Sora 2 첫 영상: 한 멤버가 자신의 첫 Sora 2 영상을 공유했습니다.

---

### Nous Research AI ▷ #ask-about-llms (6 messages):
> Sonnet 4.5, Deepseek V3, LRMTokenEconomy, Reasoning Efficiency
- Sonnet 4.5의 추론 효율성, Opus 4.1 능가: Sonnet 4.5는 Opus 4.1을 넘어선 향상된 추론 효율성을 보여주었지만, 해당 모델이 chat completions API에서 CoT를 공유하지 않기 때문에 Sonnet 4.5에 대한 데이터는 없습니다. 일부 멤버에 따르면 Deepseek V3.2의 성능은 V3.1과 매우 유사합니다.
- LRMTokenEconomy 업데이트: 한 멤버가 LRMTokenEconomy에 대한 업데이트를 공유했습니다. 이는 Reasoning Models에서 사고 효율성을 측정하는 것과 관련이 있습니다.

---

### Nous Research AI ▷ #research-papers (4 messages):
> Catastrophic Forgetting, Cognitive Architecture Surgery, AI Collaboration
- Catastrophic Forgetting 연구 시작: 한 멤버가 신경망의 catastrophic forgetting과 관련된 연구 프로젝트를 진행 중이며, 수학, 이론 물리학, AI/ML, 신경과학 분야의 협력자를 찾고 있습니다.

그들은 catastrophic forgetting이 AI가 인간처럼 지속적으로 학습하는 것을 방해하는 핵심 문제라고 언급했습니다. 그들의 프로젝트인 Cognitive Architecture Surgery (CAS)는 뇌가 정보를 라우팅하는 방식에서 영감을 받아 네트워크를 무한히 확장하는 대신 동적으로 재구성합니다.
- GitHub 프로필로 충분한가요?: catastrophic forgetting 연구 프로젝트의 협력자 모집 공고에 대한 응답으로, 한 멤버가 GitHub 링크가 지원서로 충분한지 물었습니다.

원 게시자는 관심 있는 당사자들이 이력서/CV를 DM으로 보내달라고 요청했지만, GitHub 프로필도 검토할 의향이 있는 것으로 보였습니다.

---

### Nous Research AI ▷ #interesting-links (1개 메시지):
kotykd: https://thinkingmachines.ai/blog/lora/

---

### Nous Research AI ▷ #research-papers (4개 메시지):
> Cognitive Architecture Surgery, Catastrophic Forgetting, Neural Networks, Mathematics, Theoretical Physics
- catastrophic forgetting 감소를 위한 CAS 프로젝트 착수: 한 멤버가 신경망의 catastrophic forgetting을 해결하기 위한 Cognitive Architecture Surgery (CAS) 프로젝트의 협력자를 찾고 있으며, 이는 AGI를 방해하는 핵심 문제입니다.

이 프로젝트는 뉴런을 추가하지 않고 뇌가 정보를 라우팅하는 방식에서 영감을 받아 네트워크를 동적으로 재구성하는 것을 목표로 하며, 관심 있는 협력자들은 이력서/CV 또는 GitHub 링크를 DM으로 보내달라고 요청받았습니다.
- AI/ML 분야의 학제 간 협력자 모집: 한 멤버가 신경망의 catastrophic forgetting과 관련된 수학, 이론 물리학, AI/ML 및 신경과학 분야의 연구 프로젝트 협력자를 찾고 있습니다.

관심 있는 멤버들은 이력서/CV를 DM으로 보낼 수 있습니다.

---

### Eleuther ▷ #general (13개 메시지🔥):
> LLM 연구를 위한 Discord 채널, ViT를 사용한 Fast Gradient Method, JanusPro1B에 대한 whitebox 공격 제작, Orthogonality thesis 토론, OWT Val Loss Curve를 사용한 GPT2 Small 재현 NanoGPT
- 대체 LLM 연구 허브 모색: 멤버 Paras는 이 채널의 리소스를 보완하기 위해 LLM 연구에 초점을 맞춘 다른 Discord 채널에 대해 문의했습니다.

다른 멤버 llm0090은 이 요청에 동의했고, 유일한 공개 LLM 전용 서버는 Marin이라는 답변이 나왔습니다.
- ViT 네트워크에 대한 Fast Gradient Attack 결과 부진: 멤버 emanuel65537은 ImageNet으로 학습된 ViT 모델에 이미지 증강을 사용한 fast gradient method를 적용한 실험 결과를 공유했습니다.

한 멤버가 모델이 이상한 배경과 해당 레이블만 인식했다고 보고했으며, 이는 모델을 스케일링하면 텍스처에 덜 민감해진다는 것을 시사합니다.
- Janus 및 ChatGPT에서 Whitebox 공격이 무력화되었습니다: darwin9000이라는 멤버가 JanusPro1B에 대한 whitebox 공격을 만들었지만, ChatGPT는 이러한 공격에 면역인 것으로 보이며 샘플 이미지를 첨부했습니다.
- Orthogonality Thesis: 논의 범위?: 한 멤버가 Discord의 alignment 섹션에서 orthogonality thesis에 대한 논의가 적절한지 문의했습니다.

그들은 그러한 철학적 논의가 Discord의 범위에 속하는지 의문을 제기했습니다.
- NanoGPT의 GPT2 Small Val Loss 데이터 요청: anxietyprime이라는 멤버가 OWT로 GPT2 Small을 재현하는 기본 NanoGPT에 대한 val loss 곡선을 요청했으며, 가능하다면 재현을 피하고자 했습니다.

---

### Eleuther ▷ #research (34 messages🔥):
> DeMO Paper, Psyche System Design, Distributed Training, Probability Mass Recall, Attention Implementations Benchmark
- 새로운 DeMO Paper가 곧 나옵니다: 새로운 DeMO paper가 곧 나올 예정이며, 모델 훈련에 대한 자세한 내용은 여기에 있습니다. 하지만 링크된 정보는 시스템 설계 및 모델에 대한 내용이 완전히 구식입니다.
- Bee Movie 스크립트를 사용한 Llama 3.2 1B 실험: 한 멤버가 Bee Movie 스크립트를 사용하여 Llama 3.2 1B에 대한 ANN 접근 방식을 실행하는 기본 실험을 수행했으며, 다양한 head와 layer에서 95% 이상의 probability mass recall을 달성했습니다. 비록 그들은 자신들의 구현에 버그가 있다고 의심하지만.

시퀀스 내 많은 무작위 쿼리 결과는 첨부된 이미지에 나와 있습니다.
- Probability Mass Recall 정의: Probability mass recall은 brute-force/naive attention과 겹치는 post-softmax mass의 부분을 의미하며, 관련 논문은 https://arxiv.org/abs/2509.25087에서 확인할 수 있습니다.
- TopK를 통한 성능 향상: 첨부된 이미지는 정확히 동일한 설정에서 1M Token ctx window에서 topK를 사용하면 일반적인 dense attention에 비해 730배 적은 FLOPs가 발생함을 보여줍니다.

---

### Eleuther ▷ #lm-thunderdome (14 messages🔥):
> MMLU Evaluation, Llama 3 Evaluation, Contamination issues
- MMLU Task 구성 명확화: 멤버들은 base 모델과 instruction-tuned 모델에서 MMLU를 평가하기 위한 task 구성을 논의했으며, chat template 인터페이스가 맞춤형 instruction 형식을 지정해야 한다고 언급했습니다.

평가 절차는 베이스 모델 또는 인스트럭션 튜닝된 모델 사용 여부에 따라 다를 수 있다는 점이 언급되었습니다. 이는 Llama 3 논문에서 베이스 모델의 NLL을 비교하고 인스트럭션 튜닝된 모델의 답변을 생성하여 MMLU를 평가하는 방식에서 볼 수 있습니다.
- Llama MMLU Configs 공유: 한 멤버가 Llama MMLU Configs를 공유하며, 5-shot (CoT 없음) 및 zero-shot (CoT 포함) 평가에 특정 템플릿이 사용되었음을 확인했습니다.

CoT가 없는 템플릿은 모델이 (A, B, C, D)를 즉시 생성하도록 유도하기 위해 답변을 끝에 삽입하며, 모든 MMLU 서브태스크를 평가합니다.
- MMLU 오염 문제 지속: 한 멤버가 MMLU를 사용하지 말라는 월간 알림을 주었습니다. 이는 최근 모델의 학습 데이터셋에 포함될 가능성이 높으며, 특히 2023년부터 평가 오염이 문제가 되어왔기 때문입니다.

그들은 사전 학습에서 모든 오염을 명시적으로 제거하지 않는 한 Common Crawl 또는 Fineweb을 확인할 것을 제안했으며, 지속적인 오염 문제로 인해 MMLU 사용을 피할 것을 권장했습니다.

---

### Moonshot AI (Kimi K-2) ▷ #general-chat (39 messages🔥):
> Kimi K2 Turbo 속도, Cerebras 호스팅, ML 틈새 밈, AI 슬롭 샵 웹사이트, GLM-4.6
- Kimi K2 Turbo 속도 향상: kimi-k2-turbo-preview 모델은 이제 공식 문서에 따르면 초당 60 Token의 속도를 자랑하며, 최대 100 Token까지 순간적으로 증가하고 256k의 Context Length를 유지합니다.

스크린샷에 따르면 이 모델은 평균 초당 150 Token을 처리하며, 이는 주장된 초당 15 Token보다 훨씬 빠릅니다.
- Kimi의 Cerebras 호스팅 고려: 한 사용자가 Cerebras 하드웨어에서 Kimi를 호스팅할 가능성에 대해 문의하며, 잠재적으로 초당 2k Token의 속도를 달성할 수 있다고 언급했습니다.

사용자는 이러한 속도를 달성하면 “AGI를 해제할 수 있을 것”이라고 표현했습니다.
- ML 틈새 밈: 한 사용자가 “틈새 ML 밈”이 인기를 얻고 있다는 점을 유머러스하게 언급했습니다.

Trump가 DeepSeek v3.2 및 Kimi를 사용한 DSA 릴리스에 대해 올린 게시물을 언급하며, 그들은 “Yeah 😂”라고 반응했습니다.
- AI Slop Shop 웹사이트: 한 사용자가 AI Slop Shop 웹사이트 링크를 공유하며, 재미있고 즐겁다고 설명했습니다.

그들은 특히 Thought Cancelling Headphones 제품을 강조했습니다.
- GLM-4.6 인상: 한 사용자가 “GLM-4.6이 좋아 보인다”고 짧게 언급했습니다.

GLM-4.6의 특정 Context나 기능에 대한 추가적인 세부 정보는 제공되지 않았습니다.

### GPU MODE ▷ #triton (2 messages):
> Triton, OpenAI, Meta, GPU MODE, AMD GPUs
- 블록 기반 양자화 탐색 시작: 한 멤버가 오픈소스의 고성능 블록 기반 양자화/역양자화 Triton 구현체에 대해 문의했습니다.

제공된 맥락에서 구체적인 구현체는 직접적으로 링크되거나 제안되지 않았습니다.
- Triton Developer Conference 2025 초대: Triton Developer Conference 2025가 몇 주 후에 개최되며, 동료 Triton 애호가들과 교류하고 최고 리더들의 강연을 듣기 위해 참석을 독려합니다.

등록은 [aka.ms/tritonconference2025](https://aka.ms/tritonconference2025)에서 가능합니다.
- Triton Conference 2025, 스타 연사들을 자랑합니다: Triton Conference 2025의 연사로는 OpenAI의 Phil Tillet과 Thomas Raoux가 'Triton: Today and Beyond'에 대해, Meta의 Mark Saroufim이 'GPU MODE: The State of Triton'에 대해 발표합니다.

또한 AMD에서는 AMD GPUs에서의 첫날 속도에 대해, Nvidia에서는 Blackwell GPU 백엔드에 대해, Bytedance에서는 분산 LLM 훈련에 대해 발표하는 연사들도 참여합니다.

---

### GPU MODE ▷ #cuda (2 messages):
> LDO Stride Misunderstanding
- LDO Stride 스키마 수정됨: 한 멤버가 LDO의 묘사가 잘못되었다고 지적하며, 일반적으로 column 0에서 column 8 또는 column 128/dtype_bits까지의 stride를 나타내야 한다고 제안했습니다.

다른 멤버는 실수를 인정하고 문서에 기반한 수정을 확인했습니다.
- LDO Stride 스키마 재확인됨: 한 멤버가 LDO의 묘사가 올바르다고 지적하며, 일반적으로 column 0에서 column 8 또는 column 128/dtype_bits까지의 stride를 나타내야 한다고 제안했습니다.

다른 멤버는 확인을 인정하고 문서에 기반한 수정을 재확인했습니다.

---

### GPU MODE ▷ #algorithms (1 messages):
crazy_steroids69: 뭔데

---

### GPU MODE ▷ #cool-links (3 messages):
> NVIDIA GPUs, matmul kernels, GPU architecture, PTX/SASS, warp-tiling
- NVIDIA GPU MatMul Kernels 상세 설명: 한 멤버가 GPU 아키텍처, PTX/SASS, warp-tiling, 그리고 tensor core 파이프라인을 상세히 설명하는 'Inside NVIDIA GPUs: Anatomy of high performance matmul kernels' 블로그 게시물을 공유했습니다.
- 폰트 미학 비판: 한 멤버가 NVIDIA GPU MatMul Kernels 블로그 게시물이 훌륭한 자료임에도 불구하고 폰트가 눈에 잘 들어오지 않는다고 언급했습니다.

---

### GPU MODE ▷ #beginner (3 messages):
> Nvidia CUDA Handbook, PTX ISA, PCIe expert
- PMPP를 위한 CUDA Handbook 또는 PTX ISA?: 한 멤버가 PMPP에서 넘어온 후 Nvidia CUDA Handbook 사용에 대한 조언을 구했습니다.

다른 멤버는 CUDA handbook 대신 PTX ISA를 사용할 것을 제안하면서, Nvidia의 훌륭한 문서라고 언급했습니다.
- PCIe 원인 분석 탐색: 한 멤버가 소비자용 카드에서 GPU가 버스에서 이탈하는 이유를 파악하기 위해 PCIe에 대해 배우기 위한 자료를 찾고 있습니다.

그들은 목표가 소비자용/non-SXM 카드에서 GPU가 버스에서 이탈하는 이유를 이해하는 것이라고 명시했습니다.

---

### GPU MODE ▷ #irl-meetup (1 메시지):
> PyTorch Conference SF, Meetup 조율
- PyTorch Conf SF 참석자 여러분!: SF에서 열리는 PyTorch 컨퍼런스 참석자들이 행사 중 하나에서 만남을 조율하고 있습니다.

관심 있는 분들은 DM 또는 메시지를 보내서 모임을 주선하도록 권장됩니다.
- 컨퍼런스 참석자들이 IRL Meetup을 계획합니다: SF에서 열리는 PyTorch 컨퍼런스에 참석하는 사람들이 만남을 조율하려고 노력하고 있습니다.

참석하신다면, DM 또는 메시지를 보내서 함께 즐기세요!

---

### GPU MODE ▷ #rocm (3 메시지):
> MI300의 Matrix Cores, Mesa를 사용한 SPIRV 컴파일, 디버거 업데이트
- AMD, MI300 시리즈용 Matrix Cores 공개: AMD는 MI300/325/350 시리즈용 matrix cores를 발표하며 최적화된 성능을 약속했습니다.

이 발표에는 문서와 초기 성능 수치가 포함되어 있지만, 성능 비교는 없습니다.
- Mesa 드라이버, SPIRV 컴파일 지원: 디버거는 이제 Mesa 드라이버와 디버그 정보를 사용하여 SPIRV 컴파일을 지원합니다.

한 멤버가 새로운 디버깅 기능을 보여주는 비디오를 첨부했습니다.

---

### GPU MODE ▷ #metal (2 메시지):
> FlashMLA, Metal Flash Attention, 침체된 Metal 개발자 커뮤니티
- Flash Attention, Metal에 상륙: 한 멤버가 FlashMLA를 범용 Metal Flash Attention에 적극적으로 구현하고 있습니다.

이는 flash attention의 효율성을 Metal 프레임워크에 가져오는 것을 목표로 합니다.
- Metal 개발자 커뮤니티: 황폐해졌나요?: 한 멤버가 Metal 개발자 커뮤니티의 비활동성에 대해 한탄하며, 사방에 귀뚜라미 소리만 들리는 죽은 커뮤니티라고 묘사했습니다.

이는 Metal 개발 분야 내에서 잠재적인 참여 또는 지원 부족을 시사합니다.

### GPU MODE ▷ #submissions (4 messages):
> MI300x8 Leaderboard Updates, amd-ag-gemm, amd-gemm-rs
- MI300x8, amd-ag-gemm에서 6위 달성: 한 멤버가 MI300x8을 사용하여 amd-ag-gemm 리더보드에서 512 µs의 시간으로 6위를 달성했습니다.
- MI300x8, amd-ag-gemm에 더 많은 제출 기록: MI300x8을 사용하여 amd-ag-gemm 리더보드에 더 많은 제출이 이루어졌으며, 533 µs와 891 µs의 시간이 기록되었습니다.
- MI300x8, amd-gemm-rs에서 개인 최고 기록 달성: 한 멤버가 MI300x8을 사용하여 amd-gemm-rs 리더보드에서 593 µs의 시간으로 개인 최고 기록을 달성했습니다.

---

### GPU MODE ▷ #amd-competition (2 messages):
> MFMA intrinsics, CDNA3, CDNA4
- MFMA Intrinsic Instructions 블로그 게시물 공개: AMD는 CDNA3/4 아키텍처에서 MFMA intrinsics를 사용하는 방법에 대한 블로그 게시물을 공개했으며, 해당 게시물은 rocm.blogs.amd.com에서 확인할 수 있습니다.
- AMD의 CDNA Matrix Core 최적화: 해당 블로그 게시물은 최적화된 성능을 위해 CDNA3 및 CDNA4 아키텍처에서 Matrix Core MFMA intrinsics를 사용하는 방법을 자세히 설명합니다.

---

### GPU MODE ▷ #cutlass (12 messages🔥):
> cute.print_tensor 세그폴트 발생, cute DSL return 미지원, warp mma vs wmma
- cute.print_tensor 세그폴트 발생!: 멤버들은 cute.print_tensor가 세그폴트를 일으키는 것으로 보인다고 보고했습니다. 이는 CPU에서 실행되는 @cute.jit 함수 내에 할당된 디바이스 메모리와 같이 접근 불가능한 메모리에 텐서를 출력하기 때문일 수 있습니다.
- 한 멤버는 출력 인프라에서 아직 지원되지 않는 일부 요소 데이터 타입을 사용하기 때문일 수 있다고 제안했습니다.
- cute DSL return 문 제한 검토: 한 멤버가 이 코드의 맥락에서 문서에 명시된 cute DSL의 return 문 지원 부재에 대해 문의했습니다.
- 논의 결과, 이 제한은 주로 전체 커널에 적용되며, 서브함수 내의 return 문은 일반적으로 지원된다고 명확히 했습니다. 특히 다른 cute.jit 함수에 의해 호출될 때는 지원되지만, 일반 Python 코드로 반환될 때는 지원되지 않습니다.
- warp mma 및 wmma 문서 혼동: 한 멤버가 cute.nvgpu.warp.MmaF16BF16Op 문서가 wmma 문서 대신 mma를 참조하는 이유와 16x16x16을 허용하는 대신 mma 셰이프(예: 16x8x16)를 단언하는 이유에 대해 질문했습니다.
- 해당 멤버는 warp mma가 wmma여야 한다고 제안했습니다.

---

### GPU MODE ▷ #low-bit-training (1 messages):
kitsu5116: https://arxiv.org/abs/2509.25149

### GPU MODE ▷ #penny (1 messages):
> oneshot allreduce, nccl
- oneshot allreduce가 NCCL 속도에 근접합니다: 한 사용자가 oneshot allreduce를 실험하고 있으며, 추가적인 속도 향상이 가능하다고 생각합니다.
- 현재 버전은 작은 버퍼에서 NCCL 성능의 80%를 달성하며, 이전의 60-70%에서 향상되었습니다.
- oneshot allreduce의 잠재적 속도 향상: 사용자는 oneshot allreduce 구현에서 추가적인 최적화에 대해 낙관적입니다.
- 그들은 작은 버퍼에서 NCCL 성능의 80%를 달성했다고 보고했으며, 이는 이전의 60-70%에서 크게 개선된 것입니다.

---

### Modular (Mojo 🔥) ▷ #general (2 messages):
> Mojo Python Interoperability, Level Up Congratulations
- Mojo 인터롭 현황: 한 멤버가 Mojo의 Python interoperability의 현재 상태에 대해 문의했습니다.
- 레벨업 알림: 한 사용자가 레벨 1로 승급한 것에 대해 축하를 받았습니다.

---

### Modular (Mojo 🔥) ▷ #mojo (14 messages🔥):
> C interop, Python interop, Mojo roadmap, Windows release, GPUs and accelerators on Windows
- C interop의 우발적 누락: C interop이 로드맵에서 실수로 제거되었지만, 이는 오류였으며 여전히 계획되어 있습니다.
- Mojo의 Pythonic 수용: Mojo의 Python interoperability의 현재 기능은 문서와 코드 예제에 자세히 설명되어 있으며, 사용 편의성(ergonomics) 개선을 위한 작업이 활발히 진행 중입니다.
- Mojo의 Phase 1 목표가 구체화됩니다: Modular는 로드맵에서 언어의 Phase 1에 대한 목표와 계획된 작업을 제시했습니다.
- 그들은 Mojo가 이러한 기능들을 갖춘 고성능 컴퓨팅을 위한 강력한 언어라고 생각합니다.
- Windows 릴리스는 언제쯤 이루어질까요?: Windows 지원은 compiler가 오픈 소스화된 후에 이루어질 가능성이 높습니다.
- Windows에서의 GPU 및 Accelerator 협력: 많은 GPU 또는 accelerator는 Windows에 대한 벤더 지원 부족으로 인해 Windows에서 사용할 수 없을 것입니다.

---

### Modular (Mojo 🔥) ▷ #max (17 messages🔥):
> MAX Kernels as a Library, Building Kernel Modules, comm Module Issues, Packaging of Pre-built Kernel Modules
- 사용자들이 MAX Kernels를 라이브러리로 가져오려고 합니다: 멤버들은 `kernels.nn.irfft import irfft`와 같이 MAX kernels에서 코드를 라이브러리로 가져오려고 시도했습니다.

한 멤버가 -I를 사용하여 kernel source를 가리키거나 포럼의 지침에 따라 kernel modules를 빌드할 것을 제안했습니다.
- Kernel Modules 빌드 시 ‘comm’ Module 오류 발생: kernel modules를 빌드할 때, 사용자들은 `from nn.irfft import irfft`를 임포트하려고 할 때 `error: unable to locate module 'comm'`라는 오류에 직면했습니다.

누락된 comm 라이브러리를 추가하기 위해 `./bazelw build //max/kernels/src/comm`를 실행하라는 제안이 있었는데, 이는 새로운 dependency 문제로 보였습니다.
- MAX Package에 Pre-built Kernel Modules 포함: pre-built kernel modules는 max package의 일부로 패키징되어 있으므로, `pixi add max` 후 `.pixi/envs/default/lib/mojo/`에 `nn.mojopkg`가 나타납니다.

하지만 comm module은 여전히 문제를 일으켰고, mojo package에는 `stdlib.mojopkg`와 `layout.mojopkg`만 포함되어 있었습니다.
- Kernel Imports 활성화를 위한 워크어라운드: 워크어라운드는 max package를 추가하고 Bazel을 사용하여 comm 및 internal_utils modules를 빌드하는 것입니다 (`./bazelw build //max/kernels/src/comm` 및 `./bazelw build //max/kernels/src/internal_utils`).

그런 다음, `from nn.irfft import irfft`를 활성화하기 위해 이 modules를 Pixi environment(`.pixi/envs/default/lib/mojo/`)로 복사해야 합니다.
- 다음 Nightly에 수정 사항 적용 예정: 누락된 modules는 max package distribution에 추가되고 있으므로, 다음 nightly에서는 워크어라운드가 필요하지 않을 것입니다.

사용자들은 수동 빌드를 피하고 모든 kernel modules의 함수에 즉시 접근하기 위해 `pixi add max`만 하면 됩니다.

---

### DSPy ▷ #general (25개 메시지🔥):
> LLM caching, database session to tool, DSPy Signatures & Modules & Adapters, Semantic Caching, DSPy hackathons
- LLM Caching의 미묘한 차이에 대한 논쟁 촉발: 멤버들은 LLM caching이 KV cache가 동일한 숫자 세트를 가지는지 여부에 달려 있으며, adaptors 중 하나라도 변경하면 cache가 무효화된다고 논의했습니다.

semantic caching이 유사한 입력을 제공하여 cache hit를 늘리고, 첫 N개의 Token을 caching함으로써 도움이 될 수 있다고 제안되었습니다.
- DSPy Signature Prompt Caching 문제 발생: 한 사용자가 다른 DSPy signature가 document content 이전에 다른 prompt를 생성하여 효과적인 prompt caching을 방해하는 문제를 지적했습니다.

사용자는 프롬프트 시작 부분에 있는 문서를 이동하고, chat adaptor를 서브클래싱하며, 지시사항을 시작 부분이 아닌 끝 부분으로 이동하는 것을 고려하고 있습니다.
- DSPy 해커톤: 사람들이 DSPy 중심이거나 DSPy를 사용할 수 있는 AI 중심의 해커톤을 진행하고 있는지에 대한 질문이 있었습니다.

한 멤버는 11월 17일경 AI By the Bay 컨퍼런스를 위해 캘리포니아 오클랜드에서 해커톤이 활발히 조직되고 있다고 언급했습니다.
- dspy.streamify 스트리밍 특이점 발견: 한 멤버가 dspy.streamify에서 일관되지 않은 동작을 보고하며, 사용된 adaptor에 따라 성능이 달라진다고 언급했습니다 (XML이 JSON보다 더 잘 작동합니다).

그들은 또한 XML Adapter에서 버그를 발견하고 PR을 제출했는데, 모델이 DSPy signature와 관련 없는 XML Tags를 생성하고 있었다고 말했습니다!

---

### aider (Paul Gauthier) ▷ #general (17 메시지🔥):
> Opus 4.1, aider token control, mcp browser automation
- 벤치마크 리더보드, Opus 4.1 포기: 벤치마크 리더보드가 Opus 4.1 결과가 부족하여 방치된 것으로 보이며, 인프라와 커뮤니티를 구축한 후 벤치마크를 중단하는 것에 대한 의문이 제기되고 있습니다.

한 멤버는 인프라와 커뮤니티에 투자한 후 벤치마크를 중단하는 논리에 의문을 제기했습니다.
- Aider token 제어, 모델 업그레이드: 한 멤버는 aider 외의 다른 것을 사용하는 것은 모델 다운그레이드와 같다고 주장하며, aider의 "token에 대한 완전한 제어"가 더 나은 모델 성능을 가져오는데, 이는 적은 token 수가 더 나은 모델 성능을 초래하기 때문이라고 언급했습니다.

그 멤버는 aider가 token 수를 더 작게 유지하는 능력 덕분에 모델을 타이트하게 유지함으로써 기본적으로 모델을 업그레이드하는 것이라고 설명합니다.
- MCP 브라우저 자동화 팁 요청: 한 멤버가 Arch Linux에서 mcp 브라우저 자동화를 위한 권장 사항을 요청했으며, 기본 Playwright 설치 및 Puppeteer와의 문제점을 언급했습니다.

다른 멤버는 macOS 또는 Windows용으로 설계되었지만 상세한 문서를 제공하는 mcp-chrome을 추천했습니다.
- Aider, 기본 MCP 지원 부족: 멤버들은 goose/claude/gemini-cli 모두 mcps를 가지고 있으며, 이는 프런트엔드 개발에 중요하기 때문에 aider와 mcp를 사용하는 방법에 대해 논의합니다.

한 멤버는 공식 aider는 이를 지원하지 않지만, 지원하는 포크들이 있으며 aider-ce를 링크했다고 언급했습니다.

### aider (Paul Gauthier) ▷ #questions-and-tips (5 messages):
> Anthropic Claude Sonnet 4.5, aider --install-main-branch
- Aider 사용자가 Claude Sonnet 4.5 버전 확인: 한 사용자가 aider에서 anthropic/claude-sonnet-4-5로 전환한 후, Claude 콘솔에서 최신 4.5 버전을 확인할 수 있었다고 밝혔습니다.

사용자는 콘솔의 Usage 섹션에서 모델 버전을 확인할 수 있었습니다.
- Aider main 브랜치 설치: 한 사용자가 아직 릴리스되지 않은 aider-0.86.1을 다른 사용자가 어떻게 설치했는지 질문했습니다.

다른 멤버는 main 브랜치에서 최신 버전에 접근하기 위해 `aider --install-main-branch` 명령어를 사용할 것을 제안했습니다.

---

### tinygrad (George Hotz) ▷ #general (11 messages🔥):
> Tinygrad vs PyTorch speed, Theoretical side of tinygrad, CLSPV crashes
- Tinygrad, PyTorch를 능가할 것: George Hotz는 tinygrad가 결국 NVIDIA GPU에서 PyTorch보다 훨씬 빨라질 것이라고 믿으며, 그 과정이 매우 심오하다고 언급했습니다.

그는 tinygrad가 PyTorch보다 한 세대 앞서 있으며, producer/consumer graphs, ILP memory allocation / scheduling, megakernels와 같은 새로운 기능들을 통해 연구 논문들의 최신 동향을 한 세대 뒤따르고 있다고 언급했습니다.
- Tinygrad 이론 관련 자료: 멤버들은 tinygrad의 이론적 측면을 연구하기 위한 다양한 자료들을 추천했으며, 여기에는 공식 문서도 포함됩니다.

추가 자료로는 Deep Learning with Python, How Transformer LLMs Work 강좌, Jay Alammar의 블로그 게시물, Eugene Yan의 블로그, 그리고 tinygrad notes 등이 있습니다.
- CLSPV 포크 수정 예정?: 한 멤버가 CLSPV로 테스트를 실행하는 동안 가끔 충돌이 발생한다고 보고했지만, 대부분의 테스트는 통과한다고 언급했습니다.

그들은 다른 사람들이 `pip install git+https://github.com/softcookiepp/tinygrad.git` 명령어를 사용하여 x86_64 Linux 시스템에서 자신의 포크를 시도해 볼 것을 권유했습니다.

---

### Manus.im Discord ▷ #general (6 messages):
> Manus Support, Internal Server Error, Subscription Issues
- Manus 지원 부족에 대한 사용자 불만: 여러 사용자들이 Manus 관련 문제를 겪고 있다고 보고했으며, 며칠 동안 여러 차례 이메일을 보냈음에도 Manus 지원팀으로부터 응답이 없어 불만을 표출했습니다.

사용자들은 요금이 잘못 청구되거나 Internal Server Error가 발생하고, 최고 요금제를 결제했음에도 Agent mode 사용에 제한을 받는 등의 문제들을 겪고 있습니다.
- Internal Server Error 재발: 여러 사용자들이 흔히 발생하는 Internal Server Error (10091)를 겪고 있으며, 이는 종종 고객 지원팀에 문의하거나 환불을 요청하라는 메시지와 함께 나타납니다.

한 사용자는 도움말 센터로 안내되었지만, 여러 지원 티켓을 제출한 후에도 아무런 응답을 받지 못했습니다.
- 구독 접근 제한: 사용자들은 최고 유료 요금제를 구독하고 있음에도 비정상적으로 높은 사용량으로 인해 Agent Mode에서 잠금 처리되었다고 보고하고 있습니다.

이러한 현상은 종종 Internal Server Error (10091)와 함께 발생하여, 사용자들이 비용을 지불한 기능을 활용할 수 없게 만들고 있습니다.

---

### MCP Contributors (Official) ▷ #general (3 messages):
> MCP Release Cadence, Agentic Commerce Protocol, Google AP2 Protocol
- 표준화된 MCP 릴리스 주기 요구 표면화: 한 멤버가 MCP 릴리스 주기의 표준화에 대해 문의하며, 정해진 간격 또는 명확한 질적 변화 세트가 조직의 계획 및 투자에 도움이 될 것이라고 제안했습니다.

그들은 이 빠른 진화 단계 동안 시간 기반 릴리스를 제안했으며, 향후 조정은 투표 그룹이 결정하고 이 정보를 거버넌스 모델에 포함할 것을 제안했습니다.
- MCP 프롬프트 Agentic Commerce Protocol 생성의 격차: 한 멤버가 팀이 Agentic Commerce와 협력하여 MCP를 확장하는 대신 별도의 Protocol을 생성한 이유를 이해했는지 질문했습니다.

응답은 없었습니다.
- Google AP2의 빠른 후속 조치로서의 Agentic Commerce: 한 멤버는 Agentic Commerce와 최근 발표된 Google의 AP2 protocol (Agents to Payments) 간의 유사점을 언급했습니다.

응답은 없었습니다.

---

## 🔗 링크 (424개)

1. [https://news.smol.ai/](https://news.smol.ai/)
2. [1.5 years since the Sora announcement and 10 months since Sora.com was released to the public](https://news.smol.ai/issues?pattern=sora)
3. [Meta announced their controversial Vibes app](https://about.fb.com/news/2025/09/introducing-vibes-ai-videos/)
4. [leaked](https://x.com/apples_jimmy/status/1972756684297978256?s=46)
5. [good](https://x.com/anuatluru/status/1973125101047451830)
6. [7x smaller](https://news.ycombinator.com/item?id=39386156)
7. [Sora 2](https://openai.com/index/sora-2/)
8. [https://resend-attachments.s3.amazonaws.com/7J19wf50Kuvi3KH](https://resend-attachments.s3.amazonaws.com/7J19wf50Kuvi3KH)
9. [Genie research](https://news.smol.ai/issues/25-08-05-gpt-oss)
10. [some training on video games](https://x.com/elder_plinius/status/1973124528680345871)
11. [browser output](https://x.com/jesperengelen/status/1973147038499086523)
12. [Veo 3](https://youtu.be/hlcAZ2lX_ZI)
13. [https://resend-attachments.s3.amazonaws.com/E9PP9VDCUU9CCGJ](https://resend-attachments.s3.amazonaws.com/E9PP9VDCUU9CCGJ)
14. [personal blogpost](https://blog.samaltman.com/sora-2)
15. [Sora iOS app](https://apps.apple.com/app/id6744034028)
16. [website](https://sora.com/)
17. [Sama promised earlier this year](https://www.theverge.com/openai/648130/openai-social-network-x-competitor)
18. [first viral video](https://x.com/GabrielPeterss4/status/1973120058907041902)
19. [former members](https://x.com/willdepue/status/1973089331284681110)
20. [the livestream](https://www.youtube.com/watch?v=gzneGhpXwjU)

*... 그 외 404개 링크*

---

*이 문서는 Gemini 2.5 Flash를 사용하여 자동 번역되었습니다.*
