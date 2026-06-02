# NVIDIA Cosmos 3, Nemotron 3 Ultra, and RTX Spark - 요약

**원문 URL**: https://www.latent.space/p/ainews-nvidia-cosmos-3-nemotron-3
**번역일**: 2026-06-02 06:19
**발행일**: 2026-06-02

---

### 🔥 주요 뉴스
**[NVIDIA Cosmos 3 출시 및 SOTA 달성]** — NVIDIA가 언어, 이미지, 비디오, 오디오, 액션을 통합한 Mixture-of-Transformers 아키텍처 기반의 Cosmos 3 모델을 출시했습니다. base Nano (16B) 및 Super (64B) 모델로 구성되며, Text2Image 및 Image2Video 리더보드에서 새로운 SOTA 오픈 웨이트 모델로 등극했습니다.
![X avatar for @liu_mingyu](https://pbs.substack.com/profile_images/2002841783735042048/07JFOmTh.jpg)
**[NVIDIA Nemotron 3 Ultra 공개]** — NVIDIA는 550B-A55B 규모의 효율적이고 빠른 오픈 웨이트 LLM인 Nemotron 3 Ultra를 발표했습니다. 이 모델은 새로운 미국 SOTA를 달성했으며, 특정 설정에서 300+ tok/s로 서빙될 수 있는 성능을 보입니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/f6685277-4569-4135-92cb-e7a4645246125_4096x2732.jpeg)
**[NVIDIA RTX Spark 개인용 AI 컴퓨터 발표]** — NVIDIA는 Grace + Blackwell 기반의 개인용 AI 컴퓨터인 RTX Spark를 미리 공개했습니다. 이 시스템은 최대 128GB 통합 메모리와 1 PFLOP FP4 성능을 제공하며, Microsoft, OpenClaw, Hermes Agent가 론칭 파트너로 참여합니다.
![X avatar for @NVIDIARTXSpark](https://pbs.substack.com/profile_images/2061303426479431680/BDJQPK6Q.jpg)

### 📊 모델 & 벤치마크
*   **MiniMax M3 출시:** 1M 컨텍스트, 네이티브 멀티모달리티를 갖춘 오픈 웨이트 멀티모달 에이전트/코딩 모델 M3를 출시했습니다. SWE-Bench Pro 59.0%, Terminal Bench 2.1 66.0%, MCP Atlas 74.2%의 경쟁력 있는 에이전트 벤치마크를 기록했습니다.
*   **Alibaba Qwen3.7-Plus 공개:** GUI 및 CLI 작업, 시각적 추론, 코딩, 검색 증강 QA를 통합하는 멀티모달 인터랙티브 하이브리드 에이전트 Qwen3.7-Plus를 출시했습니다.
*   **JetBrains Mellum2 출시:** 약 11T 토큰으로 학습되고 RLVR로 사후 학습된, 2.5B 활성 파라미터를 가진 12B MoE 모델 Mellum2를 출시했습니다. 라우팅, RAG, 서브 에이전트, IDE 사용을 위한 초저 레이턴시 인퍼런스를 목표로 합니다.
*   **Perplexity "Search as Code" 성능 향상:** 모델이 검색 SDK에 대해 Python 코드를 작성하는 "Search as Code" 아키텍처를 통해 내부 WANDR 벤치마크에서 0.152에서 0.386으로 성능이 향상되었다고 보고했습니다.
*   **Claude Opus 4.8 ARC-AGI-3 SOTA 달성:** Claude Opus 4.8이 ARC-AGI-3 벤치마크에서 1.5%로 새로운 SOTA를 기록했습니다.

### 🛠️ 제품 & 도구
*   **Google Gemini API 관리형 에이전트 상세화:** Gemini API에서 단일 API 호출로 추론, 코드 작성/실행, 파일 관리, 호스팅된 Linux 샌드박스 내에서 작동하는 관리형 에이전트 기능을 상세히 설명했습니다.
*   **LangChain 에이전트 툴링 확장:** Deep Agents, Context Hub, LangSmith Sandboxes/Engine을 통해 영구적인 컨텍스트, 에이전트 라이프사이클 툴링, 자동화된 실패 분류 기능을 강조했습니다.
*   **OpenAI 모델 및 Codex의 AWS Bedrock 일반 출시:** OpenAI의 프론티어 모델과 Codex가 이제 AWS / Amazon Bedrock에서 일반적으로 사용 가능하며, 기업용 워크플로우를 지원합니다.
*   **OpenAI Codex Python SDK 출시:** 스레드, 턴, 스트리밍, 재개, 이미지, 샌드박스 제어를 지원하는 Codex Python SDK를 출시했습니다.
*   **MLX-VLM v0.6.0 업데이트:** 투기적 디코딩, Anthropic 스타일 및 응답 스타일 API, 도구 호출, 새로운 멀티모달 모델 지원, 이미지/오디오 기능이 추가된 MLX-VLM v0.6.0을 출시했습니다.

### 💰 산업 동향
*   **NVIDIA Cosmos Coalition 출범:** NVIDIA는 Runway를 포함한 파트너들과 함께 Cosmos Coalition을 출범하여 월드 모델을 위한 오픈 생태계를 구축하고 있습니다.
*   **MiniMax M3의 빠른 생태계 채택:** MiniMax M3는 Novita, Vercel AI Gateway, Cloudflare AI Gateway 등 여러 인프라 벤더로부터 출시 당일(day-0) 지원을 받으며 이례적으로 빠른 생태계 채택을 보였습니다.
*   **Microsoft Security Intelligence의 npm 공급망 침해 경고:** 90개 이상의 redhat-cloud-services 패키지에 영향을 미치는 주요 npm 공급망 침해에 대한 경고를 발표했습니다. 이는 npm/GitHub/AWS/SSH 자격 증명을 훔치는 자가 증식 웜을 포함합니다.
*   **Anthropic Claude Code 사용량 사고 및 수정:** Opus 4.8 세션이 너무 많은 병렬 서브 에이전트/도구 호출을 생성하여 예기치 않게 사용량을 소모하는 버그를 수정한 후, Pro 및 Max 사용자의 5시간 및 주간 속도 제한을 재설정했습니다.
*   **Anthropic의 기밀 S-1 초안 제출:** Anthropic이 SEC에 S-1 초안을 기밀리에 제출하여 IPO 가능성을 열었습니다.

### ⚡ 인프라 & 하드웨어
*   **Lambda의 NVIDIA Quantum-X InfiniBand Photonics 스위치 최초 채택:** Lambda가 대규모 AI 클러스터에서 네트워크 전력 및 장애를 줄이기 위해 코패키지드 옵틱스를 추진하는 NVIDIA Quantum-X InfiniBand Photonics Q3450-LD 스위치를 최초로 채택했습니다.
*   **OpenAI의 Stargate Michigan 데이터센터 발표:** OpenAI는 폐쇄 루프 냉각을 사용하고 인력/교육 약속과 결합된, 계획된 1GW 데이터센터인 Stargate Michigan을 발표했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
