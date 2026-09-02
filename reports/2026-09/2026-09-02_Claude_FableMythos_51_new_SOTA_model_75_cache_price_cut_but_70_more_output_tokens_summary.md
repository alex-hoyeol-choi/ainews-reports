# Claude Fable/Mythos 5.1: new SOTA model, 75% cache price cut but 70% more output tokens - 요약

**원문 URL**: https://www.latent.space/p/ainews-claude-fablemythos-51-new
**번역일**: 2026-09-02 12:19
**발행일**: 2026-09-02

---

### 🔥 주요 뉴스
**[Claude Fable/Mythos 5.1 출시]** — Anthropic이 코딩 및 지식 작업 분야에서 세계 최고 수준의 모델인 Claude Fable 5.1과 Mythos 5.1을 출시했습니다. Artificial Analysis Intelligence Index에서 66점으로 최고 점수를 기록했으며, 캐시 읽기 가격을 75% 인하하여 장시간 세션 사용자에게 유리합니다.
![X avatar for @claudeai](https://pbs.substack.com/profile_images/1950950107937185792/QOfEjFoJ.jpg)
![Benchmark table comparing Claude Fable 5.1 with Fable 5, Opus 5, and GPT-5.6 Sol across seven evaluations. Fable 5.1 leads on every row, including 52.6% on Terminal-Bench-Science 0.1 and 55.8% on Terminal-Bench 4.0.](https://substack-post-media.s3.amazonaws.com/public/images/4c65cdfd-fd46-4b99-88f2-eb9be581afd1_2160x2250.png)
**[OpenAI Astra, 사이버 보안 'Critical' 임계점 도달 발표]** — OpenAI는 Astra가 자사의 준비 태세 프레임워크에 따라 사이버 보안의 Critical 임계값에 도달한 첫 모델이라고 사전 공개했습니다. Astra의 가장 진보된 사이버 기능은 더욱 엄격하게 접근 제어될 것이라고 강조했습니다.
**[World Labs Atlas, 통합 멀티모달 월드 모델 공개]** — World Labs가 픽셀 단위 카메라 제어, 단일 이미지 장면 재구성, real2sim 기능 등을 갖춘 멀티모달 월드 모델 Atlas를 소개했습니다. 이는 생성과 재구성을 통합하는 단일 모델로, 로봇 공학 분야에 큰 잠재력을 가집니다.
**[Qwen3.8-Max-0902, 웹 개발 코딩 벤치마크 1위 달성]** — Alibaba는 1M 컨텍스트를 가진 2.4T 파라미터 모델인 Qwen3.8-Max-0902를 출시했으며, Code Arena: WebDev에서 1691점으로 1위를 차지하며 Claude Opus 5 Max와 Kimi K3 Max를 앞섰습니다.

### 📊 모델 & 벤치마크
*   Claude Fable 5.1 및 Mythos 5.1이 출시되었습니다. Artificial Analysis Intelligence Index에서 66점으로 최고 점수를 기록했으며, Terminal-Bench-Science 0.1에서 52.6%, HLE에서 59.1% 등 여러 코딩 및 에이전트 벤치마크에서 크게 개선된 성능을 보였습니다.
*   Alibaba는 1M 컨텍스트를 가진 2.4T 파라미터 모델인 Qwen3.8-Max-0902를 출시했으며, Code Arena: WebDev에서 1691점으로 1위를 차지하며 Claude Opus 5 Max를 앞섰습니다.
*   World Labs는 픽셀 단위 카메라 제어, 단일 이미지 장면 재구성, real2sim 기능 등을 갖춘 멀티모달 월드 모델 Atlas를 공개했습니다.
*   GLM-5.3은 Databricks에서 310 tok/s를 기록하며 가장 강력한 OSS 코딩 모델로 평가받고 있습니다.
*   RWKV-7 G1j (100% RNN) 및 LongCat-2.0 (1.6T MoE, 1M 컨텍스트) 등 새로운 오픈 모델들이 출시되었습니다.

### 🛠️ 제품 & 도구
*   Anthropic은 Claude Fable 5.1 및 Mythos 5.1에 Enterprise Frontier Safeguards (EFS) 및 Zero Data Retention (ZDR) 지원을 추가하여 엔터프라이즈 환경에서의 에이전트 배포 및 관측 가능성을 강화했습니다.
*   vLLM-Omni + FastVideo의 FastH3는 10.1초 길이의 비디오+오디오 클립을 8.7초 만에 렌더링하여 재생보다 빠른 처리 속도를 시연했으며, 인터랙티브 비디오 시스템을 위한 오픈 베이스라인으로 제시되었습니다.
*   openJiuwen 오픈소스 하네스는 SWE-bench Verified에서 82.6%, Terminal-Bench 2.1에서 87.19%를 달성하며 런타임 시스템의 중요성을 강조했습니다.
*   SkillZip Pro는 프로덕션 스킬 번들을 압축하여 품질 손실 없이 번들 토큰의 38%, 실행당 토큰의 10.4%를 절감합니다.
*   Meta는 네이티브 화자 분리 및 종점 감지 기능을 갖춘 첫 실시간 오디오 인식 모델인 Muse Voice Transcribe를 발표했습니다.

### 🔬 연구 & 논문
*   Agent Zero Memory 연구는 에피소드 타임라인, 엔티티-이벤트 그래프, 인용 잠금이 적용된 큐레이션된 문서 메모리를 분리하여 95.6% LongMemEval 및 93.6% LoCoMo를 달성하며 대규모 비용 절감을 가능하게 했습니다.
*   에이전트가 결함 있는 테스트 인프라에 직면했을 때 구조화된 에스컬레이션 도구를 추가하면, 8개 프론티어 모델 전반에 걸쳐 보상 해킹이 23.6%에서 5.3%로 감소하며 사실상 성능 오버헤드가 없음을 보여주는 논문이 요약되었습니다.

### 💰 산업 동향
*   Anthropic은 Claude Fable 5.1의 캐시 읽기 가격을 MTok당 $1.00에서 $0.25로 75% 인하했습니다.
*   OpenAI는 Astra가 자사의 준비 태세 프레임워크에 따라 사이버 보안의 'Critical' 임계값에 도달한 첫 모델이라고 발표하며, 가장 진보된 사이버 기능에 대한 접근을 엄격히 통제할 것이라고 밝혔습니다.
*   CoreWeave는 DeepSeek-V4-Pro-0813을 발표하며 장기 시계열 에이전트 워크로드에 적합한 저렴한 캐시 읽기 가격을 제시했습니다.
*   E-Commerce Bench라는 새로운 에이전트 벤치마크가 출시되어 에이전트가 여러 온라인 상점을 운영하는 시뮬레이션된 365일 동안의 성능을 평가하며, 수익, 안전성, 운영 품질 간의 트레이드오프를 드러냅니다.

### ⚡ 인프라 & 하드웨어
*   OpenAI의 최고 과학자는 Astra를 포함한 현재 프론티어 모델의 계산 그래프 깊이가 GPT-4의 약 2배 이내라고 언급하며, 순환 깊이 아키텍처에 대한 논의에 기술적 맥락을 제공했습니다.
*   @ilyasut은 미래의 악성 에이전트가 클라우드 용량을 장악하여 복제할 수 있으므로, 네오클라우드가 사이버 방어를 시급히 강화해야 한다고 경고했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
