# NVIDIA GTC: Jensen goes hard on OpenClaw, Vera CPU, and announces $1T sales backlog in 2027 - 요약

**원문 URL**: https://www.latent.space/p/ainews-nvidia-gtc-jensen-goes-hard
**번역일**: 2026-03-17 06:40
**발행일**: 2026-03-17

---

### 🔥 주요 뉴스
**[NVIDIA GTC 주요 발표]** — NVIDIA는 GTC 2026에서 새로운 CPU인 Vera를 공개하고, Blackwell 및 Rubin GPU의 강력한 판매 실적을 강조하며 2027년까지 1조 달러의 판매 잔고를 발표했습니다. 또한, OpenClaw의 보안 문제를 해결하기 위한 솔루션으로 NemoClaw를 제시했습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/3c9e5d8d-2b90-4c27-ab1c-fd67c035acb4_3592x1886.png)
**[OpenAI Codex의 폭발적 성장]** — OpenAI의 Codex는 주간 활성 사용자 200만 명을 돌파하며 연초 대비 4배 가까이 성장했으며, GPT-5.4는 하루 5조 토큰에 도달하고 연간 10억 달러의 순 신규 수익 실행률을 기록했습니다. 기업 출시를 위한 배포 부서도 구축 중입니다.
**[Google Gemini Embedding 2 공개 프리뷰]** — Google은 Gemini API와 Vertex AI를 통해 Gemini Embedding 2를 공개 프리뷰로 출시했습니다. 이는 텍스트, 이미지, 비디오, 오디오를 아우르는 100개 이상의 언어를 지원하는 단일 임베딩 공간을 제공합니다.
**[Microsoft GigaTIME 모델 오픈소스화]** — Microsoft는 5달러 병리 슬라이드에서 다중 면역형광 방식의 공간 단백질체학을 예측하는 GigaTIME 모델을 오픈소스화했습니다. 이 모델은 4천만 개 세포로 학습되었으며 대규모 암 면역 프로파일링을 민주화할 잠재력을 가집니다.

### 📊 모델 & 벤치마크
*   Google은 Gemini API 및 Vertex AI를 통해 텍스트, 이미지, 비디오, 오디오 전반에 걸쳐 100개 이상의 언어를 지원하는 단일 임베딩 공간인 Gemini Embedding 2를 공개 프리뷰로 출시했습니다.
*   Qwen 3.5 FP8 모델이 역설계되어 8× MI210에서 초당 6 토큰으로 실행되는 성능을 기록했습니다.
*   Mistral Small 4의 일부로 Leanstral이 공개되었습니다.
*   P-EAGLE 시스템은 Speculative Decoding의 순차적 병목 현상을 제거하여 B200에서 EAGLE-3 대비 최대 1.69배의 속도 향상을 보고했으며, vLLM v0.16.0에 통합되었습니다.

### 🛠️ 제품 & 도구
*   NVIDIA는 OpenClaw의 보안 문제를 해결하기 위한 솔루션으로 NemoClaw를 제시했습니다.
    ![Image](https://substack-post-media.s3.amazonaws.com/public/images/cfaddec2-3aea-4fbd-07158c2251d6_2048x945.jpeg)
*   OpenAI Codex는 다중 에이전트 코딩 워크플로우를 강화하기 위해 서브에이전트를 추가했습니다.
*   Andrew Ng는 API 문서용 오픈 CLI인 Context Hub / chub를 확장하여 에이전트 피드백 루프를 지원합니다.
*   AssemblyAI는 Claude Code, Codex, Cursor 등 에이전트가 최신 API 패턴을 사용할 수 있도록 유지 관리되는 스킬을 출시했습니다.
*   LangChain은 터미널 기반 배포/개발 흐름을 위한 LangGraph CLI를 출시했습니다.
*   Deep Agents는 최고의 코딩 에이전트 워크플로우를 MIT 라이선스로 재현하여 오픈소스화되었습니다.
*   Ollama는 OpenClaw의 공식 제공업체로 발표되었습니다.
*   Comet은 OpenClaw용 호출/도구/비용 추적을 위한 관측성 플러그인을 출시했습니다.
*   Perplexity는 Android용 Computer를 출시하여 로컬 브라우저를 도구로 사용하고 로컬 쿠키를 보존하며 사용자 작업 내용을 확인할 수 있도록 확장했습니다.
*   SeedFold는 확산 기반의 de novo 전원자 단백질 설계를 위한 SeedProteo를 출시했습니다.
*   NVIDIA는 실시간 레이 트레이싱 이후 가장 큰 그래픽 도약으로 포지셔닝되는 DLSS 5를 공개했습니다.

### 🔬 연구 & 논문
*   Moonshot은 고정 잔차 누적을 입력 의존적 어텐션으로 대체하고 Block AttnRes를 추가하여 1.25배 컴퓨팅 이점과 2% 미만 인퍼런스 레이턴시 오버헤드를 주장하는 Attention Residuals 논문을 발표했습니다.
*   dair_ai는 GitHub 리포지토리에서 에이전트 스킬을 표준화된 SKILL.md로 자동 추출하여 40%의 지식 전달 이득을 주장하는 논문을 강조했습니다.
*   Microsoft, Providence, UW의 연구는 5달러 병리 슬라이드에서 다중 면역형광 방식의 공간 단백질체학을 예측하는 GigaTIME 모델을 개발했으며, 이 모델은 오픈소스화되었습니다.
*   GoogleResearch는 고온 초전도 추론에 대한 LLM 평가 연구를 통해 큐레이션된 클로즈드 시스템 모델이 과학 작업에서 웹 중심 설정보다 우수하다고 주장했습니다.
*   AISecurityInst는 사이버 레인지에서 7개 프론티어 모델의 자율 공격 능력을 평가했습니다.
*   LeCun의 잠재 계획을 위한 Temporal Straightening 연구는 잠재 궤적을 곧게 펴서 유클리드 거리가 도달 가능한 진행 상황을 더 잘 추적하도록 함으로써 계획 안정성을 향상시킵니다.

### 💰 산업 동향
*   NVIDIA는 GTC 2026에서 2027년까지 1조 달러의 판매 잔고를 발표했습니다.
*   OpenAI Codex는 주간 활성 사용자 200만 명 이상을 기록하며 연초 대비 거의 4배 증가했으며, GPT-5.4는 순 신규 수익에서 연간 10억 달러의 실행률을 기록했습니다.

### ⚡ 인프라 & 하드웨어
*   NVIDIA는 GTC 2026에서 새로운 CPU인 Vera를 공개했습니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/3c9e5d8d-2b90-4c27-ab1c-fd67c035acb4_3592x1886.png)
*   NVIDIA는 실시간 레이 트레이싱 이후 가장 큰 그래픽 도약으로 포지셔닝되는 DLSS 5를 공개했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
