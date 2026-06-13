# Fable and Mythos officially too dangerous to release - 요약

**원문 URL**: https://www.latent.space/p/ainews-fable-and-mythos-officially
**번역일**: 2026-06-13 06:51
**발행일**: 2026-06-13

---

### 🔥 주요 뉴스
*   **[Anthropic Fable/Mythos 서비스 중단]** — Anthropic은 미국 정부의 지시에 따라 Fable 5 및 Mythos 5 모델을 모든 고객에게서 회수했습니다. 국가 사이버 보안 위험(탈옥 가능성)이 이유로 제시되었으며, Anthropic은 이의를 제기 중입니다. 이 조치는 모든 고객에게 서비스 중단을 야기하며, 다운스트림 제품 및 벤치마크에도 즉각적인 영향을 미쳤습니다.
    ![X avatar for @AnthropicAI](https://pbs.substack.com/profile_images/1798110641414443008/XP8gyBaY.jpg)

### 📊 모델 & 벤치마크
*   **[Artificial Analysis, DeepSWE로 코딩 에이전트 벤치마크 교체]** — Artificial Analysis는 벤치마크 게이밍을 줄이기 위해 코딩 에이전트 인덱스의 SWE-Bench Pro를 Datacurve의 DeepSWE로 교체했습니다. 이로 인해 Claude Code + Fable 5 [max]가 77점으로 1위에 오르는 등 순위가 크게 재편되었습니다.
*   **[Moonshot, Kimi-K2.7-Code 오픈소스 출시]** — Moonshot이 1T 파라미터 MoE, 32B 활성화, 256K 컨텍스트를 특징으로 하는 코딩 모델 Kimi-K2.7-Code를 오픈소스화했습니다. Kimi Code Bench v2에서 +21.8%, Program Bench에서 +11.0% 성능 향상 및 추론 토큰 사용량 30% 감소를 보고했습니다.
*   **[MiniMax, 멀티모달 오픈 웨이트 모델 M3 출시]** — MiniMax AI가 약 428B 파라미터, 약 23B 활성화, 1M 토큰 컨텍스트를 가진 오픈 웨이트 멀티모달 모델 MiniMax M3를 출시했습니다. MiniMax Sparse Attention (MSA) 기술로 1M 토큰 인퍼런스 시 토큰당 어텐션 연산을 1/20로 줄였습니다.
*   **[Huawei, openPangu 2.0 발표 및 오픈소스 계획]** — Huawei가 6월 30일부터 아키텍처, 가중치 등을 단계적으로 오픈소스화할 예정인 MoE 스타일 모델 openPangu 2.0을 발표했습니다. Pro 버전은 505B 총 파라미터/18B 활성화, Flash 버전은 92B 총 파라미터/6B 활성화입니다.
*   **[NVIDIA, DiffusionGemma NVFP4 양자화 버전 출시]** — NVIDIA가 Google DeepMind DiffusionGemma 26B A4B IT의 NVFP4 양자화 버전인 nvidia/diffusiongemma-26B-A4B-it-NVFP4를 출시했습니다. H100 FP8에서 1,100 tok/s 이상을 달성하며 BF16에 가까운 정확도를 유지합니다.
*   **[DiffusionGemma, 속도 향상 대비 정확도 저하]** — DiffusionGemma 26B A4B는 오토리그레시브 Gemma4보다 약 3.5~4배 빨랐으나, 사실 정확도는 33개 정답/28개 오답으로 Gemma4의 45개 정답/5개 오답에 비해 현저히 낮았습니다.
*   **[LLMFan46, Gemma 4 "uncensored-heretic" 모델 릴리스]** — LLMFan46이 Gemma 4의 여러 명령어 튜닝 릴리스(31B, 26B-A4B, 12B)를 Safetensors, GGUF, NVFP4, GPTQ-Int4 등 다양한 형식으로 출시했습니다.
*   **[EpochAI Research, FrontierMath v2 업데이트]** — EpochAI Research가 문제의 42%에서 오류를 감사한 후 FrontierMath: Tiers 1–4 (v2)를 출시했습니다. GPT-5.5의 Tier 4 점수가 상승했으며, Claude Fable 5는 Tiers 1–3에서 87%, Tier 4에서 88%에 도달했습니다.
*   **[Google Research, Gemini-SQL2 SOTA 달성 및 의료 분야 성과]** — Google Research가 Gemini-SQL2를 발표하며 텍스트-투-SQL 벤치마크 BIRD에서 SOTA를 주장했습니다. 또한, 범용 프론티어 모델이 임상 의사 평가에서 전문 의료 시스템보다 뛰어난 성능을 보인 연구 결과를 발표했습니다.
*   **[Artificial Analysis, 에이전틱 인퍼런스 벤치마크 AA-AgentPerf 출시]** — Artificial Analysis가 KV 캐시 재사용, 스페큘레이티브 디코딩 등 프로덕션 최적화를 활용하는 에이전틱 인퍼런스 전용 벤치마크 AA-AgentPerf를 도입했습니다. 주요 지표는 Megawatt당 에이전트(Agents per Megawatt)입니다.

### 🛠️ 제품 & 도구
*   **[SkyPilot, LLM 코드 실행용 샌드박스 출시]** — SkyPilot가 자체 Kubernetes 클러스터에서 신뢰할 수 없는 LLM 생성 코드를 안전하게 실행하기 위한 SkyPilot Sandboxes를 출시했습니다. 1초 미만 실행, 클러스터당 50,000개 이상의 샌드박스, 호스팅 벤더 대비 4~10배 낮은 비용을 주장합니다.
*   **[Anthropic, 고객 제어 샌드박스 내 Claude Managed Agents 문서 확장]** — Anthropic은 여러 제공업체에 걸쳐 고객이 제어하는 샌드박스 내에서 Claude Managed Agents를 실행하기 위한 문서를 확장했습니다.
*   **[Fable 5, 1989년 DOS 게임 리버스 엔지니어링]** — Fable 5/Claude가 1989년 DOS 게임 실행 파일(Midwinter)을 하룻밤 만에 리버스 엔지니어링하여 602개 함수의 레이블이 지정된 맵을 생성했습니다. 결과 디코딩/도구는 MIT 라이선스로 공개되었습니다.
*   **[Fable 5, MMORPG "World of ClaudeCraft" 개발]** — 한 개발자가 Fable 5를 사용하여 며칠 만에 브라우저 기반 MMORPG "World of ClaudeCraft"를 개발했습니다. 전체 소스는 GitHub에 공개되었고, 플레이 가능한 빌드가 제공됩니다.
*   **[Claude Code 플러그인 Ponytail 출시]** — MIT 라이선스 Claude Code 플러그인 Ponytail이 "게으른 시니어 개발자" 코딩 모드를 추가했습니다. 이 모드는 에이전트가 최소화 체크리스트를 따르도록 강제하여, 5가지 작업 벤치마크에서 토큰 사용량 16% 감소, 실행 속도 4배 향상, 코드 줄 수 293줄에서 47줄로 감소를 보고했습니다.

### 🔬 연구 & 논문
*   **[Google Research, 범용 프론티어 모델의 의료 분야 성능 우위 입증]** — Google Research는 Nature Medicine 연구 결과를 통해 Google/OpenAI/Anthropic의 범용 프론티어 모델이 임상 의사 평가에서 전문 의료 시스템보다 뛰어난 성능을 보였음을 지적했습니다.

### 💰 산업 동향
*   **[미국 정부의 Anthropic Fable/Mythos 서비스 중단 지시]** — 미국 정부가 국가 사이버 보안 위험을 이유로 Anthropic에 Fable 5 및 Mythos 5 모델의 외국인 접근을 중단하도록 지시했습니다. 이는 클로즈드 소스 프론티어 API의 지정학적 위험을 부각시켰습니다.

### ⚡ 인프라 & 하드웨어
*   **[llama.cpp, EAGLE3 스페큘레이티브 디코딩 통합]** — llama.cpp가 PR #18039를 병합하여 새로운 스페큘레이티브 디코딩 API를 통해 EAGLE3 스페큘레이티브 디코딩을 추가했습니다. 이는 타겟 모델의 중간 특징에 조건화되는 인코더-디코더 방식이며, 인퍼런스 속도를 약 2~3배 향상시키는 것으로 보고되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
