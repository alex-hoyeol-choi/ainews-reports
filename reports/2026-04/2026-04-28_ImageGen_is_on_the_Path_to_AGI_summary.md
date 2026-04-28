# ImageGen is on the Path to AGI - 요약

**원문 URL**: https://www.latent.space/p/ainews-imagegen-is-on-the-path-to
**번역일**: 2026-04-28 06:18
**발행일**: 2026-04-28

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 브리핑입니다.

### 🔥 주요 뉴스
**[OpenAI, Azure 독점 계약 완화]** — OpenAI는 Microsoft와의 파트너십을 업데이트하여, Microsoft가 주요 클라우드 파트너로 남지만 OpenAI 제품을 모든 클라우드에서 사용할 수 있게 되었습니다. AWS는 OpenAI 모델이 몇 주 내에 Bedrock에 출시될 예정임을 확인했습니다.
**[GitHub Copilot, 사용량 기반 요금제로 전환]** — GitHub는 6월 1일부터 Copilot 요금제를 사용량 기반으로 변경한다고 발표했습니다. 이는 에이전틱 워크플로우의 런타임 소비 증가를 반영하는 중요한 변화입니다.
**[Xiaomi MiMo-V2.5 모델 오픈소스 출시]** — Xiaomi는 1M 토큰 컨텍스트를 지원하는 MiMo-V2.5-Pro와 MiMo-V2.5를 MIT 라이선스로 오픈소스화했습니다. Pro 모델은 복잡한 에이전트/코딩에, 더 작은 모델은 네이티브 옴니모달 에이전트에 특화되어 있습니다.
**[Google, TPU v8을 학습 및 인퍼런스 전용으로 분할]** — Google Cloud Next에서 TPU v8이 학습용 8t와 인퍼런스용 8i로 분할되었다고 발표했습니다. 이는 이전 세대 대비 2.8배 빠른 학습과 80% 향상된 인퍼런스 성능/달러를 제공합니다.

### 📊 모델 & 벤치마크
*   **GPT-5.5 벤치마크 결과:** GPT-5.5 노-씽킹은 WeirdML에서 67.1%를 기록하여 GPT-5.4의 57.4%에서 상승했으나, Opus 4.7의 76.4%에는 미치지 못했습니다. LMSYS Arena에서는 Code Arena 9위, Math 3위, Search 2위 등을 기록했습니다.
*   **Xiaomi MiMo-V2.5 모델 상세:** MiMo-V2.5-Pro는 총 1T / 활성 42B 파라미터로 FP8로 27T 토큰에 대해 학습되었으며, MiMo-V2.5는 총 310B / 활성 15B 파라미터로 48T 토큰에 대해 학습되었습니다.
*   **Kimi K2.6 리더보드 1위:** Kimi K2.6이 OpenRouter 주간 리더보드에서 현재 1위를 차지했습니다.
*   **Sakana Conductor 성능:** SakanaAILabs의 7B Conductor는 LiveCodeBench에서 83.9%, GPQA-Diamond에서 87.5%를 달성하여, 단일 워커 모델보다 뛰어난 성능을 보였습니다.
*   **AgentIR-4B 벤치마크:** AgentIR-4B는 BrowseComp-Plus에서 68%를 달성하여, 기존 대형 임베딩 모델의 52%를 능가했습니다.

### 🛠️ 제품 & 도구
*   **OpenAI Symphony 오픈소스화:** OpenAI는 이슈 트래커를 Codex 에이전트에 연결하여 "이슈 열기 → 에이전트 → PR → 사람 검토" 워크플로우를 위한 오케스트레이션 레이어인 Symphony를 오픈소스화했습니다.
*   **Google Gemma 로컬 브라우저 에이전트 시연:** Google Gemma 팀은 Gemma 4 + WebGPU를 사용하여 브라우징 기록, 탭 관리, 페이지 요약을 위한 네이티브 툴 호출 기능을 갖춘 완전 로컬 브라우저 에이전트를 시연했습니다.
*   **Cognition Devin for Terminal 출시:** Cognition은 나중에 클라우드로 핸드오프할 수 있는 로컬 셸 에이전트인 Devin for Terminal을 출시했습니다.
*   **Future AGI 평가/최적화 스택 오픈소스화:** Future AGI는 자체 개선 에이전트를 위한 평가 및 최적화 스택을 오픈소스화했습니다.
*   **LlamaIndex ParseBench 출시:** LlamaIndex의 ParseBench는 파싱 에이전트를 위한 2천 개의 검증된 엔터프라이즈 문서 페이지를 추가했습니다.

### 🔬 연구 & 논문
*   **Sakana Conductor 연구:** SakanaAILabs는 작업을 직접 해결하기보다 자연어로 프론티어 모델 풀을 오케스트레이션하기 위해 RL로 학습된 7B Conductor를 소개했습니다.
*   **코딩 에이전트 지출 연구:** SWE-bench Verified에 대한 새로운 연구는 에이전틱 코딩이 채팅/코드 추론보다 약 1000배 더 많은 토큰을 소비할 수 있으며, 더 많은 지출이 항상 정확도를 개선하지는 않는다는 점을 강조했습니다.
*   **AgentIR 연구:** AgentIR은 쿼리와 함께 추론 트레이스를 임베딩하여 연구 에이전트를 위한 리트리벌을 재구성하는 새로운 접근 방식을 제시했습니다.

### 💰 산업 동향
*   **OpenAI-Microsoft 파트너십 업데이트:** OpenAI는 Microsoft와의 파트너십을 업데이트하여, Microsoft가 주요 클라우드 파트너로 남지만 OpenAI 제품을 모든 클라우드에서 사용할 수 있게 되었습니다. 제품/모델 약정은 2032년까지, 수익 공유는 2030년까지 연장됩니다.
*   **AWS Bedrock에 OpenAI 모델 출시 예정:** AWS의 @ajassy는 OpenAI 모델이 몇 주 내에 AWS Bedrock에 출시될 예정임을 확인했습니다.
*   **GitHub Copilot 요금제 변경:** GitHub는 6월 1일부터 Copilot 요금제를 사용량 기반으로 전환한다고 발표했습니다.
*   **Codex 사용량 승수 문서화:** OpenAI는 GPT-5.4 fast는 2배, GPT-5.5 fast는 2.5배의 Codex 사용량 승수를 문서화했습니다.

### ⚡ 인프라 & 하드웨어
*   **Google TPU v8 학습/인퍼런스 분할:** Google Cloud Next에서 TPU v8이 학습용 8t와 인퍼런스용 8i로 분할되었다고 발표했습니다. 이는 이전 세대 대비 2.8배 빠른 학습과 80% 향상된 인퍼런스 성능/달러를 제공합니다.
*   **vLLM DeepSeek V4 지원:** vLLM_project는 DeepSeek V4 기본 모델에 대한 지원을 추가할 예정이며, vLLM 0.20.0 릴리스에는 DeepSeek V4 지원, FA4, TurboQuant 2비트 KV 등이 포함됩니다.
*   **FP8 KV-캐시 최적화 개선:** vLLM_project와 Red Hat/AWS는 FA3 2단계 누적 수정으로 FP8 KV-캐시 심층 분석에서 128k needle-in-a-haystack 성능이 13%에서 89%로 개선되었다고 발표했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
