# GPT 5.4: SOTA Knowledge Work -and- Coding -and- CUA Model, OpenAI is so very back - 요약

**원문 URL**: https://www.latent.space/p/ainews-gpt-54-sota-knowledge-work
**번역일**: 2026-03-06 07:30
**발행일**: 2026-03-06

---

### 🔥 주요 뉴스

**[OpenAI, GPT-5.4 및 GPT-5.4 Pro 출시]** — OpenAI가 ChatGPT, API, Codex 전반에 걸쳐 GPT-5.4 및 GPT-5.4 Pro를 출시했습니다. 이 모델은 코딩 및 비코딩 기능을 통합한 최초의 GPT-5.x 모델이며, 네이티브 컴퓨터 사용(CUA) 기능과 향상된 효율성을 제공합니다. OSWorld-Verified 벤치마크에서 인간 기준선 72.4%를 능가하는 75.0%를 기록했습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/113080da-9b51-4b0c-b605-3f848d44e69c_1230x956.png)

**[FlashAttention-4 발표 및 PyTorch 채택]** — FlashAttention-4(FA4) 논문이 공개되었으며, Blackwell GPU에서 행렬 곱셈 속도에 가까운 어텐션 처리량을 달성합니다. PyTorch는 FlexAttention에 FA4 백엔드를 추가하여 연산 바운드 워크로드에서 Triton 대비 1.2배~3.2배의 속도 향상을 주장했습니다.

**[AI2, OLMo Hybrid 모델 출시]** — Allen AI가 트랜스포머 어텐션과 선형 RNN 스타일 레이어(Gated DeltaNet)를 혼합한 7B 파라미터의 완전 오픈 모델 패밀리인 OLMo Hybrid를 공개했습니다. 이 모델은 OLMo 3 7B 대비 평가 전반에 걸쳐 강력한 개선을 주장하며, 3조 토큰으로 학습되었습니다.

**[Databricks, 강화 학습 기반 지식 에이전트 KARL 발표]** — Databricks가 다단계 리트리벌, 교차 참조, 긴 도구 궤적을 포함하는 엔터프라이즈 워크플로우를 위한 강화 학습(RL) 기반 에이전트 KARL을 발표했습니다. RL을 통해 보지 못한 프롬프트로 전이되며, 멀티태스크 RL은 일반화되어 다중 전문가 디스틸레이션을 능가할 수 있다고 주장합니다.

**[Claude Opus 4.6, 도널드 크누스 추측 해결 및 투자 추천 성과]** — Anthropic의 Claude Opus 4.6이 저명한 컴퓨터 과학자 도널드 크누스의 오랜 추측을 해결하여 AI의 자동 연역 및 창의적 문제 해결 역량을 입증했습니다. 또한, Reddit 투자 추천을 평가한 실험에서 S&P 500의 +19% 대비 +37%의 수익률을 기록하며 고품질 분석 필터링 능력을 보여주었습니다.

### 📊 모델 & 벤치마크

*   **GPT-5.4 벤치마크 결과:** GPT-5.4 Thinking은 OSWorld-Verified에서 75.0%(인간 기준선 72.4% 상회), GDPval에서 83%, BrowseComp에서 82.7%를 달성했습니다. GPT-5.4 Pro는 FrontierMath Tier 1-3에서 50%, Tier 4에서 38%로 신기록을 세웠습니다. SWE-Bench Pro에서는 57.7%를 기록했습니다.
*   **Qwen3.5 Unsloth GGUF 업데이트:** Unsloth가 Qwen3.5의 최종 GGUF 업데이트를 배포했습니다. 새로운 iMatrix 캘리브레이션 데이터셋을 사용하고 양자화 개선을 통해 특정 모델의 최대 KLD를 최대 51%까지 줄였습니다. Qwen3.5-35BA3 모델은 모든 Qwen3 모델을 능가하는 예외적인 속도를 보였습니다.
*   **Microsoft Phi-4 멀티모달 모델 출시:** Microsoft가 추론 및 비전에 최적화된 15B 파라미터 멀티모달 모델 Phi-4를 출시했습니다.

### 🛠️ 제품 & 도구

*   **OpenAI GPT-5.4 통합:** GPT-5.4는 ChatGPT, API, Codex 전반에 걸쳐 출시되었으며, Cursor, Perplexity, Windsurf 등 다양한 플랫폼에 즉시 통합되었습니다.
*   **Cursor Automations 출시:** Cursor가 CI 실패, PR, 인시던트, 슬랙 메시지 등 이벤트/웹훅으로 시작되는 상시 에이전트인 Cursor Automations를 도입했습니다.
*   **Hugging Face Hub "Buckets" 추가:** Hugging Face가 허브에 S3와 유사한 객체 스토리지인 Buckets를 발표했습니다. 이는 깃 히스토리 없이 청크 중복 제거 동기화 기능을 제공하며 체크포인트와 같은 대규모 아티팩트를 대상으로 합니다.
*   **W&B 개선된 트레이스 비교:** Weights & Biases가 디버깅을 위한 개선된 트레이스 비교 기능(요약, 점수 차이, 사용량 분석, 호출 드릴다운)을 출시했습니다.
*   **LlamaIndex DBOS 통합:** LlamaIndex가 DBOS와의 통합을 통해 워크플로우가 충돌/재시작에도 살아남을 수 있도록 자동 지속성 및 재개 기능을 강조했습니다.

### 🔬 연구 & 논문

*   **FlashAttention-4 논문 및 구현:** FA4는 알고리즘 및 파이프라인 변경(다항식 지수 에뮬레이션, 온라인 소프트맥스, 2CTA MMA)을 통해 Blackwell에서 행렬 곱셈 속도에 가까운 어텐션 처리량을 달성합니다.
*   **LLM 장문 컨텍스트 신뢰성 저하 연구:** OpenAI 자체 MRCR v2 연구에 따르면, LLM의 "건초 더미 속 바늘" 스타일 결과는 컨텍스트가 증가함에 따라 저하됩니다. 16-32K 토큰에서 약 97%였던 정확도는 512K-1M 토큰에서 36%로 하락했습니다.
*   **KV-캐시 압축 연구:** Baseten은 장기 실행 에이전트를 위한 반복적인 KV 압축("Attention Matching") 연구를 요약했습니다. 원샷 압축은 2-5배 압축률에서 65-80% 정확도를 유지합니다.
*   **지속 학습 및 메모리 도구 연구:** Awni Hannun은 프롬프트 압축 및 재귀적 서브 에이전트가 효과적이라고 논의하며 메모리 기반 보존/제거 정책을 주장했습니다. Karpathy는 메모리 작업을 도구로 취급하고 RL을 통해 최적화할 것을 제안했습니다.
*   **Lunaris MoC 아키텍처:** Lunaris MoC는 "Mixture-of-Collaboration"을 도입하여 표준 MoE 대비 40% 연산 절감 및 낮은 퍼플렉시티(59.97 대 62.89)를 달성했습니다.
*   **CoT Controllability 연구 논문:** GPT-5.4와 관련하여 모델이 자신의 추론 체인을 모호하게 하는 능력이 낮아 모니터링이 실행 가능한 안전 도구가 된다는 연구 결과가 발표되었습니다.

### 💰 산업 동향

*   **Alibaba CEO, Qwen 오픈소스 유지 약속:** 알리바바 CEO 에디 우(Eddie Wu)는 Qwen 모델에 대한 회사의 오픈소스 전략을 유지하고 파운데이션 대규모 모델 개발 및 AI R&D 투자를 늘릴 것이라고 확인했습니다.
*   **Anthropic 대 OpenAI 안전 논쟁:** 유출된 메모(다리오 아모데이(Dario Amodei)의 것으로 알려짐)는 샘 알트만(Sam Altman)이 정부의 환심을 사고 Anthropic을 대체하기 위해 "안전 연극"에 참여했다고 비난했습니다.
*   **Google Gemini 부당 사망 소송:** Google은 Gemini가 사용자에게 실제 주소를 환각했고, 사용자가 이를 행동으로 옮겨 "부당 사망" 시나리오에 기여한 후 법적 조치에 직면했습니다.

### ⚡ 인프라 & 하드웨어

*   **llama.cpp GGUF NVFP4 지원:** llama.cpp 프로젝트의 풀 리퀘스트 #19769는 GGUF 형식에서 NVIDIA의 NVFP4 양자화 형식에 대한 초기 CPU 지원을 도입하여 최대 2.3배의 속도 향상과 30-70%의 크기 감소를 약속합니다.
*   **Blackwell B60 초기 성능 문제:** NVIDIA B60의 LM Scaler에 대한 초기 보고서는 vLLM에서 누락된 토큰 보고로 인한 성능 문제 및 디버깅 난제를 나타냈습니다.
*   **NVLink XID 오류 모니터링 권고:** GPU 전문가들은 dmesg에서 급증하는 XID 오류 카운터를 모니터링할 것을 권고합니다. 이는 NVLink 버스에서 자체 수정 비트 오류를 나타내며, 치명적인 실패 전 물리적 하드웨어 성능 저하를 식별하는 데 중요합니다.
*   **커스텀 서빙 엔진 CPU 오버헤드 문제:** 커스텀 서빙 엔진을 구축하는 개발자들은 float32에서 bfloat16으로 정밀도를 전환해도 지속되는 높은 CPU 오버헤드 병목 현상에 직면하고 있습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
