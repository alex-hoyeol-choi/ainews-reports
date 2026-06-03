# Microsoft Build: MAI-Thinking-1 and MAI Family models - 요약

**원문 URL**: https://www.latent.space/p/ainews-microsoft-build-mai-thinking
**번역일**: 2026-06-03 06:19
**발행일**: 2026-06-03

---

### 🔥 주요 뉴스
*   **Microsoft Build에서 7종의 MAI 모델 공개** — Microsoft AI는 MAI-Thinking-1, MAI-Code-1-Flash, MAI-Image-2.5, MAI-Transcribe-1.5, MAI-Voice-2를 포함한 7가지 새로운 MAI 모델 제품군을 발표했습니다. 특히 MAI-Thinking-1은 35B 활성 파라미터 MoE 모델로, 256K 컨텍스트를 지원하며, 타사 모델 디스틸레이션 없이 순수 데이터로 학습되었습니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/1e8ca90a-629c-44d5-af2f-0b0cd2a60aa2_1510x886.png)
*   **Microsoft, 에이전트 중심의 Windows 및 개발 플랫폼 전략 강화** — Build에서 온디바이스 AI 및 에이전트 네이티브 Windows를 강조하며, 에이전트를 위한 보안 실행 계층, 새로운 Surface RTX Spark Dev Box, Windows AI 액세스 확장 등을 발표했습니다. GitHub Copilot 앱은 에이전트 네이티브 소프트웨어 개발을 위한 데스크톱 허브로 추진됩니다.
*   **Microsoft Web IQ 출시 및 AI 에이전트용 검색 API 공개** — AI 에이전트를 위한 새로운 그라운딩/검색 API 스택인 Web IQ를 소개했습니다. 이 API는 이미 Copilot 및 ChatGPT를 포함한 업계 주요 AI 에이전트 및 챗봇에 사용되고 있으며, 에이전트의 미래 검색 수요에 대응하기 위해 Bing 스택을 재설계했습니다.
*   **MAI-Thinking-1 기술 보고서 공개 및 투명성 강조** — Microsoft는 MAI-Thinking-1에 대한 109페이지 분량의 기술 보고서를 발표하여 학습 파이프라인, 스케일링 방법론, 데이터 큐레이션, 인프라 지표, MFU 수치 등 이례적으로 상세한 정보를 공개했습니다. 이 보고서는 합성 데이터나 디스틸레이션 없이 순수 데이터로 학습되었음을 강조합니다.
    ![X avatar for @eliebakouch](https://pbs.substack.com/profile_images/1745893660099592193/MmYemsw6.jpg)

### 📊 모델 & 벤치마크
*   **MAI-Thinking-1** — 35B 활성 파라미터 MoE 모델로 256K 컨텍스트 윈도우를 지원하며, AIME 2025에서 97%, SWE-Bench Pro에서 53%를 달성했습니다. 30T 토큰으로 사전 학습되었고, 8192개의 GB200 GPU를 사용했습니다.
*   **MAI-Code-1-Flash** — 5B 파라미터 모델로 SWE-Bench Pro에서 51%를 달성하여 Haiku급 크기/비용에 근접한 성능을 보였습니다.
*   **MAI-Image-2.5** — 이미지 편집 리더보드에서 2위를 차지했으며, Image Edit Arena에서 1401점을 기록하여 Nano Banana 2를 능가했습니다.
*   **MAI-Transcribe-1.5** — 실시간 대비 약 276배 빠른 속도와 2.4% AA-WER로 STT(Speech-to-Text) 프론티어에서 3위를 기록했습니다. 43개 언어를 지원하며 키워드 바이어싱 기능을 제공합니다.
*   **H Company Holo 3.1** — Qwen 스타일 아키텍처 기반의 0.8B에서 35B까지의 로컬 컴퓨터 사용 모델 제품군을 출시했습니다. 35B 모델은 AndroidWorld에서 79.3%를 기록했습니다.
*   **PaintBench** — 정확한 이미지 편집을 위한 새로운 벤치마크가 발표되었습니다.
*   **VSTAT** — 비디오 상태 추적을 위한 새로운 벤치마크가 공개되었으며, 프론티어 MLLM이 진화하는 세계 상태 추적에 여전히 약하다고 지적합니다.
*   **Data Agent Benchmark** — 엔터프라이즈 데이터 워크플로우를 위한 새로운 벤치마크가 출시되었습니다.

### 🛠️ 제품 & 도구
*   **Microsoft Web IQ** — AI 에이전트를 위한 새로운 그라운딩/검색 API 스택을 출시했습니다.
*   **GitHub Copilot 앱** — 에이전트 네이티브 소프트웨어 개발을 위한 데스크톱 허브로 공개되었으며, 캔버스, 기기 간 연속성, GitHub 에이전트 워크플로우 통합을 제공합니다. Copilot CLI는 탭, 피드백, 프롬프트 스케줄링, 음성 입력을 갖춘 실험적인 터미널 UI를 추가했습니다.
*   **OpenAI Codex Sites** — 팀이 아이디어/문서/계획을 인증 및 동적 데이터를 갖춘 배포된 내부 웹사이트/앱으로 전환할 수 있도록 출시되었습니다.
*   **OpenAI Codex 플러그인 확장** — 영업, 데이터 분석, 크리에이티브 프로덕션, 제품 디자인 등 역할별 플러그인을 확장하여 62개 앱과 110개 스킬에 접근할 수 있게 되었습니다.
*   **Anthropic Claude Platform CLI** — Claude Platform용 CLI를 출시하고, Claude Code의 /fork를 업그레이드하여 정확한 컨텍스트와 프롬프트 캐시를 가진 백그라운드 에이전트를 실행할 수 있게 했습니다.
*   **Nous Hermes Desktop** — Hermes 에이전트를 위한 로컬/네이티브 데스크톱 인터페이스를 출시했습니다.
*   **Cognition Devin Desktop** — 로컬/클라우드 에이전트 관리를 위한 에이전트 중립 데스크톱을 출시했습니다.
*   **Perplexity Computer** — 온디바이스 로컬 모델과 프론티어 클라우드 모델 간에 작업을 분할하는 하이브리드 에이전틱 인퍼런스를 발표했습니다.
*   **Hugging Face 하드웨어 호환성 검사기** — 새로운 하드웨어 호환성 검사기를 제공합니다.
*   **oMLX** — 네이티브 macOS 앱이 출시되었습니다.
*   **W&B Weave** — 에이전트 우선 관측성 도구로 재출시되었으며, 일반적인 하네스 전반의 통합과 실패 모드의 자동 감지 기능을 갖추고 있습니다.

### 🔬 연구 & 논문
*   **Google DeepMind Co-Scientist** — Gemini 기반의 다중 에이전트 가설 생성 시스템을 발표했습니다. 간 섬유증 표적, ALS 접근법, 노화 관련 유전적 단서 식별에 기여했다고 주장합니다.
*   **Crafter / CraftEditor** — 편집 가능한 과학 그림 생성을 위한 5개 에이전트 워크플로우를 소개했습니다.
*   **Tilde Research Wall Attention** — 대각선 망각 게이트를 가진 RoPE-free 어텐션 방법으로, 4k에서 훈련하고 200k+ 토큰으로 일반화하며 Triton 커널과 강력한 디코드 처리량을 제공합니다.
*   **로봇 비전 인코더** — 정적 이미지 사전 학습 대신 동적 인식을 인코딩하여 실제 OOD(Out-of-Distribution) 성공률을 22.5% 높였다고 주장하는 로봇 비전 인코더가 게시되었습니다.

### 💰 산업 동향
*   **Microsoft Foundry 모델 확장** — Microsoft Foundry에서 11,000개 이상의 모델을 사용할 수 있으며, 이 중 10,928개가 Hugging Face에서 온 것이라고 발표했습니다.
*   **Westmag, 로봇 액추에이터 및 드론 모터 개발을 위해 1,100만 달러 유치** — 미국 로봇 액추에이터 및 드론 모터 개발을 위해 a16z가 주도하는 1,100만 달러의 투자를 유치하며 스텔스 모드를 해제했습니다.
*   **NVIDIA, PyTorch의 OpenMDW-1.1 채택** — NVIDIA가 4개의 오픈 모델 제품군에 걸쳐 PyTorch의 개방형 AI 모델 라이선스 프레임워크인 OpenMDW-1.1을 채택했습니다.
*   **Martin Scorsese, FLUX를 스토리보딩에 활용** — Martin Scorsese 감독이 Black Forest Labs와 함께 스토리보딩을 위한 FLUX의 제한적이고 사전 제작 단계의 사용을 공개적으로 시연했습니다.

### ⚡ 인프라 & 하드웨어
*   **Microsoft MAIA 200 최적화** — MAI 모델은 MAIA 200 맞춤형 실리콘에 최적화되어, GB200 대비 달러당 성능 30% 향상 및 와트당 성능 1.4배 향상을 제공합니다.
*   **Surface RTX Spark Dev Box** — 새로운 개발자용 하드웨어인 Surface RTX Spark Dev Box가 발표되었습니다.
*   **DGX Station 및 RTX Spark 로컬 실행** — DGX Station에서 1조 파라미터 모델을 로컬로 실행하고, RTX Spark에서 120B 파라미터 모델을 로컬로 실행하는 기능이 언급되었습니다.
*   **Prime-RL Mooncake Store** — 크로스 노드 프리픽스 / KV 캐시 재사용을 위해 Mooncake Store를 vLLM과 통합했습니다.
*   **Together MiniMax-M3 서빙 최적화** — KV-블록 메이저 희소 어텐션, 페이지드 디코드, 최적화된 인덱스 스코어링, 멀티모달 전처리 등을 통해 81–125%의 처리량 개선을 달성했습니다.
*   **NVIDIA Nemotron 3 Ultra 및 RTX Spark Specs** — NVIDIA Nemotron 3 Ultra 및 RTX Spark의 사양이 발표되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
