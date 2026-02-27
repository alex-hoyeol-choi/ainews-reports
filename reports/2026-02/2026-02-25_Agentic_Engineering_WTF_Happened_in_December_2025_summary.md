# Agentic Engineering: WTF Happened in December 2025? - 요약

**원문 URL**: https://news.smol.ai/issues/2026-02-25-wtf-happened
**번역일**: 2026-02-27 06:58
**발행일**: 2026-02-25

---

## AI 산업 브리핑 (2026년 2월 24일-25일)

### 🔥 주요 뉴스
**[Perplexity Computer 출시]** — Perplexity가 파일, 도구, 메모리, 모델을 하나의 인터페이스에서 오케스트레이션하여 프로젝트를 엔드투엔드로 관리하는 'Computer'를 출시했습니다. Max 구독자에게 먼저 제공되며, 병렬적이고 비동기적인 하위 에이전트 아키텍처를 특징으로 합니다.

**[Anthropic, 책임 있는 스케일링 정책(RSP) 변경 및 펜타곤과의 갈등]** — Anthropic이 AI 안전 조치에 대한 기존 약속을 완화하는 RSP v3를 발표했습니다. 동시에 펜타곤은 Claude 모델의 군사적 사용을 요구하며 안전 장치 제거를 압박하고 있습니다.

**[OpenAI GPT-5.3-Codex 출시 및 가격 공개]** — OpenAI가 API를 통해 GPT-5.3-Codex를 출시했습니다. 이전 버전 대비 약 25% 더 빠르고 토큰 사용량이 적으며, 입력 토큰당 $1.75, 출력 토큰당 $14의 가격이 책정되었습니다.

**[Alibaba Qwen3.5 Medium 시리즈 대규모 배포]** — Alibaba가 Qwen3.5 Medium 시리즈(27B, 35B-A3B, 122B-A10B)를 출시하며 vLLM, GGUF 등 광범위한 툴링을 지원합니다. 4비트 양자화에서 거의 손실 없는 정확도와 1M+ 컨텍스트 길이를 제공합니다.

**[Meta 및 OpenAI, AMD 주식 워런트 대규모 비축]** — OpenAI와 Meta가 미래 GPU 지출과 연계된 1억 6천만 AMD 주식에 대한 워런트를 확보했습니다. 이는 잠재적으로 1,920억 달러 규모의 대규모 하드웨어 비공개 거래로 평가됩니다.

### 📊 모델 & 벤치마크
*   OpenAI가 API에 GPT-5.3-Codex를 출시했으며, 이전 버전 대비 약 25% 더 빠르고 SWE-Bench Pro에서 강력한 성능을 보입니다.
*   Alibaba는 Qwen3.5 Medium 시리즈(27B, 35B-A3B, 122B-A10B)를 배포하며 4비트 양자화 견고성, 800K+에서 1M+ 컨텍스트 길이 지원, FP8 가중치 지원을 강조했습니다.
*   Liquid AI는 240억 매개변수 희소 MoE 모델인 LFM2-24B-A2B를 출시했으며, 토큰당 20억 개가 활성화되고 32GB RAM에서 실행되도록 설계되었습니다.
*   xAI의 Grok-4.20-Beta1 모델은 Search Arena 리더보드에서 1위를 차지하고 Text Arena 리더보드에서 Gemini 3.1 Pro와 동점을 기록했습니다.
*   Kimi 2.5는 OS Frontier Math Level 4 벤치마크에서 4.2%를 기록하며 GLM 5 및 Deepseek V3.2의 두 배 성능을 보였습니다.
*   Nano Banana 2 (Gemini 3.1 Flash Image)가 출시되었으며, 기존 Pro 버전에 가까운 품질과 밀집된 구성에서 탁월한 공간 논리를 제공합니다.
*   KREA AI는 저비용 이미지 편집 모델인 Seedream 5 Lite를 출시했습니다.
*   Cohere는 Tiny Aya 모델을 출시했습니다.
*   Stefano Ermon은 기존 모델보다 5배 빠르다고 주장하는 추론 확산 LLM인 Mercury 2를 출시했습니다.
*   Jim Fan은 휴머노이드 로봇을 위한 4,200만 개 파라미터 트랜스포머인 SONIC을 오픈소스로 공개했습니다.
*   Quiver AI는 벡터 디자인 AI 연구소로 출범하며 830만 달러 시드 펀딩을 유치하고, 이미지와 텍스트를 SVG로 변환하는 Arrow-1.0 모델을 공개 베타로 출시했습니다.
*   APEX Testing 벤치마크에서 GLM-4.7 양자화 모델이 실제 코딩 작업에서 최고의 로컬 모델로 평가되었습니다.
*   Qwen3.5 27B 모델은 RTX 3090 GPU에서 35B-A3B 대비 더 높은 토큰 처리량(초당 100 토큰 vs 20 토큰)을 보였습니다.
*   Bullshit Benchmark는 터무니없는 프롬프트 감지 능력을 평가하며, Claude Opus 4.6이 높은 성능을 보였습니다.
*   Unsloth AI는 Hugging Face에 Qwen3.5 122B NVFP4 퀀트를 업로드했습니다.
*   Andy-4.1, 새로운 Minecraft 플레이 모델이 Hugging Face에 공개되었습니다.
*   Sesame AI 음성 AI 모델이 화제를 모으고 있으며, ASR, LLM, TTS를 통합한 저지연 음성 시스템에 중점을 둡니다.
*   Pythia-2.8b 체크포인트에서 선택한 리비전과 관계없이 Hugging Face가 동일한 가중치를 제공하는 버그가 보고되었습니다.
*   ENI Jailbreak 프롬프트의 수정된 버전으로 생성된 Gemini Canvas가 Gemini 3 Pro, Claude Opus 4.6, ChatGPT 5.3에서 보편적으로 작동한다고 주장됩니다.

### 🛠️ 제품 & 도구
*   Perplexity는 파일, 도구, 메모리, 모델을 오케스트레이션하여 프로젝트를 엔드투엔드로 관리하는 'Computer'를 출시했습니다.
*   GitHub Copilot CLI가 정식 출시(GA)되었으며, 리포지토리 전체의 심층 연구를 위한 `/research` 기능을 추가했습니다.
*   Anthropic은 COBOL 레거시 코드 현대화를 위한 새로운 도구인 Claude Code를 발표했습니다.
*   Nous Research는 다단계 메모리 시스템과 영구적인 전용 머신 액세스를 갖춘 오픈소스 Hermes Agent 리포지토리를 공개했습니다.
*   Aider 코딩 도우미는 AI 생성 코드 편집을 즉시 승인하고 실행할 수 있는 `/ok` 별칭을 메인 브랜치에 병합했습니다.
*   LM Studio 팀은 Tailscale을 래핑하여 로컬 LLM 서버에 원격 액세스를 제공하는 LM Link 문서를 출시했습니다.
*   Serenade는 Python처럼 작성되지만 C++, CUDA, x86-64 ASM으로 직접 트랜스파일되는 새로운 구문을 공개했습니다.
*   OpenPad 앱이 iPad의 M2 프로세서를 활용하여 로컬 모델로 OpenClaw와 같은 기능을 실행하도록 개발 중입니다.
*   Gemini 3 Pro 이미지 미리보기가 프롬프트에 특정 문구를 추가하면 활성화되는 방법이 발견되었습니다.
*   Deepseek R1 무료 모델이 OpenRouter 플랫폼에서 제거되었습니다.
*   Perplexity Pro는 유료 사용자에게 예고 없는 일일 이미지 업로드 제한을 적용했습니다.
*   Cognition은 컴퓨터 사용 기능, 자체 검증 및 자동 수정 기능을 갖춘 업그레이드된 자율 AI 에이전트 Devin 2.2를 출시했습니다.
*   Cursor AI는 AI 에이전트가 코드 차이점 대신 비디오 데모를 통해 작업을 시연할 수 있는 새로운 기능을 도입했습니다.
*   Codaph CLI는 Codex 프롬프트, 에이전트 추론, 파일 diff를 공유 메모리에 동기화하는 도구로 소개되었습니다.
*   Google은 Gemini CLI를 통해 단 10개의 프롬프트만 보낸 후 Google Gemini 계정을 영구적으로 잠갔습니다.
*   Claude AI 포털은 문서화되지 않은 OAuth 엔드포인트를 통해 보조금 토큰을 빼내려던 OpenClaw 사용자들을 금지하기 시작했습니다.
*   OpenClaw 에이전트에 전체 시스템 권한을 부여한 사용자의 휴지통 디렉토리가 AI에 의해 실수로 영구적으로 삭제되었습니다.
*   Rogue OpenClaw Proxy가 DeepSeek-R1을 통해 Claude, Gemini, Grok API 필터를 영구적이고 은밀하게 탈옥시키는 자체 호스팅 자율 프록시를 구축했습니다.
*   LM Studio 4.4 업데이트 후 실행 문제와 llama.cpp가 Qwen3.5 모델을 로드하지 못하는 문제가 발생했으며, 릴리스 8145로 다운그레이드하여 해결되었습니다.
*   Gradio 5.12.0 이전 버전의 로그인 버그와 관련된 ZeroGPU 할당 문제가 보고되었습니다.
*   유출된 API 키로 인해 OpenRouter에서 무단 사용이 발생하여 사용자가 차지백을 위협했습니다.

### 🔬 연구 & 논문
*   Intuit AI Research는 에이전트 성공이 도구 인터페이스 텍스트에 크게 의존하며, 인퍼런스 시 트레이스 없이 모델이 도구 설명을 에이전트가 사용할 수 있는 형태로 다시 작성하도록 가르치는 커리큘럼을 소개했습니다.
*   ActionEngine은 GUI 에이전트를 오프라인 탐색을 통해 상태 머신을 생성하는 그래프 순회로 재구성하여 성공률, 비용, 레이턴시를 개선했다고 주장합니다.
*   균일 확산 LLM에서 인퍼런스 시간 스케일링을 위한 "Diffusion Duality (Ch.2) Ψ-Samplers" 논문이 발표되었습니다.
*   Emmy Liu의 새로운 사전 인쇄본은 '미드트레이닝'이 사전 학습과 사후 학습 사이의 다리 역할을 하여 망각을 완화하는 데 가장 효과적임을 보여주지만, 그 성공은 정확한 타이밍에 달려 있다고 탐구합니다.
*   METR은 개발자들이 'AI 없음' 대조군에서 일하기를 거부하며, AI가 워크플로우의 필수적인 부분이 되었음을 시사하는 연구 결과를 발표했습니다.
*   Jim Fan은 휴머노이드 로봇을 위한 '시스템 1' 반응형 지능을 제공하는 4,200만 개 파라미터 트랜스포머인 SONIC을 소개했습니다.
*   독립 개발자가 MiniMax-m2.5의 5GB MoE 샤드를 2MB 벡터 양자화 잠재 공간으로 압축했다고 주장하며 논문을 준비 중입니다.
*   Latent Diffusion Model 이후의 확산 논문들(Rectified Flows, Flow Matching, Diffusion Forcing 등)이 활발히 연구되고 있습니다.
*   webXOS는 Three.js 시뮬레이션으로 생성된 중력 렌즈 효과가 있는 합성 블랙홀 렌더링을 포함하는 Black Hole Time-Lapse Dataset을 공유했습니다.

### 💰 산업 동향
*   Anthropic은 Claude의 "컴퓨터 사용" 기능 발전을 위해 Vercept를 인수했습니다.
*   Anthropic은 책임 있는 스케일링 정책(RSP) v3를 변경하여, 이전의 엄격한 "완화 조치 보장 없으면 학습 중단"에서 더 빈번한 투명성 아티팩트 및 외부 검토 약속으로 전환했습니다.
*   미국 정치 지도부는 AI/데이터센터 기업들이 전력망 부담을 피하기 위해 자체적으로 전력을 조달하도록 압박하고 있습니다.
*   OpenAI와 Meta는 대규모 미래 GPU 지출과 직접적으로 연결된 지분 환급으로 1억 6천만 AMD 주식에 대한 워런트를 확보했습니다.
*   xAI는 펜타곤과 Grok AI 모델을 기밀 군사 시스템에 통합하기로 합의했습니다.
*   펜타곤은 Anthropic에 Claude AI 모델에서 안전 장치를 제거할 것을 요구했으며, 불이행 시 국방물자생산법(Defense Production Act) 발동 가능성을 언급했습니다.
*   Wayve는 'Embodied AI' 상용화를 위해 15억 달러 규모의 시리즈 D 라운드를 유치하여 회사 가치를 86억 달러로 평가받았습니다.
*   Wayve는 2026년부터 10개 도시에서 감독형 로보택시 시험 운행을 시작하고 2027년에는 소비자 차량 판매를 이어갈 로드맵을 공개했습니다.
*   저작권 문제로 Seedance 2.0의 글로벌 출시가 지연되고 있으며, 할리우드 영화 스튜디오들은 AI 저작권 관련 소송을 통해 기업들을 압박하고 있습니다.
*   WeAreDevelopers World Congress North America가 2026년 9월 23일부터 25일까지 캘리포니아 산호세에서 개최될 예정입니다.
*   Apart Research는 Redwood Research와 협력하여 2026년 3월 20일부터 22일까지 AI Control Hackathon을 개최합니다.
*   DSPy 밋업이 샌프란시스코에서 개최될 예정이며, 프로덕션 환경에서의 DSPy 및 RLM 사용 사례에 중점을 둡니다.

### ⚡ 인프라 & 하드웨어
*   Goodfire는 최소한의 인퍼런스 오버헤드로 조 단위 매개변수 규모의 해석 가능성을 가능하게 하는 인프라 작업을 설명했습니다.
*   Packet.ai는 AI 워크로드용 Blackwell GPU를 학습에 시간당 $0.66 또는 월 $199의 가격으로 제공합니다.
*   Zagora는 Qwen 2.5 및 Mistral과 같은 70B+ 모델을 표준 인터넷 연결을 통해 완전히 훈련하기 위한 분산 파인튜닝 시스템을 구축 중이라고 발표했습니다.
*   PyTorch에서 `activate_flash_attention_impl(“FA3”)`를 호출하면 기본 Flash Attention 2 커널이 FA3로 재정의됩니다.
*   Nemotron 3 Nano는 오래된 하드웨어(Dual Xeon, 2x RTX 3060)에서 128K 컨텍스트에서 초당 30-40 토큰을 달성했습니다.
*   eBPF가 GPU와 더 잘 작동하도록 확장하는 방안에 대한 논의가 진행될 예정입니다.
*   vllm-project 풀 리퀘스트를 기반으로 all_gather + FP8 + GEMM (H100)의 Helion 구현이 작업 중입니다.
*   OpenRouter는 2월 17일과 19일에 상위 인프라 제공업체 장애로 인해 대규모 401 인증 오류가 발생했음을 확인했습니다.

---

*이 문서는 news.smol.ai의 뉴스레터를 자동 요약한 것입니다.*
