# OpenAI reports Navier-Stokes singularity find in 88 hours using Astra-next, roughly 10,000 agents and 130B tokens (>$40M), a contender for second ever Millennium Prize awarded - 요약

**원문 URL**: https://www.latent.space/p/ainews-openai-reports-navier-stokes
**번역일**: 2026-09-09 06:19
**발행일**: 2026-09-09

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 뉴스레터의 핵심 요약 브리핑입니다.

### 🔥 주요 뉴스

**[OpenAI, 나비에-스토크스 특이점 발견 보고]** — OpenAI는 약 10,000개의 에이전트가 다중 에이전트 강화 학습을 통해 88시간 만에 나비에-스토크스 방정식의 유한 시간 특이점을 발견했다고 주장하며, 이는 두 번째 밀레니엄 상 수상 후보로 거론될 수 있는 중대한 과학적 돌파구입니다. 이 시스템은 대규모 병렬 테스트 시간 컴퓨팅과 모델 자체 조직화를 활용하여 어려운 문제를 해결했습니다.
![X avatar for @OpenAI](https://pbs.substack.com/profile_images/1885410181409820672/ztsaR0JW.jpg)

**[Meta, 개인 AI 에이전트 Muse 출시]** — Meta는 상시 작동하며 앱 및 브라우저 사용이 가능한 목표 지향적 개인 AI 에이전트 Muse를 출시했습니다. Muse는 개별 보안 VM에서 실행되며 Sentinel에 의해 작업이 중재되고 비밀이 에이전트에 직접 노출되지 않는 강력한 보안 아키텍처를 특징으로 합니다.

**[OpenAI, ChatGPT Images 2.5 및 Astra 배포 확대]** — OpenAI는 Images 2.0 대비 최대 50% 낮은 레이턴시와 향상된 사실성을 제공하는 ChatGPT Images 2.5를 출시했으며, GPT-6 Astra는 이제 Plus, Pro, Business, Enterprise 사용자에게 완전히 배포되어 macOS에서 Super Smash Bros. Melee를 컴파일하고 Minecraft Nether 포털을 구축하는 등 강력한 실제 컴퓨터 사용 성능을 시연했습니다.

### 📊 모델 & 벤치마크

*   **Qwen-Drive-1.0-4B 출시:** Qwen이 자율 주행에 특화된 오픈 웨이트 VLM인 Qwen-Drive-1.0-4B를 출시했습니다. 이 모델은 3D 객체 감지, 시맨틱 점유 예측, BEV 맵 세그멘테이션 및 미래 ego-trajectory 생성을 위한 추가 모듈을 포함하며, 자율 주행 및 일반 멀티모달 벤치마크에서 경쟁력 있는 성능을 보입니다.
*   **DeepSeek Flash 4.1 API 베타 테스트:** DeepSeek V4.1 Flash가 API를 통해 내부 베타 테스트 중이며, 새로운 모델 아키텍처를 통해 네이티브 멀티모달 지원, 더 강력한 기능, 약 2.24배 빠른 처리량, 그리고 벤치마크에서 최대 30% 더 나은 토큰 효율성을 주장합니다.
*   **OpenAI Images 2.5 벤치마크 성과:** OpenAI의 Images 2.5는 텍스트-투-이미지, 이미지 편집, 다중 이미지 편집 리더보드에서 1위와 2위를 차지하며, 특히 다중 이미지 편집에서 큰 폭의 개선을 보였습니다.

### 🛠️ 제품 & 도구

*   **Meta Muse 개인 에이전트:** Meta는 영구적인 격리된 Linux VM, 브라우저 사용, WhatsApp/앱 인터페이스, Gmail, Calendar 등 다양한 서비스 커넥터를 갖춘 개인 AI 에이전트 Muse를 출시했습니다.
*   **OpenAI ChatGPT Images 2.5:** OpenAI는 Images 2.0 대비 최대 50% 낮은 레이턴시, 더 나은 사실성, 반복 편집 일관성, 지역화된 변경, 투명 배경, 가이드 생성용 Sketch 도구를 제공하는 Images 2.5를 출시했습니다.
*   **OpenAI GPT-6 Astra 배포 확대:** GPT-6 Astra가 Codex 및 ChatGPT Work의 Plus, Pro, Business, Enterprise 사용자에게 완전히 배포되어, macOS에서 Super Smash Bros. Melee를 컴파일하고 Minecraft Nether 포털을 구축하는 등 실제 컴퓨터 사용 능력을 시연했습니다.
*   **OpenAI Images 2.5 API 변형:** 속도/품질을 위한 GPT-Image-2.5 Flare와 고정밀 세부 작업을 위한 Sunburst 두 가지 API 변형이 도입되었습니다.
*   **LangChain/deepagents 하네스 프리미티브 출시:** LangChain/deepagents는 서브 에이전트 포킹 및 관리형 연결을 포함한 에이전트 하네스 설계를 위한 삶의 질(QoL) 프리미티브를 출시하여 장기 에이전트 워크로드를 위한 스택 성숙을 알렸습니다.

### 🔬 연구 & 논문

*   **OpenAI의 다중 에이전트 RL 기반 나비에-스토크스 특이점 발견:** OpenAI는 약 10,000개의 에이전트가 다중 에이전트 강화 학습을 통해 협력하여 나비에-스토크스 방정식의 유한 시간 특이점을 발견했다고 주장했습니다. 이 시스템은 단일 긴 사슬 증명 시도보다는 병렬 테스트 시간 컴퓨팅과 모델 자체 조직화를 강조합니다.
*   **Harvey + Baseten의 재귀적 언어 모델(RLM) 하네스:** Harvey와 Baseten은 루트 에이전트가 데이터 룸을 검색하고 서브 에이전트에 위임하여 발견 사항을 집계하는 RLM 하네스를 통해 합성 LAB Diligence 벤치마크에서 모델 전반의 평균 루브릭 통과율을 23%에서 62%로 향상시켰습니다.
*   **하네스 내부 후처리 학습의 중요성:** Harvey는 GLM-5.2에 대한 자체 디스틸레이션 SFT가 통과율을 46%에서 60%로, Qwen3.5-122B-A10B에 대한 GRPO가 통과율을 30%에서 63%로 향상시켰다고 보고하며, 에이전트 벤치마크가 오케스트레이션과 후처리 학습을 모델 시스템의 일부로 다루어야 함을 시사합니다.

### 💰 산업 동향

*   **Cognition 480억 달러 기업 가치로 20억 달러 이상 투자 유치:** Cognition은 480억 달러의 기업 가치로 20억 달러 이상을 유치했으며, 5월 이후 연간 매출(run-rate revenue)이 4억 9,200만 달러에서 거의 9억 달러로 성장했다고 발표했습니다.
*   **Mistral 240억 달러 기업 가치로 투자 유치:** Mistral 또한 240억 달러의 기업 가치로 상당한 투자를 유치했습니다.

### ⚡ 인프라 & 하드웨어

*   **vLLM의 긴 컨텍스트 서빙 최적화 (Hybrid HiSparse):** vLLM은 희소-MLA 모델을 위한 Hybrid HiSparse를 설명하며, KV를 GPU에 유지하고 콜드 KV 페이지를 호스트 메모리로 오프로드하여 8×H200 노드에서 1M 컨텍스트를 가진 GLM 5.3에서 동시성을 32에서 19~25개 요청으로 크게 향상시켰습니다.
*   **vLLM의 AgentX를 위한 풀 스택 최적화:** vLLM은 실제 에이전트 트래픽을 위한 AgentX에서 벤치마킹된 풀 스택 최적화 패스를 발표했으며, 파이프라인 병렬 처리, 디코드 컨텍스트 병렬 처리, 세션-스티키 라우팅의 중요성을 강조했습니다.
*   **Cohere의 오픈소스 디코드 메가커널 서빙 스택:** Cohere는 "디코드 메가커널"을 중심으로 구축된 오픈소스 서빙 스택을 도입하여 North Mini Code에서 vLLM보다 최대 1.58배 빠른 성능과 더 높은 배치 크기에서 1.25배~1.41배의 엔드-투-엔드 이득을 주장했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
