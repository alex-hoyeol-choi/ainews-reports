# DeepSeek DeepInfer: Open Source SOTA Inference running 155T toks/day/cluster making $22m/day at ~80% margin for a 81 day payback - 요약

**원문 URL**: https://www.latent.space/p/ainews-deepseek-deepinfer-open-source
**번역일**: 2026-10-21 12:38
**발행일**: 2026-10-21

---

### 🔥 주요 뉴스
*   **[DeepSeek, 프로덕션 인퍼런스 스택 DeepInfer 오픈소스화]** — DeepSeek이 최대 72시간 프롬프트 캐싱을 지원하는 프로덕션 인퍼런스 스택 DeepInfer를 오픈소스화했습니다. 이는 클러스터당 하루 155조 토큰 처리가 가능하며, 비피크 시간 기준 카드당 시간당 38달러의 수익과 80% 이상의 인퍼런스 마진을 주장합니다.
    ![X avatar for @deepseek_ai](https://pbs.substack.com/profile_images/1717417613775757312/Uk1zNOj4.jpg)
    ![](https://substack-post-media.s3.amazonaws.com/public/images/07a949cd-f727-48e2-9bd4-c4d110bf94e9_1326x1362.png)
    ![](https://substack-post-media.s3.amazonaws.com/public/images/32f1a4cb-f50f-4454-8a1b-96ffe57e72cb_680x640.png)
    ![](https://substack-post-media.s3.amazonaws.com/public/images/f8f12827-473f-94d0-41618bd7c311_1142x622.png)
*   **[OpenAI, 신약 개발 플랫폼 Orchestra Bio 인수]** — OpenAI가 신약 개발 조정 플랫폼인 Orchestra Bio를 인수하며, 생명 과학 분야에서 연구 도구를 넘어 운영 실행으로 사업을 확장했습니다. 구체적인 인수 조건은 공개되지 않았습니다.
*   **[전 OpenAI 연구 책임자, 제조 소프트웨어 기업 Arda 출시 및 대규모 자금 조달]** — 전 OpenAI 연구 책임자 Bob McGrew가 제조 소프트웨어 기업 Arda를 출시하고 Anduril을 설계 파트너로 하여 1.5B 달러 가치로 160M 달러 규모의 Series A 투자를 유치했습니다. 초기 제품은 수동 조립 라인 설계 및 운영을 지원합니다.

### 📊 모델 & 벤치마크
*   **DeepSeek V4.1 Flash, 오픈 모델 벤치마크 1위 및 사이버 보안 성능 입증** — DeepSeek V4.1 Flash 20261017 Max가 Agent Arena 및 Code Arena: WebDev에서 오픈 모델 중 1위를 차지했으며, 시뮬레이션된 기업 네트워크 작업에서 GPT-6 Sol의 평균 진행률을 능가했습니다.
*   **Meta, 30B 멀티모달 에이전트 모델 Muse Glimmer 공개** — Meta가 Muse Spark에서 증류된 오픈 30B 멀티모달 에이전트 모델 Muse Glimmer를 출시했으며, 32GB VRAM을 목표로 RTX 5090에서 4비트 양자화 및 스페큘레이티브 디코딩 헤드를 사용하여 실행됩니다.
*   **Mistral, 음성 에이전트 SDK Voxtral 3 출시 및 성능 공개** — Mistral이 배치 및 스트리밍 트랜스크립션, 다국어 TTS, 도구 호출 기능을 갖춘 음성 에이전트 SDK Voxtral 3를 출시했으며, Artificial Analysis 평가에서 Small Transcribe 3가 2.1% AA-WER로 3위를 기록했습니다.
*   **Kyutai, CPU 기반 소형 TTS 모델 Pocket TTS 출시** — Kyutai가 최대 1.9M 파라미터의 소형 Pocket TTS 변형을 출시했으며, 음성 복제 기능을 포함하여 하나의 CPU 코어에서 103배 실시간 성능을 주장합니다.
*   **Bria, 8B 오픈 웨이트 이미지 제품군 Fibo 2.0 출시** — Bria가 텍스트-투-이미지용 Dev와 증류된 Edit Turbo를 포함하는 8B 오픈 웨이트 이미지 제품군 Fibo 2.0을 출시했으며, Artificial Analysis는 선도적인 오픈 웨이트 편집 성능을 보고했습니다.
*   **Krea 3 Ultra, 경쟁력 있는 이미지 편집 품질 입증** — Krea 3 Ultra가 Arena 평가에서 다중 이미지 편집 4위, 단일 이미지 편집 8위를 기록하는 등 경쟁력 있는 이미지 편집 품질을 보여주었습니다.
*   **Artificial Analysis, HealthBench 리더보드 출시** — Artificial Analysis가 5,000개의 일반 건강 대화와 525개의 임상의 대화에 대한 HealthBench 리더보드를 출시했으며, GPT-6 Astra가 Professional 부문에서 66.0%로 선두를 달리고 Claude Sonnet 5.5가 일반 HealthBench에서 62.1%로 선두를 달립니다.
*   **Decider V1.2, 금융 문서 분류 벤치마크 ClaimBench에서 높은 정확도 달성** — Decider V1.2가 금융 문서 분류 벤치마크 ClaimBench에서 99.9%의 정확도를 달성했으며, 1,000개 청구당 0.11달러의 비용으로 99.7%를 자체 처리했습니다.

### 🛠️ 제품 & 도구
*   **DeepSeek DeepInfer, API 호환성 및 스페큘레이티브 디코딩 최적화** — DeepInfer는 Chat Completions, Messages, Responses API를 지원하는 deepseek-recipe 컴포넌트를 포함하며, DSpark를 통해 스페큘레이티브 디코딩을 적응적으로 최적화하여 프로덕션 처리량을 6% 향상시켰습니다.
*   **Perplexity Computer, Apple Silicon Mac에서 오프라인 실행 지원** — Perplexity Computer가 이제 지원되는 Apple Silicon Mac에서 오프라인으로 완전히 실행될 수 있으며, PPLX Pro 모델을 사용하여 로컬 앱 및 파일과 상호작용합니다.
*   **LangChain, Managed Deep Agents 출시** — LangChain이 사용자별 자격 증명, 범위 지정 메모리, 샌드박스 실행 및 예약된 작업을 패키징하는 Managed Deep Agents를 출시했습니다.
*   **Hugging Face, Agent Manager 출시** — Hugging Face가 Claude Code, Codex 및 기타 하네스 전반에 걸쳐 영구 세션을 오케스트레이션하는 Agent Manager를 출시했습니다.
*   **OpenAI, 12시간 API 프롬프트 캐싱 기능 추가** — OpenAI가 API에 12시간 프롬프트 캐싱 기능을 추가했으며, 이는 기본 30분 캐싱과 혼합하여 사용할 수 있고, 더 긴 보존 기간은 추가 비용이 발생합니다.
*   **OpenAI, 사용량 제한 불일치 문제 해결 및 크레딧 약속** — OpenAI가 약 40,000개 계정에서 발생한 사용량 제한 불일치 문제를 식별하고 수정했으며, 영향을 받은 사용자에게 크레딧을 제공할 예정입니다.

### 🔬 연구 & 논문
*   **Anthropic, 전갈 독소 바인더 17개 발견** — Anthropic과 Citrini가 내부 Claude 연구 모델을 사용하여 211개 단백질 설계 중 17개의 전갈 독소 바인더를 발견했으며, 모든 테스트 설계 및 실험실 데이터가 공개될 예정입니다.
*   **Sophont, 병리 슬라이드에서 공간 유전자 활동 예측 모델 Holon-S1 공개** — Sophont가 일상적인 병리 슬라이드에서 공간 유전자 활동 및 바이오마커를 예측하는 Holon-S1을 소개했으며, 잠재적으로 새로운 유방암 및 대장암 바이오마커를 식별했습니다.
*   **METR, Anthropic 모델의 안전성 평가 및 권고** — METR이 Anthropic의 대상 모델에 대한 낮은 치명적 정렬 불량 위험 결론에 동의하면서도 상당한 분석적 불일치를 식별하고, 모니터링 시스템의 엔드-투-엔드 레드팀을 권장했습니다.

### 💰 산업 동향
*   **OpenAI, 약 1.4조 달러 가치로 300억 달러 자금 조달 추진 보도** — OpenAI가 예상되는 Anthropic IPO에 앞서 약 1.4조 달러 이상의 가치로 약 300억 달러의 자금 조달을 모색하고 있다는 보도가 나왔습니다.
*   **Anthropic, 상반기 163억 달러 매출 및 6천억 달러 이상 컴퓨팅 약정 보도** — Anthropic의 투자 설명서 검토에 따르면 상반기 매출이 163억 달러에 달하고, 약 90억 달러의 컴퓨팅/인프라 지출 및 6천억 달러 이상의 미래 컴퓨팅 약정이 언급되었습니다.

### ⚡ 인프라 & 하드웨어
*   **DeepSeek DeepInfer, NVIDIA 및 Huawei Ascend 플랫폼 지원** — DeepSeek의 DeepInfer는 NVIDIA 및 Huawei Ascend 플랫폼에서 분산 인퍼런스, 추측 디코딩 등을 지원하며, 특히 Ascend 950 NPU 호환성이 확인되었습니다.
*   **DeepInfer, 초최적화된 KV-캐시 및 SWA Bounded Replay 기술 적용** — DeepInfer는 100 PiB SSD 용량의 3FS 스토리지 클러스터에 영구 블록 KV 캐시를 저장하고, SWA Bounded Replay를 통해 최신 128개 토큰만으로 단기 상태를 재구성하여 프리필 컴퓨팅을 거의 절반으로 줄입니다.
*   **SGLang, 메가커널 지원 병합 및 고성능 인퍼런스 시연** — SGLang이 메가커널 지원을 병합했으며, SemiAnalysis는 GB300 NVL72에서 사용자당 거의 1,000 토큰/초, MI355X에서 1.5배 더 높은 상호작용성을 보고했습니다.
*   **Inferact, TPU v7에서 Kimi K3에 대한 고성능 인퍼런스 보고** — Inferact가 vLLM TorchTPU의 오픈소스 메가커널을 사용하여 TPU v7에서 Kimi K3에 대해 사용자당 391 토큰/초의 인퍼런스 성능을 보고했습니다.
*   **Zyphra, AMD MI355X에서 GLM-5.3 컨텍스트 TTFT 대폭 단축** — Zyphra가 단일 노드 MI355X 테스트에서 GLM-5.3의 512K 컨텍스트 TTFT를 178.8초에서 64.6초로, 90% 캐시된 컨텍스트에서는 42.3초에서 11.8초로 단축했습니다.
*   **PyTorch 2.15, Apple Silicon Metal 커널로 성능 개선** — PyTorch 2.15가 여러 MPSGraph 경로를 Metal 커널로 대체하여 MoE 디코딩을 5~6.5배 빠르게 하고, M3 Ultra에서 Qwen3.6-35B-A3B의 토큰 생성 속도를 9.4에서 61.3 토큰/초로 증가시켰습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
