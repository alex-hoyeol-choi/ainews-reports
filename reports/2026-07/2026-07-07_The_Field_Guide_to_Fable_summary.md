# The Field Guide to Fable - 요약

**원문 URL**: https://www.latent.space/p/ainews-the-field-guide-to-fable
**번역일**: 2026-07-07 06:09
**발행일**: 2026-07-07

---

### 🔥 주요 뉴스
**[Tencent Hy3 모델 출시 및 vLLM 지원]** — Tencent가 Apache 2.0 라이선스 하에 295B MoE 모델인 Hy3를 공개했습니다. 이 모델은 21B 활성 파라미터와 256K 컨텍스트를 가지며, vLLM은 출시 당일부터 Hy3에 대한 네이티브 지원을 발표하여 최대 2.95배의 디코드 성능 향상을 보고했습니다.
**[Anthropic, Claude 내부 J-Space 연구 발표]** — Anthropic은 Claude 내부에 J-space라고 불리는 활성화 부분집합을 중심으로 하는 글로벌 워크스페이스 유사 구조에 대한 연구를 공개했습니다. 이는 모델의 "작업 메모리" 또는 내부 워크스페이스에 대한 강력한 증거로 평가되며, 오픈 웨이트 모델을 위한 Neuronpedia 데모도 함께 출시했습니다.
**[Meituan LongCat 2.0 오픈소스 및 중국 국내 칩 학습]** — Meituan이 총 1.6T 파라미터(활성 약 48B)의 MoE 모델인 LongCat 2.0의 가중치를 MIT 라이선스로 공개했습니다. 이 모델은 100% 중국 국내 칩으로 학습되었다고 보고되어 AI 하드웨어 공급망 독립성 측면에서 주목받고 있습니다.
**[MIRA, Rocket League용 플레이 가능한 월드 모델 데모 공개]** — General Intuition과 Kyutai가 Epic Games와 협력하여 Rocket League를 위한 5B 파라미터 멀티플레이어 월드 모델 MIRA를 선보였습니다. 이 모델은 단일 NVIDIA B200에서 20 fps로 실시간 2v2 경기를 실행하며, 명시적인 물리 또는 렌더링 엔진이 필요 없습니다.

### 📊 모델 & 벤치마크
*   **Tencent Hy3 출시**: Apache 2.0 라이선스의 295B MoE 모델(21B 활성 파라미터, 256K 컨텍스트)을 공개했습니다. 툴-콜링 안정성 및 환각 방지 등 신뢰성 개선에 중점을 두었습니다.
*   **AutomationBench-AA 리더보드 출시**: Artificial Analysis가 Zapier의 AutomationBench에 대한 독립적인 리더보드를 공개하여 657개 작업과 40개 시뮬레이션 SaaS 앱에서 에이전트를 평가합니다. Claude Fable 5가 48.6%로 선두를 차지했습니다.
*   **Artificial Analysis 역량 지수 도입**: 금융, 법률, 의료 등 6가지 도메인별 에이전트 역량 지수를 도입했습니다. Claude Fable 5와 Opus 4.8이 각 도메인에서 선두를 차지했습니다.
*   **MIRA 월드 모델 데모**: General Intuition과 Kyutai가 Epic Games와 협력하여 Rocket League용 5B 파라미터 멀티플레이어 월드 모델 MIRA를 선보였습니다. 단일 NVIDIA B200에서 20 fps로 실시간 2v2 경기를 실행합니다.
*   **Speechify Simba 3.2 TTS 성능 기록**: Artificial Analysis에 따르면 Speechify Simba 3.2가 Speech Arena에서 1233 Elo로 선두를 차지하며, 상위권 모델 중 가장 저렴합니다.
*   **Meituan LongCat 2.0 오픈소스**: 총 1.6T 파라미터(활성 약 48B)의 MoE 모델 가중치를 MIT 라이선스로 공개했습니다. BF16 기준 약 3.55 TB의 가중치 크기를 가집니다.

### 🛠️ 제품 & 도구
*   **Microsoft GitHub Copilot 최적화**: GitHub Copilot 하네스에서 GPT-5.5의 프롬프트 수준 최적화를 통해 출시 후 레이턴시 및 토큰 효율성을 개선했습니다.
*   **OpenAI GPT-Realtime-2.1-mini 출시**: 이전 mini와 동일한 가격으로 추론 및 툴 사용 기능을 제공하며, 캐싱 개선을 통해 p95 레이턴시를 25% 이상 감소시켰습니다.
*   **AssemblyAI Universal-3.5 Pro Realtime 출시**: AA-WER Streaming에서 4.1% WER을 기록하고 컨텍스트 프라이밍 기능을 갖춘 스트리밍 STT 모델입니다.
*   **LlamaIndex & LanceDB 멀티모달 리트리벌 파이프라인**: 지저분한 PDF를 위한 리트리벌 파이프라인을 설명했으며, 레이블링된 ESG-report 벤치마크에서 74%의 답변 정확도를 보고했습니다.

### 🔬 연구 & 논문
*   **Anthropic J-Space 연구 발표**: Claude 내부에 J-space라고 불리는 활성화 부분집합을 중심으로 하는 글로벌 워크스페이스 유사 내부 구조에 대한 연구를 발표했습니다. 또한 오픈 웨이트 모델을 위한 Neuronpedia 데모를 출시했습니다.
*   **A-TMA 연구**: 장기 실행 어시스턴트의 "고스트 메모리" 문제를 해결하여 LTP 벤치마크에서 충돌 정확도를 +0.240 향상시키는 A-TMA를 소개했습니다.
*   **ReContext 연구**: 답변 생성 직전에 모델 내부 증거를 재생하여 증거 활용을 개선하는 학습 없는 장문 컨텍스트 인퍼런스 하네스 ReContext를 발표했습니다.
*   **BlockSearch 연구**: 백만 토큰 인-컨텍스트 리트리벌을 위한 BlockSearch를 소개했습니다.

### 💰 산업 동향
*   **Meituan LongCat 2.0 중국 국내 칩 학습**: Meituan이 LongCat 2.0 모델을 100% 중국 국내 칩으로 학습시켰다고 보고되어 AI 하드웨어 공급망 독립성에 대한 중요성을 시사합니다.

### ⚡ 인프라 & 하드웨어
*   **vLLM Hy3 지원 및 성능 개선**: vLLM이 Tencent Hy3 모델을 출시 당일부터 기본 지원하며, Tencent의 프로덕션 커널 업스트림을 통해 혼합 길이 디코드에서 최대 2.95배 성능 향상 및 레이턴시 감소를 보고했습니다.
*   **SGLang DSpark 추가**: 스페큘레이티브 디코딩에 DSpark를 추가하여 신뢰도 기반의 가변 길이 검증을 가능하게 하여 높은 부하에서 처리량/레이턴시 트레이드오프를 개선했습니다. DeepSeek-V4-Pro는 B300에서 383.7 tok/s에 도달했습니다.
*   **Chutes 커널 속도 향상**: MiniMax MSA 및 GatedDeltaNet-2에 대한 주요 속도 향상을 보고했으며, RTX Pro 6000 / SM120에서 희소 어텐션 학습을 약 7배 개선하고 퓨즈드 FP8 커널을 포함합니다.
*   **Cloudflare Workers Cache 출시**: Worker 진입점 앞에 지역별 계층형 캐시인 Workers Cache를 출시했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
