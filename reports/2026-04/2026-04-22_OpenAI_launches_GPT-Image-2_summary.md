# OpenAI launches GPT-Image-2 - 요약

**원문 URL**: https://www.latent.space/p/ainews-openai-launches-gpt-image
**번역일**: 2026-04-22 00:38
**발행일**: 2026-04-22

---

### 🔥 주요 뉴스
**[OpenAI, GPT-Image-2 출시]** — OpenAI가 ChatGPT Images 2.0과 기반 gpt-image-2 모델을 ChatGPT, Codex, API 전반에 걸쳐 출시했습니다. 이 모델은 강력한 텍스트 렌더링, 레이아웃 충실도, 편집, 다국어 지원 및 이미지에 대한 "사고(thinking)" 기능을 제공하며, Arena 벤치마크에서 모든 Image Arena 리더보드 1위를 차지했습니다.
![가장 인상적인 단일 데모를 꼽으라면, 매트릭스 예시에서 보여주는 텍스트 디테일과 일관성 수준일 것입니다.](https://substack-post-media.s3.amazonaws.com/public/images/d187fe49-1184-477d-84b8-cbe7d502356e_2188x1604.png)
![또는 커스텀 Where’s Waldo:](https://substack-post-media.s3.amazonaws.com/public/images/5c619373-c1af-4ac0-b85d-f6bb3e4e78fe_1451x2048.png)
![또는 커스텀 Where’s Waldo:](https://substack-post-media.s3.amazonaws.com/public/images/5c619373-c1af-4ac0-b85d-f6bb3e4e78fe_1451x2048.png)
**[Hugging Face, ml-intern 오픈소스 에이전트 출시]** — Hugging Face가 논문 읽기, 데이터셋 수집, 학습 작업 실행 등을 자동화하는 오픈소스 에이전트 ml-intern을 발표했습니다. 이 에이전트는 Qwen3-1.7B의 GPQA 과학적 추론을 10시간 내 10%에서 32%로 향상시키고, HealthBench에서 Codex를 60% 능가하는 등 엔드투엔드 연구 루프 자동화에서 강력한 성능을 보였습니다.
**[Moonshot, Kimi K2.6 및 FlashKDA 커널 출시]** — Moonshot이 1조 개 파라미터의 Mixture-of-Experts 아키텍처를 가진 오픈소스 멀티모달 AI 모델 Kimi K2.6을 출시했습니다. Kimi K2.6은 장기 코딩 및 자율 작업 오케스트레이션에 최적화되어 있으며, Moonshot은 또한 FlashKDA라는 CUTLASS 기반 Kimi Delta Attention 커널을 오픈소스화하여 H20에서 flash-linear-attention 대비 1.72배~2.22배의 프리필 속도 향상을 달성했습니다.
**[Google, Deep Research Max 출시]** — Google/DeepMind가 Gemini API를 통해 Deep Research와 Deep Research Max를 업데이트 출시했습니다. Gemini 3.1 Pro 기반의 이 모델은 협업 계획, 멀티모달 입력, 코드 실행, 네이티브 차트/인포그래픽 생성 기능을 제공하며, DeepSearchQA에서 93.3%, BrowseComp에서 85.9%, HLE에서 54.6%의 벤치마크 점수를 기록했습니다.

### 📊 모델 & 벤치마크
*   OpenAI의 gpt-image-2 모델은 Arena Image 리더보드에서 text-to-image 1512점, single-image edit 1513점, multi-image edit 1464점으로 1위를 기록했습니다.
*   Hugging Face의 오픈소스 에이전트 ml-intern은 Qwen3-1.7B의 GPQA 과학적 추론을 10시간 내 10% → 32%로 향상시키고, HealthBench에서 Codex를 60% 능가하는 성능을 보였습니다.
*   Moonshot의 Kimi K2.6은 1조 개 파라미터의 Mixture-of-Experts 아키텍처를 가진 오픈소스 멀티모달 AI 모델로, 장기 코딩 및 자율 작업 오케스트레이션에 최적화되어 최대 300개의 서브 에이전트를 지원합니다.
*   Kimi K2.6은 장기 코딩 작업에서 Qwen3.5-0.8B 인퍼런스 처리량을 15 tok/s에서 193 tok/s로 개선하고, 거래 엔진 재작업에서 중간 처리량 185%, 최고 처리량 133% 향상을 달성했습니다.
*   Google Deep Research Max는 DeepSearchQA에서 93.3%, BrowseComp에서 85.9%, HLE에서 54.6%의 벤치마크 점수를 기록했습니다.
*   LightOn은 Apache 2.0 라이선스 하에 149M 파라미터 리트리벌 모델 LateOn과 DenseOn을 출시했으며, LateOn은 BEIR에서 57.22 NDCG@10, DenseOn은 56.20을 기록하여 최대 4배 큰 모델들을 능가했습니다.
*   Google Gemma 4 26B A4B는 M4 Max에서 ~18 tok/s/request로 10개 이상의 동시 요청을 처리하는 로컬 동시성 데모를 선보였습니다.
*   Kimi K2.6은 GPT-5.4, Claude Opus 4.6, Gemini 3.1 Pro와 비교하여 General Agents, Coding, Visual Agents 카테고리에서 강력한 성능을 보였습니다.
*   Gemma 4 Vision 모델은 `--image-min-tokens` 및 `--image-max-tokens` 설정을 560과 2240으로 조정하여 Qwen 3.5, Qwen 3.6, GLM OCR을 비전 작업에서 능가할 수 있음을 보여주었습니다.
*   Google의 Gemma-4-E2B 모델은 비상 상황에서 응급 기도 확보, 물 정화 등 중요한 생존 주제에 대해 '단호한 거부'를 발행하는 지나치게 공격적인 안전 필터로 인해 비효율적이라는 비판을 받았습니다.
*   Gemma 4 26B-A4B GGUF 벤치마크에서 Unsloth GGUF가 양자화 후 정확도 유지 측면에서 최고 성능을 보였으며, 22개 크기 중 21개에서 다른 모델들을 능가했습니다.
*   Qwen3.6-35B-A3B와 Gemma4 26B-A4B-it 모델 비교에서 Qwen3.6은 코딩 및 일반 작업에서 높은 에너지를 보였으나 메서드를 더 자주 환각하는 경향이 있으며, Gemma4는 복잡한 프롬프트와 백엔드 스크립팅에 더 적합한 안정적인 성능을 보였습니다.
*   Qwen 3.6 Max가 Qwen Chat 웹사이트에 출시되었으며, AiBattle에서 현재 중국 모델 중 가장 높은 AA-Intelligence Index 점수 52점을 기록했습니다.

### 🛠️ 제품 & 도구
*   OpenAI의 gpt-image-2 모델은 Figma, Canva, Firefly, fal, Hermes Agent 등 다운스트림 도구에 통합되고 있습니다.
*   Hugging Face가 논문 읽기, 데이터셋 수집/재포맷, 학습 작업 실행 등을 자동화하는 오픈소스 에이전트 ml-intern을 발표했습니다.
*   Hermes 에이전트 플랫폼은 Skillkit 네이티브 지원, 새로운 macOS GUI인 Scarf, 그리고 더 깊은 계층적 분해를 위한 서브 에이전트의 스폰 너비 및 재귀적 스폰 깊이 지원을 추가했습니다.
*   DSPy 3.2는 RLM 개선 사항, 옵티마이저 체이닝, LiteLLM 디커플링을 출시했습니다.
*   LangChain은 deepagents 배포를 위한 커스텀 인증을 추가했습니다.
*   Google/DeepMind가 Gemini API를 통해 업데이트된 Deep Research와 Deep Research Max를 출시했으며, 멀티모달 입력(PDF/CSV/이미지/오디오/비디오), 코드 실행, 네이티브 차트/인포그래픽 생성, 실시간 진행 스트리밍 기능을 제공합니다.
*   vLLM은 recipes.vllm.ai를 재설계하여 모델 페이지를 실행 가능한 배포 레시피에 매핑하고, 대화형 명령 빌더, NVIDIA 및 AMD 지원, 텐서/전문가/데이터 병렬 변형 모델 처리, 에이전트를 위한 JSON API를 노출했습니다.
*   Claude Pro 플랜에서 Claude Code 기능이 제거되었습니다.

### 🔬 연구 & 논문
*   LightOn은 14억 개의 쿼리-문서 쌍을 포함하는 통합 데이터셋과 FineWeb-Edu 기반의 새로 고침된 웹 데이터셋을 발표했습니다.
*   LlamaIndex는 실제 엔터프라이즈 문서 내 차트 이해를 위한 ParseBench라는 새로운 벤치마크를 발표했습니다.
*   새로운 연구 결과는 에이전트가 해결책이 파일이나 엔드포인트에 명시적으로 노출되어 있을 때조차 환경 단서를 무시하는 경향이 있음을 보여주었습니다.
*   Google Research의 ReasoningBank는 성공 및 실패 궤적 모두로부터 학습하는 메모리 구성에 대한 연구를 진행했습니다.

### 💰 산업 동향
*   Cursor는 xAI와 600억 달러 규모의 인수 권리 계약을 체결했습니다.
*   Clement Delangue는 오픈소스 AI를 제한하려는 로비 활동이 재개될 수 있다고 경고했습니다.

### ⚡ 인프라 & 하드웨어
*   Moonshot은 FlashKDA라는 CUTLASS 기반 Kimi Delta Attention 커널 구현을 오픈소스화했으며, H20에서 flash-linear-attention 기준선 대비 1.72배~2.22배의 프리필 속도 향상을 주장합니다.
*   8x MI300X에서 Kimi K2.6 + DFlash가 508 tok/s를 기록하여, 기준선 자기회귀 설정 대비 5.6배의 처리량 향상을 보였습니다.
*   새로운 UD-IQ4_NL_XL quant가 도입되어 16GB VRAM 내에 들어맞으며, 기존 모델들 사이의 중간 지점을 제공합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
