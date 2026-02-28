# OpenAI closes $110B raise from Amazon, NVIDIA, SoftBank in largest startup fundraise in history @ $840B post-money - 요약

**원문 URL**: https://www.latent.space/p/ainews-openai-closes-110b-raise-from
**번역일**: 2026-02-28 11:59
**발행일**: 2026-02-28

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 뉴스 브리핑입니다.

### 🔥 주요 뉴스
*   **[OpenAI, 1,100억 달러 투자 유치]** — OpenAI가 Amazon, NVIDIA, SoftBank로부터 총 1,100억 달러의 투자를 유치하며 8,400억 달러의 사후 가치를 기록했습니다. 이는 인프라 확장 및 AI 대중화를 위한 자금으로 활용될 예정이며, NVIDIA는 3 GW의 인퍼런스 및 2 GW의 학습 용량을, Amazon은 AWS를 통한 독점 클라우드 제공 및 Trainium 용량을 약속했습니다.
*   **[Anthropic, 미 국방부와의 갈등]** — Anthropic이 대규모 국내 감시 및 완전 자율 무기 활성화를 거부하자, 미 국방부로부터 "국가 안보 공급망 위험"으로 지정될 수 있다는 주장이 제기되었습니다. Anthropic은 공식 성명을 통해 법적 대응 의사를 밝히며, 국방부 계약 범위를 벗어난 고객 제한에 이의를 제기할 것이라고 강조했습니다.
*   **[Sakana AI, 즉각적인 LoRA 어댑터 생성 기술 공개]** — Sakana AI는 하이퍼네트워크를 활용하여 단일 포워드 패스에서 LoRA 어댑터를 생성하는 Doc-to-LoRA 및 Text-to-LoRA 방법을 발표했습니다. 이 기술은 파인튜닝/디스틸레이션 작업을 즉각적인 가중치 업데이트로 전환하여 빠른 적응과 "영구 메모리" 기능을 가능하게 합니다.

### 📊 모델 & 벤치마크
*   **Alibaba, Qwen3.5 시리즈 출시:** 27B 덴스, 122B A10B MoE, 35B A3B MoE 모델을 Apache 2.0 라이선스로 공개했으며, 262K 컨텍스트를 지원하고 YaRN을 통해 1M까지 확장 가능합니다. Artificial Analysis는 27B 모델의 인텔리전스 인덱스 점수를 42로 보고했습니다.
*   **Arena 리더보드 업데이트:** 2026년 2월 기준 텍스트 부문 상위 모델은 GLM-5 (1455), Qwen-3.5 397B A17B (1454), Kimi-K2.5 Thinking (1452)이며, 코드 부문 1위는 GLM-5 (1451)입니다. Arena는 재현 가능한 리더보드를 위한 오픈소스 랭킹 패키지인 Arena-Rank를 강조했습니다.
*   **Perplexity, 양방향 임베딩 모델 오픈소스화:** Perplexity는 리트리벌 성능 향상을 위해 양방향 "Qwen3 재학습" 임베딩 모델(0.6B/4B)을 MIT 라이선스로 오픈소스화했다고 알려졌습니다.

### 🛠️ 제품 & 도구
*   **OpenAI, Deployment Safety Hub 출시:** 배포 안전 문서인 "시스템 카드"를 검색할 수 있는 웹사이트를 출시하여 배포 안전 문서에 대한 접근성을 높였습니다.
*   **vLLM, ROCm 어텐션 백엔드 출시:** vLLM은 AMD GPU용 7가지 어텐션 백엔드를 발표했으며, 환경 변수 스위치를 통해 AMD GPU에서 최대 4.4배의 디코딩 처리량 개선을 보고했습니다.

### 🔬 연구 & 논문
*   **Sakana AI, Doc-to-LoRA 및 Text-to-LoRA:** 하이퍼네트워크를 사용하여 작업 설명이나 긴 문서를 1초 미만의 레이턴시로 어댑터 가중치로 컴파일하는 방법을 제시했습니다. Doc-to-LoRA는 기본 모델 컨텍스트 윈도우보다 약 5배 긴 시퀀스에서 거의 완벽한 정확도를 보고합니다.
*   **DeepSeek DualPath I/O 논문:** DeepSeek, THU, PKU 연구진이 RDMA를 통해 디코드 노드의 유휴 스토리지 NIC 대역폭을 활용하는 Prefill/Decode의 시스템 수준 재설계를 제안했습니다. 이는 에이전틱 긴 컨텍스트 인퍼런스를 위한 KV-cache 이동 병목 현상을 목표로 하며, DS-660B에서 1.87배의 속도 향상을 주장합니다.
*   **Databricks MosaicAI, 오프-폴리시 RL OAPL 공개:** OAPL(Optimal Advantage-based Policy Optimization with lagged inference policy)을 GRPO와 동등하거나 능가하며 약 3배 적은 학습 세대를 사용하는 안정적인 오프-폴리시 대안으로 소개했습니다.
*   **Experiential Reinforcement Learning (ERL) 개념 제시:** 표준 RLVR과 달리 에피소드 내 성찰/재시도 및 디스틸레이션을 삽입하는 ERL이 소개되었으며, Sokoban에서 81%의 성능 향상을 보고했습니다.

### 💰 산업 동향
*   **OpenAI, 1,100억 달러 투자 유치 세부 사항:** SoftBank 300억 달러, NVIDIA 300억 달러, Amazon 500억 달러(초기 150억 달러, 조건 충족 시 350억 달러 추가)를 투자했습니다.
*   **NVIDIA, OpenAI에 3 GW 인퍼런스 및 2 GW 학습 용량 제공:** NVIDIA는 OpenAI에 3 GW의 전용 인퍼런스 용량과 Vera Rubin 시스템에서의 2 GW 학습 사용을 포함한 투자를 진행했습니다.
*   **Amazon, OpenAI와의 파트너십 강화:** Amazon Bedrock에서 OpenAI가 구동하는 "Stateful Runtime Environment"를 제공하고, AWS가 OpenAI Frontier를 위한 독점적인 서드파티 클라우드 제공업체가 됩니다. 또한 AWS 인프라를 통해 Trainium3 및 차세대 Trainium4 칩을 포함한 기가와트 규모의 Trainium 용량(8년간 1,000억 달러 가치)을 제공합니다.
*   **Anthropic, 미 국방부의 "공급망 위험" 지정에 법적 대응 시사:** Anthropic은 미 국방부 장관의 발언에 대한 공식 성명을 통해, 국방부 계약 범위를 벗어난 고객을 제한하는 것에 대한 분쟁 및 모든 공급망 위험 지정에 법정에서 이의를 제기할 것이라고 밝혔습니다.


---

## 📷 이미지

![Image](https://substackcdn.com/image/fetch/$s_!fhcB!,w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F5dd10ca4-c51f-4905-acbf-c1bc803b5ca7_890x600.png)

![Image](https://substackcdn.com/image/fetch/$s_!ax2C!,w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F89dd9766-2fb1-4d42-86f2-6afd1fdfa06d_1206x1401.webp)

![Image](https://substackcdn.com/image/fetch/$s_!YaNo!,w_5760,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Ff262d5b1-7a48-45f4-ae8c-b2646931577f_2910x514.png)

![Image](https://substackcdn.com/image/fetch/$s_!Xhe0!,w_2400,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F5e25815d-e755-44e5-b77b-81fb495c7821_2564x2006.png)

![Image](https://substackcdn.com/image/fetch/$s_!Iqub!,w_2400,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F93ed2a68-ee2f-4599-b965-d993d697115b_2590x2038.png)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
