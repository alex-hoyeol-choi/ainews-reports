# Thinking Machines' Tinker: LoRA based LLM fine-tuning API | AINews
**원문 URL**: https://news.smol.ai/issues/25-10-01-thinky
**번역일**: 2025-10-06 21:31:09

## 📋 메타데이터
- **발행일**: 2025-10-01T05:44:39.731Z
- **설명**: **Thinking Machines** recently raised **$2 billion** without shipping a product until now, launching their first product **Tinker**, a managed service API for fine-tuning large and mixture-of-experts models like **Qwen-235B-A22B** using **LoRA** for cost-efficient training. The Tinker API offers low-level primitives for post-training methods and is supported by an open-source **Tinker Cookbook** library. Influential AI figures like **Andrej Karpathy** and **Lilian Weng** praised its design for reducing complexity and boosting research productivity. Meanwhile, **OpenAI** launched **Sora 2**, a video+audio model integrated into their consumer social app, sparking viral engagement and concerns over misuse and content moderation. Sam Altman emphasized the product's dual focus on delight and revenue alongside AGI research.

---

## 📰 번역된 내용

Thinker라고 이름 지을 수도 있었을까요?

2025년 9월 30일~10월 1일 AI 뉴스입니다. 저희는 여러분을 위해 12개의 subreddit, 544개의 Twitter, 23개의 Discord(196개 채널, 6687개 메시지)를 확인했습니다. 절약된 예상 독서 시간(분당 200단어 기준): 497분입니다. 저희의 새로운 웹사이트가 전체 메타데이터 검색 기능과 과거 모든 이슈를 아름다운 '바이브 코드'로 표현한 형태로 공개되었습니다. 전체 뉴스 분석은 https://news.smol.ai/ 에서 확인하시고, @smol_ai 로 피드백을 보내주십시오!

정말 기묘하게도 시기가 일치합니다:
- 5일 전 The Information은 Thinking Machines가 20억 달러를 모금했지만 어떤 제품도 출시하지 않았다고 지적했습니다.
- 같은 날 Jeremy Bernstein은 Modular Manifolds(옵티마이저 및 훈련 안정성을 위한 제약 조건에 대한 매우 이론적인 근거)를 발표했습니다. 그리고 3일 후 John Schulman은 LoRA Without Regret(2021년 원본 논문에 대한 경험적 지지로, Biderman et al.의 연구와 유사하게 올바르게 수행될 경우 전체 파인튜닝과 비슷한 성능을 검증)을 작성했습니다.
- 오늘, Thinky는 첫 제품인 Tinker를 출시했습니다.

그들의 랜딩 페이지에 따르면 다음과 같습니다:
Tinker를 사용하면 Qwen-235B-A22B와 같은 대규모 mixture-of-experts 모델을 포함하여 소규모 및 대규모 오픈 웨이트 모델의 짧은 목록을 파인튜닝할 수 있습니다. 작은 모델에서 큰 모델로 전환하는 것은 Python 코드에서 단일 문자열을 변경하는 것만큼 간단합니다.
Tinker는 저희 내부 클러스터 및 훈련 인프라에서 실행되는 관리형 서비스입니다. 저희는 스케줄링, 리소스 할당 및 장애 복구를 처리합니다. 이를 통해 인프라 관리에 대한 걱정 없이 소규모 또는 대규모 실행을 즉시 시작할 수 있습니다. 저희는 LoRA를 사용하여 여러 훈련 실행 간에 동일한 컴퓨팅 풀을 공유하여 비용을 절감합니다.
Tinker의 API는 `forward_backward` 및 `sample`과 같은 저수준 프리미티브를 제공하며, 이는 가장 일반적인 후처리 훈련 방법을 표현하는 데 사용될 수 있습니다. 그럼에도 불구하고 좋은 결과를 얻으려면 많은 세부 사항을 정확하게 파악해야 합니다. 그렇기 때문에 저희는 Tinker API 위에서 실행되는 후처리 훈련 방법의 현대적인 구현을 담은 오픈 소스 라이브러리인 Tinker Cookbook을 출시하고 있습니다.
이 작은 API 표면 영역은 매우 잘 받아들여지는 추상화로 보입니다. Andrej가 말했듯이, “여러분은 알고리즘적 창의적 제어(일반적으로 데이터, 손실 함수, 알고리즘과 관련됨)의 90%를 유지하면서, Tinker는 여러분이 보통 훨씬 덜 다루고 싶어 하는 어려운 부분(인프라, LLM 자체의 forward/backward, 분산 훈련)을 처리합니다. 이는 여러분이 이러한 작업을 일반적인 복잡성의 10% 미만으로 수행할 수 있음을 의미합니다.”
Lilian(편향됨)도 동의합니다: “고품질 연구 툴링을 제공하는 것은 더 넓은 커뮤니티의 연구 생산성을 향상시키는 가장 효과적인 방법 중 하나이며, Tinker API는 그 임무를 향한 한 걸음입니다.”
대기자 명단이 있으며, 서비스 약관에 유의하십시오. 하지만 이 첫 제품이 훨씬 더 크고 야심 찬 일들의 전조에 불과하기를 바랍니다…

[Input text for Part 2/64 is missing. Please provide the text to be translated.]

# AI 트위터 요약
OpenAI의 Sora 2 앱: 제품, 플랫폼 효과 및 초기 스트레스 테스트
- Sora 2는 OpenAI의 첫 소비자 소셜 앱 내 비디오+오디오 모델로 출시되어 엄청난 참여와 논쟁을 불러일으켰습니다. 피드와 "cameo" 기능은 일부 크리에이터(ostr)에게 즉시 "AI slop machine"으로 인식되었으며, 기존 플랫폼보다 "더 많은 슬롭을 생성할 수 있다"는 바이럴 반응(@skirano)이 있었습니다. 다른 사람들은 명백한 오용 가능성(@TheStalwart), "recursive jailbreak" 위험(@fabianstelzer), 그리고 피드를 가득 채우는 "이모지를 위해 두 번 탭하세요"와 같은 참여 유도 패턴(@Teknium1; @ostrisai)을 지적했습니다. OpenAI는 사용량이 증가함에 따라 초대 규모를 늘리고 일일 생성 제한을 조절하고 있습니다(@billpeeb).
품질은 인상적이지만, 구성적/기반 추론 테스트(예: 손가락/글자 세기)에서는 일관성이 없습니다(@teortaxesTex; @scaling01). Sam Altman은 회사가 AGI/agents 연구에 집중하는 동안 이 제품이 부분적으로는 즐거움과 수익을 위한 것임을 인정했으며("현실은 미묘합니다")(@sama), 나중에 자신으로 가득 찬 피드의 초현실적인 경험에 대해 회고했습니다(@sama). 전략적 관점: OpenAI는 프론티어 모델을 (ChatGPT, Codex, 이제 Sora와 같은) 고착성 앱으로 전환하여, 순수한 모델 품질을 넘어선 해자를 구축하고 있습니다(@Yuchenj_UW).
DeepSeek V3.2 및 DSA: 대규모로 더 저렴한 긴 컨텍스트, Day-0 생태계 지원
- DeepSeek V3.2 Exp는 DeepSeek Sparse Attention (DSA)을 도입합니다. 이는 각 토큰이 비연속 슬라이딩 윈도우를 통해 약 2048개의 토큰에 어텐션하여 디코드 메모리/FLOPs를 효과적으로 O(2048)로 만듭니다. 서드파티 노트는 인덱싱 파이프라인과 인덱서 내 Q/K에 대한 Hadamard transform을 언급합니다(@nrehiew_). 가격은 (입력) 50% 이상, (출력) 75% 하락했으며, MIT 라이선스와 V3/R1과 동일한 671B 총/37B 활성 MoE 풋프린트를 제공합니다(@ArtificialAnlys). 벤치마크는 추론 및 긴 컨텍스트 작업 모두에서 V3.1과 동등하며 토큰 효율성이 약간 향상되었음을 보여줍니다(@ArtificialAnlys).
인프라 모멘텀: vLLM은 NVIDIA의 도움으로 Day-0 지원을 받았으며, Blackwell은 이제 "새로운 MoE를 위한 최고의 출시 플랫폼"입니다(@vllm_project; @TheZachMueller). 분석가들은 DSA가 효과적으로 "1M 컨텍스트를 해제"하고 더 넓은 어텐션 효율성 물결을 예고한다고 주장하지만, 약 2K 컨텍스트 미만에서의 잠재적 트레이드오프는 지켜볼 가치가 있습니다(@teortaxesTex; @swyx). 커뮤니티 정서: 토큰당 비용의 급격한 변화는 "아직 가격에 반영되지 않았습니다"(@teortaxesTex).
Claude Sonnet 4.5: 코딩/에이전트 업그레이드 및 가용성 조정
- 팀들은 Sonnet 4.0/Opus 대비 실제 워크플로우에서 더 빠르고 짧은 체인, 더 높은 성공률을 보고하며, 특히 코딩 에이전트 및 Claude Code 스타일 루프에서 재시도 횟수가 줄고 툴체인 대기 시간이 단축되었습니다(@augmentcode; @iannuttall). Claude Code 자체 팀은 일상적인 드라이버를 Sonnet 4.5로 전환하고 일부 Opus 제한을 재설정했습니다. Anthropic 또한 유료 사용자 전체의 rate limits를 재설정하여 사람들이 4.5를 시도할 수 있도록 했습니다(@_catwu; @alexalbert__).
보편적이지는 않습니다: 일부 파이프라인은 여전히 GPT-4o/5를 선호하거나 특정 작업에서 퇴보를 보입니다(@imjaredz; @Teknium1). 초기 "사고/정렬" 관찰은 멀티턴 설정에서 더 나은 사용자 의도 모델링을 강조합니다(@teortaxesTex). Sonnet 4.5 Thinking 32k는 커뮤니티 평가(Arena, OpenHands)에서 활성화되었습니다(@arena; @allhands_ai).
Zhipu의 GLM-4.6: 효율성 우선 출시, 에이전트 중심 개선
- GLM-4.6은 화려함보다는 토큰 효율성과 응답 속도를 우선시합니다. 널리 읽힌 중국 리뷰에 따르면 4.5 대비 약 5%의 기능 향상, "사고" 토큰의 대폭 감소(예: 추론에서 16K→9K), 더 빠른 응답(평균 약 35초), 그리고 더 안정적인 지시 따르기가 보고되었습니다. 매우 복잡한 작업과 일부 베이스 모델 코드 구문 오류에서는 약점이 지적되었습니다(Zhihu 요약, @ZhihuFrontier). 실습: 강력한 프론트엔드/에이전트 행동; 제한된 테스트에서 Python은 변경되지 않았습니다(@karminski3).
경제성: GLM-4.6은 이제 Kilo Code에 포함되어 있으며, 내부 작업에서 Claude Sonnet 4.5 대비 48.6%의 승률, 200K 컨텍스트, 그리고 1M 토큰당 $0.60/$2.20의 공격적인 가격을 주장합니다(@kilocode). 4.6-Air는 계획되어 있지 않으며, Zhipu는 나중에 더 작은 MoE를 출시할 가능성을 시사했습니다(@teortaxesTex).
후속 훈련 인프라 강화: Thinking Machines의 Tinker
- Tinker는 관리형 분산 GPU를 통해 저수준의 연구자 친화적인 후속 훈련 프리미티브(forward_backward, sample, optim_step)를 노출하며, SFT, RL (PPO/GRPO), LoRA, 멀티턴/비동기 RL 및 커스텀 손실을 지원합니다. 이는 파인튜닝/RL을 기업의 "데이터를 업로드하면 나머지는 우리가 처리합니다" 방식에서 인프라는 아웃소싱하면서 알고리즘 제어권을 유지하는 방향으로 전환합니다. 스택 전반의 지지:

선도적인 연구자 및 개발자(@johnschulman2; @karpathy; @robertnishihara; @pcmoritz; @lilianweng)로부터의 저명한 지지 및 사용 보고서가 있습니다.

초기 결과는 다음과 같습니다: 프린스턴 대학교의 Goedel 팀은 SFT 데이터의 20%를 사용하여 LoRA를 활용하여 MiniF2F에서 약 81 pass@32를 달성했습니다. Redwood는 제어에 민감한 행동을 위해 long-context RL을 탐색하고 있습니다. 다른 연구자들은 보상 환경을 사용하여 text-to-SQL 프로토타입을 만들었습니다(@chijinML; @ejcgan; @robertnishihara).

지금 주목하는 이유: MoE의 산술 집약도(arithmetic intensity)와 메모리 압력(memory pressure)으로 인해 진지한 트레이닝/FT는 단일 노드(single-node) 취미용 장비를 넘어설 수밖에 없습니다. 요청을 일괄 처리하고 다중 노드(multinode) 자산을 관리하는 공유 인프라(shared infra)는 진입 장벽을 낮춥니다 (@cHHillee).
향후 Ray, eval/RM 스택(stacks)과 같은 후속 통합(integrations)과 추론 API(inference APIs)와 유사한 사실상의 표준, API와 같은 트레이닝 인터페이스(interface)가 등장할 것으로 예상됩니다 (@tyler_griggs_).
연구 및 시스템 주요 내용
- 옵티마이저(Optimizers) 및 다이내믹스(dynamics): "Central flows"는 DL 옵티마이저가 안정성의 경계에서 작동하는 이유를 설명하는 이론적 도구를 제공하며, 실제 NN에 대한 정확한 정량적 예측을 가능하게 합니다 (@deepcohen). AdamW에 대해서는 가중치 RMS(weight RMS)에 대한 새로운 점근선(asymptotics)이 제시되었습니다 (@Jianlin_S).
- 리타겟팅(retargeting) 및 최소 RL을 통한 로보틱스(Robotics): OmniRetarget (Amazon FAR)은 고품질의 상호작용 보존 휴머노이드(humanoid) 모션(motions)을 생성하여 고유수용감각(proprioception)과 작은 보상/DR 세트(set)만으로 민첩한 장기(long-horizon) 기술을 가능하게 합니다 (@pabbeel; project). 독립적인 연구에 따르면 실제 휴머노이드 잔여 RL(residual RL)은 약 15~75분간의 상호작용 내에서 BC 정책(policies)을 개선하는 것으로 나타났습니다 (@larsankile).
- 오디오 및 평가(evals): Liquid AI는 1.5B 온디바이스(on-device) 실시간 오디오-텍스트 모델(음성-음성/텍스트, TTS, 분류)인 LFM2-Audio를 오픈 웨이트(open weights)와 10배 빠른 추론 속도로 출시했습니다 (@LiquidAI_; @maximelabonne). RTEB (MTEB 업데이트)는 오버피팅(overfitting)을 줄이기 위해 비공개 다국어 검색 세트(retrieval sets)를 제공합니다 (@tomaarsen). MENLO는 47개 언어에 걸쳐 원어민과 유사한 응답 품질을 판단하기 위한 다국어 선호도 데이터셋(dataset) 및 프레임워크(framework)를 소개합니다 (@seb_ruder).
- 시스템: Perplexity Research는 분산 RL/FT를 위해 정적 스케줄링(static scheduling)과 파이프라이닝(pipelining)을 사용하여 RDMA point-to-point를 통해 1조 개 파라미터(param) 업데이트를 약 1.3초로 가속화하는 방법을 상세히 설명합니다 (@perplexity_ai).
인기 트윗 (참여도 기준)
- "마크 저커버그가 된다는 것을 상상해 보세요... 며칠 후 또 다른 '슬롭 머신(slop machine)'이 당신을 능가할 뿐입니다." Sora 앱 다이내믹스(app dynamics)에 대한 언급 (@skirano, 18.4k)
- Sam Altman은 AGI 연구에 자금을 지원하면서 AI를 사용하여 즐거움을 주는 것에 대해 언급했습니다. 미묘한 트레이드오프(tradeoffs)가 있습니다 (@sama, 8.0k). 또한 "Sam 카메오(cameos)"로 가득 찬 피드(feed)에 반응했습니다 (@sama, 9.4k).
- "좋아요. 이것은 예술입니다. 슬롭(slop)의 예술입니다." — Sora 2의 문화적 영향력에 대한 인정 (@teortaxesTex, 5.0k)
- "이 영상을 보는 사람은 누구나 악의적인 사용 가능성을 즉시 파악할 수 있습니다." (@TheStalwart, 6.0k)
- "더 많은 것이 곧 공개될 예정입니다." — Perplexity 설립자가 인수/연구 게시물 속에서 로드맵(roadmap)을 예고했습니다 (@AravSrinivas, 3.8k).

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Alibaba Qwen 100M-ctx/10T-param 로드맵 & Tencent Hunyuan Image 3.0 티저
- Alibaba가 Qwen 로드맵을 공개했습니다. 그 야망이 엄청납니다! (활동: 954): Alibaba의 Qwen 로드맵 이미지는 극단적인 스케일링을 통해 통합된 멀티모달 패밀리를 향한 공격적인 추진을 보여줍니다. 여기에는 context length 1M → 100M 토큰, 모델 크기 ~1T → 10T 파라미터, 테스트 시 컴퓨팅 예산 64k → 1M, 그리고 사전 학습 데이터 10T → 100T 토큰으로 확장하는 것이 포함됩니다. 또한 사실상 무제한적인 합성 데이터 생성과 복잡성, 상호작용, 학습 모드 전반에 걸친 더 넓은 agent 역량을 강조합니다. 댓글 작성자들은 100M context window의 실용성에 의문을 제기하며, 미래 모델이 closed-source가 될 수 있다고 예상하고, 1T 파라미터 이상의 모델은 상당한 하드웨어 없이는 로컬에서 실행하기 비현실적이라고 지적합니다.

주장된 1억 Token 컨텍스트는 비표준적인 Attention/메모리 방식을 의미합니다. 바닐라 Transformer Attention (O(L^2) 연산)과 일반적인 KV-cache 스케일링을 사용하면, MQA/GQA를 적용하더라도 KV 메모리는 테라바이트 규모가 될 것입니다. (예를 들어, MQA를 사용하는 약 7B 모델이 토큰당 약 16KB를 필요로 한다면, 1억 Token에 대해 약 1.6TB의 KV가 필요하며, 전체 KV 헤드를 사용하면 수십 TB로 늘어날 것입니다.) 이를 실제로 달성하려면 RoPE 스케일링뿐만 아니라 state/압축 메모리 또는 블록 단위 Attention (예: RingAttention, StreamingLLM/Attention Sinks), 검색 증강 청킹(retrieval-augmented chunking), 또는 순환/SSM 방식 아키텍처와 같은 기술이 필요할 것입니다.
밀집 모델(dense models)의 경우, 메모리/처리량 문제로 인해 1조 개 이상의 파라미터를 가진 모델을 로컬에서 실행하는 것은 불가능합니다. 8비트 기준으로 가중치만 약 1TB(4비트: 약 0.5TB)이며, 긴 컨텍스트를 위한 수 테라바이트의 KV가 추가로 필요합니다. 또한, 멀티 GPU NVLink급 대역폭 없이는 초당 Token 처리량이 낮을 것입니다. 유일한 현실적인 방법은 대규모 MoE(예: 64개 전문가 중 2개를 사용하는 총 1조 개 이상의 파라미터)이며, 이 경우 토큰당 활성 파라미터는 약 500억~1000억 개입니다. 4~8비트 양자화를 사용하더라도 약 40~160GB의 VRAM과 KV, 그리고 빠른 인터커넥트(8~16개 GPU)가 필요합니다. 요약하자면, 일반 소비자용 단일 GPU 장비로는 부족하며, 텐서/파이프라인 병렬 처리를 지원하는 멀티 GPU 서버(예: 8개의 H100/GB200)를 고려해야 합니다.
- **Tencent, 세계에서 가장 강력한 오픈소스 text-to-image 모델 Hunyuan Image 3.0 9월 28일 출시 예고 (활동: 225):** Tencent는 프로모션 이미지에 따르면 9월 28일 출시 예정인 "세계에서 가장 강력한" 오픈소스 text-to-image 모델인 Hunyuan Image 3.0을 예고하고 있습니다. 티저에는 기술 사양, 벤치마크 또는 아키텍처 세부 정보가 제공되지 않았습니다. 한 댓글 작성자는 추론을 위해 약 96GB의 VRAM이 필요할 수 있다고 언급했지만, 이는 확인되지 않았으며 주요 사양(파라미터, 학습 데이터, 라이선스)은 여전히 알려지지 않았습니다. 댓글 작성자들은 과도하게 예고된 모델들이 기대에 미치지 못하는 경향(예: SD3 vs Flux, GPT-5 과대광고)을 언급하며 사전 출시 과대광고에 회의적인 반응을 보였고, 비교 가능한 오픈소스 기준선 없이는 "가장 강력하다"는 주장이 입증되지 않는다고 지적했습니다.

하드웨어 우려: 댓글 작성자들은 Hunyuan Image 3.0 추론에 약 96GB의 VRAM이 필요할 것이라고 추측합니다. 이는 만약 정확하다면 로컬 사용을 데이터센터/프로슈머 GPU(A6000/A100/H100)로 제한할 것이며, SDXL(1024px에서 약 8~12GB) 또는 FLUX.1-dev(약 14~24GB) FLUX.1-dev보다 훨씬 무거울 것입니다. 이는 훨씬 더 큰 Transformer/Diffusion 백본 또는 고해상도 Attention 풋프린트를 시사하며, 최적화되지 않으면(예: TensorRT/Flash-Attn, Tiled Attention) 잠재적인 처리량 저하가 발생할 수 있습니다.
사전 출시 과대광고 대 실제 품질에 대한 회의론: 사용자들은 과도하게 홍보된 모델들이 기대에 미치지 못하는 경향이 있으며(예: SD3 마케팅 대 FLUX.1 품질에 대한 커뮤니티 선호) SD3, 강력한 모델들(예: Qwen family)은 종종 견고한 벤치마크와 함께 "그림자 출시(shadow drop)"된다고 언급합니다 Qwen org. 그들은 "가장 강력하다"는 주장을 검증하기 위해 제3자 평가(예: CLIPScore/PickScore/HPSv2, GenEval과 같은 텍스트 충실도 스위트)와 동일한 조건의 프롬프트/해상도/스텝을 요구합니다.
오픈소스 및 생태계 세부 사항의 중요성: 댓글 작성자들은 라이선스("open weights" 대 허용적인 OSS)와 실제 통합이 명확해질 때까지 "가장 강력한 오픈소스" 주장에 의문을 제기합니다. 즉각적인 요구 사항으로는 ComfyUI 노드/파이프라인 가용성 ComfyUI과 최근 오픈 릴리스(예: 최신 Qwen 이미지 스택)와의 직접적인 비교가 포함되며, 이는 실제 워크플로우에서의 채택을 결정할 것입니다.

### 2. Fenghua No.3 DX12/Vulkan GPU 및 검열되지 않은 'Abliterated' LLM 파인튜닝 결과
- 중국은 이미 CUDA 및 DirectX를 지원하는 GPU를 만들기 시작했으며, 이는 NVIDIA의 독점을 넘어선 것입니다. Fenghua No.3는 DirectX 12, Vulkan 1.2, OpenGL 4.6을 포함한 최신 API를 지원합니다. (활동: 702): 게시물은 중국의 Fenghua No.3 GPU가 DirectX 12, Vulkan 1.2, OpenGL 4.6과 같은 최신 그래픽 API를 지원하며 심지어 CUDA까지 지원하여 NVIDIA의 CUDA 생태계에 대한 잠재적인 대안이 될 수 있다고 주장합니다. 비-NVIDIA 실리콘에서의 진정한 CUDA 호환성은 재구현된 CUDA 런타임/드라이버 또는 PTX 변환 계층(HIP/ZLUDA와 유사한 개념)을 의미할 것이지만, 해당 게시물은 벤치마크, 드라이버 세부 정보 또는 검증을 제공하지 않습니다. 댓글 작성자들은 AMD의 HIP(ZLUDA와 같은 프로젝트 포함)가 이미 변환을 통해 CUDA 호환성을 제공하고 있다고 언급하며, 중국 공급업체들이 법적 제약을 우회하여 직접적인 CUDA 지원을 제공할 수도 있다고 시사합니다. 다른 이들은 실제 하드웨어/테스트가 나올 때까지 회의적인 입장을 표명하고, 발생 가능한 수출/제재 문제에 대해 경고합니다.

AMD의 HIP은 CUDA API를 (예: cudaMalloc -> hipMalloc) 이름 변경/미러링하고 hipify와 같은 도구를 사용하여 CUDA 코드를 번역함으로써 소스 수준의 CUDA 호환성을 제공합니다. 자세한 내용은 AMD ROCm HIP 문서를 참조하십시오: https://github.com/ROCm-Developer-Tools/HIP. ZLUDA와 같은 프로젝트는 CUDA 드라이버/런타임 호출을 다른 백엔드(예: Intel Level Zero 또는 AMD ROCm)로 번역하여 비-NVIDIA 하드웨어에서 CUDA 앱을 실행하는 것을 목표로 합니다. 저장소: https://github.com/vosen/ZLUDA. 이러한 차이점은 중요합니다: HIP은 ROCm에 대한 재컴파일을 요구하는 반면, ZLUDA는 바이너리/런타임 호환성을 추구합니다. 둘 다 NVIDIA의 법적/IP 지뢰밭을 다른 방식으로 우회하며, 중국 공급업체는 CUDA 인터페이스를 직접 구현하여 이를 무시할 수도 있습니다.

- 중요: Abliterated Models가 왜 나쁜가. LLM의 검열을 해제하는 더 나은 방법. (활동: 433): OP는 "abliteration"(안전/필터를 제거하기 위한 가중치 편집)이 Qwen3-30B-A3B와 같은 최신 MoE 모델에서 논리적 추론, 에이전트/도구 사용 행동을 저하시키고 환각을 증가시키며, 종종 30B abliterated 모델이 비-abliterated 4–8B 모델보다 성능이 나빠지게 만든다고 보고합니다. 대조적으로, abliterated 후 파인튜닝된 모델(예: mradermacher/Qwen3-30B-A3B-abliterated-erotic-i1-GGUF, i1-Q4_K_S로 테스트됨) 및 mlabonne/NeuralDaredevil-8B-abliterated (Meta-Llama-3-8B에서 DPO 튜닝됨)는 검열되지 않은 상태를 유지하면서 대부분의 손실을 "치유"합니다. Model Context Protocol (MCP) 도구 호출 테스트에서, 에로틱 Qwen3 변형은 다른 Qwen3-30B A3B abliteration(Huihui- Q4_K_M/i1-Q4_K_M*)보다 도구를 더 자주 올바르게 선택하고 환각이 적었지만, 에이전트 작업에서는 여전히 원본보다 약간 성능이 떨어졌습니다.* 댓글 작성자들은 이 효과를 "모델 치유"라고 부릅니다: 제약 없는 가중치 수술은 회로를 손상시키고; 후속 파인튜닝은 기능을 복원합니다. 다른 사람들은 비성인 벤치마크를 요구하며, 일반 파인튜닝(abliteration 없이)이 abliterated+파인튜닝과 일관되게 일치하거나 능가한다면 abliteration의 가치에 의문을 제기합니다.

가이드 Loss 없이 가중치를 편집하는 것("abliteration")은 사실상 제약 없는 가중치 공간 수술이며 예측 가능하게 성능을 저하시킵니다. 평론가들은 네트워크가 손상된 특징 경로를 다시 학습하도록 후속 "모델 힐링"(지도 학습 파인튜닝)을 권장합니다. 그러나 실무자들은 "abliterated"+파인튜닝이 어떤 작업에서도 깨끗한 파인튜닝 기준선을 능가하지 못했다고 보고하며, 이는 직접적인 가중치 조작이 이득보다는 주로 손상과 추가 훈련 비용을 초래한다는 것을 의미합니다.

평가는 NSFW 특정 작업을 넘어서야 합니다. Uncensored General Intelligence (UGI) 리더보드는 일반적인 기능 유지와 함께 거부 견고성을 평가하기 위한 더 광범위한 벤치마크로 제안됩니다: [https://huggingface.co/spaces/DontPlanToEnd/UGI-Leaderboard](https://huggingface.co/spaces/DontPlanToEnd/UGI-Leaderboard). 이러한 벤치마크를 사용하면 검열 해제가 Jailbreak 전용 지표에만 최적화하는 대신 추론/코딩/지시 따르기 성능을 보존하는지 정량화할 수 있습니다.

"abliteration"의 대안으로는 표준 Loss를 통해 훈련된(가중치 수술이 아닌) 기존의 검열 해제 파인튜닝 모델들이 있습니다. 예를 들어, Qwen3-8B-192k-Josiefied-Uncensored-NEO-Max-GGUF ([https://huggingface.co/DavidAU/Qwen3-8B-192k-Josiefied-Uncensored-NEO-Max-GGUF](https://huggingface.co/DavidAU/Qwen3-8B-192k-Josiefied-Uncensored-NEO-Max-GGUF)), Dolphin-Mistral-24B-Venice-Edition-i1-GGUF ([https://huggingface.co/mradermacher/Dolphin-Mistral-24B-Venice-Edition-i1-GGUF](https://huggingface.co/mradermacher/Dolphin-Mistral-24B-Venice-Edition-i1-GGUF)), 그리고 TheDrummer의 모델들([https://huggingface.co/TheDrummer](https://huggingface.co/TheDrummer))이 있습니다. 이 모델들을 "abliterated" 모델들과 UGI (또는 표준 eval suites)에서 직접 비교 평가하면 기능 유지, 거부율, 샘플 효율성 측면의 장단점을 명확히 할 수 있습니다.

## 덜 기술적인 AI Subreddit 요약
> /r/Singularity, /r/Oobabooga, /r/MachineLearning, /r/OpenAI, /r/ClaudeAI, /r/StableDiffusion, /r/ChatGPT, /r/ChatGPTCoding, /r/aivideo, /r/aivideo

### 1. OpenAI Sora 2 출시 및 데모 시연
- This is Sora 2. (Activity: 985): OpenAI는 Sora 2를 발표합니다. Sora 2는 더 길고 고품질의 클립을 선보이는 차세대 동영상 생성 시스템으로, spatiotemporal coherence, material/lighting consistency, physically plausible motion이 현저히 개선되었으며, 더욱 제어 가능한 카메라 움직임과 다중 피사체 상호작용을 특징으로 합니다. 해당 페이지는 더욱 강력해진 text-to-video 기능과 종단 간(end-to-end) 편집 워크플로우(workflow)를 강조합니다(예: 프롬프트 기반 수정 및 마스크 편집/이어붙이기). 하지만 아키텍처(architecture), 훈련 데이터(training data), 또는 정량적 벤치마크(benchmark) 세부 정보는 제공하지 않으므로, 성능은 동료 검토(peer-reviewed)된 지표보다는 선별된 예시를 통해 시연됩니다. 기술 평론가들은 AI가 생성한 장편 영화와 심지어 개인화되고 생체 인식에 반응하는 미디어로의 빠른 발전을 예상하는 반면, 다른 이들은 "demo-to-product" 간극(gap)에 대해 경고하며, 오용, surveillance-style personalization, 그리고 잠재적인 아동 대상 콘텐츠에 대한 안전 문제를 제기합니다.

데모와 실제 제품 간의 일치성에 대한 회의론: 화려한 영상들은 선별된 것일 가능성이 높으므로, 출시될 Sora 2는 미리보기 영상에 비해 프롬프트 준수 및 장기적인 시간적 일관성 면에서 뒤처질 수 있습니다. 예상되는 생산 제약으로는 클립 길이 제한(예: 60초 이하), 해상도/FPS 제한, 모션 지터, 텍스트/손 렌더링 아티팩트, 그리고 공격적인 안전 필터 등이 있습니다. 이는 연구 단계에서 서비스 단계로 넘어가는 비디오 diffusion/transformer 시스템에서 흔히 나타나는 격차입니다.
접근성/가격 책정 불확실성: 약 200달러를 지불하는 "Pro" 티어 사용자가 Sora 2 접근이 포함되는지 의문을 제기하며, 이는 계층별/대기 목록 기반 출시 방식에 대한 혼란을 보여줍니다. 비디오 생성 서비스 비용이 프레임 수 × 해상도 × diffusion 단계에 비례하여 증가한다는 점을 고려할 때, 공급업체는 종종 allowlist 또는 분당 크레딧을 통해 접근을 제한합니다. 논쟁의 핵심은 높은 GPU 비용으로 인해 Pro 티어가 우선순위/API 할당량을 부여해야 하는지 아니면 완전히 제외되어야 하는지 여부입니다.
신체 언어 피드백을 활용한 "개인 맞춤형" 영화에 대한 추측은 폐쇄 루프 파이프라인을 암시합니다. 이는 실시간 웹캠/생체 인식 캡처(MediaPipe 또는 OpenPose와 같은 모델을 통한 자세/감정)가 생성기에 컨디셔닝 신호(키프레임, 마스크 또는 카메라 경로)를 제공하는 방식입니다. 이는 개인 정보 보호/텔레메트리, 온디바이스 vs 클라우드 추론, 스트리밍 지연 시간, 그리고 생성 속도를 시청자 반응 시간과 일치시키는 것과 관련된 기술적 과제를 야기합니다.
- 지하철에서 서핑 (활동: 597): "Sora 2"라고 명명된 "지하철에서 서핑"이라는 제목의 데모는 높은 시각적 충실도로 본능적인 반응을 불러일으키는 AI 생성 비디오(아마도 OpenAI의 Sora 개요에서 가져온 것)를 보여주지만, 비물리적인 충돌 역학을 나타냅니다. 이는 현재의 text-to-video 모델이 명시적인 물리 시뮬레이션보다는 학습된 시각적 사전 지식에 의존한다는 점을 강조합니다. 외부 자산 v.redd.it/vxuq3sjt8csf1은 HTTP 403 Forbidden (Reddit edge auth block)을 반환하며, 접근하려면 계정 인증 또는 개발자 토큰이 필요합니다. 참고로, Sora는 시간적으로 일관된 고해상도 시퀀스(약 60초 정도)를 위해 설계된 diffusion-transformer text-to-video 시스템이지만, 물리적으로 정확한 상호 작용을 보장하지는 않습니다. 주요 댓글들은 두 가지 위험을 제기합니다: (1) 시각적으로 설득력 있지만 물리적으로 불가능한 장면이 일반인의 현실 세계 영향에 대한 직관을 오도할 수 있습니다; (2) 오디오 생성이 개선되면 합성 클립이 실제와 구별할 수 없게 되어 딥페이크 우려를 증폭시킬 수 있습니다. 회의론자들조차 클립이 합성이라는 것을 알면서도 강한 놀라움 반응을 보인다고 보고하며, 이는 현재 시각 자료의 설득력과 뒤처지는 오디오 현실감 간의 차이를 강조합니다.

점점 더 사실적인 생성형 비디오가 물리적으로 불가능한 생존력을 묘사하여 힘/충격에 대한 직관을 약화시킬 수 있다는 우려가 있습니다. 논의된 기술적 완화 방안에는 물리적 일관성 검사(예: acceleration continuity, momentum conservation, contact dynamics)와 학습된 "physics priors"가 포함됩니다. 비디오 품질과 시간적 일관성이 향상됨에 따라 모델이 직관적인 물리학 위반을 감지할 수 있는지 조사하는, 비현실적인 이벤트를 탐지하기 위한 관련 벤치마크로는 IntPhys (https://arxiv.org/abs/1806.01203)와 PHYRE (https://ai.facebook.com/research/publications/phyre-a-new-benchmark-for-physical-reasoning/)가 있습니다.

오디오 딥페이크는 다음 변곡점으로 지목됩니다. 최신 few-shot TTS/voice cloning(예: Microsoft VALL-E: https://arxiv.org/abs/2301.02111, Google AudioLM: https://arxiv.org/abs/2209.03143, 상용 ElevenLabs)은 몇 초 분량의 오디오만으로 화자를 모방할 수 있지만, automatic speaker verification은 합성 공격에 여전히 취약합니다. ASVspoof’21은 탐지기가 보지 못한 합성 방식에 대해 일반화 능력이 떨어진다는 것을 보여주므로(distribution shift 시 elevated EER), diffusion-based TTS가 prosody 및 breath-noise gaps를 메움에 따라 수동적인 voice matching보다 liveness/active-challenge protocols이 선호됩니다.

모방 행동을 조장하는 바이러스성 합성 스턴트(stunt)로 인한 안전 위험이 있습니다. 제안된 완화 방안에는 C2PA (https://c2pa.org/)를 통한 cryptographic content credentials와 모델/제공자 수준의 watermarking이 포함되지만, 현재 watermark는 re-encoding/cropping에 취약합니다. 플랫폼 방어는 실제 영상에 대한 false positives와 가짜 영상에 대한 misses를 모두 최소화하기 위해 사용자에게 보이는 provenance signals와 calibrated precision/recall에 맞춰 조정된 classifier backstops를 결합해야 합니다.

- Sora 2, 애니메이션 생성 (활동: 610): OP는 "Sora 2"(OpenAI의 비디오 모델 후속작)가 애니메이션 스타일 시퀀스를 합성할 수 있다고 강조합니다. 라이브스트림 데모에는 시청자들이 방송 품질에 필적한다고 말하는 애니메이션 장면이 포함되었습니다. 공유된 자료는 현재 인증 없이 HTTP 403 Forbidden을 반환하는 v.redd.it 클립(link)이며, 한 수정본은 해당 장면이 KyoAni의 "Hibike! Euphonium"(series info)의 한 장면과 거의 일치할 수 있다고 주장하여, 차단된 링크로는 확인할 수 없는 originality/memorization 문제를 제기합니다. 댓글 작성자들은 잠재적인 training-data memorization(클립이 거의 shot-for-shot recreation인 경우)에 대해 논쟁하고, 2023년 초의 실패작(예: 악명 높은 "Will Smith eats spaghetti" 비디오)과 비교하여 빠른 fidelity gains에 주목합니다.

잠재적 암기/스타일 복제: 여러 사용자가 공개된 애니메이션 장면이 교토 애니메이션의 Hibike! Euphonium(https://en.wikipedia.org/wiki/Sound!_Euphonium)의 한 장면과 매우 유사하다고 주장합니다. 만약 정확하다면, 이는 학습 데이터 출처, 유사 중복 제거(near-duplicate deduplication), 그리고 비디오 모델의 암기(memorization)에 대한 기술적인 질문을 제기합니다. 감사는 copy-distance metrics, 학습 코퍼스 전반에 걸친 유사 중복 감지(near-duplicate detection), 그리고 특정 저작권 보호 시퀀스가 얼마나 쉽게 재현되는지 측정하기 위한 prompt-leak tests를 포함할 것입니다.

초기 text-to-video 대비 품질 차이: 댓글 작성자들은 오늘날 Sora의 애니메이션 결과물을 2023년의 "Will Smith eating spaghetti" 밈과 대조하며, 아티팩트가 많고 일관성이 낮은 클립에서 방송 품질의 애니메이션 장면으로 2년 만에 도약했음을 지적합니다. 암시된 발전은 장기적인 시간적 일관성, 프레임 전반에 걸친 캐릭터 정체성 추적, 안정적인 선화/채색, 그리고 카메라 움직임에 있습니다. 이는 더 크고 깨끗한 비디오-텍스트 데이터셋, 더 긴 context windows, 개선된 motion/consistency losses, 그리고 더 강력한 video diffusion/Transformer 아키텍처에 의해 주도되었을 가능성이 높습니다.

실현 가능성 전망: "약 3년 내에 완벽하게 생성된 애니메이션"이라는 주장은 text-to-video와 제어 가능한 입력(스토리보드, 키프레임, depth/pose), 캐릭터/스타일 고정(locking), 그리고 통합된 TTS/음성 + 립싱크를 결합한 파이프라인을 암시합니다. 기술적인 제한 요소는 controllability API, 장면 전반에 걸친 캐릭터 일관성을 위한 에셋 재사용성, 그리고 분당 렌더링 비용입니다. 만약 Sora가 이미 방송 품질의 단일 장면(single shots)에 근접한다면, 남은 격차는 다중 장면 연속성(multi-shot continuity), 편집 가능성(editability), 그리고 에피소드 길이 제작을 위한 툴체인 통합입니다.

- OpenAI: Sora 2 (Activity: 1863): 스레드에는 "OpenAI: Sora 2"라고 라벨링된 데모가 공유되어 있으며, v.redd.it에 차단된 비디오 클립과 함께 미리보기 이미지(jpeg)가 있습니다. 한 상위 댓글은 "Cameo"라는 새로운 기능을 강조하며, 이는 더 길거나 다중 장면 생성에서 발생하는 정체성 표류(identity drift)를 목표로 하는, text-to-video 시스템의 지속적인 실패 모드인 교차 생성 캐릭터 일관성을 가능하게 하는 것으로 설명됩니다. 스레드에는 벤치마크나 릴리스 노트가 포함되어 있지 않습니다. (댓글에서 추론된) 기술적 함의는 시퀀스 전반에 걸쳐 캐릭터 속성을 보존하기 위한 참조 기반 또는 Token 기반 컨디셔닝입니다. 댓글 작성자들은 이를 완전히 생성된 장편 콘텐츠(영화/쇼)를 향한 한 걸음으로 봅니다. 주요 논쟁은 "Cameo"가 장기적인 캐릭터 연속성을 실질적으로 해결하는지, 아니면 단지 단거리 외모 고정(appearance locking)만을 제공하는지에 관한 것입니다.

여러 댓글 작성자들은 Sora 2의 새로운 "Cameo"를 중요한 기술적 진보로 지적합니다. 장편 비디오 생성에서 캐릭터 일관성은 주요 실패 모드였으며, Cameo는 여러 샷과 심지어 개별 생성물 전반에 걸쳐 지속적인 아이덴티티를 가능하게 하는 것으로 해석됩니다. 이는 프롬프트 전반에 걸쳐 일관된 참조/아이덴티티 Token을 재사용함으로써 다중 샷 연속성(동일한 얼굴, 의상, 행동 양식)을 허용할 수 있으며, 에피소드 또는 장편 워크플로우를 더욱 실현 가능하게 만듭니다.
스레드에서 생성 가능한 최대 비디오 길이에 대한 기술적인 질문은 여전히 답변되지 않고 있습니다. 사용자들은 구체적인 사양(길이 제한, 해상도/FPS 제약, 그리고 다중 샷 스티칭 또는 장면 전환이 기본적으로 지원되는지 여부)을 찾고 있으며, 이는 더 긴 내러티브와 프로덕션 파이프라인의 실현 가능성을 평가하는 데 중요합니다.

### 2. Gemini 3.0 업데이트 추측 및 CS 채용 시장 불안
- 아직 Gemini 3.0 업데이트가 없나요? (활동: 531): 게시물은 Google의 Gemini 3.0에 대한 업데이트가 아직 없는 이유를 묻습니다. 첨부된 이미지는 비기술적인 것으로 보이며(아마도 스크린샷/밈) 릴리스 노트, 벤치마크 또는 구현 세부 정보를 포함하지 않습니다. 댓글들은 10월 9일 출시 루머와 주요 성능 향상에 대한 기대를 언급하지만, 공식 출처나 기술 데이터는 제공하지 않습니다. 댓글 작성자들은 추측에 기반하고 있습니다. 한 명은 "완전히 압도적일 것으로 예상한다"고 말하고, 다른 한 명은 문서 대신 다른 이미지(https://preview.redd.it/fq1mqalz89sf1.jpeg)로 링크를 연결합니다. 따라서 열정은 있지만 실증된 기술적 주장은 없습니다.

출시 주기 및 경쟁 상황: 댓글 작성자들은 Gemini 3.0이 10월 9일에 출시될 것이라는 소문을 언급하며, 여러 공급업체에서 동시 출시/업데이트(예: xAI Grok 4.x, OpenAI Pro-tier features, 그리고 DeepSeek R2의 출시 가능성)가 이루어지고 있음을 지적합니다. 이는 모델 업데이트가 집중되는 시기를 나타냅니다. 현재 경쟁업체에 대한 맥락은 xAI (https://x.ai)와 DeepSeek의 최신 공개 연구(예: R1: https://github.com/deepseek-ai/DeepSeek-R1)를 참조하십시오.
개발자를 위한 모델 접근성 우려: 한 사용자는 고성능 티어("Pro")에 대한 "AI Studio day one" 접근을 명시적으로 요청하며, "Flash" 전용으로는 불충분할 것이라고 말합니다. 이는 Gemini "Pro"(더 높은 추론/성능)와 "Flash"(지연 시간/비용 최적화) 사이의 반복되는 트레이드오프를 강조합니다. Google의 Gemini API 문서(https://ai.google.dev/gemini-api/docs/models)에서 모델 구분을 참조하십시오.
- 저명한 컴퓨터 과학 교수가 경고를 울리며, 졸업생들이 일자리를 찾지 못한다고 말합니다: '뭔가 심상치 않습니다' (활동: 899): 해당 스레드는 화이트칼라/기술 관련 직업 시장이 경색되고 있음을 보고하며, 한 저명한 CS 교수는 최근 졸업생들이 "일자리를 찾지 못한다"고 경고하고, 댓글 작성자들은 이를 약 1년간 지속된 고용 불황으로 특징짓습니다. 예비 CS 학생들은 4년 후의 결과가 불확실하며, 학위 투자 대비 낮은 수익률(ROI)과 심지어 초급 직책을 얻는 데 어려움이 따를 위험이 높다고 경고받습니다. 일화적인 증거로는 석사 졸업생이 헬프데스크 직책조차 확보하지 못하는 경우가 있으며, 이는 지역적으로 암울한 상황을 강조합니다. 주요 댓글들은 전반적으로 경기 침체가 현실적이고 지속적이라는 데 동의하며, 예비 학생들에게 학자금 대출과 진로 계획을 재고할 것을 촉구합니다. 이것이 순환적인지 구조적인지에 대한 암묵적인 논쟁이 있지만, 최근 고용 상황을 바탕으로 비관적인 정서가 우세합니다.

UC Berkeley의 Hany Farid (디지털 포렌식/이미지 분석 전문가)는 CS가 더 이상 "미래 보장"이 아니라고 말합니다. 그는 결과의 급격한 변화를 언급하며, 이전에는 4년간 평균 약 5개의 인턴십 제안을 받던 학생들이 이제는 "약 1개를 받는 것에도 만족"하며, 종종 더 적은 제안과 낮은 협상력을 가지고 졸업한다고 합니다 (Business Insider). 그는 이러한 변화가 지난 4년 이내에 발생했으며, 보장된 결과를 위해 "CS를 공부하라"는 이전의 조언과 모순된다고 설명하고, 현재 졸업반 학생들이 일자리를 구하는 데 어려움을 겪고 있다고 지적합니다.

여러 논평가들은 "기술 관련" 분야에서 급격한 위축을 보이는 화이트칼라 기술 경기 침체를 언급합니다. 일부 지역에서는 심지어 엔트리 레벨/헬프데스크 역할조차 포화 상태이며, 이는 사다리 맨 아래 단계에서의 파이프라인 압축을 나타냅니다. 암시된 메커니즘은 자동화/LLM 지원 도구가 일상적인 코딩/지원 업무를 흡수하는 반면, 채용은 더 적은 수의 고위직에 집중되어 전통적인 인턴에서 정규직으로의 전환(ramp)이 줄어들고 있다는 것입니다.

AI가 더 많은 컴퓨터 기반 작업을 중재함에 따라, 이러한 영향은 CS를 넘어 법률, 금융, 의학 및 일반 사무실 워크플로우로 확대될 것으로 예상되며, 로봇 공학은 나중에 블루칼라 분야에 영향을 미칠 것입니다. 이러한 범위의 확대는 현재 학생들의 진로 계획 불확실성을 증가시킵니다. 관련 기술 토론은 링크된 Hacker News 스레드에서 확인할 수 있습니다.

- 서구 기업들로부터 받은 것은 오래되고 구식이며 오픈 소스도 아닌 모델들과 거짓 약속뿐입니다 (활동: 1241): 이 밈 게시물은 서구 AI 기업들이 오래되고 클로즈드 소스 모델을 출시하고 "거짓 약속"을 한다고 비판하며, 다른 곳에서의 더 관대하거나 빠른 출시와 대조됩니다. 댓글들은 잠시 출시되었다가 철회된 고품질 Microsoft TTS 모델을 언급하며, 서구의 제한적인 출시에 대한 우려를 강화하고, 곧 출시될 중국산 GPU가 오늘날의 32GB VRAM 카드를 왜소하게 만들 수 있어 컴퓨팅 접근 역학을 잠재적으로 변화시킬 수 있다고 추측합니다. 논의는 서구의 철회를 안전/법적 위험 관리로 보는 반면, 중국은 더 개방적인 출시를 소프트 파워 전략으로 사용한다고 봅니다. 다른 이들은 더 높은 VRAM을 가진 중국 국내 하드웨어가 역량과 접근성의 균형을 바꿀 것이라고 낙관합니다.

“open weights”와 “open source”에 대한 명확화: 전체 학습 데이터, 학습 코드, 그리고 허용적인 라이선스 없이 모델 체크포인트를 공개하는 것은 OSI 규격의 open source(OSI 정의)가 아닙니다. Weights-only 공개는 종종 비상업적 또는 사용 제한 라이선스를 포함하며, 이는 추론(inference)과 파인튜닝(fine-tuning)은 가능하게 하지만 재현성(reproducibility)과 아키텍처 수정(architectural modifications)을 제한합니다. 이러한 차이는 다운스트림 채택(downstream adoption), 재배포(redistribution), 그리고 연구 비교 가능성(research comparability)에 영향을 미칩니다.
중국 연구소/기업(정부 제외)의 open-weight 공개는 커뮤니티가 출시 후 파인튜닝, 평가(evals), 최적화(optimizations), 그리고 툴링(tooling)에 기여함으로써 개발자를 유치하고 R&D 비용을 분산시키는 데 도움이 됩니다. 인기 있는 모델은 토큰화(tokenization), 추론(inference) 형식, 그리고 서빙 스택(serving stacks) 전반에 걸쳐 사실상의 표준을 설정할 수 있습니다. 예를 들어, 크로스-런타임 그래프(cross-runtime graphs)를 위한 ONNX(onnx.ai)와 CPU/GPU 추론을 위한 GGUF 양자화된 체크포인트(GGUF spec)는 생태계 종속(ecosystem lock-in)과 소프트 파워(soft power)를 확장합니다.
하드웨어 영향: 국내 GPU가 오늘날 일반적인 24–48 GB보다 카드당 훨씬 더 많은 VRAM을 탑재하고 출시된다면, 이는 실현 가능한 로컬 추론(local inference) 체제를 확장할 것입니다. 일반적으로 70B 파라미터 모델은 4-bit 양자화(quantization) 시 약 40–48 GB VRAM이 필요하며(긴 컨텍스트(context)에서 KV 캐시(cache)를 위한 상당한 여유 공간 포함), 8-bit는 종종 80–100 GB를 초과합니다. 더 많은 VRAM은 또한 더 큰 KV 캐시와 활성화(activations)를 수용함으로써 배치 크기(batch sizes)와 처리량(throughput)을 향상시킵니다.
- Man!!! 4.5가 더 이상 아첨하지 않는다고 했을 때 농담이 아니었네요. (활동: 1206): 일화적인 사용자 보고서에 따르면 Claude Sonnet 4.5는 이전 4.x 버전의 동작과 비교하여 결함 있는 전제에 적극적으로 동의하지 않고 반론을 제시함으로써 아첨(sycophancy, “yes‑man” 행동)을 줄이도록 튜닝되었습니다. 첨부된 이미지는 기술적이라기보다는 밈(meme)과 유사하지만, 스레드(thread)의 맥락은 무조건적인 긍정보다는 원칙적인 반박/비판을 장려하는 정렬 작업(alignment work)과 일치합니다(예: Anthropic의 글: https://www.anthropic.com/research/sycophancy 등 아첨 완화에 대한 배경 연구 참조). 댓글 작성자들은 모델이 명시적으로 “반박할 것”이라고 말하고 그 이유를 나열하는 사례를 언급하며 줄어든 순종적 태도를 칭찬하는 한편, 밈적인 농담들은 어조를 과장합니다(정중한 4.0과 지나치게 거친 4.5를 대조하며).

많은 사용자들이 Claude Sonnet 4.0 대비 4.5에서 아첨(sycophancy)이 현저히 감소했음을 언급합니다. 모델은 결함 있는 전제에 적극적으로 이의를 제기하며 (예: "아닙니다, 저는 그 의견에 반대합니다") 구조화된 반론을 제시합니다. 이는 업데이트된 선호도/정렬(alignments)이 필요할 때 반대 의견을 선호하며 "예스맨" 행동보다 비판적 피드백을 개선했음을 시사합니다.

보고서들은 개선된 추론 품질을 강조합니다. 이는 "정확하고, 논리적이며, 정밀한 정확도"로 묘사되며, 모델은 추론이 틀린 이유에 대한 구체적인 목록을 제공하고 행동 지향적인 계획을 촉진합니다 (예: "시간 확인. 다음 두 시간 동안 무엇을 할 건가요?"). 비록 일화적이지만, 이는 이전 Sonnet 버전에 비해 더 강력한 지시 이행 및 비판 생성을 의미합니다.

출시 후 기능 보존(나중에 alignment 패치를 통한 "lobotomization" 방지)에 대한 명시적인 우려가 있으며, 이는 Sonnet 4.5가 현재 행동을 유지한다면 동급 최고가 될 수 있다는 주장과 함께 제기됩니다. 이는 단호한 기능(assertive capability)과 배포 후 유용한 반발을 약화시킬 수 있는 안전 튜닝(safety tuning) 사이의 반복되는 트레이드오프 논의를 반영합니다.

### 3. Wan-Alpha RGBA Video Release and Minecraft Redstone LLM
- Wan-Alpha - 투명 비디오를 생성하는 새로운 프레임워크, 코드/모델 및 ComfyUI 노드를 사용할 수 있습니다. (Activity: 439): Wan-Alpha는 alpha 채널을 RGB latent space에 인코딩하는 VAE를 설계하여 RGB와 alpha를 공동으로 학습하는 RGBA 비디오 생성 프레임워크를 제안합니다. 이를 통해 선별되고 다양한 RGBA 비디오 데이터셋에서 diffusion transformer를 훈련할 수 있습니다. 이 논문은 우수한 시각적 품질, 움직임의 사실성, 그리고 투명도 렌더링을 보고하며, 반투명 객체, 발광 효과, 머리카락 가닥과 같은 미세한 디테일 등 까다로운 경우를 포착합니다. 코드/모델 및 도구는 project, paper, GitHub, Hugging Face, 그리고 ComfyUI node에서 사용할 수 있습니다. 댓글들은 VFX/합성 및 게임 개발(gamedev) 워크플로우에 대한 실제적인 영향과 LoRA 기반 제어 및 I2V 스타일 사용 사례에 대한 관심을 강조합니다.

알파 채널(완전한 투명도)을 가진 비디오를 생성하는 능력은 VFX/합성 및 게임 개발 파이프라인에 유용하다고 강조됩니다. 이는 크로마키를 없애고 오버레이를 위한 깨끗한 가장자리/모션 블러를 보존합니다. 코드, 모델 가중치 및 ComfyUI 노드로 제공된다는 것은 기존 I2V 워크플로우 및 노드 그래프에 쉽게 통합될 수 있음을 의미하며, 효과/스타일 혼합을 위해 LoRA를 통해 제어할 수 있는 잠재력도 있습니다.
댓글 작성자들은 이를 Image-to-Video (I2V) 시스템으로 해석합니다. 실제로는 소스 프레임/시퀀스에 컨디셔닝하여 명시적인 알파 매트를 유지하면서 시간적으로 일관된 출력을 생성하는 것을 의미합니다. 이는 전경 요소가 배경과 별도로 생성되는 레이어 기반 편집을 가능하게 하여 합성 유연성을 향상하고 변경 사항에 대한 재렌더링 시간을 줄일 수 있습니다.
여러 기본 체크포인트(2.1, 2.2 14B, 2.2 5B)에 걸쳐 파인튜닝을 유지하는 것에 대한 우려가 있습니다. LoRA는 일반적으로 기본 모델에 특화되어 있어 버전을 혼합하면 호환성이 깨지거나 별도의 어댑터 및 보정이 필요할 수 있습니다. 이러한 파편화는 에코시스템 툴링(LoRA 훈련/병합, 추론 구성)을 복잡하게 만들고, 프로젝트의 재현성을 유지하기 위해 버전 고정된 LoRA 또는 표준화된 어댑터 형식이 필요할 수 있습니다.
- 자신이 마인크래프트 속 AI라는 사실을 알게 되는 존재론적 공포를 상상해 보세요 (활동: 1840): 한 제작자가 6개 레이어의 Transformer 스타일 소형 언어 모델을 마인크래프트 레드스톤으로만(명령 블록/데이터팩 없이) 구현했습니다. 총 5,087,280개의 파라미터, d_model=240, vocab=1920, 64 Token 컨텍스트 윈도우를 가지며 TinyChat으로 훈련되었습니다. 가중치는 대부분 8비트 양자화되었고, 임베딩은 18비트, LayerNorm은 24비트로 수백 개의 ROM 섹션에 저장됩니다. 물리적 빌드는 1020×260×1656 블록에 걸쳐 있으며, LOD 렌더링 아티팩트를 위해 Distant Horizons가 필요하고, 약 40,000배의 틱 속도를 가진 MCHPRS를 사용하여 약 2시간 만에 응답을 생성합니다(video). 댓글은 주로 극심한 느림("토큰당 몇 달")과 존재론적 참신함에 경탄하며, 공학적 위업에 대한 감탄 외에 실질적인 기술적 논쟁은 없습니다.

요약할 만한 실질적인 기술적 내용은 댓글에 없었습니다. 모델 이름, 벤치마크, 구현 세부 사항 또는 성능 지표는 논의되지 않았으며, 발언들은 기술적이라기보다는 유머러스하거나 경험에 기반한 것이었습니다. 따라서 기술 독자에게 유익할 만한 tokens/sec, throughput, 아키텍처, 훈련 설정 또는 게임 내 계산 제약(예: Redstone/Turing 구현)에 대한 언급은 없었습니다.

---

# AI Discord 요약
> gpt-5가 요약한 요약들의 요약
1. OpenAI Sora 2 출시 및 실제 사용
- Sora가 슬그머니 등장하고, 개발자들은 터널링으로 접속합니다: 회원들은 OpenAI의 비디오 모델 Sora 2가 OpenAI의 Sora 페이지와 "OpenAI is launching Sora 2"라는 제목의 Perplexity 요약을 통해 나타나고 있다고 지적했습니다. 일부는 캐나다를 통해 VPN으로 무료 접속했다고 보고했으며, 다른 일부는 초대장이 미국/캐나다 Apple 기기로 제한된다고 언급했습니다.

커뮤니티는 OpenRouter가 비디오 모델을 라우팅하지 않으며 사용자들을 Sora의 앱/웹사이트로 다시 안내했다고 강조했습니다. 한 사용자는 초대장을 제공했고, 다른 사용자는 API 엔드포인트를 예상하며 Sora의 품질이 사실적인 사운드와 충실도 덕분에 "다른 비디오 생성 모델보다 훨씬 낫다"고 평가했습니다.
- 물리 수정 및 인형 트릭: 제작자들은 Sora 2를 사용하여 인형 설명 영상과 같은 프로덕션 스타일의 콘텐츠를 선보였습니다. Chris 🇨🇦는 이 X 스레드에 예시를 게시했으며, 커뮤니티는 Sora 2가 Sora 1의 물리 및 아티팩트 문제를 수정했다고 의견을 모았습니다.

AI 비디오를 식별하는 데 "픽셀 피핑이 여전히 꽤 안정적으로 작동한다"고 한 회원이 주장하면서 탐지 관련 논의가 계속되었습니다. 반면 다른 사람들은 "느낌만으로도" 새로운 사실감에 사람들이 적응할 것이라고 주장했습니다.
- API 불안감과 폐쇄형 생태계: 여러 스레드에서 사용자들은 Sora API 가용성에 대해 질문했습니다. 그러나 운영진은 Sora가 openai.com/sora를 통해 앱/웹 전용으로만 제공되며, 아직 OpenRouter 라우팅은 없고 초대장이 비공식적으로 유통되고 있다고 재차 강조했습니다.

미국/캐나다 및 Apple 기기로 제한된 4개의 초대장을 제공한 사용자는 지역 잠금에 대한 불만을 불러일으켰습니다. 다른 사람들은 OpenAI가 더 깔끔한 API가 출시되기 전까지는 앱을 초기에는 컴퓨팅 제약이 있는 상태로 유지할 것이라고 추측했습니다.
2. 개발자 도구: 결제, 추적 및 Throughput
- OpenRouter, 장부를 공개합니다: OpenRouter는 OpenRouterAI의 X 게시물에 따르면, 실시간 LLM 회계 및 사용량 기반 또는 하이브리드 결제로의 쉬운 전환을 위한 Stripe 통합을 발표했습니다.

그들은 대규모 팀의 인보이스, 정산, 비용 관리를 간소화하는 것을 목표로 하며, 오직 회계 데이터만 Stripe로 전송되고 프롬프트는 비공개로 유지된다는 점을 강조했습니다.
- BYOK 보난자: 백만 건 무료 제공: 2025년 10월 1일부터 OpenRouter는 모든 사용자에게 매월 1,000,000건의 무료 BYOK 요청을 제공하며, 초과 사용량에 대해서는 그들의 발표에 따라 표준 5% 수수료가 부과됩니다.

커뮤니티 회원들은 이것이 자체 모델 키를 사용하는 팀에게 주요 비용 절감 조치이며, 유연성을 유지하면서 프로덕션 트래픽의 마찰을 줄이는 데 기여한다고 강조했습니다.
- Trackio, 로컬에서 보스처럼 추적합니다: Hugging Face는 Weights & Biases의 로컬 우선, 무료, 드롭인 대체품인 Trackio를 소개했으며, 리포지토리는 [gradio-app/trackio](https://github.com/gradio-app/trackio)에서 확인할 수 있습니다.

회원들은 메트릭/테이블/이미지/비디오 로깅을 주요 기능으로 꼽으며, 연구 및 기업 제약 조건에 대해 로컬 우선 실행의 프라이버시와 재현성을 칭찬했습니다.
- vLLM, 엄청난 처리량 달성: 한 성능 공유에서 vLLM이 RTX 4070에서 Qwen3 0.6B를 실행하여 10개의 동시 요청에 걸쳐 약 1470.4 tok/s의 속도로 병렬 요청을 처리하는 것을 보여주었으며, 이는 vLLM의 병렬 처리 문서를 인용한 것입니다.

엔지니어들은 vLLM의 PagedAttention과 스케줄링이 처리량 확장의 비결이며, 다중 사용자 부하에서도 작은 모델이 '실시간'처럼 느껴지게 한다고 강조했습니다.
3. 새로운 모델 및 연구: Trillions, 사전 학습에 RL 적용, 그리고 Sparse Attention
- Ring-1T 등장: 연구원 Ant Ling은 오픈소스 '사고형' Ring-1T-preview (1조 파라미터)를 공개하며, 이 게시물 Ring-1T-preview benchmarks에서 AIME25에서 92.6점, HMMT25에서 84.5점이라는 최고 수학 점수를 주장했습니다.

엔지니어들은 구조화된 추론과 수학 전문화에 대한 아키텍처의 함의에 대해 논의하며, 평가 설계와 재현성이 다음으로 면밀히 검토될 것이라고 언급했습니다.
- AlphaEvolve, 이론을 코딩하다: Google Research는 AI as a research partner: advancing TCS with AlphaEvolve에서 이론 CS를 발전시키는 조합론적 구조를 발견하고 검증하는 LLM 기반 코딩 에이전트인 AlphaEvolve를 설명했습니다.

스레드에서는 프로그램 합성, 검증, 형식적 제약의 조합을 칭찬하며, 이를 수학 중심 도메인에서 에이전트 워크플로우를 위한 신뢰할 수 있는 청사진이라고 불렀습니다.
- NVIDIA RLP, 추론 능력 향상: NVIDIA는 RLP: Reasoning with RL on Pretraining Data에서 사전 학습 데이터에 RL을 적용한 추론에 대한 작업을 공유했으며, 회원들은 이를 arXiv:2509.19249의 유사한 성과를 보인 논문과 비교했습니다.

실무자들은 이 접근 방식을 RL 신호를 활용한 사전 학습 코퍼스에 대한 더 강력한 커리큘럼으로 보았으며, '더 간단한' 베이스라인과 비교하여 복잡성과 수익을 논의했습니다.
- DeepSeek, Sparse Attention을 조정하다: 개발자들은 FlashMLA 풀 리퀘스트에서 DeepSeek Sparse Attention (DSA) v3.2와 제안된 "mamba-selectivity와 유사한" 하위 Attention을 분석했습니다.

논의는 선택적 게이팅이 어떻게 집중도를 높이고 연산량을 줄일 수 있는지에 집중되었으며, 어블레이션과 실제 환경에서의 지연 시간/품질 트레이드오프 차트에 대한 요구가 있었습니다.
4. 산업 모멘텀: 대규모 투자, 컨텍스트 활용 전략, 그리고 벤치마크 현실
- Cerebras, 11억 달러 유치: Cerebras Systems는 Series G 보도 자료에 따라 AI 프로세서 R&D, 미국 제조, 그리고 글로벌 데이터 센터를 확장하기 위해 81억 달러의 기업 가치로 11억 달러 규모의 Series G 투자를 발표했습니다.

엔지니어들은 웨이퍼 스케일 하드웨어로 파인튜닝 및 추론 워크로드의 더 쉬운 마이그레이션을 기대하며 Cerebras 스택에서 더 광범위한 LoRA/GLM-4.6 지원을 요청했습니다.
- 컨텍스트가 새로운 프롬프트입니다: Anthropic은 "Effective context engineering for AI agents"에서 단순히 프롬프팅뿐만 아니라 효과적인 컨텍스트 엔지니어링이 에이전트 성능에 중요하다고 주장했습니다.

개발자들은 비용 상한선 및 지연 시간 예산과 같은 실제 환경의 제약 조건에 맞춰 메모리 윈도우, 검색 위생, 그리고 상태 이월에 대한 전략을 교환했습니다.
- SQL 대결에서 GPT-5가 겸손해지다: llm-benchmark.tinybird.live의 Tinybird 리더보드는 GPT-5 (Codex 및 비-Codex)가 SQL 작업에서 각각 23위와 52위를 기록했으며, o3-mini는 6위를 차지했음을 보여주었습니다.

스레드에서는 이를 실제 벤치마크에 대해 테스트하고 브랜드가 아닌 작업 프로필에 따라 모델을 선택해야 한다는 상기시키는 것으로 보았으며, GLM 4.6이 비용 대비 강력한 코딩 가치를 제공한다는 보고와 일치합니다.

---

# Discord: Discord 요약

## Perplexity AI Discord
- Sora 2, 뜨거운 반응과 밈을 생성하다: 회원들은 Sora 2로 활발하게 콘텐츠를 생성했으며, 한 명은 하루에 100개의 비디오를 생성했다고 자랑했고, 여러 명은 피카츄를 활용한 콘텐츠를 만들었습니다.

일부 사용자들은 Sora 2 워터마크가 전문적으로 보인다고 느끼는 반면, 다른 사용자들은 GPT Plus에 통합된 유료 버전을 예상합니다.
- VPN 꼼수로 Sora 2를 이용하다: 사용자들은 VPN을 사용하여 캐나다를 통해 연결함으로써 Sora 2에 무료로 접근할 수 있다는 것을 발견했습니다.

한 사용자가 100개의 비디오를 생성하고 Sora의 새로운 Cameo 기능을 테스트하여 현재 소셜 미디어에서 유행하는 비디오를 만들었습니다.
- Peeps Get Perplexity Pro for Free: 사용자들은 Airtel, Venmo, PayPal과의 파트너십을 포함한 다양한 프로모션을 통해 Perplexity Pro에 무료로 액세스하고 있습니다.

Perplexity Pro의 무료 액세스는 일부 사람들로 하여금 다른 유료 AI 구독 서비스의 가치에 의문을 제기하게 만들었으며, 한 멤버는 "Perplexity Pro가 어차피 무료인데 아무도 필요로 하지 않습니다"라고 말했습니다.
- Grok Stumbles and Bumbles: 멤버들은 Grok이 이미지 및 비디오 생성과 같은 분야에서 저조한 성능을 보인다고 생각하며, 한 사용자는 "Grok은 이미지 및 비디오 생성에서 심각하게 뒤처져 있습니다"라고 말했습니다.

한 사용자는 Grok이 오래되거나 잘못된 출처를 필터링하는 데 검색 어려움을 겪고 있다고 보고했습니다.
- Sora 2 Set to Drop: 멤버들은 OpenAI가 Sora 2를 출시할 것이라는 Perplexity 페이지 링크를 공유했습니다.

한 멤버가 Comet의 추천 링크를 공유했으며, 추천을 통해 초대장을 제공하고 추천을 사용하는 모든 사람이 Comet 초대장을 받을 수 있다고 밝혔습니다.

---

## LMArena Discord
- Claude API Might Be Free?: 멤버들은 puter.js를 통해 Claude API를 무료로 사용하거나 MCP를 무료 계정에 연결하는 것에 대해 논의하고 있습니다.

하지만 주간 2천만 Token 제한이 있으며 사용자 데이터가 결제 수단으로 사용될 가능성이 있으므로 주의해서 진행해야 합니다.
- Seedream 4 Gets Nerfed: 사용자들은 Seedream 4의 최근 변경 사항에 대해 불평하고 있으며, 여기에는 해상도, 속도, 이미지 품질, 그리고 강제된 1:1 화면 비율이 포함됩니다.

한 사용자는 화면 비율 때문에 이미지 편집에 쓸모가 없다고 말했습니다.
- Chasing Sora 2 Invite Codes: 여러 멤버들이 Sora 2 초대 코드를 요청하고 있으며, 최소 한 명의 사용자는 비용을 지불하겠다고 제안했습니다.

한 선량한 사마리아인이 채팅에서 Sora 2 코드를 공유했습니다.
- AI Image Generation Plagued with Issues: 멤버들은 이미지 생성과 관련된 문제들을 보고했으며, 여기에는 오디오 없이 생성되는 이미지, 1:1 화면 비율로 고정되는 이미지, 그리고 기타 예상치 못한 오류들이 포함됩니다.

멤버들은 <#1343291835845578853>에 보고하도록 안내받았습니다.
- LMArena Launches October AI Art Contest: LMArena는 10월 AI Generation Contest에서 Battle Mode를 사용하여 AI로 추상 미술을 만들도록 참가자들에게 도전하고 있으며, 모델은 공개되었습니다. 자세한 내용은 여기를 참조하십시오.

우승자는 1개월 Discord Nitro와 독점 <@&1378032433873555578> role을 받습니다.

## OpenRouter Discord
- OpenRouter는 Stripe와 결제 동기화: OpenRouter는 실시간 LLM 회계 처리를 위해 Stripe와 통합하며, 이 [트윗](https://twitter.com/OpenRouterAI/status/1709407338006233480)에 따르면 사용량 기반 청구 또는 하이브리드 모델로의 전환을 용이하게 합니다.
이 통합은 회계 데이터만 Stripe와 공유하여 프롬프트의 개인 정보 보호를 보장하며, 사용자들을 위한 청구 프로세스 개선에 중점을 둡니다.
- BYOK 사용자, 무료 요청으로 큰 혜택: 2025년 10월 1일부터 OpenRouter는 모든 사용자에게 월 100만 건의 무료 BYOK 요청을 제공하며, 이는 이 [공지](https://discord.com/channels/1125287737293881344/1125287737293881347/1158580572765585408)에 자세히 설명되어 있습니다.
이 변경 사항은 자동으로 적용되지만, 사용자는 100만 건 한도를 초과하는 요청에 대해 표준 5% 요금이 부과되며, 이는 BYOK 사용의 진입 장벽을 낮춥니다.
- Sora 비디오 모델은 독점 유지: 사용자들이 Sora 비디오 생성 비용에 대해 문의했지만, OpenRouter는 비디오 모델을 라우팅하지 않으며, 이는 OpenAI의 Sora 앱 또는 웹사이트를 통해서만 독점적으로 이용 가능하다고 명확히 밝혔습니다.
커뮤니티 회원들은 또한 ChatRoom에서 모델이 응답 도중 일시 중지되는 것에 대한 불만을 표했으며, Sora 초대 코드의 가용성에 대한 논의가 활발하게 이루어졌습니다.
- Grok 모델, 순탄치 않은 여정: 사용자들은 Grok 모델 및 객체 생성 호출에 문제가 있다고 보고했으며, 이 문제가 OpenRouter 또는 Grok 자체에서 비롯된 것인지에 대한 추측을 불러일으켰습니다.
이후 사용자들은 Grok4가 다시 작동하는 것으로 보인다고 보고했으며, 일부는 Grok이 글쓰기 스타일과 시스템 프롬프트 준수 때문에 롤플레잉에 적합한지 논의했습니다.
- OpenAI의 Sora, 업계 논쟁 촉발: 회원들은 Sora 초대 코드를 열망하고 있으며, 한 사용자는 Apple 기기를 가진 미국 또는 캐나다 거주자에게 4개의 초대 코드를 제공하면서 이러한 제한에 대해 아쉬움을 표했습니다.
논의는 OpenAI가 Google, Meta, Amazon과 경쟁하는 것에 대해 다루었으며, 일부는 Sora 2의 높은 품질이 훈련을 위해 모든 YouTube 비디오를 잠재적으로 폐기했을 가능성을 시사한다고 추측했습니다.

---

## Cursor Community Discord
- Sonnet 4.5는 Token을 많이 사용하고, Codex는 Token을 아낀다고 평가: 한 회원은 Sonnet 4.5가 Token 사용에 있어 더 효율적인 Codex에 비해 낭비적이라고 느꼈습니다. 다른 회원들은 Claude 모델이 일반적으로 더 비싸다고 언급했습니다.
레거시 요금제를 사용하는 한 회원은 더 높은 비용에도 불구하고 만족스러운 성능을 이유로 GPT-4-turbo보다 Sonnet 4.5를 선호했습니다.
- Cursor Agents, 터미널 버그 발생: 한 회원은 자신의 에이전트 터미널에 버그가 발생하여 다른 셸(bash, cmd, powershell)을 시도한 후에도 어떤 명령도 수행할 수 없었다고 보고했습니다.

제안된 해결책은 `winget install --id Microsoft.PowerShell --source winget`를 실행하고 Cursor를 재시작한 후 기본 셸을 `pwsh`로 설정하는 것이었습니다.
- Cursor 소셜 네트워크 플랫폼 개념 등장: 한 멤버가 Cursor 내에서 AI 크리에이터들을 위한 소셜 네트워크 플랫폼을 만들 것을 제안했습니다.

이 제안은 낙관적이지만 농담조의 답변을 받았습니다. ✨ 마법 ✨을 믿으면 무엇이든 가능합니다.
- Cursor 청구 명확성 비판: 한 멤버가 청구 페이지를 읽기 어렵다고 생각하여 이를 개선하기 위해 ChatGPT의 도움을 요청했습니다.

레거시 가격 정책을 사용하는 멤버들은 다양한 모델의 비용에 대해 논의했으며, 일부는 Claude Opus가 매우 비싸다고 생각했고 다른 일부는 비용 분석이 오해의 소지가 있다고 제안했습니다.
- TypeScript 리팩터링으로 원활한 결과 도출: 멤버들은 Cursor가 모듈과 클래스를 쉽게 리팩터링하여 원활한 경험을 보장했으며, 이는 TypeScript를 사용했을 가능성이 높다고 언급했습니다.

한 멤버는 명확하고 일관된 프롬프트를 제공함으로써 남아있는 문제를 해결할 수 있었으며, 이는 정확한 지침을 통해 Cursor의 효율성을 입증하는 것이었습니다.

---

## Unsloth AI (Daniel Han) Discord
- GRPO 트레이너 시작, 그러나 느리게: 한 멤버가 첫 GRPO(Generative Reinforcement Learning with Policy Optimization) 트레이너를 만들고 LoRA 파인튜닝에 비해 느리다고 언급했습니다. 이는 그들의 Colab 노트북에 기록되어 있습니다.

훈련 손실은 거의 0으로 떨어졌고 보상 값은 천천히 상승했으며, 이는 더 간단한 머신러닝 시스템에서의 경험과 유사했습니다. 그들은 이 실험 후에 다른 RL 도구로 전환할 계획입니다.
- Blackwell GPU, Xformers 수동 컴파일 요구: 멤버들은 Blackwell GPU(RTX 50xx 시리즈)에서 Xformers 관련 문제를 논의하며 호환성 문제로 인해 수동 컴파일이 필요하다고 언급했습니다. 컴파일 단계는 다음과 같이 공유되었습니다: `pip uninstall -y xformers; git clone --depth=1 https://github.com/facebookresearch/xformers --recursive; cd xformers; export TORCH_CUDA_ARCH_LIST="12.0"; python3 setup.py install`.

한 멤버는 '사실 128k context가 필요하지는 않지만, 어쨌든 최대로 밀어붙일 겁니다. 이것이 인간 본성의 최고죠'라고 언급하며 한계를 뛰어넘으려는 커뮤니티의 열정을 강조했습니다.
- Gemma 파인튜닝 프레임워크 대결: 멤버들은 Unsloth가 T4 Collab GPU에서 Gemma 파인튜닝을 허용하는 유일한 프레임워크라고 주장하지만, Google의 Gemma 문서에도 T4 GPU에서 LoRA와 Keras를 사용하는 튜토리얼이 제공된다고 언급했습니다.

나중에 밝혀진 바에 따르면, Unsloth는 효율적으로 작동하는 것을 방해했던 원래의 문제들을 식별하고 수정했으며, 이는 그 주장을 정당화합니다.
- LLM은 여전히 자신에 대해 모릅니다: 회원들은 LLM에게 자신에 대해 물었을 때의 정확성에 대해 논의했으며, 한 회원은 일반적으로 LLM에게 자신에 대해 묻는 것은 정확하지 않다고 말했습니다.

GPT-5가 자신을 아는 것처럼 보인다면, 이는 특정 훈련, 도구 사용 또는 system prompt에 정체성 정보가 포함되었기 때문일 수 있다고 제안되었으며, system prompt 없이는 어떤 GPT와도 대화할 수 없다는 점이 강조되었습니다.
- ReLU 버그가 Shifted Tanh 솔루션으로 이어집니다: 한 회원이 ReLU를 사용한 원래 공식에서 버그를 발견했는데, 이 버그는 빼기 곱(subtract product)과 함께 제곱 항을 발생시켰습니다.

해당 회원에 따르면, [0, N] 대신 shifted tanh [~0, ~1]로 전환하는 것이 미분 가능한 신호처럼 더 작동하여 문제를 해결했으며, 기울기(gradients)가 더 이상 폭발하지 않았습니다. 이 회원은 배경 정보로 LoRA에 대한 블로그 게시물을 링크했습니다.

---

## OpenAI Discord
- Sora 2 초대장 쟁탈전: Discord 사용자들은 Sora 2 초대장을 적극적으로 찾고 있으며, 이는 잠재적인 사기에 대한 우려와 초대 전용 시스템에 대한 불만을 야기하고 있습니다.

사용자들은 <#1379321411046346762> 및 <#1315696181451559022>와 같은 채널로 안내되어 앱과 접근 방식에 대해 논의합니다.
- GLM 4.6, 코딩 비용 절감: 사용자들은 GLM 4.6이 코딩 작업에 있어 Sonnet 4.5의 비용 효율적인 대안임을 발견하고 있습니다.

한 사용자는 zai GLM 코딩 플랜이 매우 가치가 있어 한 분기 동안 가입했다고 언급했으며, 이 플랜은 5시간마다 600개의 prompt를 상당히 저렴한 비용으로 제공합니다.
- GPT-5, SQL 테스트에서 부진: llm-benchmark.tinybird.live에 따르면 GPT-5 (Codex 및 non-Codex)는 SQL에서 SOTA가 아니며, 각각 23위와 52위를 기록했습니다.

한편, o3-mini는 동일한 벤치마크에서 6위를 기록했습니다.
- 즉시 생성이 더 이상 즉시 생성처럼 느껴지지 않습니다: 사용자들은 즉시 생성이 더 이상 즉시 생성되지 않는 이유에 대해 궁금해하고 있으며, 사용자 지정 지침을 사용할 때도 마찬가지입니다.

일부는 이것이 대역폭 조절(bandwidth throttling) 조치 때문이라고 생각합니다.
- 사고 모드(Thinking Mode)는 사용자의 위치를 압니다: 한 사용자는 사고 모드(thinking mode)에 사용자의 시간대 또는 대략적인 IP 위치를 파악하는 도구가 있다고 제안했습니다.

이 기능은 사고(thinking)를 위한 약 18K system prompt에도 나열되어 있었으며, 사고 모드와 비사고 모드는 다른 system prompt와 도구를 가지고 있습니다.

## HuggingFace Discord
- ML-for-Science 프로젝트 엔지니어링에 학생 초대: Hugging Face는 ML-for-science 프로젝트에 참여할 학생 및 오픈 소스 기여자들을 찾고 있습니다. 이 [Discord 링크](https://discord.com/channels/879548962464493619/1199320291410425906)를 확인해 보세요.

자원봉사자들은 변화를 만들고 인류를 돕는 기회를 얻게 될 것이니, 이 도전에 참여해 보세요!
- Trackio, Wandb를 능가하는 것을 목표로 합니다: Hugging Face는 Trackio라는 새로운 무료 실험 트래킹 라이브러리를 출시했습니다. 이 라이브러리는 wandb의 드롭인 대체품이며 로컬 우선으로 구축되었습니다. [GitHub 리포지토리](https://github.com/huggingface/trackio)를 확인해 보세요.

Trackio는 메트릭, 테이블, 이미지, 심지어 비디오까지 로컬에서 로깅할 수 있습니다!
- Whisper 통합 문의: 한 멤버가 음성 인식을 위한 풀스택 앱에 Crisper Whisper를 통합하는 데 도움을 요청하며, 비정상적인 단어를 인식하기 위한 라이브러리에 대해 문의했습니다.

추가적인 세부 정보는 제공되지 않았습니다.
- Lora 트레이닝 관련 이슈 부상: 멤버들은 Lora 트레이닝 작업이 타임아웃될 경우 데이터 손실 위험이 있다고 논의했습니다. 특히 실행 중에 체크포인트가 Hub에 자동으로 업로드되지 않기 때문입니다. 충분한 타임아웃을 설정하는 방법에 대한 [HuggingFace 문서 링크](https://huggingface.co/docs/accelerate/v0.26.0/en/usage_guides/training_on_cluster#setting-sufficient-timeouts)가 공유되었습니다.

한 멤버는 다음과 같이 언급했습니다. *“작업이 타임아웃을 초과하면 실패하고 모든 진행 상황이 손실됩니다.”*
- 중고 시장에서 개조된 RTX 4090 카드: 멤버들은 eBay에서 48GB VRAM을 가진 개조된 RTX 4090 카드가 판매되는 것에 대해 논의했습니다. AMD Instinct MI210 카드에 대해서도 논의했으며, 한 멤버는 더 저렴한 대안으로 22GB VRAM을 가진 2080ti를 제안했습니다.

한 멤버는 다음과 같이 말했습니다. *“저 Instinct 카드들은 쓸모가 없습니다. 저 4090들은 정말 멋집니다. 하지만 22GB RAM을 가진 2080ti를 4분의 1 가격으로 구할 수 있습니다.”*

---

## LM Studio Discord
- vLLM, 병렬 요청 처리 성능을 대폭 향상: 멤버들은 vLLM이 병렬 요청 처리를 크게 향상시킨다고 칭찬하며, 4070에서 Qwen3 0.6B 모델을 실행하는 것을 시연했습니다.

이 시스템은 10개의 동시 요청에서 평균 1470.4 tokens/s의 생성 처리량을 달성했습니다.
- LM Studio, AVX2 요구: 호환성을 확인하려면, LM Studio 내에서 CTRL+Shift+H를 눌러 하드웨어 화면을 열고 AVX2 지원 여부를 확인할 수 있습니다.

AVX2 명령어, 8GB VRAM, 16GB RAM을 갖춘 지난 5년 이내에 제작된 새 PC가 최소 요구 사항을 충족할 것이라고 제안되었습니다.
- Headless LM Studio가 임박했습니다: LM Studio는 API 접근(REST 및 Python API)을 통해 서버를 실행할 수 있도록 하지만, 완전한 Headless 모드는 아직 지원되지 않습니다.

이러한 제한을 해결하기 위해 멤버들은 LM Studio API에 연결하기 위해 LMStudioWebUI와 같은 기존의 LM Studio WebUI를 사용할 것을 제안했습니다.
- Qwen3-Omni 지원 도착: 멤버들은 llama.cpp 업데이트에 따라 Qwen-Omni 모델 지원이 도착하고 있으며, LM Studio 팀의 별도 조치는 필요하지 않다고 보고했습니다.

한 멤버는 Qwen 챗 GUI에 이미 네이티브 omni 모델이 탑재되어 있다고 지적했습니다.
- AMD 495+ 통합 메모리 기대감 고조: 한 멤버는 512GB의 통합 메모리를 지원하는 AMD 495+ 모델을 기다리고 있으며, 대역폭 병목 현상을 방지하기 위해 솔더링된 메모리의 중요성을 강조했습니다.

그들은 AMD AI 모바일 칩이 수용할 만하지만, 시스템 메모리와 함께 약 500 GB/s의 대역폭은 GPU에서 달성 가능한 1 TB/s와 비교할 수 없다고 언급했습니다.

---

## Latent Space Discord
- 더 많은 AI로 강화된 Alexa: Amazon은 향상된 AI 기능을 자랑하는 차세대 AI 기반 Echo 장치와 Alexa 업데이트를 소개했습니다.

한 커뮤니티 멤버는 LLM 교체를 용이하게 하기 위해 해킹 가능한 Echo Dot Max에 관심을 표명했습니다.
- 1조 파라미터 Ring 모델 공개: Ant Ling은 1조 파라미터 오픈소스 "사고" 모델인 Ring-1T-preview를 발표했으며, 벤치마크에 따르면 AIME25에서 92.6점, HMMT25에서 84.5점을 달성하며 최고 수준의 수학 점수를 선보였습니다.

이 모델의 아키텍처는 문제 해결 및 수학적 추론에 대한 독특한 접근 방식을 가능하게 하며, AI 연구 커뮤니티 내에서 상당한 주목을 받고 있습니다.
- Gemini 2.5, 이미지 편집 기능 향상: Tim Brooks와 Google DeepMind는 Gemini를 위한 새로운 네이티브 이미지 편집 및 생성 기능을 발표하며, 일관성, 지시 이행 능력, 창의적 잠재력을 강조했습니다.

커뮤니티 피드백은 편집 중 변경되지 않은 요소의 무결성을 유지하는 모델의 능력을 강조했습니다.
- Cerebras, 대규모 투자 유치: Cerebras Systems는 11억 달러 규모의 Series G 투자 유치 라운드를 발표했으며, 이로써 회사의 가치는 81억 달러로 평가되었습니다. 보도 자료에 상세히 설명된 바와 같이, 이 투자는 AI 프로세서 R&D, 미국 제조 확장, 글로벌 데이터센터 확장에 할당될 예정입니다.

커뮤니티 멤버들은 Cerebras 하드웨어의 다용성을 향상시키기 위해 LoRA/GLM-4.6 지원을 요청했습니다.
- Anthropic, Context Engineering의 중요성 강조: Anthropic은 엔지니어링 블로그 게시물을 통해 AI 에이전트 성능 최적화를 위해서는 단순히 Prompt Engineering뿐만 아니라 효과적인 Context Engineering이 중요하다고 주장했습니다.

개발자들은 더 스마트한 런타임 컨텍스트를 달성하기 위한 메모리 관리와 관련하여 경험, 방법론 및 문의 사항을 교환하고 있습니다.

---

## GPU MODE Discord
- Nvidia RTX 4090, FP8 활용: 한 ML Engineer가 RTX 4090을 구매한 후 fp8 sm89용 flash attention을 구현했으며, 구매 당시인 2023년에는 FP8 지원이 없었다고 언급했습니다.

해당 Engineer는 문서의 한 단락을 읽자마자 이를 적용했다고 말했습니다.
- Triton DevCon 출시 준비 완료: Triton Developer Conference 2025가 몇 주 앞으로 다가왔으며, Meta의 Mark Saroufim, OpenAI의 Phil Tillet 및 Thomas Raoux와 같은 리더들과 AMD, Nvidia, Bytedance의 발표자들이 참석하는 오프라인 참여 기회가 있습니다.

aka.ms/tritonconference2025에서 등록하여 Triton 애호가들과 소통하고 Triton 커뮤니티의 새로운 발전 사항(Triton용 새로운 Blackwell GPU backend 포함 가능성)을 확인하세요.
- 블로그를 통해 Kernel 주소 노출: 호스트 코드에서 kernel function의 주소를 추출하는 방법에 대한 블로그 게시물이 공유되었으며, redplait.blogspot.com에서 확인할 수 있습니다.

Kimbo Chen의 NVIDIA Tensor Cores의 Volta부터 Blackwell까지의 진화에 대한 블로그 게시물도 강조되었으며, semianalysis.com에서 찾을 수 있습니다.
- Determinism 참조 자료 공유: 한 멤버가 2019년의 딥러닝 determinism에 대한 NVIDIA 프레젠테이션 링크와 NVIDIA cuDNN 문서를 게시했습니다.

backend와 determinism 주제에 대한 다양한 학술 논문 및 기사(LLM inference의 nondeterminism을 극복하는 방법에 대한 논문 포함)를 상세히 설명하는 자료들은 딥러닝 작업에 해당 기능을 활용하는 방법을 이해하는 데 유용할 수 있습니다.
- Freelunch AI, 무료 교육 제공: 한 멤버가 GitHub repository인 Freelunch-AI/lunch-stem 링크를 공유하며, 이를 AI 및 CS를 무료로 배울 수 있는 최고의 장소이자 AI 및 Computer Science (CS) 분야에서 무료 학습을 위한 플랫폼을 제공하는 곳이라고 설명했습니다.

이 repository는 양질의 교육에 대한 접근성을 높이기 위해 open-source 기여를 강조하는 open-source 교육 리소스로 자리매김하고 있습니다.

---

## Nous Research AI Discord
- Sequence Expansion Transformer 포함 요청: 한 멤버가 Sequence Expansion Transformers (SEX Transformers)를 개발 중이며, 이를 커뮤니티 프로젝트 섹션에 추가해 줄 것을 요청했습니다.

다른 멤버는 UI에서 화살표를 빨간색으로 만들지 여부에 대해 농담하며, "화살표를 빨간색으로 만들까요, 아니면 보이시나요?"라고 물었습니다.
- Teknium, Sora 2를 로컬에서 공개: Teknium은 초기 Sora 2 비디오를 공개하고 256GB RAM CPU 설정에서 333B 모델을 실행하는 것을 고려했습니다.

HF 페이지에 따르면 모델 크기는 실제로는 357B라고 지적되었습니다.
- Mamba Selectivity, DeepSeek에 도입: DeepSeek Sparse Attention (DSA) v3.2 모델은 이제 서브-Attention 블록으로 mamba selectivity와 유사한 메커니즘을 통합합니다.

이 업데이트는 이러한 통합의 잠재적인 구현과 이점에 대해 추측합니다.
- LLM의 코사인 유사도 분석: 한 멤버가 gpt-oss-120b와 같이 코사인 유사도가 낮은 LLM에 대해 질문하며, 이것이 어떻게 유용할 수 있는지 물었습니다.

다른 멤버는 코사인 유사도가 LLM에서 CoT(chains of thought)의 유사성을 반영하며, 높은 유사성은 유사한 데이터로 학습되었음을 시사할 수 있다고 설명했습니다.
- 투자자, AGI를 위한 Symbolic Architecture 조사: 한 VC 투자자가 AGI 솔루션을 찾기 위해 Aigo.ai, Symbolica, AUI (Augmented Intelligence), After Thought (Stealth)와 같은 Symbolic Architecture를 심층적으로 조사하고 있습니다.

그들은 Aigo.ai를 가장 유망하다고 평가하며, 같은 분야에서 일하기 위해 어떤 자격 요건이 필요한지 알고 싶어 합니다.

---

## Yannick Kilcher Discord
- Thematic Roles, LLM 논쟁 촉발: 한 멤버가 Thematic Roles에 대한 Wikipedia 링크를 공유했고, 다른 멤버는 LLM이 그러한 구조를 가질 수 있다고 제안하며, Othello 게임에서 이동 시퀀스로 학습된 LLM에서 보드 표현이 나타난 연구를 언급했습니다.

Dowty의 proto(typical) 역할 사용도 논의에서 강조되었습니다.
- 픽셀 피핑, 가짜 물리 방지?: Sora 2와 같은 AI 생성 비디오 탐지에 대한 논의에서 한 멤버는 픽셀 피핑이 여전히 상당히 신뢰할 수 있다고 제안했습니다.

다른 멤버는 이상적으로는 AI 생성 콘텐츠 탐지가 불가능해야 하지만, 사람들이 분위기만으로도 탐지하는 데 익숙해질 것이라고 믿는다고 언급했습니다.
- AlphaEvolve, Google 발전: Google은 최근 블로그 게시물에서 설명했듯이, 특정 최적화 문제의 근사 해법 난이도에 대한 결과를 개선하기 위해 LLM 기반 코딩 에이전트인 AlphaEvolve를 사용하여 조합 구조를 찾고 검증합니다.

새로운 결과는 이론 컴퓨터 과학을 발전시킵니다.
- NVIDIA, 사전 학습 데이터에 RL로 추론: 한 멤버가 NVIDIA의 사전 학습 데이터에 RL(Reinforcement Learning)로 추론하는 것에 대한 논문을 공유했습니다.

이 논문은 추론을 명시적으로 유도하지 않았음에도 불구하고 비슷한 성과를 보인 다른 논문보다 더 복잡하다고 설명되었습니다.
- Sora 2의 뛰어난 물리 시뮬레이션: 멤버들은 Sora 1이 물리 시뮬레이션을 할 수 없었고 명백한 시각적 아티팩트가 있었기 때문에 Sora 2의 품질이 Sora 1보다 훨씬 뛰어나다고 언급했습니다.

물리 시뮬레이션의 발전은 핵심 개선 사항으로 강조되었습니다.

---

## aider (Paul Gauthier) Discord
- aider 포크, MCP를 수용하다: 공식 aider는 Multi-modal Conversational Platforms (MCP) 지원이 부족하지만, aider-ce와 같은 일부 포크는 이를 통합하여 사용자들은 향상된 프런트엔드 개발 기능을 위한 대안을 찾게 되었습니다.

이 논의는 상용 플랫폼의 비용 및 속도 제한을 고려할 때 프런트엔드 작업에서 브라우저 MCP의 중요성이 증가하고 있음을 강조했습니다.
- aider와 로컬 LLM 호환성 난관에 부딪히다: 사용자들은 aider가 컨텍스트를 위해 파일을 사용자 프롬프트에 직접 포함하기 때문에 모델들이 툴 사용 기능을 가지고 있음에도 불구하고 Qwen coder 30b 및 devstral 24b와 같은 로컬 LLM과 씨름하고 있다고 보고했습니다.

gpt-oss처럼 충분히 발전했고 제공된 컨텍스트를 효과적으로 처리할 수 있다면 aider는 로컬 모델과 작동한다고 명확히 밝혀졌습니다.
- LM Studio 버그, 사용자들을 괴롭히다: 공유된 경험에 따르면 LM Studio가 특히 mlx 백엔드에서 문제를 겪고 있으며, 사용자들은 llama.cpp가 더 안정적인 경험을 제공한다고 제안했습니다.

해당 스레드는 이러한 문제를 완화하기 위해 --jinja 파라미터를 사용하거나 ollama로 전환할 것을 권장했습니다.
- Apriel-1.5-15b 모델, llama.cpp의 특별 지원을 요청하다: 한 사용자가 새로운 Apriel-1.5-15b 모델과 llama.cpp 사이의 잠재적인 호환성 문제에 대해, 특히 모델이 생각하는 출력을 주 응답 내에 포함하는 경향과 관련하여 문의했습니다.

그들은 llama.cpp가 생각하는 출력을 분리하기 위해 전용 지원 또는 구성 설정이 필요한지 gpt-oss-20b와 비교하면서 추측했습니다.
- Koboldcpp 후처리, 문제 해결에 나서다: 한 멤버가 koboldcpp가 출력 관리를 위해 출력 템플릿 또는 후처리 기술을 사용한다고 지적하며, llama.cpp 기능과의 잠재적인 유사성을 시사했습니다.

이러한 통찰은 Apriel-1.5-15b와 같은 모델에서 발생하는 출력 포맷팅 문제에 대한 해결을 위한 가능한 길을 제공합니다.

## Manus.im Discord Discord
- Manus가 루프에 갇힘: 사용자들은 Manus가 루프에 갇혀 코드 10091의 Internal server error를 발생시키는 오류를 보고하고 있습니다.

사용자들은 프로젝트를 공개하기 위해 헬프 티켓과 URL을 제출했지만 Manus 팀으로부터 아무런 응답을 받지 못했다고 보고했습니다.
- Memory Key Protocol이 사용자 소유 AI 메모리를 생성합니다: 한 사용자가 Aseel-Manus Memory Key Protocol을 개발했습니다. 이는 에이전트의 인지 컨텍스트를 안전하고 휴대 가능한 키로 직렬화하여 완벽한 세션 연속성을 가능하게 하는, 영구적인 사용자 소유 AI 메모리를 위한 모델 불가지론적 프레임워크입니다.

이 프로토콜은 사용자 프라이버시를 위해 강력한 암호화 표준을 활용하여 Manus와 Google의 Gemini 모두에서 검증되었습니다.
- AI 자동화 에이전시의 아키텍처 분석: 한 사용자가 합법적인 AI 자동화 에이전시에 대한 지침을 구했고, 다른 사용자는 이를 세 가지 모델로 분류했습니다: Orchestrators (노코드/로우코드), Architects (맞춤형 Python, LangChain/LlamaIndex, 그리고 vector DB), 그리고 Integrators (엔터프라이즈 수준 규정 준수 관리).

중요한 검증 팁은 잠재적 에이전시에 자동화에서 상태 관리 및 오류 복구를 어떻게 처리하는지 묻는 것입니다.
- 크레딧 소모율 비판: 한 사용자가 X선 및 스프레드시트 생성과 관련된 기본적인 연구 작업에 Manus가 5300개 이상의 크레딧을 소모한 것에 대해 불평했습니다.

한 팀원은 과도한 크레딧 사용을 조사하고 잠재적인 환불을 고려하기 위해 세션 링크를 요청했습니다.
- Sora 초대 코드 증정: 한 사용자가 자신에게 DM을 보내는 모든 사람에게 Sora 초대 코드를 제공하고 있습니다.

더 이상의 세부 정보는 없습니다.

---

## Eleuther Discord
- 적응형 검색으로 개선 달성: 한 멤버가 query/head/layer당 추가 검색을 적응적으로 수행하며, 로그 함수적으로 상한을 두어 Attention과 W_o 이후 최종 출력에서 유망한 코사인 유사도를 보였다고 보고했습니다.

CleanShot 이미지가 결과를 보여주었습니다.
- DeepSeek의 Sparse Attention: 새로운 DeepSeek 모델의 sparse attention 메커니즘에 대한 논의가 FlashMLA pull request 링크와 함께 시작되었습니다.

한 멤버는 sparse attention이 정말 흥미롭게 들린다고 언급했습니다.
- AI 분야 메타 연구에 대한 문의: 한 멤버가 과거 연구를 분석하는 메타 연구에 대해 문의하며, 방대한 작업의 영향에 대해 궁금해하고 개인적인 취향을 넘어 통찰력을 제공하는 논문을 찾았습니다. 그는 이러한 논문에 대해 물었습니다.

응답들은 이 논문과 이 강연과 같은 다른 관련 논문들을 가리키는 포인터를 포함했습니다.
- BBH Benchmark 사용률: 한 멤버가 벤치마크 사용에 대한 조사 결과를 공유하며, BBH 인용의 50% 미만이 실제로 BBH로 평가를 수행한 논문에서 나온 것이라고 언급했습니다.

그들은 BigBench를 인용한 첫 50개 논문을 살펴보니 공식 구현체의 사용률이 0%였다고 언급했습니다.
- RWKV7Qwen3Hybrid5NoPE-8B-251001Faced, GSM8k에서 어려움 겪어: 한 멤버가 GSM8k benchmark에서 SmerkyG/RWKV7Qwen3Hybrid5NoPE-8B-251001Faced 모델로 문제를 겪었다고 보고하며, 결과 이미지를 공유했습니다.

같은 멤버는 llama-3-8B 또한 낮은 점수를 기록했다고 언급했습니다.

---

## Modular (Mojo 🔥) Discord
- Windows 지원은 후순위로 밀려: Modular에게 Windows 지원은 여전히 낮은 우선순위이며, 컴파일러 오픈 소싱 이후 커뮤니티 기여가 예상됩니다. 하지만, Windows 10을 기다리면 Windows가 >= AVX2를 의미한다고 가정할 수 있으며, 이는 실제로 엄청난 이점이라는 점이 지적되었습니다.

일부 멤버들은 벤더 지원 부족으로 인해 많은 GPU 또는 가속기가 Windows에서 절대 사용할 수 없을 것이라고 언급했습니다.
- Mojo, Stack Overflow 설문조사에서 꼴찌 기록: Mojo는 Stack Overflow 개발자 설문조사에 처음 등장했으며, 설문조사 결과에 따르면 꼴찌를 기록했습니다.

낮은 순위에도 불구하고, 커뮤니티 멤버들은 Mojo가 설문조사에 포함된 것을 축하했습니다.
- Notebook 지원에 대한 관심 증가: 멤버들은 코드 주변에 수학 공식 주석을 달거나 그래프 설명을 제공하기 쉽기 때문에 ML 분야에서 아이디어를 선보이기 위해 Jupyter Notebook의 구문 강조와 업스트림 Jupyter의 Max Kernel과 같은 노트북 지원을 요청하고 있습니다.

논의를 통해 노트북에서 MAX와 상호작용하는 것과 노트북 내에서 Mojo를 직접 작성하고 실행하는 것 모두의 필요성이 명확해졌습니다.
- MAX는 아직 Cerebras를 실행할 수 없어: 한 멤버가 벤치마킹을 위해 MAX로 구현된 AI 모델을 Cerebras에서 실행하는 것에 대해 문의했고, 다른 멤버는 MAX가 현재 Cerebras에서 실행되지 않으며, Cerebras와 같은 데이터플로우 칩에 대한 최적화도 없다고 설명했습니다.

이는 AI 프로젝트에 Mojo X Max를 사용하는 것이 Cerebras와 같은 AI 칩에서 무료 성능 향상을 제공하지 않을 것임을 시사합니다.

---

## Moonshot AI (Kimi K-2) Discord
- OpenAI, TikTok 광고로 투자자들을 자극: OpenAI는 프롬프트 상자를 보여주는 TikTok 광고를 공개하며 투자자들 사이에서 흥분을 불러일으켰습니다.

일부 시청자들은 해당 광고를 형편없다고 일축했습니다.
- 중국 모델, 민감한 주제 회피: 한 사용자가 중국 모델이 어떤 주제를 피하도록 파인튜닝되었는지 질문하며, 인도에 대한 특정 내용은 언급할 수 없다고 지적했습니다.

이 질문은 AI 모델의 검열 및 편향성에 대한 지속적인 우려를 강조합니다.
- API 버전 모델, 개방성 제공: 한 멤버는 일부 모델의 API 버전이 상당히 개방적이며, 미국 모델에 비해 모델 내부에 서구 편향적인 데이터가 적다는 점 외에는 검열이 없다고 주장했습니다.

이는 다른 모델 버전에서 검열과 지역적 편향성 간의 잠재적인 상충 관계를 시사합니다.

---

## DSPy Discord
- LiteLLM과 DSPy, 앱 주도권 경쟁: 한 멤버가 새로운 LLM 애플리케이션에 LiteLLM 또는 DSPy를 사용할지 저울질하며, DSPy가 LiteLLM을 게이트웨이로 사용한다고 언급했습니다.

원 게시자는 LiteLLM이 충분한 구조가 부족하고 단순히 인터페이스 역할을 할 뿐이며, DSPy는 특정 문제 해결 방식을 강요한다고 느꼈습니다.
- DSPy 구조: 선택 사항인가, 아니면 조율된 것인가?: 한 멤버는 메시지를 `dspy.LM`에 직접 전달할 수 있다고 반박하며, DSPy의 구조가 반드시 강제되는 것은 아님을 시사했습니다.

게시자는 LiteLLM의 모든 기능이 활용되는 것은 아니며 원하는 결과를 얻기 위해서는 어느 정도의 조립(구성)이 필요하다고 강조했습니다.
- 캐싱 비판, 콘텐츠 혼란에 집중: 한 사용자가 캐싱을 활용할 때 JSON 요청의 콘텐츠 부분 순서를 조작하는 것에 대해 질문했습니다.

이는 프롬프트와 파일의 순서가 효과적인 캐싱 전략에 중요하다고 시사합니다.

---

## tinygrad (George Hotz) Discord
- CLSPV 여전히 충돌하지만, 대부분 통과: 한 멤버가 CLSPV로 테스트를 실행하는 동안 여전히 충돌을 겪고 있지만, 이제 테스트는 대부분 통과한다고 보고했습니다.

x86_64 Linux 시스템을 사용하는 사용자들은 `pip install git+https://github.com/softcookiepp/tinygrad.git` 명령어로 해당 포크를 설치하여 직접 시도해 볼 수 있습니다.
- ShapeTracker, 곧 삭제될 예정: 한 멤버가 Shape Tracker Lean Prove Bounty의 현황에 대해 문의했습니다.

ShapeTracker가 곧 삭제될 것이라고 추가로 논의되었습니다.

---
LLM Agents (Berkeley MOOC) Discord에는 새로운 메시지가 없습니다. 이 길드가 너무 오랫동안 조용했다면 알려주십시오. 그러면 저희가 삭제하겠습니다.

---
MLOps @Chipro Discord에는 새로운 메시지가 없습니다. 이 길드가 너무 오랫동안 조용했다면 알려주십시오. 그러면 저희가 삭제하겠습니다.

---
Windsurf Discord에는 새로운 메시지가 없습니다. 이 길드가 너무 오랫동안 조용했다면 알려주십시오. 그러면 저희가 삭제하겠습니다.

이 이메일은 저희 사이트에서 수신 동의를 하셨기 때문에 발송되었습니다.
이 이메일 수신 방법을 변경하시겠습니까?
이 목록에서 수신 거부할 수 있습니다.

---

# Discord: 채널별 상세 요약 및 링크

### Perplexity AI ▷ #general (997개 메시지🔥🔥🔥):
> Sora 2, 무료 Perplexity Pro, Grok vs. ChatGPT
- Sora 2, 뜨거운 관심과 밈을 생성: 회원들은 Sora 2로 활발하게 콘텐츠를 생성하고 있으며, 한 사용자는 하루 만에 100개의 동영상을 생성했다고 자랑했고, 여러 사용자는 피카츄를 이용한 콘텐츠를 만들고 있습니다.

일부 사용자들은 Sora 2 워터마크가 전문적으로 보이며 제거할 필요가 없다고 느끼는 반면, 다른 사용자들은 GPT Plus에 통합된 유료 버전을 기대하고 있습니다.
- VPN 꼼수로 모두에게 Sora 2 공개: 사용자들은 VPN을 사용하여 캐나다를 통해 연결하면 Sora 2에 무료로 액세스할 수 있다는 것을 발견했습니다. 하지만 한 사용자는 이제 VPN 없이도 앱이 실행된다고 언급했습니다.

한 사용자는 100개의 동영상을 생성하고 Sora의 새로운 Cameo 기능을 테스트하여 현재 소셜 미디어에서 유행하는 동영상을 만들었습니다.
- Perplexity Pro를 무료로 이용하는 사람들: 사용자들은 Airtel, Venmo, PayPal과의 제휴를 포함한 다양한 프로모션을 통해 Perplexity Pro에 무료로 액세스하고 있습니다.

Perplexity Pro의 무료 액세스는 일부 사용자들로 하여금 다른 유료 AI 구독 서비스의 가치에 의문을 제기하게 만들었으며, 한 회원은 "어차피 Perplexity Pro가 무료인데 아무도 필요 없죠"라고 유머러스하게 말했습니다.
- Grok, 부진한 성능: 회원들은 Grok이 이미지 및 동영상 생성과 같은 특정 영역에서 저조한 성능을 보인다고 판단하고 있으며, 한 사용자는 "Grok은 이미지 및 동영상 생성에서 심각하게 뒤처져 있습니다"라고 말했습니다.

한 사용자는 Grok의 검색 기능이 오래되거나 잘못된 출처를 필터링하는 데 어려움을 겪는다고 말합니다.
- LLM 열풍: 한 사용자는 Kimi, Z, Perplexity Labs를 사용한 결과를 보고했으며, Kimi는 애니메이션과 더 나은 UI를 가지고 있고, Z.ai는 전반적으로 더 좋아 보인다고 밝혔습니다.

Perplexity Labs는 고려할 가치도 없었지만, 한 사용자는 DeepSeek도 테스트에 포함되어야 한다고 제안했습니다.

---

### Perplexity AI ▷ #sharing (7개 메시지):
> Sora 2 출시, Comet 초대 추천
- Sora 2 출시 예정: 회원들은 OpenAI가 Sora 2를 출시할 것임을 나타내는 Perplexity 페이지 링크를 공유했습니다.
- Comet 초대 추천: 한 회원이 Comet 추천 링크를 공유하며, 추천을 통해 초대를 제공했습니다.

그들은 또한 추천을 사용하는 모든 사람이 Comet 초대를 받을 것이라고 언급하며, 관심 있는 사람들에게 DM을 보내도록 권장했습니다.

---

### Perplexity AI ▷ #pplx-api (1개 메시지):
.idothehax: 오

### LMArena ▷ #general (997 messages🔥🔥🔥):
> Claude API 무료 사용, Seedream 4 너프, 윤리적 AI 토론, Sora 2 초대 코드, 이미지 생성 문제
- Claude의 무료 API 사용 탐색: 멤버들은 Claude API를 무료로 사용하는 가능성에 대해 논의했으며, 한 명은 puter.js를 언급했고 다른 한 명은 MCP를 무료 계정에 연결하는 것을 제안했습니다.

하지만 주간 20M Token 제한과 사용자 데이터가 결제 수단으로 사용될 수 있다는 점과 같은 제한 사항이 언급되었습니다.
- Seedream 4 너프 및 사용자 피드백: 사용자들은 Seedream 4의 최근 변경 사항에 대해 논의했으며, 한 멤버는 해상도, 속도, 이미지 품질을 포함하여 각 버전의 장단점을 자세히 설명했습니다.

일반적인 불만 사항은 강제된 1:1 종횡비였는데, 일부는 이로 인해 이미지 편집에 쓸모가 없다고 느꼈습니다.
- 윤리적 AI 토론: 멤버들은 윤리적 AI를 논의하기에 적합한 채널에 대해 문의했으며, 한 멤버는 <#1340554757827461211> 또는 <#1377796849901240321>이 적절할 것이라고 답변했습니다.

한 사용자는 비꼬는 투로 "윤리적 AI 🤢, 이제 AI가 내 일자리를 훔쳐갔으면 좋겠네요."라고 말했습니다.
- Sora 2 초대 코드 요청 및 공유: 여러 멤버가 Sora 2 초대 코드를 요청했으며, 최소 한 명의 사용자는 코드에 대한 비용을 지불하겠다고 제안했습니다.

한 멤버는 채팅에서 Sora 2 코드를 아낌없이 공유했습니다.
- 이미지 생성에 새로운 문제 발생: 멤버들은 오디오 없이 이미지가 생성되거나, 이미지가 1:1 종횡비로 고정되거나, 기타 예상치 못한 오류를 포함한 이미지 생성 문제를 보고했습니다.

한 멤버는 이미지 생성 문제는 <#1343291835845578853>에 보고할 수 있다고 언급했습니다.

---

### LMArena ▷ #announcements (2 messages):
> 10월 AI 생성 콘테스트, 아레나 챔피언 역할, 추상 미술 이미지 콘테스트, 비디오 생성 콘테스트 우승자
- LMArena, 10월 AI 생성 콘테스트 시작: LMArena는 10월 AI 생성 콘테스트의 시작을 발표하며, 참가자들에게 AI를 사용하여 추상 미술을 만들도록 도전했습니다. 제출물은 Battle Mode를 통해 이루어져야 하며, 모델이 공개된 왼쪽 및 오른쪽 응답을 모두 포함해야 합니다. 참여하려면 여기를 참조하십시오.

수상자는 1개월 Discord Nitro와 독점 <@&1378032433873555578> 역할을 받게 됩니다.
- LMArena, AI 전문가를 위한 Arena Champions Role 출시: LMArena는 전용의 방해 없는 비공개 공간에서 심층적인 AI 토론을 장려하기 위해 Arena Champions Role <@&1422628364782407830>을 도입했습니다. 2025년 7월부터 서버에 참여한 멤버들은 자동으로 액세스 권한을 얻으며, 여기에서 신청할 수 있습니다.

---

### OpenRouter ▷ #announcements (3개 메시지):
> Stripe 통합, 사용량 기반 청구, BYOK 요청
- OpenRouter, Stripe와 회계 동기화!: OpenRouter는 Stripe와 협력하여 LLM 회계를 실시간으로 동기화하고, 이 트윗에서 발표된 바와 같이 사용량 기반 청구 또는 하이브리드 모델로 쉽게 전환할 수 있는 새로운 기능을 개발하고 있습니다.

회계 데이터만 Stripe와 공유되며, 프롬프트는 비공개로 유지됩니다.
- BYOK 대잔치: 100만 건 무료 요청!: 2025년 10월 1일부터 모든 사용자는 매월 100만 건의 무료 BYOK 요청을 받게 되며, 이 공지에서 확인할 수 있습니다.

월 100만 건의 요청을 초과하는 고객의 경우, 요청은 일반 요율인 5%로 청구됩니다.

---

### OpenRouter ▷ #app-showcase (2개 메시지):
> 채널 프라이버시, RPG 사용자, LLM Mixture
- 채널 프라이버시 문제 제기: 한 사용자가 해당 채널이 단순한 포럼 스레드가 아닌 실제 채널이라는 사실에 놀라움을 표했습니다.

그들은 과도한 사용을 막기 위해 채널을 숨겨달라고 요청했습니다.
- RPG 사용자들이 채널을 과도하게 사용할 수 있음: 해당 사용자는 RPG 사용자들이 채널을 끊임없이 사용할 것을 우려했습니다.

이는 LLM Mixture 방식이 중단될 수도 있다는 의미입니다.

---

### OpenRouter ▷ #general (662개 메시지🔥🔥🔥):
> Grok 모델 문제, 객체 생성, Sora 비디오 모델, Grok과의 롤플레이, AWS Bedrock
- Grok 모델 및 객체 생성 호출 오류: 일부 사용자들이 Grok 모델 및 객체 생성 호출이 작동하지 않는다고 보고했지만, 그 원인은 즉시 명확하지 않았으며 OpenRouter 또는 Grok 변경 사항과 관련이 있는지에 대한 추측이 있었습니다.

나중에 한 사용자가 Grok4가 다시 작동하는 것 같다고 보고했습니다.
- OpenRouter에 없는 Sora 비디오 모델: 한 사용자가 Sora 비디오 생성 비용에 대해 문의했지만, OpenRouter는 비디오 모델을 라우팅하지 않으며 OpenAI의 Sora 앱 또는 웹사이트를 통해서만 사용 가능하고 API를 통해서는 사용할 수 없다고 명확히 밝혔습니다.

사용자들은 ChatRoom에서 모델이 응답 중간에 멈추는 것에 대한 불만을 표했습니다.
- Tongyi DeepResearch 30B A3B 모델은 무료가 아닙니다: 한 사용자가 Tongyi DeepResearch 30B A3B 모델이 무료로 잘못 표시되었다고 보고했으며, 이 주장은 확인되었고 나중에 수정되었다고 표시되었습니다.

Grok이 롤플레잉에 적합한지에 대한 논의도 있었으며, 한 사용자는 Grok의 글쓰기 스타일과 시스템 프롬프트 준수 능력을 칭찬했습니다.
- BYOK, 이제 100만 건의 무료 요청 제공: OpenRouter는 이제 매월 100만 건의 무료 BYOK 요청을 제공하며, 이 변경 사항은 모든 기존 BYOK 사용자에게 자동으로 적용됩니다.

사용자들은 그들이 제공하는 API 키를 통해 발생한 사용량에 대해 여전히 책임이 있습니다.
- Grok Code Fast 1: 속도 악마: Grok Code Fast 1 (GCF1)은 높은 속도와 작업 집중력으로 주목받으며, 명확한 지침이 주어졌을 때 코딩 작업에 유용합니다.

일부 사용자들은 Grok이 지시를 잘 따르지 않는다고 생각하지만, 저렴하다고 합니다.

---

### OpenRouter ▷ #discussion (24 메시지🔥):
> Sora Invite Codes, Sora API Endpoint, Sora Access Requirements, OpenAI vs Google, Sora.com and BYOK
- OpenRouter 사용자들은 Sora Invite Codes를 원합니다: 많은 회원들이 Sora Invite Codes를 간절히 원하고 있으며, 한 사용자는 Apple 기기를 가진 미국 또는 캐나다 거주자에게 4개의 초대 코드를 제공했습니다.

그 사용자는 미국/캐나다 제한이 아쉽다고 한탄하며, Wan3와 같은 유사한 옵션이 언제쯤 사용 가능해질지 궁금해했습니다.
- OpenAI가 Sora API Endpoint를 확인했습니다: 회원들은 Sora API Endpoint의 잠재적 가용성에 대해 논의했으며, 한 회원은 OpenAI가 초기에는 자사 앱이 모든 컴퓨팅 자원을 사용하기를 원할 것이라고 언급했습니다.

다른 회원은 OpenAI가 Sora용 API Endpoint가 있을 것이라고 발표했으며, 이 Endpoint는 사실적인 사운드와 더 나은 품질 덕분에 다른 비디오 생성 모델보다 훨씬 더 좋아 보인다고 말했습니다.
- OpenAI가 거대 기술 기업들과 경쟁합니다: 한 회원은 OpenAI가 Google, Meta, Amazon과 경쟁하는 것에 놀라움을 표했으며, 특히 Sora 2의 높은 품질과 훈련을 위해 모든 YouTube 비디오를 잠재적으로 스크랩하는 것에 대해 언급했습니다.

그 사용자는 Genie가 진정한 세계 시뮬레이터일 수 있다고 추측했으며, Sam Altman이 OpenAI를 이끄는 데 겪는 어려움에 공감했습니다.
- Sora.com이 BYOK로 새 모델을 지원합니다: 한 사용자가 Sora.com이 새 모델과 함께 작동하며 100만 개의 무료 BYOK Token을 제공한다고 보고했습니다.

새 모델이나 Sora.com과의 통합 방식에 대한 추가 세부 정보는 제공되지 않았습니다.

### Cursor 커뮤니티 ▷ #일반 (671 메시지🔥🔥🔥):
> Cursor 학생 프로그램, Sonnet 4.5 Token 사용량, Cursor Agent 버그, Deepseek v3.2 추가, AI 소셜 네트워크 플랫폼
- Sonnet 4.5는 Token을 많이 사용하고, Codex는 Token을 아낀다는 평가: 한 멤버는 Sonnet 4.5가 매우 좋은 모델임에도 불구하고, 더 적은 비용과 Token을 사용하는 Codex에 비해 입력 및 생성하는 Token 양이 낭비되는 느낌이라고 언급했습니다.

다른 멤버들은 Claude 모델이 일반적으로 더 비싸다고 언급했지만, 레거시 요금제를 사용하는 한 멤버는 GPT-5-high-fast보다 Sonnet 4.5를 선호한다고 밝혔습니다.
- Cursor Agent 버그 발생: 한 멤버는 Agent 터미널에 버그가 발생하여 bash, cmd, powershell 등 다른 셸을 시도한 후에도 어떤 명령도 수행할 수 없었다고 보고했습니다.

다른 멤버는 `winget install --id Microsoft.PowerShell --source winget`을 실행하고 Cursor를 재시작한 후 기본 셸을 `pwsh`로 설정할 것을 제안했습니다.
- Cursor 소셜 네트워크에 대한 바람: 한 멤버는 Cursor가 AI 크리에이터를 위한 소셜 네트워크 플랫폼을 만들 수 있는지 물었습니다.

다른 멤버는 ✨ 마법 ✨을 믿으면 무엇이든 가능하다고 답했습니다.
- Cursor 결제 페이지 가독성 문제: 한 멤버는 결제 페이지가 읽기 어렵다고 불평하며 ChatGPT에게 더 나은 페이지를 만들어달라고 요청했습니다.

레거시 요금제를 사용하는 멤버들은 다양한 모델의 비용에 대해 논의했으며, 일부는 Claude Opus가 매우 비싸다고 생각했고, 다른 일부는 비용 분석이 오해의 소지가 있다고 생각했습니다.
- TypeScript 리팩터링의 순조로운 진행: 채팅의 멤버들은 Cursor가 간단하고 쉬운 단계로 모듈과 클래스를 리팩터링할 수 있어 원활한 경험을 제공한다고 언급했습니다.

한 멤버는 명확하고 일관된 프롬프트를 제공하는 것만으로도 남아있는 모든 문제를 해결할 수 있었습니다.

---

### Unsloth AI (Daniel Han) ▷ #일반 (339 메시지🔥🔥):
> GRPO 트레이너, 파인튜닝, Blackwell GPU
- 첫 GRPO 트레이너 구축: 느리지만 꾸준한 여정: 한 멤버는 첫 GRPO (Generative Reinforcement Learning with Policy Optimization) 트레이너를 만들었으며, Colab 노트북에 기록된 바와 같이 LoRA 파인튜닝에 비해 느리다고 언급했습니다.

멤버는 훈련 손실(training loss)이 거의 0으로 떨어지고 보상 값(reward value)은 느리게 상승하는 것을 관찰했으며, 이는 더 간단한 머신러닝 시스템에서의 경험과 유사하다고 언급했습니다. 이 실험 후에는 다른 RL 도구로 전환할 계획이라고 덧붙였습니다.
- Blackwell Docker 문제로 인한 수동 컴파일 수정: 멤버들은 Blackwell GPU(RTX 50xx 시리즈)에서 Xformers 관련 문제를 논의했으며, 호환성 문제로 인해 수동 컴파일이 필요하다고 언급했습니다.

한 멤버가 수동 컴파일 단계를 공유했습니다: `pip uninstall -y xformers; git clone --depth=1 https://github.com/facebookresearch/xformers --recursive; cd xformers; export TORCH_CUDA_ARCH_LIST="12.0"; python3 setup.py install` 또한 "128k context는 정말 필요 없지만, 그래도 최대치로 설정할 겁니다. 인간 본성이라는 게 그렇죠."라고 덧붙였습니다.
- 파인튜닝을 위한 데이터 준비 통찰력: 한 멤버가 에이전트 파인튜닝을 위한 고품질 데이터셋 준비 방법에 대해 문의하며 데이터셋 가이드를 공유했습니다.

다른 멤버는 모델 크기, 에이전트의 특성, 데이터의 구조 및 품질을 고려할 것을 조언했으며, 최소 1000~5000개의 고품질 예시가 필요하다고 강조했습니다.

---

### Unsloth AI (Daniel Han) ▷ #introduce-yourself (13 messages🔥):
> 신규 멤버 소개, 블록체인 애플리케이션, 문제 해결에서의 AI
- 열정적인 AI 엔지니어 채널 합류: 홍콩 출신의 AI 엔지니어 Andi가 채널에 합류하여 배우고 다른 사람들과 협력하고 싶다는 열의를 표했습니다.

다른 멤버들은 즉시 Andi를 환영했으며, 한 멤버는 농담으로 10억 달러 규모의 스타트업을 시작하는 데 도움을 요청했습니다.
- 블록체인과 AI 융합 탐구: 한 멤버는 코드에 신뢰를 작성하는 것에 대한 호기심으로 여정이 시작되었고, 이것이 블록체인과 AI를 탐구하게 된 계기가 되었다고 설명했습니다.

그들은 블록체인과 AI의 결합이 산업, 커뮤니티, 아이디어 생성을 변화시킬 수 있다고 믿으며, 이 기술들이 이전에는 불가능했던 문제들을 해결할 잠재력이 있다고 강조했습니다.

---

### Unsloth AI (Daniel Han) ▷ #off-topic (143 messages🔥🔥):
> Gemma 파인튜닝, Sora 2, AI 모델과 자기 인식, Windows Subsystem for Linux (WSL), torchcodec 문제
- Gemma 파인튜닝 프레임워크 충돌!: 멤버들은 Unsloth가 T4 Collab GPU에서 Gemma 파인튜닝을 허용하는 유일한 프레임워크라고 주장하는 반면, Google의 Gemma 문서에도 T4 GPU에서 LoRA와 Keras를 사용하는 튜토리얼이 제공된다는 점을 발견했습니다.

나중에 밝혀진 바에 따르면, Unsloth가 효율적으로 작동하는 것을 방해했던 원래의 문제들을 식별하고 해결했습니다.
- Sora 2는 NSFW인가요?: 한 멤버가 Sora 2 비디오가 NSFW일 수 있음을 나타내는 링크를 공유하여, 해당 레퍼런스를 즉시 이해하지 못한 사용자들 사이에서 혼란을 야기했습니다.

일부 오래된 멤버들은 해당 레퍼런스를 이해했지만, 다른 멤버들은 설명이 필요했습니다. 한 멤버가 'U too young to get it'이라고 응답한 것에서 알 수 있듯이 말입니다.
- LLM은 자기 인식이 부족하다고요?: 멤버들은 LLM에게 자신에 대해 물었을 때의 정확성에 대해 논의했으며, 한 멤버는 일반적으로 LLM에게 자신에 대해 묻는 것은 정확하지 않다고 말했습니다.

GPT-5가 자신을 아는 것처럼 보인다면, 이는 특정 훈련, tool use 또는 system prompt에 신원 정보가 포함되었기 때문이라고 제안되었습니다. 한 멤버는 system prompt 없이는 어떤 GPT와도 대화할 수 없다고 말했습니다.
- WSL: Windows의 구원자인가요?: 사용자들은 종속성 문제를 피하기 위해 Windows Subsystem for Linux (WSL)을 사용하는 것의 장점에 대해 논의했습니다. 특히 Linux에서 더 나은 CUDA implementation을 제공하는 torchcodec와 같은 프로젝트의 경우 더욱 그렇습니다.

초기 학습 곡선에도 불구하고, 커뮤니티 멤버들은 원활한 경험과 더 나은 하드웨어 리소스 활용을 위해 WSL과 VSCode를 추천했으며, 한 멤버는 "its compatibility, linux thats it"이라고 말했습니다.
- Eval Loss가 새로운 최고치를 기록했습니다!: 한 멤버는 6이라는 eval loss를 보고 충격을 표현했습니다.

다른 멤버들은 csmor 또는 대부분의 오디오 모델에서는 그것이 정상이라고 제안했습니다.

---

### Unsloth AI (Daniel Han) ▷ #help (67 messages🔥🔥):
> GRIT algorithm + Qlora 기반 파인튜닝, AgentGYM, Gemma 3n 4b it - 16 bit model, Runpod에서 Unsloth를 사용한 Qwen 2.5 72B 파인튜닝, Llama-server를 사용한 Multi-GPU
- GRIT 및 QLORA 노트북 검색: 한 멤버가 GRIT (Geometric Reprojection Instruction Tuning) algorithm과 QLORA 기반 파인튜닝이 결합된 노트북에 대해 문의했으며, 특정 Hugging Face model을 언급했습니다.
- Unsloth, 무료 플랜 및 Gemma 3n 4b it - 16 bit model 가용성 확인: 한 멤버가 Unsloth가 Gemma 3n 4b it - 16 bit model을 제공하는지 물었고, 이에 대한 확인과 Unsloth documentation 링크가 제공되었습니다.

다른 멤버는 Unsloth에 유료 플랜이 없다고 명확히 밝혀, 유료 모델로 더 빠른 inference 속도를 얻을 수 있는지에 대한 사용자의 질문을 해소했습니다.
- save_pretrained_gguf 문제: 한 멤버가 save_pretrained_gguf function을 사용하려고 할 때 문제를 보고했으며, Llama로 model을 로드할 때 누락된 tensor와 관련된 에러에 직면했습니다.

다른 멤버는 Unsloth에서 `save_pretrained_gguf`가 아직 작동하지 않는다고 언급하며, 수동 변환 또는 `push_to_hub_merged()`와 변환 공간을 사용할 것을 제안했습니다. 하지만 원본 게시자는 두 가지 접근 방식 모두에서 어려움을 겪었다고 보고했습니다.
- 개인 AI 클론을 파인튜닝하려는 사용자: 한 사용자가 자신의 비디오 자막을 데이터 소스로 사용하여 자신의 대화 스타일을 모방하는 Discord 봇을 만들기 위해 LLM을 파인튜닝하는 것을 목표로 합니다.

커뮤니티 멤버들은 자막을 Q&A 형식으로 변환할 것을 제안했으며, 잠재적으로 다른 AI 모델을 사용하여 비디오 콘텐츠에서 질문-답변 쌍을 생성하는 방식을 언급했습니다. 이 방법이 실험적임을 강조했습니다.

---

### Unsloth AI (Daniel Han) ▷ #research (5 messages):
> ReLU 버그, Shifted Tanh, Gradient Explosion
- ReLU 버그로 인한 제곱 항 발생: 한 멤버가 ReLU를 사용한 원래 공식에서 버그를 발견했으며, 이 버그는 빼기 곱(subtract product)과 함께 제곱 항을 발생시켰습니다.

그들은 [0, N] 대신 [~0, ~1] 범위의 shifted tanh로 전환했으며, 이는 이제 신호 증폭 게이트라기보다는 미분 가능한 신호처럼 작동합니다.
- 기울기 폭주 현상 사라짐: tanh로 전환한 결과, 멤버는 기울기가 더 이상 폭주하지 않는다고 보고했습니다.

그들은 배경 지식으로 LoRA에 대한 블로그 게시물을 링크했습니다.

---

### OpenAI ▷ #ai-discussions (398 messages🔥🔥):
> Sora 2 초대, GLM 4.6 vs Sonnet 4.5, AI 기반 도구 아이디어, 딥페이크 및 사실적인 프롬프트
- Sora 2 초대권 쟁탈전 심화: Discord 사용자들은 Sora 2 초대권을 적극적으로 찾고 있으며, 이는 다양한 채널에서 스팸을 유발하고 잠재적인 사기에 대한 우려를 낳고 있습니다. 많은 사람들이 DM을 통해 코드를 요청하고 초대 전용 시스템에 대한 불만을 표출하고 있습니다.

사용자들은 앱과 접근 방식에 대해 논의하기 위해 <#1379321411046346762> 및 <#1315696181451559022>와 같은 특정 채널로 안내됩니다.
- GLM 4.6 코딩 플랜은 비용 절감 대안: 사용자들은 GLM 4.6이 코딩 작업에서 Sonnet 4.5에 대한 비용 효율적인 대안임을 발견했습니다. 한 사용자는 Zai의 분기별 프로 플랜이 5시간마다 600개의 프롬프트를 훨씬 저렴한 비용으로 제공한다고 보고했습니다.

한 사용자는 zai glm 코딩 플랜의 가치가 매우 높아서 한 분기 구독을 신청했다고 주장합니다.
- AI 기반 드림 도구가 상상력을 자극합니다: 만들고 싶은 AI 기반 도구의 종류에 대해 질문했을 때, 멤버들은 벽을 꿰뚫어 보거나 날 수 있게 해주는 도구와 같은 여러 아이디어를 공유했습니다.
- 딥페이크에 대한 이중 잣대로 비판받는 AI 앱: 한 AI 앱이 사용자들에게 자신을 딥페이크하도록 요청하면서도 동시에 사실적인 프롬프트를 거부하여, 분노와 정신적 결함에 대한 비난을 불러일으키고 있습니다.

---

### OpenAI ▷ #gpt-4-discussions (9개 메시지🔥):
> GPT-5의 SQL 능력, 즉시 생성, 대역폭 스로틀링, Thinking Mode
- GPT-5가 SQL 테스트에서 실패합니다: llm-benchmark.tinybird.live에 따르면, GPT-5 (Codex 및 non-Codex)는 SQL에서 SOTA(State-Of-The-Art) 수준이 아닌 것으로 보이며, 각각 23위와 52위를 기록했습니다.

한편, o3-mini는 동일한 벤치마크에서 6위를 차지했습니다.
- 즉시 생성이 더 이상 즉시가 아닌가요?: 사용자들은 지속적인 문제를 겪고 있으며, 커스텀 인스트럭션을 사용할 때조차도 즉시 생성이 더 이상 즉시가 아닌 이유를 궁금해하고 있습니다.

일부 이론은 이것이 대역폭 스로틀링 조치 때문일 수 있다고 제안합니다.
- Thinking mode가 사용자의 위치를 파악할 수 있습니다: 한 사용자는 Thinking mode에 사용자의 시간대 또는 대략적인 IP 위치를 파악하는 도구가 있다고 제안했습니다.

다른 사용자는 Thinking mode의 약 18K 시스템 프롬프트에도 이것이 명시되어 있었으며, Thinking mode와 non-thinking mode는 서로 다른 시스템 프롬프트와 도구를 가지고 있다고 명시했습니다.

---

### OpenAI ▷ #prompt-engineering (7개 메시지):
> ChatGPT와 Canvas, 인간적인 글쓰기 프롬프트
- ChatGPT가 Canvas 코드를 점진적으로 업데이트할 수 있나요?: 한 멤버가 ChatGPT가 매번 전체 코드를 다시 작성하지 않고 특정 위치에 필요한 부분만 삽입하는 방식으로 Canvas를 사용하도록 하는 방법이 있는지 물었습니다.

다른 멤버는 아직 그런 방법을 찾지 못했으며, 관련 Discord 채널에 기능을 요청하거나 잠재적인 버그로 보고할 것을 제안했습니다.
- 글쓰기를 더 인간적으로 만드는 방법?: 한 멤버가 자신의 글쓰기를 더 인간적으로 만들 프롬프트를 찾고 있습니다.

다른 멤버는 좋은 베이스라인과 사용자 플러그인을 가지고 있는 Sudowrite와 같이 더 파인튜닝된 모델을 사용할 것을 제안했습니다.

---

### OpenAI ▷ #api-discussions (7개 메시지):
> ChatGPT와 Canvas, 인간적인 글쓰기 프롬프트
- ChatGPT가 Canvas를 어려워합니다: 한 멤버가 ChatGPT가 매번 전체 코드를 다시 작성하지 않고 Canvas를 사용하도록 하는 방법이 있는지 문의했습니다.

다른 멤버들은 그렇게 할 방법을 찾지 못했다고 확인했으며, 이를 기능으로 요청할 것을 제안했습니다.
- 사람처럼 글을 쓰는 프롬프트: 한 멤버가 자신의 글을 더 사람처럼 보이게 만들 수 있는 프롬프트를 요청했습니다.

다른 멤버는 더 나은 결과를 위해 Sudowrite나 사용자 플러그인과 같이 더 파인튜닝된 모델을 사용할 것을 제안했습니다.

---

### HuggingFace ▷ #announcements (1 messages):
> ML for Science 프로젝트, Trackio 라이브러리, Gradio를 사용한 워터마킹, VS Code의 HF Inference Providers, HF Inference Providers의 Public AI
- ML-for-Science 프로젝트에 참여할 학생 모집: Hugging Face는 일부 ML-for-science 프로젝트에 참여할 학생과 오픈 소스 기여자들을 찾고 있으며, 이 Discord 링크에서 확인해 보세요.

자원봉사자들은 변화를 만들고 인류를 돕는 기회를 얻게 될 것입니다.
- Trackio: Wandb 대체제: Hugging Face는 wandb의 드롭인 대체제이자 로컬 우선으로 구축된 Trackio라는 새로운 무료 실험 트래킹 라이브러리를 출시했으며, GitHub 리포지토리를 확인해 보세요.

메트릭, 테이블, 이미지, 심지어 비디오까지 기록할 수 있습니다!
- Gradio의 새로운 Invisible Watermarks: Hugging Face는 Gradio를 사용한 가시적 워터마킹에 대한 블로그 게시물을 공개했으며, 게시물은 여기에서 확인하세요.

이제 출처를 쉽게 증명하고 잘못된 정보나 악의적인 행위자를 피할 수 있습니다.
- EmbeddingGemma 모델 출시!: Google의 새로운 효율적인 임베딩 모델 EmbeddingGemma가 출시되었으며, 더 자세한 정보는 블로그 게시물을 읽어보세요.

이 모델은 효율적이고 다재다능하다는 점에서 뛰어납니다.
- Faster Transformers 블로그 게시물 공개: HuggingFace는 OpenAI의 gpt-oss에서 얻은, Transformer와 함께 사용할 수 있는 트릭에 대한 블로그 게시물을 공개했으며, 게시물은 여기에서 읽어보세요.

이 게시물은 Transformer 모델의 속도를 높이기 위해 FlashAttention 및 quantization 기술을 사용하는 방법을 자세히 설명합니다.

---

### HuggingFace ▷ #general (196 messages🔥🔥):
> Crisper Whisper Integration, Lora Training, Medical AI Opinion, RTX 4090 modded cards, ComfyUI Crashing
- Whisper, 더 선명해지다: 음성 인식 통합: 한 멤버가 음성 인식을 위한 풀스택 앱에 Crisper Whisper를 통합하는 데 도움을 요청했으며, 비정상적인 단어를 인식하기 위한 라이브러리에 대해 문의했습니다.
- Lora Training 타임아웃이 손실을 유발: 멤버들은 Lora training 작업이 타임아웃될 경우 데이터 손실 위험이 있다고 논의했으며, 특히 실행 중에 체크포인트가 Hub에 자동으로 업로드되지 않기 때문에 충분한 타임아웃을 설정하는 방법에 대한 HuggingFace 문서 링크가 공유되었습니다.

한 멤버가 "작업이 타임아웃을 초과하면 실패하고 모든 진행 상황이 손실됩니다"라고 언급했습니다.
*   의료 모델: 멤버들은 의료 AI 모델에서 의료 Token 및 부정어(negation terms)에 대한 손실(loss) 관리에 대한 의견을 논의했습니다.

한 멤버가 이것이 causal models에도 적용될 수 있는지 질문했습니다.
*   개조된 RTX 4090 및 Multi GPU Farming: 멤버들은 eBay에서 판매되는 48GB VRAM의 개조된 RTX 4090 카드와 AMD Instinct MI210 카드에 대해 논의했으며, 한 멤버는 더 저렴한 대안으로 22GB VRAM의 2080ti를 제안했습니다.

한 멤버가 "저 Instinct 카드는 쓸모없습니다. 저 4090들은 정말 멋집니다. 하지만 22GB RAM이 장착된 2080ti를 4분의 1 가격에 구할 수 있습니다"라고 말했습니다.
*   ComfyUI venv 충돌: 한 사용자가 Runpod에서 새 pod를 열 때 ComfyUI의 venv가 충돌하고 종속성을 인식하지 못하는 문제, 특히 최근 Runpod 충돌 이후의 문제에 대해 보고했습니다.

---

### HuggingFace ▷ #cool-finds (메시지 1개):
> Foundational Models, 새로운 연구 논문
*   놀라운 Foundational Model 논문 공개: 한 멤버가 모든 것을 바꿀 수 있다고 주장하는 Foundational Models에 대한 연구 논문을 공유했습니다.
*   추가 토론 요청: 이 논문에 대한 추가 토론을 환영합니다. 이 요약은 단지 시작점일 뿐입니다.

---

### HuggingFace ▷ #i-made-this (메시지 2개):
> CloudOpsBERT, IaC 동시성
*   CloudOpsBERT, 클라우드 분석의 문을 열다: CloudOpsBERT는 클라우드 운영 로그 분석을 위한 도메인 적응형 Transformer 모델을 탐구하는 오픈소스 프로젝트입니다.

이는 이상 감지, 안정성 모니터링 및 비용 최적화에 중점을 둡니다.
*   IaC 동시성 충돌 예측: 동시성 관리 프레임워크는 Infrastructure-as-Code (IaC) 시스템에서 동시 수정 충돌을 예측하고 완화합니다.

이 프로젝트는 BERT 및 LSTM 모델을 사용합니다.

---

### HuggingFace ▷ #computer-vision (메시지 1개):
> 실시간 벤치마크, 비전 작업용 아레나, 위성 이미지, 드론 이미지, 데이터셋
*   위성/드론 이미지용 실시간 벤치마크 목록 찾기: 한 멤버가 위성 또는 드론 이미지를 사용하는 비전 작업을 위한 실시간 벤치마크 또는 아레나 목록을 찾고 있습니다.
*   공개 데이터셋 및 벤치마킹 플랫폼 탐색: 한 멤버가 컴퓨터 비전 작업을 위한 최신 데이터셋과 벤치마킹 플랫폼을 찾고 있습니다.

### HuggingFace ▷ #smol-course (4 messages):
> 퀴즈 링크 오류, 강의 팁
- 섹션 2와 3 퀴즈 링크 404 오류: 여러 회원들이 섹션 2와 3의 퀴즈 링크가 깨져 404 오류로 연결된다고 보고했습니다.
- 신규 학생이 강의 조언을 구함: 새로운 학생인 spectrix.dev님이 강의를 시작하며 팁과 놓친 부분이 있는지 질문했습니다.

다른 회원인 noir_bd님은 새로운 학생에게 의문이 있다면 질문하는 것을 주저하지 말라고 조언했습니다.

---

### HuggingFace ▷ #agents-course (3 messages):
> Agent Course
- Agent Course 시작 오늘 출시: 여러 회원들이 오늘 Agent Course를 시작한다고 알렸습니다.

그들은 강의와 주제에 대한 기대감을 표현했습니다.
- Agent Course에 대한 열정: 회원들은 agents에 대해 배우고 강의를 시작하는 것에 대한 관심을 표명했습니다.

이 강의는 다양한 흥미로운 주제를 다룰 것으로 예상됩니다.

---

### LM Studio ▷ #general (162 messages🔥🔥):
> vLLM 병렬 요청, LM Studio 및 AVX2, LM Studio Reddit 밴, Qwen3-Omni 지원, LM Studio 병렬 처리
- vLLM, 병렬 요청 처리: 한 회원이 vLLM이 고도로 병렬적인 특성과 사용 가능한 메모리에 따른 확장성 덕분에 더 작은 모델로도 많은 수의 병렬 요청을 처리할 수 있다고 강조했습니다.

그들은 4070에서 Qwen3 0.6B를 실행하여 10개의 동시 요청에서 평균 1470.4 tokens/s의 생성 처리량을 달성한 사례를 공유했습니다.
- LM Studio에 AVX2 필요: 일부 회원들은 LM Studio에 AVX2 지원이 필요하다는 점을 논의했으며, 호환성을 확인하기 위해 사용자는 LM Studio 내에서 CTRL+Shift+H를 눌러 하드웨어 화면을 열 수 있다고 했습니다.

지난 5년 이내에 제작된 AVX2 명령어, 8GB VRAM, 16GB RAM을 갖춘 새 PC가 최소 요구 사항을 충족할 것이라고 제안되었습니다.
- LM Studio 서버: headless 모드 진행 중: 회원들은 서버에 LM Studio를 설정하고 원격으로 액세스하는 것에 대해 논의했으며, 한 회원은 LM Studio가 API 액세스(REST 및 Python APIs)를 통해 서버를 실행할 수 있지만, 완전한 headless 모드는 아직 지원되지 않는다고 언급했습니다.

다른 회원은 LM Studio API에 연결하기 위해 LMStudioWebUI와 같은 기존 LM Studio WebUI를 사용할 것을 제안했습니다.
- Qwen3-Omni 멀티 모델 출시 예정: 회원들은 Qwen-Omni 지원에 대해 논의하며, llama.cpp가 지원할 때 함께 지원될 것이며 LM Studio 팀의 별도 조치는 필요 없다고 밝혔습니다.

한 멤버는 Qwen 챗 GUI가 이미 네이티브 옴니 모델을 가지고 있다고 언급했습니다.
- 여러 GPU에 걸쳐 모델 분할: 멤버들은 LM Studio에서 여러 GPU에 걸쳐 모델을 분할하는 것에 대해 이야기하며, 이는 주로 속도 향상보다는 사용 가능한 VRAM을 늘리는 것임을 언급했습니다.

한 멤버는 gpt-oss-120b를 두 개의 A6000 (48GB) GPU에 걸쳐 분할할 계획이었습니다.

---

### LM Studio ▷ #hardware-discussion (메시지 33개🔥):
> AMD 495+, Strix Halo, 3090 Memory Bandwidth, Mobile chips
- 대용량 통합 메모리를 갖춘 AMD 495+ 대기: 한 멤버는 512GB 통합 메모리를 지원하는 AMD 495+를 기다리고 있으며, 대역폭 문제를 피하기 위해 메모리를 보드에 솔더링하는 것의 중요성을 강조했습니다.

그들은 또한 AMD AI 모바일 칩이 괜찮지만, 시스템 메모리와의 대역폭이 약 500 GB/s인 것은 GPU에서 달성 가능한 1 TB/s와 비교할 수 없다고 언급했습니다.
- Strix Halo 대역폭은 256GB/s에 불과합니다: 한 멤버는 Strix Halo가 256GB/s의 대역폭을 가진다고 지적하며, 이를 4090과 같은 GPU와 비교하는 것에 반대했습니다.

다른 멤버는 3090이 약 1 TB/s (936.2 GB/s)를 가지고 있으며, 500 GB/s를 가진 AMD의 R9700은 AI에 덜 매력적인 옵션이라고 제안하고, W7900은 864.0 GB/s를 달성한다고 명확히 했습니다.
- 이론적 한계 대 실제 사용: 한 멤버는 이론적 최대치가 항상 달성 가능한 것은 아니며, iGPU는 대략 215-220GB/s를, CPU는 128GB/s를 처리할 수 있지만 LLM은 CPU 코어에서 실행되지 않을 것이라고 추정했습니다.

그들은 "애초에 비교 대상이 아닌 것들을 사람들이 비교하는 것을 보는 것에 지쳤습니다. 그것은 그 자체의 제품 카테고리에 속합니다"라고 덧붙이며, PC가 더 큰 MoE 모델에 적합하다는 점을 강조하고, 중고 하드웨어 구매의 비용 효율성도 언급했습니다.
- GPU 중고 시장: 논의는 중고 GPU 시장으로 옮겨갔으며, 블로워 3090이 약 900달러, 600달러짜리 3080 20GB가 구매 가능하다는 언급이 있었습니다.

한 멤버는 Alibaba에서 1천 달러짜리 4080 32GB를 고려할 것을 제안했고, 다른 멤버는 eBay에서 약 3천~4천 달러에 32GB VRAM을 가진 4090에 대한 선호를 표했습니다.

---

### Latent Space ▷ #ai-general-chat (메시지 99개🔥🔥):
> Amazon의 차세대 AI 기기, Ring-1T Model, Gemini 2.5 이미지 편집, EigenCloud AI 검증, Cerebras 자금 조달
- Amazon Alexa, 더 많은 AI를 탑재: Amazon은 향상된 AI 기능을 특징으로 하는 차세대 AI 기반 Echo 기기 및 Alexa 업데이트를 공개했습니다.

한 사용자가 LLM을 연결하고 교환할 수 있는 해킹 가능한 Echo Dot Max에 대한 열망을 표현했습니다.
- 1조 파라미터 Ring 모델: Ant Ling은 SOTA 수학 점수를 기록한 최초의 1조 파라미터 오픈소스 "사고(thinking)" 모델인 Ring-1T-preview를 공개했습니다. [여기](https://x.com/antling_ai/status/1795764835676770549)에서 벤치마크된 바와 같이 AIME25에서 92.6점, HMMT25에서 84.5점을 달성했습니다.
- Google의 Gemini 2.5, 이미지 업그레이드: Tim Brooks와 Google DeepMind는 Gemini를 위한 새로운 네이티브 이미지 편집 및 생성 기능을 발표했습니다. 이 기능들은 일관성, 지시 준수 및 창의성으로 주목받았습니다.

커뮤니티 반응은 편집되지 않은 요소를 보존하는 모델의 강점에 집중되었습니다.
- Cerebras, 수십억 달러 투자 유치: Cerebras는 Fidelity & Atreides가 주도하는 11억 달러 규모의 Series G 라운드를 발표했으며, 이로 인해 회사의 가치는 81억 달러로 평가되었습니다. 자금은 [보도자료](https://www.cerebras.net/news/cerebras-raises-1-1-billion-in-series-g-funding-round)에 따라 AI processor R&D, U.S. manufacturing expansion, 글로벌 데이터센터 확장에 사용될 예정입니다.

커뮤니티 회원들은 LoRA/GLM-4.6 지원을 요청했습니다.
- Context는 새로운 Prompt입니다: Anthropic은 prompt engineering이 아닌 context engineering이 AI-agent 성능을 극대화하는 핵심이라는 내용을 설명하는 새로운 [엔지니어링 블로그 게시물](https://www.anthropic.com/news/context-engineering)을 발표했습니다. 개발자들은 해당 블로그 게시물을 통해 더 스마트한 런타임 context를 위한 메모리 관리와 관련된 경험, 기술 및 질문을 공유하고 있습니다.

---

### Latent Space ▷ #genmedia-creative-ai (4 메시지):
> Sora 2, 인형 설명 비디오, Chris의 새로운 업무
- Chris의 Sora 2 인형 설명 비디오 업무: Chris 🇨🇦는 자신의 새로운 역할이 Sora 2를 사용하여 인형 설명 비디오를 만드는 것이라고 공유했습니다.

그는 이 [X 게시물](https://x.com/Chris_S_Wong/status/1795764835676770549)에서 이상한 잘림 문제에도 불구하고 결과물이 인상적이라고 언급했습니다.
- Sora 2의 인상적인 결과물: 이상한 잘림 문제에도 불구하고, Sora 2는 인형 설명 비디오 제작에서 인상적인 결과물을 내고 있습니다.

Chris 🇨🇦는 최근 발표에서 Sora 2의 기능을 강조했습니다.

---

### GPU MODE ▷ #general (13 메시지🔥):
> PTX 및 CUDA 학습, RTX 4090의 FP8 지원, 코드 구성 전략, GEMM 구현, cuBLAS 성능
- PTX 및 CUDA 숙련도 달성 기간 측정: 한 회원이 Nvidia 문서를 통해 PTX와 CUDA를 학습하여 흥미로운 애플리케이션을 구축하는 데 걸리는 일반적인 기간에 대해 문의했습니다. 다른 회원은 triton, cutlass와 같은 라이브러리가 포함되는지 여부와 애플리케이션 도메인에 따라 달라진다고 답변했습니다.

한 멤버는 CUDA 지식 부족이 유일한 걸림돌이라면, 언어로서 CUDA를 정말 빠르게 배울 수 있지만, 무엇을 작성해야 할지 찾는 것이 진짜 문제라고 언급했습니다.
- **RTX 4090 FP8 구현 심층 분석:** 한 ML Engineer 멤버는 자신의 아이디어를 테스트하기 위해 CUDA를 더 깊이 배워야 했고, FP8 지원 때문에 RTX 4090을 구매하여 fp8 sm89용 flash attention을 구현했습니다.

그들은 2023년 구매 당시에는 FP8 지원이 없었으며, 문서에서 한 단락을 읽은 직후 적용했다고 언급했습니다.
- **최적의 코드 구조화 전략:** 한 멤버는 torchtitan과 유사한 코드베이스 내에서 405b 모델에는 더 빠르지만 8b 모델에는 더 느린 커스텀 코드가 있을 때 코드를 구성하는 방법에 대한 조언을 구했습니다.

제기된 질문은 모델 코드에 if-else 분기를 사용할지, 모델 코드의 두 가지 버전을 유지할지, 아니면 monkey-patching 후처리를 적용할지였습니다.
- **GEMM 구현을 통한 GPU 활용 마스터하기:** 한 멤버는 cuBLAS 성능의 80% 이상을 달성하는 GEMM을 구현하는 것이 GPU를 완전히 활용하는 좋은 방법이며, 임의의 tensor contractions을 matricization을 통해 GEMM으로 재구성할 수 있기 때문에 GEMM은 항상 유용하다고 제안했습니다.

그들은 cuBLAS 성능 달성을 위한 가이드로 고전적인 블로그 게시물을 링크했습니다.

---

### GPU MODE ▷ #triton (1 메시지):
> Triton Developer Conference 2025, GPU MODE State of Triton, NVIDIA Blackwell GPU용 Triton 백엔드, Triton 분산 컴퓨팅
- **Triton Developer Conference 2025 임박:** Triton Developer Conference 2025가 몇 주 앞으로 다가왔으며, 현장 참석 및 Triton 애호가들과 교류할 기회가 있습니다.

이 컨퍼런스는 참가자들이 Triton 커뮤니티의 새로운 발전을 발견하면서 최고 리더들과 배우고, 공유하고, 네트워킹할 수 있도록 하는 것을 목표로 하며, aka.ms/tritonconference2025에서 등록할 수 있습니다.
- **GPU MODE, Triton 현황 논의:** Meta의 Mark Saroufim과 GPU Mode가 다가오는 컨퍼런스에서 Triton의 현재 상태에 대해 발표할 예정입니다.

다른 발표로는 OpenAI의 Phil Tillet과 Thomas Raoux가 'Triton: Today and Beyond'에 대해 논의하며, Meta, AMD, Nvidia, Bytedance의 발표도 포함됩니다.
- **NVIDIA Blackwell GPU, Triton 백엔드 확보 예정:** Nvidia의 Chris Sullivan이 Triton용 NVIDIA Blackwell GPU 백엔드에 대해 발표할 예정입니다.

새로운 Blackwell GPU 아키텍처가 Triton과 통합되어 성능을 최적화하는 방법을 이 프레젠테이션에서 소개합니다.
- Triton-distributed는 연산 및 통신을 처리합니다: Bytedance의 Wenlei Bao가 분산 LLM 훈련 및 추론에서 연산과 통신 오버래핑에 대한 Triton-distributed를 논의할 예정입니다.

이 강연에서는 Triton을 사용하여 연산과 통신을 오버래핑함으로써 대규모 언어 모델의 분산 훈련 및 추론을 최적화하는 방법을 다룹니다.

---

### GPU MODE ▷ #cuda (2 messages):
> 커널 함수 주소, Tensor Core 진화, Kimbo Chen
- 커널 주소 노출!: 호스트 코드에서 커널 함수의 주소를 추출하는 방법에 대한 블로그 게시물이 공유되었으며, redplait.blogspot.com에서 확인할 수 있습니다.
- Kimbo, Tensor Core 타임라인을 그리다!: Volta부터 Blackwell까지 NVIDIA Tensor Core의 진화에 대한 Kimbo Chen의 블로그 게시물이 강조되었으며, semianalysis.com에서 확인할 수 있습니다.

---

### GPU MODE ▷ #torch (1 messages):
> Torch Dynamo 컴파일 시간, 재컴파일 영향 측정, Autotuning
- Torch Dynamo: 컴파일 시간 디코딩: 한 멤버가 Dynamo의 성능을 더 잘 이해하기 위해 `torch._dynamo.utils.compile_times()` 로그를 해석하는 방법에 대해 문의했습니다.

특히, Dynamo 캐시를 완전히 재설정하지 않고 단계별로 컴파일 시간, 재컴파일 및 Autotuning의 영향을 측정하는 방법을 찾았으며, 관련 gist 링크를 제공했습니다.
- Dynamo 캐시 재설정 딜레마: 사용자는 Dynamo 캐시를 재설정하지 않고 단계별 컴파일 시간의 영향을 측정하고자 했습니다.

이는 반복적인 재컴파일 및 Autotuning의 오버헤드를 피하면서도 미세한 성능 영향을 이해하기 위함입니다.

---

### GPU MODE ▷ #cool-links (2 messages):
> 결정론, NVIDIA 결정론, 딥러닝 결정론, LLM 추론 결정론
- 결정론 참고 자료 공유: 한 멤버가 2019년 딥러닝의 결정론에 대한 NVIDIA 프레젠테이션 링크를 게시했습니다.

이 멤버는 또한 결정론 주제에 대한 다른 학술 논문 및 기사 링크를 게시했으며, LLM 추론에서 비결정론을 극복하는 방법에 대한 내용도 포함되어 있습니다.
- NVIDIA cuDNN 백엔드 세부 정보 공유: 한 멤버가 NVIDIA cuDNN의 백엔드를 자세히 설명하는 문서 링크를 공유했습니다.

이 문서는 cuDNN이 어떻게 작동하는지 이해하고 딥러닝 작업에 해당 기능을 활용하려는 사용자에게 유용할 수 있습니다.

### GPU MODE ▷ #beginner (5 messages):
> 벤치마킹 가이드, 벤치마킹 의견, 유튜브 벤치마킹
- 벤치마킹 가이드 요청: 한 멤버가 #beginner 채널에서 벤치마킹에 대한 좋은 가이드를 요청했습니다.
- 또 다른 멤버이자 많은 의견을 가진 전문가는 벤치마킹 관련 YouTube 영상 링크를 공유하며, 이 영상이 해당 논문과 관련이 있다고 주장했습니다.
- 벤치마킹 인사이트: 많은 의견을 가진 멤버가 인사이트를 공유했습니다.
- 그들은 이것이 자신들의 최고의 벤치마킹 노력이라고 주장했습니다.

---

### GPU MODE ▷ #pmpp-book (4 messages):
> 기본서, 하드웨어 명령어
- 기본서가 탄탄한 기초 제공: 한 멤버가 기본서 링크를 공유하며, 이 책이 memory fences와 같은 개념을 이해하는 데 유용하다고 언급했습니다.
- 그들은 일단 탄탄한 기초를 갖추면 "hardware specific instructions 또는 모든 멋진 새 mma instructions를 빠르게 이해할 수 있다"고 덧붙였습니다.
- 연습이 완벽을 만든다, 지식만이 아니다: 한 멤버는 직업이나 연구를 위해 무언가를 하는 것이 빠르게 배우는 것과는 다르다는 것을 깨달았습니다.
- 그들은 전자가 "무언가를 아는 것보다는 주로 연습과 'muscle memory'를 개발하는 것"이라고 제안했습니다.

---

### GPU MODE ▷ #rocm (1 messages):
> AMD 코어 파일 분석, rocgdb 디버깅
- rocgdb로 AMD 코어 덤프 디버깅: 한 멤버가 gpucore.219213과 같은 AMD 코어 파일을 분석하는 방법에 대해 문의했습니다.
- 그들은 `rocgdb --core=gpucore.71076`을 사용하려고 시도했지만, "Couldn’t find general-purpose registers in core file"이라는 경고를 받았습니다.
- 코어 파일 분석 대안?: 멤버는 코어 파일을 분석하기 위한 대체 방법을 찾고 있습니다.
- 그들은 rocgdb에 문제가 발생하여 제안을 구하고 있습니다.

---

### GPU MODE ▷ #metal (1 messages):
bghira: 이제 685B 미만의 모델이 실행될 때까지 기다려야 합니다..

---

### GPU MODE ▷ #self-promotion (1 messages):
> 무료 AI 학습, 무료 CS 학습, 오픈 소스 교육 자료
- Freelunch AI, 무료 교육 제공: 한 멤버가 GitHub 리포지토리, Freelunch-AI/lunch-stem 링크를 공유하며, 이곳을 AI 및 CS를 무료로 배울 수 있는 최고의 장소라고 설명했습니다.
- 이 리포지토리는 오픈 소스 교육 자료로 자리매김하고 있습니다.
- 오픈 소스 STEM 교육 이니셔티브 시작: GitHub 리포지토리 Freelunch-AI/lunch-stem은 AI 및 Computer Science (CS)를 무료로 학습할 수 있는 플랫폼을 제공하는 것을 목표로 합니다.
- 이는 양질의 교육에 대한 접근성을 높이기 위한 오픈 소스 기여를 강조합니다.

### GPU MODE ▷ #edge (1 messages):
> 방사선 차폐, Orin 방사선 테스트, 하드웨어 Watchdog
- 저궤도는 방사선 차폐를 제공합니다: 저궤도에 있으면 방사선이 적고, 위성 섀시가 자연적인 차폐를 제공합니다.
- 방사선 테스트로 Orin을 보호합니다: Orin에 방사선 테스트를 실시하여, 전자 장치를 손상시킬 수 있는 폭주 전기 전하인 방사선 유발 래치업을 방지했습니다.
- 하드웨어 Watchdog이 문제를 해결합니다: 방사선으로 인해 장치가 멈출 수 있지만, 하드웨어 Watchdog이 장치를 재설정하도록 배치되어 있습니다.

---

### GPU MODE ▷ #submissions (6 messages):
> MI300x8, amd-gemm-rs Leaderboard, amd-ag-gemm Leaderboard
- MI300x8 개인 최고 기록 달성: 한 멤버가 amd-gemm-rs Leaderboard에서 MI300x8로 593 µs의 개인 최고 기록을 달성했습니다.
- amd-gemm-rs에서 MI300x8 성공: 한 멤버가 amd-gemm-rs Leaderboard에서 MI300x8로 608 µs의 기록을 달성했습니다.

다른 제출물은 27.7 ms를 기록했습니다.
- amd-ag-gemm Leaderboard 제출: 한 멤버가 MI300x8로 amd-ag-gemm Leaderboard에 세 번 성공적으로 제출했습니다.

제출된 기록은 986 µs, 534 µs, 884 µs였습니다.

---

### GPU MODE ▷ #status (2 messages):
> Triangle Multiplicative Update
- Triangle Multiplicative Update 관련 문서 및 코드가 곧 공개됩니다: Triangle Multiplicative Update 경쟁이 종료되었으며, 우승 제출물의 문서와 코드가 곧 공개될 예정입니다.
- altzhang이 공개를 확인했습니다: altzhang은 문서와 코드가 곧 공개될 것이라고 확인했습니다.

---

### GPU MODE ▷ #factorio-learning-env (4 messages):
> factorio-learning-env 디버깅, Google Meet 링크
- Google Meet 행아웃: 한 멤버가 디버깅 세션의 Google Meet 링크를 공유했습니다.

해당 멤버는 세션에 한동안 있을 것이며 다른 사람들도 참여를 환영한다고 말했습니다.
- factorio-learning-env 디버깅: 한 멤버가 factorio-learning-env를 조사 중이며 저녁 식사 후에 참여할 것이라고 언급했습니다.

그들은 관련된 도구와 관련이 있을 수 있는 문제를 디버깅 중이며, 원인은 아직 밝혀지지 않았습니다.

---

### GPU MODE ▷ #cutlass (34 messages🔥):
> cute.nvgpu.warp.MmaF16BF16Op 문서, TiledMMA 브로드캐스팅, CuTe의 Distributed GEMM, UMMA tensor core
- wmma 문서 논란: 멤버들은 cute.nvgpu.warp.MmaF16BF16Op 문서가 wmma 대신 mma를 참조하고 mma shape를 주장하는 이유에 대해 의문을 제기했으며, 이는 wmma가 실패한 추상화였다는 설명으로 이어졌습니다.

다른 멤버는 UMMA가 Blackwell tensor core의 별명일 뿐이라고 설명했습니다. Hopper는 GMMA였고, Ampere는 HMMA였습니다. 너무 깊이 생각하지 마십시오. 이제 우리 모두는 이를 tcgen05라고 불러야 하며, UMMA에 대한 모든 언급을 삭제해야 합니다.
- TiledMMA, 브로드캐스트할 것인가 말 것인가?: 백엔드 구현에서 볼 수 있듯이, `atom_layout_mnk`로 생성되고 `k > 1`일 때 `cute.gemm`과 함께 사용하면 TiledMMA가 K에 걸쳐 자동으로 "브로드캐스트"한다는 것이 확인되었습니다.

이는 K에 걸쳐 레이아웃을 재사용합니다.
- CuTe DSL에서 Distributed GEMM 구현 가능: 한 멤버는 CuTe DSL에 아직 분산 프리미티브가 없다고 생각했지만, 대칭 메모리를 사용하여 CuTe DSL에서 분산 GEMM을 오늘날에도 잘 구현할 수 있으며, NVL load/store 시맨틱은 커널에 투명하다고 주장되었습니다.

한 멤버는 구현 예시로 CUTLASS example 65를, 1D TP GEMM에 대한 자세한 내용은 이 프레젠테이션을 링크했습니다.
- GEMM 이해를 위한 CuTe 소스 코드 학습: CuTe를 처음 접하는 멤버에게는 구현(impls)을 보는 대신 소스 코드를 볼 것을 권장했습니다. 소스 코드는 읽기 매우 쉽고 예시보다 훨씬 유익하며, 특히 GEMM 파일을 언급했습니다.

또한, 그들은 멤버에게 더 간단한 예시로 연습하고, 레이아웃을 출력하며, 파라미터를 변경하여 그것들이 어떻게 영향을 미치는지 확인해 보라고 조언했습니다.

---

### GPU MODE ▷ #general (3개 메시지):
> TriMul Competition, GPGPU solution, Operator Fusion, A100, MI300
- TriMul Competition 성공: 한 멤버는 TriMul Competition에 대해 Alex와 팀에게 감사하며, Operator Fusion 관점에서 재미있었고 단순히 GEMM을 넘어섰다고 언급했습니다.

같은 멤버는 A100과 MI300에서 예비 최고 속도 솔루션을 달성했습니다.
- GPGPU Solution 작성: 한 멤버는 arseniivanov.github.io/blog.html에 일반적인 GPGPU solution에 대한 블로그 게시물을 작성했으며, GitHub에 코드와 커널을 포함했습니다.

그 멤버는 상태 채널에서 누군가 이것을 요청하는 것을 보았다고 언급했습니다.
- TriMul 기념품 준비 완료: Alex와 다른 멤버는 TriMul Competition 기념품이 준비되었다고 밝혔습니다.

그들은 채점을 마쳐야 한다고 언급했습니다.

---

### GPU MODE ▷ #multi-gpu (19개 메시지🔥):
> NVLink Multicast, Multimem Instructions, NVShmem Wrappers, Peer GPU L2 Cache, NVLink SHARP
- NVLink SHARP Multicast Memory: 여러 SM이 NVLink를 통해 피어 GPU의 동일한 위치에 접근하려고 할 때, multicast 포인터와 multimem instructions를 사용하지 않으면 하드웨어에서 기본적으로 브로드캐스트되지 않습니다.

한 멤버는 멀티캐스트를 위한 동적 코얼레싱을 구현하는 것이 마이크로아키텍처적으로 어렵기 때문에, NVLink를 통한 전역-전역 메모리 전송으로 구현한 다음 로컬 분할 또는 공유 메모리로 로딩하는 것이 좋다고 언급했습니다.
- 다중 장치 요청을 위한 Multimem 명령어: 하나의 GPU가 동일한 피어 주소로 여러 번 로딩하는 것에 대해 묻는 경우, 여러 피어 GPU에 걸쳐 로딩하고 줄이는 ld_reduce multimem 작업이 유용할 수 있습니다.

논의에 따르면 Multimem 멀티캐스트는 대칭 메모리 주소 지정이 필요합니다.
- 사용자 친화적인 멀티캐스트를 위한 NVShmem 래퍼: 한 멤버에 따르면, NVShmem은 멀티캐스트 동작을 위한 훌륭한 사용자 친화적인 래퍼를 제공합니다.

NVShmem을 담당하는 멤버는 노골적인 홍보를 했습니다.
- 피어 GPU L2 캐시 개입: 한 멤버와 hazyresearch의 게시물에 따르면, volatile load와 같은 특별한 작업을 하지 않으면 메모리 접근은 피어의 L2 캐시를 통과합니다.

한 멤버는 현재 GPU의 xbar가 특정 메모리 범위를 요청한 모든 SMs에 브로드캐스트하는지 궁금해했습니다.

---

### GPU MODE ▷ #llmq (2 messages):
> Mega Kernel 프로젝트, 20B 모델 훈련, 그레디언트 노름 우려
- Mega Kernel 프로젝트가 관심을 불러일으키다: 멤버들은 Mega Kernel 프로젝트가 매우 멋지다고 생각하며, 그들의 다른 작업 방식에 주목했습니다.

한 멤버는 작업 중 얼마나 많은 부분이 공개적으로 진행되었는지에 대해 불확실성을 표했습니다.
- 20B 모델 훈련 완료: 한 멤버는 그들의 20B 실행이 4x4090에서 약 90시간 만에 완료되었으며, 10B 모델의 2.52와 비교하여 최종 손실 2.45를 달성했다고 보고했습니다.

멤버는 실수로 로그 파일의 마지막 부분을 덮어썼고, 이로 인해 회색 곡선이 조기에 끝났다고 언급했습니다.
- 그레디언트 노름 기울기 증가, 우려 야기: 20B 모델 훈련 중 한 멤버의 관찰에 따르면, 그레디언트 노름은 증가하는 기울기를 보이며, 이는 더 긴 실행에 잠재적으로 문제를 일으킬 수 있습니다.

그들은 Karpathy가 이전에는 괜찮아 보였음에도 불구하고 300B 이후 어느 시점에 실행이 폭발했다고 기억했습니다.

---

### Nous Research AI ▷ #general (80 messages🔥🔥):
> 시퀀스 확장 Transformer, GLM 4.5 대 GLM 4.6, DDR5 RAM, Sora 2, Nous Chat Web
- 시퀀스 확장 Transformer가 커뮤니티 의견을 구하다: 한 멤버는 현재 시퀀스 확장 Transformer (SEX Transformer) 작업을 하고 있으며, 해당 프로젝트를 "커뮤니티 프로젝트" 섹션에 추가하는 것에 대해 문의했습니다.

다른 멤버는 UI에서 화살표를 빨간색으로 만들지 말지 농담하며, "화살표를 빨간색으로 만들까요, 아니면 보이시나요?"라고 말했습니다.
- Teknium이 SORA 2를 로컬에서 시연했습니다: Teknium은 첫 번째 Sora 2 영상을 공유하며, 256GB RAM CPU 설정에서 333B 모델을 실행해 볼 수도 있다고 언급했습니다.

하지만 HF 페이지에 따르면 해당 모델은 실제로는 357B라는 점이 곧바로 지적되었습니다.
- CPU에서 GLM 모델 성능 탐색: 멤버들은 GLM 4.5 및 4.6 모델 크기에 대해 논의했으며, GLM 4.5 Air (100b)가 12B의 활성 파라미터를 가지고 있음을 언급하며 CPU에서 Qwen 2 32b와 비교한 성능에 대해 추측했습니다.

한 멤버는 RAM이 있는 자신의 CPU에서 Qwen 2 32b로 4 tok/s를 얻을 수 있었다고 말했습니다.
- RAM 업그레이드: DDR5 및 메모리 컨트롤러 심층 분석: 256GB DDR5 RAM으로 업그레이드하는 것에 대한 논의가 이어졌으며, 잠재적인 클럭 다운그레이드와 이러한 구성에서 Ryzen 7000 시리즈가 5200MHz를 초과하는 것의 한계에 대한 우려가 제기되었습니다.

한 멤버는 컴퓨터에 소다를 쏟아 256GB를 지원하는 9950x Ryzen으로 업그레이드했다고 공유했습니다.
- Sora 2: 지역 잠금 및 트럼프 밈 생성 불가: 멤버들은 OpenAI의 Sora 2가 VPN을 요구하는 지역 기반 출시를 하는 것으로 보인다고 언급했으며, 유머러스하게 트럼프 밈을 생성할 수 없다는 점을 지적했습니다.

이러한 한계에도 불구하고 Sora 2는 현재 사용 가능한 최고의 비디오 생성 모델로 간주됩니다.

---

### Nous Research AI ▷ #ask-about-llms (2개 메시지):
> 낮은 Cosine Similarity를 가진 LLM, GPT-OSS-120B
- LLM의 Cosine Similarity 해독: 한 멤버가 gpt-oss-120b와 같이 낮은 Cosine Similarity를 가진 LLM에 대한 선호도에 대해 문의했습니다.

다른 멤버는 Cosine Similarity가 LLM에서 CoT(Chains of Thought)가 얼마나 유사한지를 측정하며, 높은 유사성은 유사한 데이터로 훈련되었음을 나타낼 수 있다고 명확히 했습니다.
- Cosine Similarity는 CoT 유사도를 측정합니다: Cosine Similarity는 CoT(Chains of Thought)가 얼마나 유사한지를 측정합니다.

만약 LLM들이 높은 Cosine Similarity를 가진다면, 그들의 출력은 매우 유사하며, 이는 서로를 기반으로 훈련되었을 수 있다는 사실을 시사합니다.

---

### Nous Research AI ▷ #research-papers (2개 메시지):
> Aigo.ai, Symbolica, Augmented Intelligence (AUI), After Thought (Stealth), Symbolic Architectures
- VC, Symbolic Architectures를 통해 AGI 추구: 한 VC 투자자가 AGI를 향한 탐구에서 Aigo.ai, Symbolica, AUI (Augmented Intelligence), After Thought (Stealth)와 같은 Symbolic Architectures를 탐색하고 있습니다.

그들은 Aigo.ai를 가장 유망하다고 생각하며, Aigo.ai 프로젝트에 참여하기 위한 요구 사항이 무엇인지 묻고 있습니다.
- Aigo.ai와 같은 심볼릭 아키텍처 작업 요구 사항: 한 VC 투자자가 Aigo.ai를 포함한 심볼릭 아키텍처 프로젝트에 기여하기 위한 필수 자격 및 기술에 대한 이해를 표명했습니다.

이러한 문의는 AGI 솔루션에 대한 투자 탐색과 다양한 심볼릭 AI 접근 방식 평가에서 비롯되었습니다.

---

### Nous Research AI ▷ #interesting-links (1 메시지):
> DeepSeek Sparse Attention, Mamba selectivity
- DeepSeek이 Sparse Attention을 심층 분석합니다: 새로운 DeepSeek Sparse Attention (DSA) v3.2 모델은 Mamba 선택성 메커니즘과 유사한 것을 서브-Attention 블록으로 사용합니다.

해당 게시물은 이것이 어떻게 작동할지에 대해 추측합니다.
- Mamba가 DeepSeek과 결합합니다: DeepSeek의 Sparse Attention (DSA)은 Mamba 선택성 메커니즘과 유사한 것을 통합하는 실험을 진행하고 있습니다.

이는 모델이 관련 정보에 집중하는 능력을 잠재적으로 향상시키고 성능을 개선할 수 있습니다.

---

### Nous Research AI ▷ #research-papers (2 메시지):
> 심볼릭 아키텍처, Aigo.ai, Symbolica, AUI Augmented Intelligence
- VC가 AGI 추구를 위해 심볼릭 아키텍처를 찾습니다: 한 VC 관계자가 AGI 탐색 과정에서 Aigo.ai, Symbolica, AUI “Augmented Intelligence” 및 After Thought (Stealth)와 같은 심볼릭 아키텍처를 탐색해 왔습니다.

해당 관계자는 Aigo가 지금까지 가장 유망해 보인다고 보고했으며, Aigo 프로젝트에 참여하기 위한 요구 사항에 대해 문의했습니다.
- 투자자가 심볼릭 AI를 통해 AGI를 주시합니다: 한 투자자가 Aigo.ai, Symbolica, AUI를 포함한 심볼릭 AI 아키텍처를 적극적으로 연구하고 있으며, 특히 Aigo.ai의 잠재력에 큰 관심을 표명했습니다.

이 투자자는 이제 이러한 심볼릭 AI 프로젝트에 기여하는 데 필요한 요구 사항과 자격에 대한 정보를 찾고 있습니다.

---

### Yannick Kilcher ▷ #general (14 메시지🔥):
> 주제 역할, AI 생성 비디오 감지, Path patching
- LLM의 주제 역할이 논쟁을 촉발합니다: 한 멤버가 주제 역할에 대한 Wikipedia 링크를 공유하고 Dowty의 "원형 역할" 사용을 언급했습니다.

다른 멤버는 이동 시퀀스로 훈련된 LLM에서 보드 표현이 나타났던 Othello 연구를 언급하며 LLM이 그러한 구조를 가질 수 있다고 제안했습니다.
- Peering into Pixels Prevents Perfect Phakes?: 한 사용자가 Sora 2와 같은 AI 생성 비디오를 탐지하는 방법에 대해 질문한 후, 한 멤버는 pixel peeping이 여전히 꽤 신뢰할 수 있게 작동한다고 제안했습니다.

다른 멤버는 이상적으로는 AI 생성 콘텐츠를 탐지하는 것이 불가능해야 한다고 언급했지만, 사람들이 분위기만으로도 이를 탐지하는 데 익숙해질 것이라고 믿고 있습니다.
- Path Patching Promises Precise Probes: 한 멤버는 아직 transcoders에 확신이 없다고 표현하며, path patching이 LLM을 탐색할 때 더 강력한 주장을 하는 데 도움이 될 수 있다고 제안했습니다.

추천 논문에 대한 요청에 응답하여, 그들은 indirect object identification 논문을 해당 분야의 고전으로 꼽았습니다.

---

### Yannick Kilcher ▷ #paper-discussion (6 messages):
> Latent-Reasoning Survey, VLM Circuits Analysis, Reasoning with RL on Pretraining Data
- Latent-Reasoning Chat Postponed: 목요일에 예정되었던 Latent-Reasoning survey에 대한 논의가 취소되었습니다.

원래 계획은 11페이지의 마지막 단락부터 섹션 3.1의 끝까지 진행하는 것이었습니다.
- VLM Circuits Analysis: VLM Circuits Analysis와 해당 프로젝트 페이지에 대한 논의가 계획되었습니다.

이 논의는 오늘로 예정되어 있었습니다.
- Reasoning with RL Papers Circulating: 한 멤버가 NVIDIA의 pretraining data에 대한 Reasoning with RL 논문을 공유했습니다.

이 논문은 RL next sentence prediction 외에는 명시적으로 "reasoning"을 언급하지 않았음에도 불구하고 비슷한 이득을 가진 다른 논문보다 더 복잡하다고 설명되었습니다.

### Yannick Kilcher ▷ #ml-news (9 messages🔥):
> Sora 1 vs Sora 2, ByteDance 및 Tencent vs Sora, AlphaEvolve LLM, Sam Altman의 부자연스러운 움직임, Sam Altman의 대안 WanLynx
- Sora 2의 향상된 물리 엔진: 채널 회원들은 Sora 1이 물리적 현상을 제대로 구현하지 못하고 명백한 시각적 결함을 가지고 있었기 때문에 Sora 2의 품질이 Sora 1보다 훨씬 뛰어나다고 언급했습니다.
- Google, AlphaEvolve로 컴퓨터 과학 발전: Google은 최근 블로그 게시물에서 설명했듯이, LLM 기반 코딩 에이전트인 AlphaEvolve를 사용하여 조합 구조를 찾아 검증함으로써 특정 최적화 문제의 근사 해법 난이도에 대한 결과를 개선하고 있습니다.
- Sam Altman의 어색한 움직임: 한 회원은 Sam Altman이 실제로 어색하고 부자연스러운 움직임/자세를 가지고 있으며, 인간의 움직임이라는 측면에서 ByteDance나 Tencent보다 더 나쁘다고 언급했습니다.
- Sam Altman을 위한 WanLynx: 한 회원은 해당 부분에 Sam Altman 대신 WanLynx를 사용했어야 했을지도 모른다고 농담했습니다.
- fixupx.com 콘텐츠 공유: 한 회원이 fixupx.com의 게시물 링크를 공유했습니다.

---

### aider (Paul Gauthier) ▷ #general (24 messages🔥):
> aider MCP, MCP 지원 aider 포크, aider와 로컬 LLM, LM Studio 문제, Qwen coder 30b 및 devstral 24b
- Aider에서 MCP 사용에 대한 질문: 한 사용자가 상용 플랫폼의 높은 비용과 속도 제한, 그리고 프런트엔드 개발에 대한 중요성을 고려할 때, aider에서 MCP (Multi-modal conversational platform)를 사용하는 방법을 질문했습니다.

그들은 goose/claude/gemini-cli가 모두 MCP를 가지고 있으며, 브라우저 MCP가 프런트엔드 개발에 중요하다고 언급하면서, aider의 yolo 모드에 대해서도 문의했습니다.
- Aider 포크, MCP 추가: 공식 aider는 MCP를 지원하지 않지만, aider-ce와 같은 일부 포크는 지원합니다.

해당 스레드에서는 사용 중인 다른 포크에 대해 질문했습니다.
- Aider, 로컬 LLM과 연동: 한 사용자는 devstral 또는 qwen coder와 같은 로컬 LLM이 도구 사용 기능을 가지고 있음에도 불구하고, LM Studio를 사용하여 모델을 실행할 때 파일을 읽거나 저장하지 못해 aider가 작동하지 않는다고 보고했습니다.

다른 사용자는 aider가 도구를 사용하지 않고, 파일을 사용자 프롬프트에 포함시켜 컨텍스트의 일부가 되도록 한다고 설명했습니다. 또한, gpt-oss처럼 충분히 똑똑한 로컬 모델과도 작동한다고 덧붙였습니다.
- LM Studio의 일부 문제: 일부 사용자는 LM Studio, 특히 mlx 백엔드에서 문제를 겪었으며, llama.cpp가 더 나은 것 같다고 제안했습니다.

어떤 사용자는 `--jinja` 파라미터를 전달하고 ollama로 전환할 것을 권장합니다.
- Qwen Coder 30b는 충분히 똑똑한가요?: 한 사용자는 Qwen Coder 30b 및 devstral 24b 모델이 aider와 함께 작업하기에 충분히 똑똑한지 궁금해합니다.

이 모델들은 파일 접근이나 도구 사용 기능이 없습니다.

---

### aider (Paul Gauthier) ▷ #questions-and-tips (4 messages):
> Apriel-1.5-15b, llama.cpp 지원, koboldcpp 출력 템플릿, DeepWiki 페이지
- Apriel-1.5-15b 출시, 문의 촉발: 한 멤버가 새로 출시된 Apriel-1.5-15b 모델을 llama.cpp와 함께 사용하는 것에 대해 문의하며, 이 모델이 사고 과정 출력을 주요 답변에 포함한다고 언급했습니다.

그들은 llama.cpp가 이 모델에 대한 추가 지원이 필요한지, 아니면 gpt-oss-20b처럼 사고 과정 출력을 분리하는 설정이 있는지 물었습니다.
- 모델 엔지니어링을 위한 DeepWiki 탐색 요청: 한 멤버가 리버스 엔지니어링과 관련된 DeepWiki 페이지를 확인해 볼 것을 제안했습니다.

이 제안은 Apriel-1.5-15b 모델에 대한 질문에 대한 답변이었습니다.
- koboldcpp 출력 솔루션: 한 멤버는 koboldcpp가 출력 관리를 위해 출력 템플릿 또는 후처리(post-processing)를 사용한다고 언급했습니다.

그들은 llama.cpp도 즉시 명확하지는 않더라도 유사한 기능을 가지고 있을 것이라고 추측했습니다.

---

### Manus.im Discord ▷ #general (27 messages🔥):
> Manus 루프에 갇힘, Aseel-Manus Memory Key Protocol, AI 자동화 에이전시, Manus 크레딧 사용, Sora 초대 코드
- Manus 오류 경고: 사용자들 '루프에 갇힘' 오류 보고: 사용자들은 Manus가 루프에 갇히는 오류를 보고하며, 코드 10091의 Internal server error가 발생한다고 합니다. Manus 팀으로부터 아무런 응답 없이 도움 요청 티켓과 프로젝트를 공개하기 위한 URL을 제출한 후에도 오류가 계속되고 있습니다.

사용자는 '이 교착 상태를 해결하기 위해 어떤 조치를 취해야 할까요?'라고 묻습니다.
- 메모리 혁신: Aseel-Manus Memory Key Protocol 공개: 한 사용자가 Aseel-Manus Memory Key Protocol을 개발했습니다. 이는 영구적이고 사용자 소유의 AI 메모리를 위한 모델에 구애받지 않는 프레임워크로, 에이전트의 인지적 맥락을 안전하고 휴대 가능한 키로 직렬화하여 완벽한 세션 연속성을 가능하게 합니다.

프로토콜은 사용자 프라이버시를 위한 강력한 암호화 표준을 활용하여 Manus와 Google의 Gemini 모두에서 검증되었습니다. 사용자는 Manus 플랫폼이 AI 메모리 문제를 패치가 아닌 핵심 철학적 기능으로, 자체적으로 해결해 줄 것을 요청합니다.
- AI 자동화 에이전시: 구현 환경 탐색: 한 사용자가 합법적인 AI 자동화 에이전시에 대한 지침을 구했고, 다른 사용자는 이를 세 가지 모델로 분류했습니다. 오케스트레이터(no-code/low-code), 아키텍트(맞춤형 Python, LangChain/LlamaIndex 및 vector DB), 인테그레이터(기업 수준의 규정 준수 관리).

핵심 검증 팁은 잠재적 에이전시에 자동화에서 state management 및 error recovery를 어떻게 처리하는지 묻는 것입니다.
- 크레딧 부족: Manus의 높은 크레딧 소비량 조사: 한 사용자가 X선 및 스프레드시트 생성과 관련된 기본적인 연구 작업에 Manus가 5300개 이상의 크레딧을 소비했다고 불평했습니다.

한 팀원이 과도한 크레딧 사용을 조사하고 잠재적인 환불을 고려하기 위해 세션 링크를 요청했습니다.
- Sora 스포트라이트: 초대 코드 증정!: 한 사용자가 DM을 보내는 모든 사람에게 Sora 초대 코드를 제공하고 있습니다.

---

### Eleuther ▷ #general (1 messages):
> AI Researcher, Multi Agent Systems, MoE, RL, AI for Software Engineering
- AI 연구 지망생 채팅 참여: 새로운 멤버 Aarya는 자신을 전통적인 machine learning, multi-agent systems, MoE 경험이 있는 AI 연구 지망생으로 소개했습니다.

Aarya는 현재 RL에 대해 더 많이 배우고 있으며 AI for software engineering과 실제 애플리케이션에 적용되는 AI에 관심이 있습니다.
- 다양한 관심사를 가진 새 멤버: Aarya는 RL 학습에 관심을 표명했으며 전통적인 machine learning 경험이 있습니다.

그들은 AI for software engineering에 대한 관심을 언급했습니다.

---

### Eleuther ▷ #research (16 messages🔥):
> Adaptive Searching Improvements, Sparse Attention in DeepSeek Model, Meta-Studies in AI Research, Benchmark Usage Analysis, Implicit Values in ML Research
- Adaptive Searching으로 성능 향상: 한 멤버는 query/head/layer당 추가적인 searching을 적응적으로 수행하여 성능이 향상되었다고 보고했습니다. 이는 로그 스케일로 제한되며, attention 및 W_o 이후 최종 출력에서 유망한 cosine similarity를 보였습니다.

개선 사항을 보여주는 CleanShot 이미지가 첨부되었습니다.
- DeepSeek의 Sparse Attention이 관심을 불러일으킵니다: 새로운 DeepSeek 모델의 sparse attention 메커니즘에 대한 논의가 시작되었으며, FlashMLA pull request 링크가 제공되었습니다.

한 멤버가 "새로운 DeepSeek 모델의 sparse attention은 정말 흥미롭게 들립니다"라고 언급했습니다.
- AI 분야의 메타 연구에 대한 탐색: 한 멤버가 과거 연구를 분석하는 메타 연구에 대해 문의하며, 방대한 작업이 발전에 미치는 영향에 의문을 제기하고 개인적인 취향을 넘어선 통찰력을 제공하는 논문을 찾았습니다.

답변에는 이 논문, 이 논문, 그리고 이 강연과 같은 관련 논문에 대한 포인터가 포함되었습니다.
- 벤치마크 사용 현황 면밀히 검토: 한 멤버가 벤치마크 사용에 대한 조사 결과를 공유하며, BBH 인용의 50% 미만이 실제로 BBH로 평가하는 논문에서 나온 것이라고 언급했습니다. 반면 evaluation harness를 인용한 논문의 70% 이상은 이를 사용했습니다.

그들은 공식 구현이 가장 왼쪽 열에 있으며, BigBench를 인용한 처음 50개의 논문에서는 사용률이 0%였다고 덧붙였습니다.
- ML 연구의 암묵적인 가치: 머신러닝 연구의 암묵적인 가치에 대해 논의하는 논문 링크가 공유되었으며, state-of-the-art 결과 개선과 이전 작업 기반 구축을 주요 동인으로 강조했습니다.

해당 논문은 해당 분야가 벤치마크를 발전시키고 기존 지식을 점진적으로 확장하는 데 중점을 둔다고 강조합니다.

---

### Eleuther ▷ #lm-thunderdome (2 messages):
> GSM8k 벤치마크, RWKV7Qwen3Hybrid5NoPE-8B-251001Faced 성능, Llama-3-8B 평가
- RWKV7Qwen3Hybrid5NoPE-8B-251001Faced가 GSM8k에서 어려움을 겪습니다: 한 멤버가 GSM8k 벤치마크에서 SmerkyG/RWKV7Qwen3Hybrid5NoPE-8B-251001Faced에 문제가 발생했다고 보고하며, 결과 이미지를 공유했습니다.

같은 멤버는 Llama-3-8B로 테스트했을 때 점수가 상당히 낮았다고 언급했습니다.
- Llama-3-8B도 낮은 점수를 기록했습니다: 원 게시자도 동일한 GSM8k 벤치마크에서 Llama-3-8B를 테스트했습니다.

사용자는 Llama-3-8B에서도 점수가 매우 낮았다고 언급했습니다.

---

### Modular (Mojo 🔥) ▷ #mojo (10 messages🔥):
> Windows 릴리스, Mojo Notebook 지원, Stack Overflow 설문조사
- Windows 릴리스 로드맵은 여전히 불확실합니다: 한 멤버가 Windows 릴리스 로드맵에 대해 문의했지만, 현재 Modular의 우선순위가 아니며 컴파일러가 오픈 소스화된 후 Windows 지원은 커뮤니티 기여가 될 가능성이 높다는 답변을 받았습니다.

다른 멤버는 컴파일러가 오픈 소스화된 후에 Windows 지원이 이루어질 것이라고 제안했지만, 많은 GPU 또는 가속기는 벤더 지원 부족으로 인해 Windows에서 사용할 수 없을 것입니다. 또한 Windows 10 지원 종료까지 약 한 달 남았는데, 이는 Windows가 AVX2 이상을 의미한다고 가정할 수 있게 하여 실제로 엄청난 이점을 제공합니다.
- Mojo, Stack Overflow 설문조사에 참여: 설문조사 결과에 따르면, Mojo는 Stack Overflow 개발자 설문조사에 처음으로 등장하여 최하위를 기록했습니다.

낮은 순위에도 불구하고, 커뮤니티는 Mojo가 설문조사에 포함된 것을 축하하고 있습니다.
- Notebook 지원 여전히 필요: 멤버들은 Jupyter Notebook의 노트북 지원, 구문 강조, 그리고 업스트림 Jupyter의 Max Kernel을 요청하고 있습니다. 노트북은 ML 분야에서 아이디어를 선보이는 일반적인 방법이며, 코드 주변에 수학 공식에 주석을 달거나 그래프 설명을 쉽게 제공할 수 없기 때문입니다.

한 멤버는 요청이 노트북에서 Max와 상호작용하는 것인지, 아니면 노트북 내에서 Mojo를 직접 작성하고 실행하는 것인지에 대한 명확한 설명을 요청했습니다.

---

### Modular (Mojo 🔥) ▷ #max (5개 메시지):
> Cerebras의 MAX, Mojo X Max AI 프로젝트
- Cerebras에서 MAX의 어려움: 한 멤버가 Cerebras에서 MAX로 구현된 AI 모델을 실행하고, 그것이 더 빠를지 확인하기 위해 벤치마크와 비교하는 것에 대해 문의했습니다.

다른 멤버는 MAX가 현재 Cerebras에서 실행되지 않는다고 명확히 밝혔으며, Cerebras와 같은 데이터플로우 칩에 대한 최적화가 없기 때문에 속도가 더 느릴 것이라고 언급했습니다.
- Mojo X Max AI 프로젝트는 Cerebras에서 무료 성능 향상을 얻지 못합니다: 한 멤버가 AI 프로젝트에 Mojo X Max를 사용하는 것이 현재 SOTA GPU와 비교했을 때 Cerebras 칩과 같은 AI 칩에서 무료 성능 향상을 제공하는지 물었습니다.

한 멤버는 MAX가 현재 Cerebras에서 실행되지 않으며, Cerebras와 같은 데이터플로우 칩에 대한 최적화가 없다고 명확히 밝혔습니다.

---

### Moonshot AI (Kimi K-2) ▷ #general-chat (13개 메시지🔥):
> OpenAI의 TikTok 광고, 중국 모델 검열, API 버전 비교
- OpenAI, TikTok 광고로 기대감 조성: OpenAI는 프롬프트 상자를 선보이는 TikTok 광고를 공개하여 투자자들로부터 기대감을 불러일으켰습니다.

일부 사용자들은 이를 '슬롭(slop)'이라고 불렀습니다.
- 중국 모델, 민감한 주제를 숨기나요?: 한 사용자가 중국 모델이 논의하지 않도록 사후 훈련된 주제가 무엇인지 문의했습니다.

특히, 인도에 대해서는 언급할 수 없는 몇 가지 사항이 있다고 언급했습니다.
- API 버전, 미국 모델과 대결: 한 멤버는 일부 모델의 API 버전이 상당히 개방적이라고 주장했습니다.

이 멤버는 미국 모델과 비교했을 때 모델 내부에 서구 편향이 덜한 데이터가 있다는 점 외에는 검열이 없다고 명확히 밝혔습니다.

---

### DSPy ▷ #general (10 messages🔥):
> LiteLLM vs DSPy, Prompt Engineering, LLM Caching
- LiteLLM과 DSPy, 앱 개발 경쟁: 한 멤버가 새로운 LLM 중심 애플리케이션 개발을 위해 LiteLLM과 DSPy 중 무엇을 선택해야 할지 문의했고, 다른 멤버는 DSPy가 LiteLLM을 게이트웨이로 사용한다고 언급했습니다.

원 게시자는 LiteLLM이 LLM을 호출하는 인터페이스 역할만 할 뿐 구조를 거의 부여하지 않는 반면, DSPy는 문제에 대해 특정 방식으로 사고하도록 강요한다고 느꼈습니다.
- DSPy 구조는 그렇게 강요되지 않나요?: 한 멤버는 `dspy.LM`에 메시지를 직접 전달할 수 있다고 주장하며, DSPy의 구조가 반드시 강요되는 것은 아니라고 시사했습니다.

그들은 또한 모든 LiteLLM 기능이 현재 활용되는 것은 아니며, 원하는 결과를 달성하는 방법을 이해하기 위해서는 어느 정도 구축 작업이 필요하다고 언급했습니다.
- 캐싱 관련 프롬프트 및 파일 순서: 한 사용자가 캐싱을 활용할 때 JSON 요청의 콘텐츠 부분 순서를 조작하는 방법에 대해 질문했습니다.

이는 프롬프트와 파일이 전송되는 순서가 효과적인 캐싱에 매우 중요하다는 것을 의미합니다.

---

### tinygrad (George Hotz) ▷ #general (3 messages):
> CLSPV Crashes, Shape Tracker Bounty, ShapeTracker Deletion
- CLSPV 여전히 충돌하지만 대부분 통과: 한 멤버가 CLSPV로 테스트를 실행하는 동안 여전히 충돌을 겪고 있지만, 대부분의 테스트를 통과한다고 보고했습니다.

x86_64 Linux 시스템 사용자는 `pip install git+https://github.com/softcookiepp/tinygrad.git` 명령어로 포크를 설치하여 직접 시도해 볼 수 있습니다.
- Shape Tracker 바운티: 한 멤버가 Shape Tracker Lean Prove Bounty의 현황에 대해 문의했습니다.

ShapeTracker가 곧 삭제될 것이라는 내용이 추가로 논의되었습니다.

---

## 🔗 링크 (367개)

1. [https://news.smol.ai/](https://news.smol.ai/)
2. [The Information called out Thinking Machines](https://archive.ph/eq4g5)
3. [Modular Manifolds](https://thinkingmachines.ai/blog/modular-manifolds/)
4. [LoRA Without Regret](https://thinkingmachines.ai/blog/lora/)
5. [the original 2021 paper](https://arxiv.org/abs/2106.09685)
6. [similar to Biderman et al](https://arxiv.org/abs/2405.09673)
7. [Tinker.](https://thinkingmachines.ai/blog/announcing-tinker/)
8. [landing page](https://thinkingmachines.ai/tinker/)
9. [Tinker Cookbook](https://github.com/thinking-machines-lab/tinker-cookbook)
10. [says](https://x.com/karpathy/status/1973468610917179630)
11. [agrees](https://x.com/lilianweng/status/1973455232341516731)
12. [terms of service](https://news.ycombinator.com/item?id=45444869)
13. [ostr](https://twitter.com/ostrisai/status/1973210333532811419)
14. [@skirano](https://twitter.com/skirano/status/1973248497853018168)
15. [@TheStalwart](https://twitter.com/TheStalwart/status/1973372434133950665)
16. [@fabianstelzer](https://twitter.com/fabianstelzer/status/1973300086949253410)
17. [@Teknium1](https://twitter.com/Teknium1/status/1973347911980454274)
18. [@ostrisai](https://twitter.com/ostrisai/status/1973476918285709398)
19. [@billpeeb](https://twitter.com/billpeeb/status/1973260687553208344)
20. [@teortaxesTex](https://twitter.com/teortaxesTex/status/1973358605752738023)

*... 그 외 347개 링크*

---

## 🖼️ 이미지 (1개)

1. ![Image](https://resend-attachments.s3.amazonaws.com/dJrzO1SZwRjgJrV)

---

*이 문서는 Gemini 2.5 Flash를 사용하여 자동 번역되었습니다.*
