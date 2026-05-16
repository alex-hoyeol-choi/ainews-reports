# Cerebras' $60B IPO: Slowly, then All at Once - 요약

**원문 URL**: https://www.latent.space/p/ainews-cerebras-60b-ipo-slowly-then
**번역일**: 2026-05-16 06:18
**발행일**: 2026-05-16

---

### 🔥 주요 뉴스
**[Cerebras, $60B 시가총액으로 IPO]** — AI 하드웨어 기업 Cerebras가 IPO를 통해 $60B의 시가총액을 기록하며, 오랜 기간의 역발상 하드웨어 베팅에 대한 시장의 인정을 받았습니다. CFO Bob Komin은 Cerebras가 모든 크기의 모델을 서비스하며, 현재 내부 OpenAI 5.4 및 5.5를 포함한 조 단위 파라미터 모델을 서비스하고 있다고 밝혔습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/5fea6bb8-3298-434e-afef-3eea148ba10c_2048x1263.png)
**[OpenAI, Codex 모바일/앱 출시 및 높은 채택률 기록]** — OpenAI가 Codex 모바일 앱을 출시하며 코딩 에이전트 플랫폼을 확장했습니다. 출시 첫 주에 100만 건 이상의 앱 다운로드를 기록했으며, 주간 활성 사용자 400만 명 이상, 사용자당 메시지 5배 증가를 달성했습니다.
**[OpenAI, ChatGPT에 개인 금융 경험 도입]** — OpenAI가 미국 Pro 사용자들을 위해 ChatGPT에 개인 금융 경험을 발표했습니다. 이는 안전한 금융 계좌 연결, 지출 분석, 사용자 승인 데이터 기반 Q&A 기능을 포함합니다.
**[Anthropic, Claude 속도 제한 재설정]** — Anthropic이 모든 사용자의 5시간 및 주간 Claude 속도 제한을 재설정했습니다. 이는 컴퓨팅 가용성 증가 또는 경쟁에 대한 대응으로 해석됩니다.

### 📊 모델 & 벤치마크
*   Epoch AI의 도메인별 ECI에 따르면 Claude는 소프트웨어 엔지니어링에서 강점을 보이지만, 수학 분야에서는 일반 능력 지수에 비해 저조한 성능을 나타냈습니다.
*   OpenAI의 내부 금융 벤치마크에서 GPT-5.5 Thinking은 79/100점, GPT-5.5 Pro는 82.5/100점을 기록하며 복잡한 개인 금융 작업에서 높은 성능을 보였습니다.
*   Qwen 소형 모델 MTP GGUF가 새로운 llama.cpp 추측 디코딩 파라미터 덕분에 기존 대비 1.8배 더 빠르게 실행됩니다.
*   ParseBench 리더로 Infinity-Parser2-Pro (35B)와 Flash (2B)가 500만 개 이상의 합성 파싱 샘플과 공동 RL 알고리즘을 통해 문서/요소/차트 파싱 작업에서 인정받았습니다.

### 🛠️ 제품 & 도구
*   Ollama가 로컬/오픈 모델 실행 및 클라우드 모델 추천과 함께 Codex 앱 지원을 추가했습니다.
*   Zed가 Codex와 동일한 구독/속도 제한 모델을 유지하며 에이전트에서 ChatGPT 구독 액세스를 지원합니다.
*   GitHub Copilot 팀은 사용자 경험이 모델 단독보다는 코딩 하네스(컨텍스트 어셈블리, 도구 사용, 실행 루프, 메모리)에 의해 더 많이 형성된다고 강조하며, 에이전트 병합 및 AI 설명이 포함된 터미널 위험 평가 배지 등의 기능을 선보였습니다.
*   LangChain이 LangSmith Engine, SmithDB, 관리형 Deep Agents, 샌드박스, 게이트웨이 및 컨텍스트 허브를 포함하는 Interrupt를 발표했습니다.
*   ClawRouter가 Hermes Agent를 통합하여 Teknium의 OpenClaw를 능가하는 토큰 볼륨을 주장했습니다.
*   vLLM이 Baseten의 vLLM-Omni 프로덕션 배포를 강조했으며, 이는 다단계 오디오, 스트리밍 멀티모달 및 실시간 TTS 워크로드를 위한 것입니다.
*   vLLM이 재료 결정 구조 생성 기능을 갖춘 오픈소스 과학 멀티모달 파운데이션 모델인 Intern-S2-Preview에 대한 Day-0 지원을 출시했습니다.
*   Capa는 OpenAPI 스펙을 Cloudflare 서비스 바인딩으로 변환하여 Stripe, GitHub, Slack, Twilio, Kubernetes와 같은 플랫폼에서 5,852개의 생성된 메서드를 제공합니다.
*   Weaviate v1.37은 속성별 악센트 폴딩, 속성별 불용어 프리셋, BM25 토큰화 디버깅을 위한 /v1/tokenize 엔드포인트를 추가했습니다.
*   Cohere는 시각적 파싱과 검색 임베딩을 사용하여 어려운 문서에 대한 리트리벌을 위한 스택으로 Compass를 추진했습니다.

### 🔬 연구 & 논문
*   새로운 연구는 올바른 에이전트 하네스로 래핑된 grep 스타일 텍스트 검색이 코딩 에이전트 작업에서 임베딩 기반 리트리벌과 일치하거나 능가할 수 있음을 보여주었습니다.
*   새로운 벤치마크 제안인 FutureSim은 실제 이벤트를 시간적으로 재생하여 Codex/Claude Code와 같은 네이티브 하네스에서 지속적인 업데이트 및 예측을 테스트합니다.
*   SODA 옵티마이저는 하이퍼파라미터를 추가하지 않고 가중치 감쇠 튜닝을 제거하며, 기본 옵티마이저를 개선하여 Muon을 능가한다는 주장을 했습니다.
*   Meta 연구원들은 모델이 지속적인 캐시에 유지할 키/값을 학습하여 KV 캐시 크기를 줄이고 디코딩 속도를 향상시키는 Self-Pruned KV attention을 제안했습니다.
*   "Learning, Fast and Slow"는 RL을 통한 가중치에서의 느린 학습과 GEPA로 최적화된 컨텍스트/프롬프트에서의 빠른 학습을 결합하여 데이터 효율성, 적응성, 적은 망각을 주장했습니다.
*   Pedagogical RL과 Late Interaction은 단순히 올바른 출력뿐만 아니라 올바르고 가르칠 수 있는 롤아웃 분포로부터 학습할 것을 주장합니다.

### 💰 산업 동향
*   Anthropic의 가치가 $900B, 5월 말까지 ARR이 $45B에 달할 것으로 예상되며, 이는 이전 체크포인트보다 급격히 증가한 수치입니다.

### ⚡ 인프라 & 하드웨어
*   NVIDIA는 Ollama를 통해 DGX Spark에서 Hermes Agent를 로컬로 실행하는 실용적인 배포 경로를 발표했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
