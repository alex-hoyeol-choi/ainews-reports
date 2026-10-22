# OpenAI’s Patch the Planet program is 1 of 2 parties to discover PHP2Shell vulnerabilities in core PHP affecting 70% of the web, using GPT-5.6 Sol; coordinated response over 2 months - 요약

**원문 URL**: https://www.latent.space/p/ainews-openais-patch-the-planet-program
**번역일**: 2026-10-22 12:39
**발행일**: 2026-10-22

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 뉴스레터 요약 브리핑입니다.

### 🔥 주요 뉴스
**[OpenAI, GPT-5.6 Sol로 PHP 핵심 취약점 발견]** — OpenAI의 "Patch the Planet" 프로젝트가 GPT-5.6 Sol을 활용하여 웹의 70%에 영향을 미치는 PHP2Shell 취약점(CVE-2026-109618, CVE-2026-109619)을 독립적으로 발견했습니다. Google Cloud에 인수된 Wiz도 Gemini 4 Argon을 사용하여 이 취약점을 독립적으로 찾아냈으며, 이는 2개월간의 공동 대응으로 이어졌습니다.
![X avatar for @lcfr_hax](https://pbs.substack.com/profile_images/2109847783171563521/X9NyMzto.jpg)
![](https://substack-post-media.s3.amazonaws.com/public/images/2f193200-5a32-4d16-8cef-d36ab44b0848_1440x1290.png)
**[Waymo, 로보택시 안전성 데이터 공개 및 확장 계획 발표]** — Waymo는 2억 7,130만 라이더 전용 마일에서 100만 마일당 0.01건의 심각한 부상/사망 사고를 보고하며, 이는 인간 운전 대비 심각한 충돌 사고 95%, 부상 사고 82% 감소를 의미합니다. Waymo는 50억 달러의 부채 조달을 통해 2027년 말까지 차량 수를 약 4천 대에서 2만 대로 확장할 계획입니다.
**[삼성, 2027년 HBM 생산량 100% 선판매 및 가격 인상 전망]** — 삼성은 빅테크 고객과의 다년 계약을 통해 내년 HBM 생산량의 100%와 범용 DRAM 생산량의 약 70%를 선판매한 것으로 알려졌습니다. 이로 인한 메모리 공급 부족으로 2027년 1분기 HBM 가격은 150~200%, DRAM 가격은 두 자릿수 상승할 것으로 예상됩니다.
**[NVIDIA 칩 공급 부족 심화: 중국 주요 기업 350억 달러 이상 주문]** — ByteDance, Alibaba, Tencent 등 중국 주요 기업들이 350억 달러 이상의 NVIDIA 칩(RTX PRO 5500 약 300만 개)을 주문했습니다. NVIDIA는 요청 수량의 5~10%만 이행 가능하며, 2027년까지 전 세계 RTX PRO 5500 생산량이 300만 개로 제한되는 반면 중국 수요는 600만 개를 초과합니다.

### 📊 모델 & 벤치마크
*   Recursive는 총 40B, 활성 2.5B 파라미터의 Apache-2.0 코딩 MoE 모델 Flint를 출시했으며, Terminal-Bench 2.1에서 54.9%, SWE-bench Pro v2에서 89.7%, SWE-bench Verified에서 74.2%를 기록했습니다.
*   Ornith AI는 Qwen 3.5/Gemma 계보를 파인튜닝한 122B MoE 추론 모델 Ornith-1.5-122B를 출시했으며, RL 기반 자기 개선 루프와 262K 컨텍스트(YaRN 스케일링으로 1M까지 확장 가능)를 특징으로 합니다.
*   Kyutai는 CPU 실시간 음성 복제 TTS 스택인 Pocket TTS-small을 1.9M, 6.9M, 18.2M 파라미터 변형으로 압축하여 출시했으며, 1.9M 모델은 CPU에서 약 25배 실시간 처리량을 달성합니다.
*   Artificial Analysis는 의료 추론 벤치마크 MLCR-AA를 업데이트하여 Sonnet 5.5와 GPT-6 Astra가 41.7%로 동점을 기록했으며, Claude는 완전성에서, OpenAI는 기록 기반 정확성에서 강점을 보였습니다.
*   NVIDIA의 10억 미만 파라미터 Nemotron 3.5 Parse 모델이 ParseBench 문서 이해 벤치마크에서 1위를 차지했습니다.
*   Fibo 2 Edit (HF 모델)은 빠르고 "검열되지 않은" 이미지 편집 모델로 보고되었으며, 간단한 편집에서 품질 손실 없이 일부 품질 향상을 보였습니다.

### 🛠️ 제품 & 도구
*   OpenAI는 PHP2Shell 취약점 노출 여부를 운영자가 확인할 수 있도록 Codex 스킬을 공개했습니다.
*   Anthropic은 Opus-5.5 기반의 선제적 개인 비서 Claude Duet을 연구 프리뷰로 출시했으며, Slack 모니터링 및 비동기적 작업 완료 기능을 제공합니다.
*   Cohere는 Rerank 5를 Pro 및 Fast 티어로 출시했으며, 옵트인 Context Focus 기능으로 정확성을 유지하면서 최대 41% 낮은 토큰 소비를 주장합니다.
*   Kling 4.0이 공식 API 액세스를 출시했으며, 복잡한 모션 안정성, 참조 일관성 및 시네마틱 제어에 중점을 둡니다.
*   Anthropic의 API 버전 2026-10-21은 Messages에서 `temperature`, `top_p`, `top_k` 파라미터를 제거하며, 새로운 SDK는 이를 기본으로 사용합니다.
*   한 사용자는 Claude를 인터랙티브 에이전트로 활용하여 삼성 TV의 타이젠 OS 문제를 해결하고, 개인 정보 보호 설정을 변경하며, 맞춤형 런처를 구축하는 데 성공했습니다.
*   다른 사용자는 Claude Code를 사용하여 삼성 TV API를 모킹하여 기본 광고가 많은 홈 화면을 대체하는 맞춤형 웹 스타일 런처를 개발했습니다.
*   한 사용자는 Claude Code를 활용하여 1,100만 개 이상의 뉴스 기사에서 파생된 집계된 클러스터 메타데이터를 쿼리하여 글로벌 뉴스 패턴을 분석했습니다.
*   Unitree는 최대 8시간의 내구성을 가진 더 견고한 H2 휴머노이드 변형인 H2-X "쿵푸 레전드 가디언"을 발표했으며, 서비스 및 경비 플랫폼으로 포지셔닝됩니다.

### 🔬 연구 & 논문
*   Recursive의 Eureka Machine은 아이디어 구상, 구현 및 검증 전반에 걸쳐 참여하여 Flint 모델의 희소 아키텍처 선택, 저비트 학습 및 커널에 기여했으며, 거의 품질 손실 없이 71%의 크기 감소를 달성했습니다.
*   Perplexity와 NVIDIA는 셀프 디스틸레이션의 약점을 해결하는 JOLT(Jointly Optimized Learning for Teacher-Student)를 개발하여, MATH 벤치마크에서 GRPO와 동일한 성능을 6.5배 적은 학습 토큰으로 달성했습니다.
*   OpenAI의 GPT-Rosalind는 수백만 개의 쥐 뇌 세포 유전자 발현 결과와 문헌을 연결하여 DCTN1 교란과 콜레스테롤 수송 장애, 소뇌 뉴런의 TSC1 및 TSC2 교란 차이 등 테스트 가능한 생물학적 가설을 32분 만에 생성했습니다.
*   OO-Harness는 특수 서브클래스, 실행에서 파생된 설계 교훈 및 라우팅을 통해 동일한 Gemini 3.5 Flash 실행기로 AutomationBench를 61.6%에서 77.4%로, Workspace-Bench를 25.5%에서 39.5%로 향상시켰습니다.
*   Agent S4는 성공 레이블 없이 궤적에서 도구를 구축하는 메타 에이전트로, open-27B OSWorld V2에서 21.3%(수동 구축 인터페이스 대비 3.8배), ScienceBoard에서 58.6%(41.4%에서 상승)를 달성했습니다.
*   SuperMimic은 학습된, 미분 가능한 월드 모델 대리자와 시간 역전파를 결합하여 129,514개 동작에 걸쳐 하나의 GPU로 3시간 만에 휴머노이드 학습을 완료했다고 보고했으며, 이는 기존 SOTA 설정 대비 1,000배 이상의 GPU-시간 감소를 의미합니다.

### 💰 산업 동향
*   Cloudflare는 PHP2Shell 취약점의 예정된 패치 출시 전에 초기 WAF 완화 조치를 배포했습니다.
*   NSA는 PHP2Shell 취약점에 대해 즉각적인 업데이트를 권고했으며, 적시에 완화가 불가능할 경우 시스템을 오프라인으로 전환할 것을 조언했습니다.
*   OpenAI의 프론티어 모델과 Codex 워크플로우가 Google Cloud Model Garden에 제공될 예정입니다.
*   BBC 보도에 따르면 Google의 고용 계약이 공개 비판을 무기한으로 제한하여 AI 안전성 및 군사적 용도에 대한 논의를 저해한다는 주장이 제기되었습니다.
*   Anthropic은 연례 공익 보고서를 발표하고, 실험 물리학자 Christopher Stubbs를 장기 공익 신탁에 임명하며 공익 거버넌스를 업데이트했습니다.
*   Linux 커널은 Linus Torvalds의 커밋 14c8977을 통해 새로운 코드 제출 시 AI 사용 선언("Assisted-by") 요구 사항을 더 이상 적용하지 않기로 했습니다.
*   중국은 증가하는 메모리 수요에 대응하여 CXMT와 같은 국내 공급업체를 통해 RAM/DRAM 생산량을 두 배로 늘릴 계획이며, 이는 점진적으로 가격 인상 속도를 늦출 것으로 예상됩니다.

### ⚡ 인프라 & 하드웨어
*   DeepSeek은 스펙큘레이티브 디코딩, 동적 프리필 크기 조정 등을 결합한 오픈소스 대규모 인퍼런스 프레임워크 DeepInfer를 출시했으며, 단일 클러스터에서 하루 155조 토큰 처리량을 주장합니다.
*   Google은 익숙한 PyTorch 툴링을 통해 학습 및 서빙을 위한 TorchTPU를 오픈소스화했으며, SGLang의 플러그인은 Meta에서 프로덕션 인퍼런스를 구동합니다.
*   NVIDIA의 DSX POD는 AI 인프라를 컨테이너화된 빌딩 블록으로 패키징하여 용량 확장을 며칠 만에 가능하게 하며, Lambda는 DSX MaxLPS를 사용하여 16개의 전력 예산 내에서 19개의 HGX B200 노드를 작동하는 것을 시연했습니다.
*   EAGLE-4는 하드웨어/워크로드 보정 드래프트 트리를 사용하는 소스 사용 가능한 스펙큘레이티브 디코딩 스택으로 출시되었으며, Qwen3.8-27B에 대해 바닐라 디코딩 대비 3.59배의 속도 향상을 보고합니다.
*   RTX 3090 "GPU 언락" 커널/모듈이 NVIDIA의 FP32 누적 텐서 연산 제한을 제거하여 BF16 텐서 수학 처리량을 실질적으로 높일 수 있다고 주장되었습니다 (예: BF16 텐서 파이프에서 82→155 TFLOPS).

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
