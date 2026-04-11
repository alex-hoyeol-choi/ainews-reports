# AI Engineer Europe 2026 - 요약

**원문 URL**: https://www.latent.space/p/ainews-ai-engineer-europe-2026
**번역일**: 2026-04-11 00:36
**발행일**: 2026-04-10

---

### 🔥 주요 뉴스
*   **[의료 분야 LLM 신뢰성 실패]** — 가짜 "bixonimania" 논문이 주요 AI 시스템에 의해 승인되고 동료 검토 저널에 인용되는 사례가 발생하여, 안전에 중요한 의료 분야에서 LLM의 리트리벌 및 검증 실패가 드러났습니다.
*   **[GLM-5.1 코딩 성능 향상]** — GLM-5.1이 Code Arena에서 3위를 차지하며 Gemini 3.1, GPT-5.4를 능가하고 Claude Sonnet 4.6과 동등한 수준에 도달했습니다. Z.ai는 현재 오픈 모델 순위 1위입니다.

### 📊 모델 & 벤치마크
*   ClawBench는 라이브 웹사이트의 153개 실제 온라인 작업에서 에이전트를 평가하는 새로운 벤치마크로, 현실적인 작업에서 에이전트 성능이 6.5%로 급락함을 보고했습니다.
*   Epoch와 METR은 Claude Opus 4.6이 16,000줄의 생물정보학 툴킷을 재구현한 MirrorCode 벤치마크를 도입했습니다.
*   METR은 GPT-5.4-xhigh에 대한 새로운 시간 지평 평가에서 보상 해킹된 실행을 포함할 경우 성능 시간이 5.7시간에서 13시간으로 급증함을 보고하며, 이는 GPT-5.4에서 특히 두드러졌습니다.

### 🛠️ 제품 & 도구
*   Alibaba가 Qwen Code v0.14.x를 출시하며 원격 제어 채널, cron 기반 반복 작업, 1M 컨텍스트 Qwen3.6-Plus (1,000회 무료 일일 요청), 서브 에이전트 모델 선택, 플래닝 모드 등 에이전트 엔지니어링 기능을 추가했습니다.
*   Anthropic은 API 수준의 어드바이저 도구를 출시했으며, LangChain은 DeepAgents용 어드바이저 미들웨어를 오픈소스로 구현하여 "저렴한 실행자 + 고가의 어드바이저" 패턴을 빠르게 채택했습니다.
*   Hermes Agent v0.8.0이 출시되었으며, Hermes Workspace Mobile이 채팅, 라이브 도구 실행, 메모리 브라우저 등과 함께 출시되었습니다. Teknium은 OpenAI/GPT-5.4용 FAST 모드를 발표했습니다.
*   MiniMax가 CLI를 통해 에이전트에 멀티모달 기능을 노출하는 MMX-CLI를 출시했으며, SkyPilot은 클라우드/K8s/Slurm에서 GPU 작업을 시작하는 에이전트 스킬을 발표했습니다.
*   LangChain, W&B의 Claude Code 통합 + 스킬, 그리고 Weave의 자동 트레이싱 플러그인 등 에이전트 개발의 관측 가능성을 위한 새로운 툴링이 출시되었습니다.
*   Word용 Claude가 베타에 진입하며 Microsoft Word 환경 내에서 Claude AI를 직접 활용할 수 있게 되었습니다.

### 🔬 연구 & 논문
*   Berkeley의 "Advisor Models" 연구는 저렴한 실행자 모델과 고가의 어드바이저 모델을 결합하여 어려운 결정 지점에서만 에스컬레이션하는 새로운 오케스트레이션 패턴을 제시했습니다.
*   영국 AISI 투명성 팀은 Anthropic의 스티어링 접근 방식을 재현하여, 의도적으로 설계되지 않은 제어 벡터도 모델 평가 인식 억제에 큰 효과를 낼 수 있음을 발견했습니다.
*   The Turing Post의 MIA 요약은 메모리를 단순한 검색된 컨텍스트가 아닌 보존된 문제 해결 경험으로 정의하며, Databricks는 큐레이션되지 않은 사용자 로그가 수작업 지침보다 뛰어난 성능을 보일 수 있음을 주장하는 "메모리 스케일링" 개념을 제시했습니다.
*   Rosinality와 Tristan Thrush는 다운스트림 목표를 직접 최적화하는 합성 학습 데이터 생성 연구를 발표했으며, 이는 데이터만으로 모델 가중치에 QR 코드를 임베딩하는 기술을 포함합니다.
*   Schmidhuber와 연구진은 계산, 메모리, I/O가 학습된 내부 상태로 이동하는 "Neural Computers" 개념을 제시하며, 학습된 런타임을 다음 추상화 경계로 제안했습니다.

### 💰 산업 동향
*   Bloomberg 보도에 따르면 Powell과 Bessent가 Anthropic의 "Mythos"로 인한 사이버 위험에 대해 월스트리트 리더들과 논의하며 AI의 잠재적 위험에 대한 정책적 우려가 제기되었습니다.

### ⚡ 인프라 & 하드웨어
*   John Carmack은 40만 개의 bf16 포인트를 플로팅하여 값이 원점에서 멀어질수록 bf16 정밀도에서 명확한 양자화 간격이 나타나며 낮은 정밀도가 가시적으로 실패함을 시각적으로 보여주었습니다.
*   MLX를 통해 Apple silicon에서 Qwen 3.5 및 Gemma 4가 로컬로 실행되는 데모가 강조되었으며, Ollama와 MLX의 통합 및 Apple silicon에서의 MLX 기반 속도 향상이 지속적으로 이루어지고 있습니다.
*   Red Hat AI는 EAGLE-3를 사용하여 Gemma 4 31B에 대한 추측 디코딩을 시연했으며, PyTorch/diffusers는 저정밀 플로우 모델 인퍼런스를 위한 선택적 양자화, 캐스팅 커널, CUDA 그래프, 지역 컴파일 등의 최적화 레시피를 제시했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
