# Gemini 4 Argon: GDM’s answer to Astra/Fable, with 1M output - 요약

**원문 URL**: https://www.latent.space/p/ainews-gemini-4-argon-gdms-answer
**번역일**: 2026-10-01 12:29
**발행일**: 2026-10-01

---

### 🔥 주요 뉴스
**[Google DeepMind, Gemini 4 Argon 출시 및 1M 토큰 출력 지원]** — Google DeepMind가 코딩, 기업 지식 작업 및 사이버 방어를 위한 Gemini 4 Argon을 공개했습니다. 이 모델은 업계 최초로 최대 1M 출력 토큰을 지원하는 실험적인 Long Decode Continuation 기능을 제공하며, 19개 공개 벤치마크 중 13개에서 SOTA를 달성했습니다. 초기 접근은 Fairwind Program의 정부 사용자 및 신뢰할 수 있는 사이버 방어자로 제한됩니다.
![X avatar for @GoogleDeepMind](https://pbs.substack.com/profile_images/1695024885070737408/-M-HSH5P.jpg)
**[OpenAI, GPT-6.1 Sol 및 에이전트 스택 공개]** — OpenAI는 MathArena에서 새로운 1위를 차지한 GPT-6.1 Sol을 출시했습니다. 또한 DevDay를 통해 자체 클라우드 컴퓨터를 가진 영구 에이전트인 'dots', Decisions API, 컴퓨터 사용 기능을 포함한 새로운 에이전트 스택을 소개하며, 최대 300 토큰/초의 초고속 인퍼런스 속도를 언급했습니다.
**[GLM-5.3, 높은 사이버 역량과 로컬 인퍼런스 지원]** — Zhipu/Z.ai의 오픈 웨이트 GLM-5.3이 ExploitBench에서 50/410개의 엔드투엔드 V8 익스플로잇을 기록하며 Anthropic의 Claude Mythos Preview에 근접한 자율 사이버 역량을 보였습니다. ggml-org/llama.cpp에 GLM-5.3-Flash / GLM5-Next 지원이 추가되어 320B 하이브리드 텍스트+비전 모델의 로컬 인퍼런스가 가능해졌습니다.
**[OpenAI, Moonshot AI 연관 추론 추출 캠페인 적발]** — OpenAI는 Moonshot AI와 관련된 개인들이 이틀 동안 4천 명 이상의 사용자로부터 1만 6천 건의 시도를 포함하는 숨겨진 추론 추출 캠페인을 벌였다고 밝혔습니다. 이 공격은 Astra 모델에서도 이번 주까지 작동했으며, 패치 전파에 어려움이 있었습니다.

### 📊 모델 & 벤치마크
*   **Gemini 4 Argon:** GPT-6 Astra 및 Claude Opus 5.5에 대한 19개 공개 벤치마크 중 13개에서 1위를 차지했으며, DeepSWE에서 77.9%를 기록했습니다. Artificial Analysis Intelligence Index에서 53점을 기록하여 GPT-6 Astra와 동률을 이루었고, AA-Omniscience에서의 환각 비율은 15%로 Astra의 51%보다 낮았습니다. Vals Index에서 68.9%로 1위를 차지했으며, 30개의 Vibe Code Bench 앱을 완벽하게 구축했습니다.
*   **GPT-6.1 Sol:** MathArena에서 새로운 1위를 차지했으며, Code Arena WebDev에서 1759점으로 3위를 기록하여 GPT-6 Sol보다 70점 앞섰습니다.
*   **GPT-6 Luna:** 이미지 인코딩 버그 수정으로 Intelligence Index 1점이 추가되었습니다.
*   **GLM-5.3:** ExploitBench에서 50/410개의 엔드투엔드 V8 익스플로잇을 기록하여 Claude Mythos Preview의 56/410에 근접한 자율 사이버 역량을 보였습니다.
*   **Ling-3.1-flash:** 500B 모델로, GPT-5.6 Sol 및 Opus 5에 근접한다고 보고되었으며, Mobile App Arena에서 오픈 웨이트 모델 중 2위를 차지했습니다.
*   **Solar Mini 4 (Upstage):** 총 350억 / 활성 30억 파라미터를 보고했으며, Intelligence Index에서 24점을 기록했습니다.
*   **AA-Video-T2V v2.0 (Artificial Analysis):** 6만 8천 개 이상의 인간 투표로 1080p에서 평가된 새로운 비디오 벤치마크가 출시되었으며, Wan 3.0이 분당 $12로 1위를 차지했습니다. Utopai X (MiniMax H3의 후속 학습 모델)가 2위로 데뷔했습니다.

### 🛠️ 제품 & 도구
*   **Gemini 4 Argon:** 최대 1M 출력 토큰을 지원하는 Long Decode Continuation 기능을 포함하며, 표준 가격은 1M 입력/출력 토큰당 $4/$20입니다.
*   **OpenAI DevDay 에이전트 스택:** 자체 클라우드 컴퓨터를 가진 영구 에이전트인 'dots', Decisions API, 컴퓨터 사용 기능을 소개했습니다.
*   **ChatGPT Sites:** 이제 MCP 서버를 호스팅하고 이를 설치 가능한 플러그인으로 전환할 수 있습니다.
*   **Perplexity pplx-embed-v2-context-9b-preview:** Hugging Face에 공개된 새로운 컨텍스트 임베딩 모델로, 전체 문서를 한 번 인코딩한 후 청크 벡터를 풀링하는 방식을 사용합니다.
*   **Cohere Embed 5:** Pro 및 Fast 변형을 포함하는 새로운 임베딩 제품군으로, 공유 임베딩 공간에서 인덱싱 및 리트리벌이 가능합니다.
*   **Ideogram 4.5:** 아티팩트 없는 다중 턴 편집을 목표로 하는 편집 모델로, 오픈 웨이트를 약속했습니다.
*   **Praxis-1 (Runway):** 로보틱스 정책 성능이 3인칭 비디오와 예측 가능하게 스케일링되는 오픈 웨이트 월드 액션 모델을 출시했습니다.
*   **Cloudflare 에이전트 샌드박스:** 에이전트용 컨테이너를 재구축하여 p50 상호작용까지 걸리는 시간을 648ms로 6배 단축했으며, 스냅샷 기능은 베타 버전입니다.
*   **Cloudflare AutoRouter:** 내부 테스트에서 약 30% 낮은 지출을 보인 모델 라우터입니다.
*   **SynthID Bio (Google DeepMind):** AI 생성 단백질에 대한 워터마킹 기술이 Nature에 게재되었으며, 오픈소스 툴이 함께 제공됩니다.

### 🔬 연구 & 논문
*   **Context Language Models (Meta):** CLM은 컨텍스트를 편집 가능한 파일로 취급하고 가중치에 학습된 컨텍스트 관리 정책을 사용하여, 24시간 멀티 리포지토리 에이전트 스웜 작업에서 동일한 컴퓨팅으로 65% 더 높은 점수를 기록했습니다.
*   **TaH2 (적응형 추론 컴퓨팅):** 룩어헤드 뎁스 슈퍼비전은 모델에게 어떤 하드 토큰이 추가 루프를 받을 자격이 있는지 가르쳐, 일치하는 테스트 시간 컴퓨팅에서 정확도 3.4%p 증가와 53% 더 가파른 스케일링 슬로프를 보고합니다.
*   **AutoBenchmark (Meta):** 벤치마크 생성을 자동화하는 프로젝트로, 아이디어 구상 단계에서의 인간 피드백이 에이전트 단독 작업보다 우수함을 보여줍니다.
*   **Stratego (Nature 논문):** RL과 불완전 정보 하의 테스트 시간 컴퓨팅을 기반으로 구축된 최초의 초인적인 Stratego AI를 제시하는 Nature 논문이 발표되었습니다.
*   **프리필/디코드 분리 (연구):** 새로운 정상 상태 분석은 분리가 동일한 배치 크기와 처리량에서 평균 상호작용성을 약 1/(디코드 시간 비율)만큼 증가시킨다고 주장합니다.
*   **AI as Compiler (연구):** 모델이 Triton을 PTX로 직접 번역하며, 검증기가 정확성, 경쟁 조건 및 교착 상태를 확인합니다. B200에서 FlashAttention에 대한 속도 향상이 1.37배에 달합니다.
*   **에이전트 보고서 (프리프린트 논문):** LLM이 작성한 에이전트 작업 보고서의 투명성에 의문을 제기하는 새로운 프리프린트 논문이 발표되었습니다.

### 💰 산업 동향
*   **Factory vs Cognition 분쟁:** Factory는 고문 Chris Degnan이 Cognition 이사회 회의에 참석하며 기밀을 누설했다고 주장하며 해임했으며, Cognition은 같은 날 Degnan을 CRO로 발표했습니다.
*   **Greg Brockman 정치 자금 기부 철회:** Greg Brockman은 Leading the Future 슈퍼 PAC에 약속했던 두 번째 2,500만 달러 기부를 철회했습니다.
*   **OpenAI 재정 현황 (NYT 보도):** OpenAI가 연간 매출 700억 달러에 육박하며, 1조 4천억 달러 기업 가치로 300억 달러를 조달하기 위한 협상 중이며, IPO는 내년으로 연기되었다고 보도되었습니다.
*   **Flow, 5천만 달러 시리즈 B 자금 조달:** 하드웨어 엔지니어링을 위한 AI 툴링을 구축하는 Flow가 7억 5천만 달러 기업 가치로 5천만 달러 시리즈 B 자금을 조달했습니다.
*   **Apollo Research, 임베디드 평가 원칙 발표:** 프론티어 랩에 직원과 유사한 접근 권한을 받는 외부 평가자를 위한 원칙을 발표했습니다.

### ⚡ 인프라 & 하드웨어
*   **Huawei DeepSeek:** Ascend 950에 최적화된 TileLang을 포함한 오픈소스 Ascend 툴킷을 출시했습니다.
*   **Vera Rubin (Cognition/CoreWeave):** Cognition이 CoreWeave를 통해 Vera Rubin의 첫 고객이 되었으며, 동일한 디코드 속도에서 GB200의 토큰 처리량의 약 4.8배를 보고했습니다.
*   **DFlash 드래프트 (Ornith-1.5):** 새로운 드래프트 모델이 최대 2.54배의 무손실 속도 향상을 제공합니다.
*   **llama.cpp GLM-5.3-Flash / GLM5-Next 지원:** ggml-org/llama.cpp#27773 PR이 병합되어 320B 하이브리드 텍스트+비전 모델에 대한 로컬 인퍼런스를 가능하게 했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
