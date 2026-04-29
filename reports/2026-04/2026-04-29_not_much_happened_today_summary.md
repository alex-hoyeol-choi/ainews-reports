# not much happened today - 요약

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today
**번역일**: 2026-04-29 06:18
**발행일**: 2026-04-29

---

### 🔥 주요 뉴스
**[NVIDIA Nemotron 3 Nano Omni 출시]** — NVIDIA가 256K 컨텍스트를 가진 오픈 30B/A3B 멀티모달 MoE 모델인 Nemotron 3 Nano Omni를 공개했습니다. 이 모델은 텍스트, 이미지, 비디오, 오디오 및 문서를 아우르는 에이전틱 워크로드를 위해 구축되었으며, Open ASR 리더보드에서 5.95%의 WER을 기록하고 유사 오픈 옴니 모델 대비 약 9배의 처리량을 주장합니다.
**[vLLM v0.20.0 업데이트 및 하드웨어 지원 강화]** — vLLM이 v0.20.0 버전을 출시하며 MoE 서빙 효율성을 크게 개선했습니다. TurboQuant 2비트 KV cache, FA4 재활성화, 퓨즈드 RMSNorm을 통한 2.1% 종단간 레이턴시 개선이 포함되며, Blackwell, Jetson Thor, ROCm, Intel XPU, GB200/Grace-Blackwell 등 광범위한 하드웨어 지원을 추가했습니다.
**[GPT-5.5 Pro, 벤치마크 신기록 달성]** — GPT-5.5 Pro가 Epoch Capabilities Index에서 159점을 기록하고 FrontierMath에서 Tier 1-3 52%, Tier 4 40%라는 새로운 최고 기록을 달성했습니다. 특히 이전에 어떤 모델도 해결하지 못했던 두 가지 Tier 4 문제를 해결하며 성능 우위를 입증했습니다.
**[Poolside, 오픈 웨이트 코더 모델 Laguna XS.2 및 M.1 공개]** — Poolside가 첫 공개 모델인 Laguna XS.2 (33B/3B 활성 MoE)와 Laguna M.1 (225B/23B 활성 MoE)을 Apache 2.0 라이선스로 출시했습니다. 이 코딩 모델들은 하이브리드 어텐션과 FP8 KV cache를 특징으로 하며 Qwen-3.5에 근접하는 성능을 주장합니다.
**[Mistral Workflows 공개 프리뷰 출시]** — Mistral이 엔터프라이즈 AI 프로세스를 위한 오케스트레이션 레이어인 Workflows를 공개 프리뷰로 선보였습니다. 이 플랫폼은 AI 시스템을 영속적이고 관측 가능하며 내결함성을 가진 프로덕션 환경으로 전환하는 것을 목표로 합니다.

### 📊 모델 & 벤치마크
*   Poolside Laguna XS.2 및 M.1 모델이 출시되었습니다. 이들은 각각 33B/3B 및 225B/23B 활성 MoE 코딩 모델로, Apache 2.0 라이선스 하에 공개되었으며 Qwen-3.5에 근접하는 성능을 주장합니다.
*   NVIDIA Nemotron 3 Nano Omni가 공개되었습니다. 이 30B/A3B 멀티모달 MoE 모델은 256K 컨텍스트를 지원하며, Open ASR 리더보드에서 5.95%의 WER을 기록하고 유사 모델 대비 약 9배의 처리량을 제공합니다.
*   Microsoft TRELLIS.2가 오픈소스 4B 이미지-투-3D 모델로 공개되었습니다. 이 모델은 최대 1536³ PBR 텍스처 에셋을 생성하며 네이티브 3D VAE를 기반으로 합니다.
*   GPT-5.5 Pro가 Epoch Capabilities Index에서 159점을 달성하고 FrontierMath에서 Tier 1-3 52%, Tier 4 40%의 새로운 최고 기록을 세웠습니다. 이는 이전에 해결되지 않았던 두 가지 Tier 4 문제를 포함합니다.
*   Lysandre가 트랜스포머를 에이전트 친화적으로 만들기 위한 새로운 벤치마크를 발표했습니다.
*   VibeBench는 모델이 실제 작업에서 어떻게 느껴지는지를 측정하기 위해 1,000명의 소프트웨어 엔지니어에 의한 주관적 테스트를 제안했습니다.
*   LlamaIndex의 ParseBench는 OCR 벤치마크가 취소선 및 위첨자와 같은 의미론적 서식을 놓쳐 에이전트에게 의미를 실질적으로 변경할 수 있음을 지적했습니다.
*   Keller Jordan이 Muon 및 AdamW와 같은 옵티마이저를 비교하기 위한 경량 Modded-NanoGPT 옵티마이저 벤치마크를 출시했습니다.

### 🛠️ 제품 & 도구
*   vLLM v0.20.0이 출시되었습니다. 이 버전은 TurboQuant 2비트 KV cache, FA4 재활성화, 새로운 vLLM IR 기반, 퓨즈드 RMSNorm을 통한 2.1% 종단간 레이턴시 개선 등 MoE 서빙 효율성에 중점을 둡니다.
*   Mistral이 엔터프라이즈 AI 프로세스를 영속적이고 관측 가능하며 내결함성을 가진 프로덕션 시스템으로 전환하는 오케스트레이션 레이어인 Workflows를 공개 프리뷰로 출시했습니다.
*   Ammaar가 MLX를 사용하여 Gemma 4를 온디바이스에서 완전히 실행하는 바이브 코딩 앱을 오픈소스화했습니다.
*   Hermes 에이전트 하네스가 지시 따르기 및 실용적인 워크플로우에서 OpenClaw를 능가하는 성능을 보인다고 보고되었습니다.
*   Hugging Face의 ML Intern이 네이티브 메트릭 로깅과 Trackio 통합 기능을 추가하여 관측 가능한 학습 작업을 생성할 수 있게 되었습니다.

### 🔬 연구 & 논문
*   World-R1은 기존 비디오 모델이 이미 3D 구조를 인코딩하며 RL을 통해 아키텍처 변경이나 추가 비용 없이 이를 '활성화'할 수 있다고 주장합니다.
*   Rosinality가 DeepSpeed와 OpenRLHF에서 SFT 성능을 저하시키는 버그를 발견했으며, 이는 이전 연구 결과에 영향을 미칩니다.
*   Arjun Kocher가 DeepSeek-V4 논문의 Compressed Sparse Attention에 대한 충실한 구현을 발표했습니다.
*   che_shr_cat은 단일 블록 트랜스포머가 명시적인 스크래치패드와 역 라우팅 초기화가 있을 때만 Extreme Sudoku를 해결할 수 있음을 보여주었습니다.

### ⚡ 인프라 & 하드웨어
*   vLLM v0.20.0은 Blackwell, Jetson Thor, ROCm, Intel XPU, 그리고 GB200/Grace-Blackwell 설정을 포함한 광범위한 하드웨어 지원을 업데이트했습니다.
*   SemiAnalysis는 B200/B300/H200/GB200 분산형 설정에서 DeepSeek V4 Pro의 초기 서빙 결과를 강조하며, B300이 특정 워크로드에서 H200보다 최대 8배 빠를 수 있다고 주장했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
