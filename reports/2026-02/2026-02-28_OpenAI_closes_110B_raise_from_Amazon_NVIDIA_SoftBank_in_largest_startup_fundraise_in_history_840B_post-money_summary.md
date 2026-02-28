# OpenAI closes $110B raise from Amazon, NVIDIA, SoftBank in largest startup fundraise in history @ $840B post-money - 요약

**원문 URL**: https://www.latent.space/p/ainews-openai-closes-110b-raise-from
**번역일**: 2026-02-28 13:28
**발행일**: 2026-02-28

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 핵심 AI 뉴스 브리핑입니다.

### 🔥 주요 뉴스
**[OpenAI, 1,100억 달러 투자 유치 및 8,400억 달러 기업 가치 달성]** — OpenAI가 Amazon, NVIDIA, SoftBank로부터 총 1,100억 달러의 투자를 유치하며 8,400억 달러의 포스트머니 기업 가치를 기록했습니다. 이 투자는 인프라 확장에 사용될 예정이며, NVIDIA는 3GW의 인퍼런스 및 2GW의 학습 용량을, Amazon은 AWS를 OpenAI Frontier2의 독점 클라우드 제공업체로 지정하고 8년간 2GW의 Trainium 용량을 제공할 예정입니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/5dd10ca4-c51f-4905-acbf-c1bc803b5ca7_890x600.png)

**[Anthropic, 미국 국방부의 '공급망 위험' 지정에 반발]** — Anthropic이 대규모 국내 감시 및 완전 자율 무기 활성화에 대한 공개적인 거부 입장을 표명하자, 미국 국방부는 Anthropic을 "국가 안보에 대한 공급망 위험"으로 지정했습니다. Anthropic은 이 지정에 대해 법정에서 이의를 제기할 것이라고 밝혔으며, 이는 AI 거버넌스 및 계약 범위에 대한 중요한 선례를 남길 것으로 예상됩니다.

**[Sakana AI, Doc-to-LoRA 및 Text-to-LoRA 기술 공개]** — Sakana AI가 단일 포워드 패스에서 LoRA 어댑터를 생성하는 하이퍼네트워크 기반의 Doc-to-LoRA 및 Text-to-LoRA 방법을 발표했습니다. 이 기술은 파인튜닝/디스틸레이션/긴 컨텍스트 프롬프팅을 "즉각적인 가중치 업데이트"로 전환하여, 긴 컨텍스트 윈도우보다 약 5배 긴 시퀀스에서 거의 완벽한 정확도를 보고합니다.

### 📊 모델 & 벤치마크
*   Alibaba가 Apache 2.0 라이선스의 Qwen3.5 모델군(27B 밀집형, 122B A10B MoE, 35B A3B MoE)을 출시했으며, 모두 262K 컨텍스트를 지원하고 YaRN을 통해 1M까지 확장 가능합니다.
*   Arena 리더보드(2026년 2월)에서 텍스트 부문은 GLM-5, Qwen-3.5 397B A17B, Kimi-K2.5 Thinking이 상위권을 차지했으며, 코드 부문은 GLM-5가 1위, Kimi-K2.5와 MiniMax-M2.5가 공동 2위를 기록했습니다.
*   Perplexity가 리트리벌 성능 향상을 위해 양방향 "Qwen3-재학습" 임베딩 모델(0.6B/4B)을 MIT 라이선스로 오픈소스화했습니다.

### 🛠️ 제품 & 도구
*   OpenAI가 배포 안전 문서("시스템 카드")에 대한 접근성을 높이기 위해 검색 가능한 "Deployment Safety Hub" 웹사이트를 출시했습니다.
*   Arena가 재현 가능한 리더보드를 위한 오픈소스 랭킹 패키지인 Arena-Rank를 공개했습니다.

### 🔬 연구 & 논문
*   DeepSeek, THU, PKU 연구진이 RDMA를 통해 디코드 노드의 유휴 스토리지 NIC 대역폭을 활용하는 Prefill/Decode의 시스템 수준 재설계를 제안하는 DualPath I/O 논문을 발표했습니다.
*   Databricks MosaicAI가 엄격한 온-폴리시 루프보다 운영상 간단하며 GRPO와 유사하거나 더 나은 성능을 3배 적은 학습 세대로 달성하는 오프-폴리시 RL 대안인 OAPL(Optimal Advantage-based Policy Optimization with Lagged Inference Policies)을 소개했습니다.
*   경험적 강화 학습(ERL)이 에피소드 내 반성/재시도 및 디스틸레이션을 삽입하여 Sokoban에서 81%의 성능 향상을 보고했으나, 파이프라인 복잡성 및 연산 트레이드오프가 존재한다고 분석되었습니다.
*   Albert Gu가 Mamba-2의 일부 결과에 실질적인 영향을 미친 초기화 버그가 있었음을 명확히 했습니다.

### 💰 산업 동향
*   OpenAI의 1,100억 달러 투자 유치에는 SoftBank 300억 달러, NVIDIA 300억 달러, Amazon 500억 달러가 포함되었으며, 이는 OpenAI의 인프라 확장 및 ASI 전략 발전에 기여할 것입니다.
*   미국 국방부가 Anthropic을 "국가 안보에 대한 공급망 위험"으로 지정한 사건은 AI 모델 배포의 윤리적 경계, 거버넌스 선례, 그리고 계약업체에 대한 정부의 영향력에 대한 논쟁을 촉발했습니다.

### ⚡ 인프라 & 하드웨어
*   vLLM이 ROCm용 7가지 어텐션 백엔드를 발표하며 AMD GPU에서 최대 4.4배의 디코드 처리량 향상을 보고했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
