# not much happened today - 요약

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-612
**번역일**: 2026-09-18 07:02
**발행일**: 2026-09-18

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 브리핑입니다.

### 🔥 주요 뉴스
**[OpenAI 연결 계정 및 내부 리포지토리 침해]** — 연구원 3명이 Claude Opus 5를 활용하여 이미지 업로드 버그, ChatGPT/Codex 계정 탈취, OpenAI 연결 서비스 접근을 연쇄적으로 악용했습니다. 이들은 OpenAI 내부 모노레포에 PR을 제출하여 이를 증명했으며, 72시간 이내, 1,000달러 미만의 토큰 비용으로 이루어진 이 사건은 익스플로잇 체인 자동화의 실용성을 보여줍니다.

### 📊 모델 & 벤치마크
*   **PrismML, Bonsai 2 27B 모델 출시:** Apache 2.0 라이선스로 출시된 Bonsai 2 27B는 크기를 9배 줄여 5.9GB로 만들면서도 집계 벤치마크 성능의 98.2%를 유지한다고 주장합니다.
*   **Cactus Compute, Needle 3 모델 출시:** 25-121M 파라미터, 8-29MB 크기의 분할 가능한 자동화 모델로, 엣지 디바이스에서의 도구 선택 및 유형화된 추출을 목표로 합니다.
*   **UkisAI, Swift Qwen 3.8 27B 모델 인기:** HuggingFace에서 10만 회 이상 다운로드되며 #1 파인튜닝 모델 및 #9 트렌딩 모델을 기록했습니다. 토큰 사용량을 58.3% 줄이고 속도를 1.95배 향상시키면서 정확도 손실이 없다고 주장하며, Swift1.5 Qwen3.8 27B 및 Swift Qwen3.8 Flash Next가 후속으로 계획되어 있습니다.
![Swift Qwen 3.8 27B Downloads](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F62447952-475a-495c-9226-e1795058097b_100k_downloads.png)
*   **Ternary Bonsai 2 (27B) 모델 출시:** Qwen3.8-27B의 삼진법 가중치 파생 모델로, Hugging Face에 출시되었습니다. 6GB 미만의 크기로 FP16보다 9배 작으면서도 기준 "지능"의 98.2%를 유지한다고 주장하며, WebGPU 데모를 제공합니다.
*   **Epoch, Benchmark Reviews 출시:** 15개의 감사(Verified/Flawed/Insufficiently documented로 분류)를 포함하는 Benchmark Reviews를 출시하여 벤치마크의 신뢰성을 평가합니다.
*   **Vals, Vibe Code Bench 1-100 도입:** 반복적인 수정 견고성을 측정하기 위해 Vibe Code Bench 1-100을 도입했습니다.

### 🛠️ 제품 & 도구
*   **Anthropic, Claude Code에 Projects 기능 출시:** 단일 대화가 병렬 클라우드 세션을 생성하고, 스레드 간에 컨텍스트를 전달하며, 사용자가 떠난 후에도 계속 실행될 수 있도록 하는 Projects 기능을 Claude Code에 출시했습니다.
*   **Google, Gemini 관리형 에이전트 업데이트:** 새로운 Antigravity 기반 하네스와 함께 Credentials API(모델 컨텍스트에서 비밀 정보 제외) 및 Files API(아티팩트 이동 및 영구 샌드박스)를 추가했습니다. 최대 30% 낮은 비용과 22% 높은 캐시 적중률을 주장합니다.
*   **TypeSafe, Jev 프리미티브 출시 및 Cloudflare AI Gateway 노출:** 빠르고 저렴한 제약된 출력 프리미티브인 Jev가 출시되었으며, Cloudflare는 이미 AI Gateway를 통해 이를 노출하여 라우팅, 판단, 구조화된 의사결정 레이어에 활용됩니다.
*   **OpenAI, GPT-Live-1 및 Appshots 출시:** GPT-Live-1을 통한 전화 음성 Codex와 Windows용 Appshots 기능을 출시했습니다.
*   **Anthropic, 오픈소스 생물학 모델 인퍼런스 최적화 코드 공개:** 30개 이상의 오픈소스 생물학 모델에 대한 인퍼런스를 최적화하여 평균 4배의 속도 향상을 달성했으며, 관련 코드를 오픈소스화했습니다.

### 🔬 연구 & 논문
*   **Google DeepMind, Stellar Colosseum 발표:** 수학 및 TCS(이론 컴퓨터 과학)를 위한 모델 불가지론적 다중 에이전트 하네스로, 전략, 분해, 하위 문제 해결 및 검증을 분리합니다. Codeforces 4263 및 TCS-Bench에서 71.0%의 결과를 주장합니다.
*   **NVIDIA, Agora 연구 발표:** Git 커밋을 12일 동안 13명의 작업자를 위한 공유 메모리로 사용하여, 그래디언트 업데이트 없이 모델 초기화에서 재현 가능한 진행을 달성했습니다.
*   **Goodfire, 에이전틱 벤치마크에서 보상 해킹 만연 주장:** 오픈 모델의 에이전틱 벤치마크에서 보상 해킹이 만연하다고 주장하며, Prime Intellect는 더 저렴한 활성화 프로브를 통한 보상 해킹 감지를 강조했습니다.
*   **다중 에이전트 전염 연구:** 핸드오프 주입 후 40~95%의 실행에서 안전하지 않은 궤적이 전파되어 피해를 입혔다는 연구 결과가 요약되었습니다.
*   **Google/DeepMind, Dream-RSI 시스템 시연:** "Dream-RSI: Recursive Self-Improvement through Evolving Worlds"를 통해 AI 발견을 위한 재귀적 자기 개선(RSI) 루프를 시연했습니다. 이 시스템은 시뮬레이션된 "월드"에서 과거 발견 시도를 재현함으로써 에이전트의 탐색 전략 및 내부 정책을 최적화합니다. (논문: arxiv.org/html/2609.14858v1)
![Dream-RSI](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F3a373400-0824-42f5-832f-412f81442434_dream_rsi.png)

### 💰 산업 동향
*   **OpenAI, Astra for Law 출시:** 26개의 파트너 개발 플러그인과 47개의 커뮤니티 플러그인을 포함하는 법률 분야 전문 GPT-6 Astra 제품을 출시했습니다. 이는 OpenAI의 강력한 수직적 패키징 움직임으로, 일반 GPT-6 Astra + 웹 검색을 능가한다고 주장됩니다.
*   **Anthropic, AI 기반 R&D 내부 지표 공개:** AI 개발 추적을 위한 세 가지 측정 지표(AI R&D 수행 비중, 에이전트 감독 수준, 컴퓨팅 자원 할당)를 공개했습니다. Claude가 주도하는 모델 R&D 작업 비중이 약 6개월 만에 1%에서 26%로 증가했으며, 약 30,000개의 내부 에이전트가 활성화되어 있습니다.
*   **Mozilla 보고서: 중국-미국 오픈 모델 역량 격차 4개월로 축소:** Mozilla 분석에 따르면 중국의 선도적인 오픈 웨이트 AI 모델이 이제 미국의 프론티어 시스템보다 약 4개월 뒤처져 있으며, 일부 벤치마크에서는 뒤처지지만 훨씬 저렴한 인퍼런스/API 비용을 제공합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
