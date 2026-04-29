# not much happened today

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today
**번역일**: 2026-04-29 06:18
**발행일**: 2026-04-29

---

# [AINews] 오늘은 별다른 소식이 없었습니다

### 조용한 하루였습니다.
AINews를 Substack으로 이전하면서 매일 Matt Levine 스타일의 사설을 제공하겠다고 약속했지만, 어떤 날은 별다른 소식이 없는 경우도 있습니다. 현재 인퍼런스 수요와 멀티 에이전트에 대한 짧은 에세이를 작업 중이지만, 오늘은 그런 날이 아닙니다.
Nvidia Nemotron, Poolside, Alec Radford에서 흥미로운 모델들이 출시되었지만, 이들 중 어떤 모델이 시간의 시험을 견뎌낼지는 불분명합니다. GPT-6에 대한 기대감이 고조되고 있습니다.
> 2026년 4월 27일~28일 AI 뉴스입니다. 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 발행물을 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
인퍼런스 시스템, vLLM 0.20, 그리고 DeepSeek V4를 둘러싼 하드웨어/커널 경쟁
- vLLM의 최신 릴리스는 메모리 및 MoE 서빙 효율성에 중점을 둡니다. vLLM v0.20.0은 4배의 KV 용량을 위한 TurboQuant 2비트 KV cache, SM90+에서 MLA 프리필을 위해 재활성화된 FA4, 새로운 vLLM IR 기반, 2.1%의 종단간 레이턴시 개선을 보고한 퓨즈드 RMSNorm과 함께 Blackwell의 DeepSeek V4 MegaMoE, Jetson Thor, ROCm, Intel XPU, 그리고 더 쉬운 GB200/Grace-Blackwell 설정을 아우르는 지원 업데이트를 출시했습니다. 이와 동시에 SemiAnalysis는 B200/B300/H200/GB200 분산형 설정에서 DeepSeek V4 Pro의 초기 서빙 결과를 강조하며, 이 워크로드에서 B300이 H200보다 최대 8배 빠를 수 있다고 주장하고 있습니다. 또한 EP dispatch + EP combine + GEMMs + SwiGLU를 단일 메가 커널로 융합하는 DeepGEMM MegaMoE를 사용한 vLLM 0.20 벤치마킹이 곧 있을 것이라고 언급했습니다.
- DeepSeek 지원: 여러 게시물에서 서빙 트레이드오프에 초점을 맞췄습니다. Jeremy Howard는 DeepSeek V4의 프리필 지원이 많은 제공업체에서 중단한 기능이라고 언급했으며, Maharshi는 동적 활성화 양자화의 오버헤드를 지적하며 캘리브레이션 비용에도 불구하고 정적 양자화가 인퍼런스 속도에서 종종 우위를 점한다고 주장했습니다. 대체 스택 이식성에 대한 관심도 커지고 있습니다. teortaxesTex는 DeepSeek이 TileKernels를 통해 CUDA 종속성에서 구조적으로 벗어나고 있다고 주장하며, 모델 벤더들이 NVIDIA 전용 배포보다는 이기종 또는 국내 가속기 플릿에 최적화하는 경향이 커질 수 있다고 시사했습니다.
오픈 모델 출시: Poolside Laguna XS.2, NVIDIA Nemotron 3 Nano Omni, 그리고 TRELLIS.2
- Poolside는 배포 친화적인 오픈 웨이트 코더 모델을 통해 첫 공개 모델을 출시했습니다. @poolsideai는 총 33B / 3B 활성 MoE 코딩 모델인 Laguna XS.2를 발표했으며, 이 모델은 자체적으로 학습되었고 Apache 2.0 라이선스로 출시되었으며 단일 GPU에서 실행 가능하다고 홍보하고 있습니다. Poolside의 더 넓은 범위의 릴리스에는 Laguna M.1과 에이전트 하네스도 포함되었으며, 회사가 자체 데이터, 학습 인프라, RL 및 인퍼런스 스택을 사용하여 처음부터 학습시켰음을 강조했습니다. 커뮤니티 요약은 더 자세한 정보를 제공했습니다. Aymeric Roucher는 하이브리드 어텐션, FP8 KV cache를 갖춘 두 가지 코더 모델(225B/23B 활성 및 33B/3B 활성)을 설명했으며, Qwen-3.5에 근접하는 성능을 주장했습니다. Ollama는 이를 즉시 출시했습니다.
- NVIDIA의 Nemotron 3 Nano Omni는 그날의 가장 큰 인프라 네이티브 모델 출시였습니다. @NVIDIAAI는 텍스트, 이미지, 비디오, 오디오 및 문서를 아우르는 에이전틱 워크로드를 위해 구축된 256K 컨텍스트를 가진 오픈 30B / A3B 멀티모달 MoE인 Nemotron 3 Nano Omni를 소개했습니다. 스택 전반에 걸쳐 즉시 배포되었습니다. OpenRouter, LM Studio, Ollama, Unsloth, fal, Fireworks, DeepInfra, Together, Baseten, Canonical 등 모두 당일 출시를 발표했습니다. 주요 사양은 후속 게시물에서 밝혀졌습니다. Piotr Żelasko는 이를 Parakeet 인코더로 지원되는 음성/오디오 이해 기능을 갖춘 NVIDIA의 첫 번째 옴니 릴리스로 설명했으며, 현재는 영어 전용이고 Open ASR 리더보드에서 5.95%의 WER을 기록했습니다. 여러 호스트들은 유사한 오픈 옴니 모델 대비 약 9배의 처리량을 언급했습니다.
- 다른 주목할 만한 모델/논문 출시: Microsoft의 TRELLIS.2는 최대 1536³ PBR 텍스처 에셋을 생성하는 오픈소스 4B 이미지-투-3D 모델로, 16배 공간 압축을 사용하는 네이티브 3D VAE를 기반으로 구축되었습니다. 월드 모델 측면에서, World-R1은 기존 비디오 모델이 이미 3D 구조를 인코딩하고 있으며 RL을 통해 '깨울' 수 있다고 주장합니다. 이는 아키텍처 변경, 추가 비디오 학습 데이터, 추가 인퍼런스 비용이 필요 없다고 합니다.
에이전트, 로컬 우선 툴링, 그리고 프로덕션 오케스트레이션
- 에이전트 빌더들은 데모에서 프로덕션 프리미티브로 전환하고 있습니다. Mistral은 엔터프라이즈 AI 프로세스를 영속적이고 관측 가능하며 내결함성을 가진 프로덕션 시스템으로 전환하는 것을 목표로 하는 오케스트레이션 레이어인 Workflows를 공개 프리뷰로 출시했습니다. 관련 게시물들도 같은 주제를 반복했습니다. Sydney Runkle은 영속적인 실행을 장기 실행 에이전트의 핵심 요구 사항으로 설명했으며, threepointone은 영속성, 스트리밍 및 재개 기능을 갖춘 서브 에이전트 / 도구형 에이전트에 대한 작업을 설명했습니다.
- 로컬/오프라인 에이전트는 열망에서 신뢰할 수 있는 워크플로우로 발전했습니다. Teknium은 "완전히 오프라인 에이전트가 가능하다"고 주장했으며, Niels Rogge는 데스크톱 정리를 위한 Pi + 로컬 모델을 시연했고, Google Gemma는 로컬 코딩 에이전트를 위한 튜토리얼을 공유했습니다. Hugging Face의 로컬 지원 노력은 채택 수치에서도 나타났습니다. Clement Delangue는 300,000명의 사용자가 로컬에서 실행할 수 있는 것을 찾기 위해 Hub에 하드웨어 사양을 추가했다고 말했습니다. 이를 보완하여 Ammaar는 MLX를 사용하여 Gemma 4를 온디바이스에서 완전히 실행하는 바이브 코딩 앱을 오픈소스화했으며, Kimmonismus는 오픈 모델을 사용하는 비공개 브라우저 기반 로컬 에이전트 개념인 Sigma를 강조했습니다.
- Hermes 및 인접 에이전트 하네스들이 실제 환경에서 관심을 얻고 있습니다. SecretArjun, somewheresy를 포함한 여러 게시물과 Telegram을 통해 Hermes를 배포하거나 의료 문헌 추출에 사용하는 사용자들은 Hermes가 지시 따르기 또는 실용적인 워크플로우에서 OpenClaw를 능가한다고 보고했습니다. 연구 에이전트 측면에서는 Hugging Face의 ML Intern이 Spaces에서 유행했으며, 나중에는 블랙박스가 아닌 관측 가능한 학습 작업을 만들기 위해 네이티브 메트릭 로깅 + Trackio 통합 기능을 얻었습니다.
벤치마크, 평가, 그리고 주목할 만한 연구 결과
- 모델 벤치마킹은 여전히 파편화되어 있지만, 몇 가지 주목할 만한 신호가 있었습니다. Epoch는 GPT-5.5 Pro가 Epoch Capabilities Index에서 159점에 도달했으며, FrontierMath에서 Tier 1-3에서 52%, Tier 4에서 40%라는 새로운 최고 기록을 달성했다고 보고했습니다. 여기에는 이전에 어떤 모델도 해결하지 못했던 두 가지 Tier 4 문제가 포함됩니다. 별도로 Greg Kamradt는 GPT-5.5 및 Opus 4.7에 대한 ARC-AGI-3 테스트가 완료되었으며, 현재 실패 모드를 분석 중이라고 말했습니다.
- 몇 가지 새로운 벤치마크는 보다 현실적인 에이전트 및 엔지니어링 행동을 목표로 합니다. Lysandre는 트랜스포머를 에이전트 친화적으로 만들기 위한 벤치마크를 발표했으며, VibeBench는 모델이 실제 작업에서 어떻게 느껴지는지를 측정하기 위해 1,000명의 자격을 갖춘 소프트웨어 엔지니어에 의한 주관적 테스트를 제안했습니다. 문서 인텔리전스 측면에서, LlamaIndex의 ParseBench는 OCR 벤치마크가 취소선 및 위첨자와 같은 의미론적 서식을 놓치며, 이는 에이전트에게 의미를 실질적으로 변경한다고 강조했습니다.
- 구체적인 엔지니어링 시사점을 가진 연구 노트: Rosinality는 DeepSpeed와 OpenRLHF에서 SFT 성능을 저하시키는 버그를 지적했으며, 이는 이전 연구에 영향을 미칩니다. Arjun Kocher는 DeepSeek-V4 논문의 Compressed Sparse Attention에 대한 충실한 구현을 발표했습니다. che_shr_cat은 단일 블록 트랜스포머가 명시적인 스크래치패드와 역 라우팅 초기화가 있을 때만 Extreme Sudoku를 해결할 수 있으며, 그렇지 않으면 성능이 0이라고 보여주었습니다. 최적화 측면에서, Keller Jordan은 Muon 및 AdamW와 같은 메서드를 재현 가능한 스피드런 스타일 작업에서 비교하도록 설계된 경량 Modded-NanoGPT 옵티마이저 벤치마크를 출시했습니다.
플랫폼 경제학, API 가격, 그리고 클로즈드 모델 신뢰성 우려

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-not-much-happened-today&utm_source=paywall-free-trial&utm_medium=web&utm_content=195821425&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-not-much-happened-today&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
