# Dreamer joins Meta Superintelligence Labs — 9 month retro of Personal Superintelligence - 요약

**원문 URL**: https://www.latent.space/p/ainews-dreamer-joins-meta-superintelligence
**번역일**: 2026-03-24 07:18
**발행일**: 2026-03-24

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 간결한 한국어 브리핑입니다.

### 🔥 주요 뉴스
**[Meta, 개인 초지능 에이전트 개발 가속화]** — Meta Superintelligence Labs(MSL)가 개인 지능형 에이전트 기술을 보유한 Dreamer를 'execuhire'했습니다. 이는 12월의 Manus 20억 달러 인수 이후 Meta가 소비자 에이전트 역량을 강화하기 위한 전략적 움직임입니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/7af96441-4647-4d95-8ff4-9a507e6a50d8_1192x1348.png)
**[Anthropic Claude, macOS 데스크톱 제어 기능 출시]** — Claude는 이제 Claude Cowork 및 Claude Code를 통해 macOS 연구 프리뷰에서 마우스, 키보드, 화면을 제어하여 임의의 앱을 조작할 수 있습니다. 이는 에이전트의 작업 표면을 API 및 브라우저 샌드박스를 넘어 크게 확장한 것입니다.
**[JEPA 기반 LeWorldModel, 월드 모델 학습 간소화]** — LeWorldModel은 교사-학생 트릭이나 복잡한 휴리스틱 없이 픽셀에서 직접 안정적인 엔드투엔드 JEPA 학습을 구현했습니다. 15M 파라미터, 1 GPU로 1초 미만의 플래닝이 가능하며, 기존 월드 모델 대비 약 48~50배 빠른 플래닝 속도를 보입니다.
**[Meta, 자기 개선 에이전트 연구 발전]** — Hyperagents / DGM-H는 에이전트가 작업 행동뿐만 아니라 미래 개선을 생성하는 절차까지 개선할 수 있도록 Darwin Gödel Machine 아이디어를 확장했습니다. 이는 이전 자기 개선 시스템의 주요 한계를 해결하는 메타 수준의 개선입니다.
**[Cursor, 코딩 에이전트 위한 Instant Grep 출시]** — Cursor는 수백만 개의 파일에 대한 정규식 검색을 밀리초 단위로 수행하는 Instant Grep을 출시했습니다. 이는 코딩 에이전트가 대규모 레포지토리를 효율적으로 탐색하는 데 중요한 검색 레이턴시 병목 현상을 해결합니다.

### 📊 모델 & 벤치마크
*   **Sakana AI, 일본어 특화 Namazu alpha 모델 및 Sakana Chat 출시:** 일본 사용자를 위한 Sakana Chat을 출시했으며, 이는 업스트림 편향을 줄이고 일본의 맥락과 가치를 반영하도록 파인튜닝된 새로운 Namazu alpha 모델 제품군을 기반으로 합니다.
*   **Luma Uni-1, 새로운 생성형 미디어 모델 공개:** Luma는 "동시에 픽셀을 생각하고 생성하는" 모델로 홍보되는 Uni-1을 공개했습니다.
*   **NVIDIA Kimodo, 프롬프트 가능한 모션/타임라인 모델 출시:** 700시간의 모션 캡처 데이터로 학습된 Kimodo는 인간 및 로봇 스켈레톤을 모두 지원하며 Hugging Face에서 사용할 수 있습니다.
*   **WebArena-Infinity, 에이전트 벤치마크 환경 생성 비용 대폭 절감:** 브라우저 환경 구축 비용을 각 환경당 10시간 미만, 100달러 미만으로 줄였으며, 기존 WebArena/OSWorld보다 더 어렵고 검증 가능한 브라우저 사용 작업을 생성합니다.

### 🛠️ 제품 & 도구
*   **Anthropic Claude, macOS 데스크톱 제어 기능 출시:** Claude는 Claude Cowork 및 Claude Code를 통해 macOS 연구 프리뷰에서 마우스, 키보드, 화면을 제어하여 임의의 앱을 조작할 수 있습니다.
*   **에이전트 스택, 장기 실행 워크플로우로 수렴:** Hermes Agent, 통합 브라우저 및 터미널 기능을 추가한 T3 Code, 다중 에이전트 병렬 실행을 위한 Command Center, 자율 작업을 위한 Parchi / BYOK 워크플로우 등 에이전트 하네스 레이어가 성숙하고 있습니다.
*   **Google Devs 및 LlamaIndex, LlamaParse + Gemini 3.1 Pro 통합으로 문서 파싱 정확도 향상:** 어려운 금융 PDF에서 구조화된 데이터를 추출하는 워크플로우를 강조하며, 복잡한 표에서 약 15%의 정확도 향상을 주장했습니다.
*   **LlamaIndex, 경량 파싱 도구 LiteParse 출시:** URL 및 스트림을 지원하고 VLM 의존성 없이 더 가벼운 파싱 경로를 목표로 하며, 에이전트가 저렴하고 빠르게 호출할 수 있도록 설계되었습니다.
*   **Cursor, 코딩 에이전트 위한 Instant Grep 출시:** 수백만 개의 파일에 대한 정규식 검색을 밀리초 단위로 수행하며, 인덱싱/알고리즘 트레이드오프에 대한 기술 문서를 함께 공개했습니다.
*   **MiniMax, 멀티모달 API 통합 구독 "Token Plan" 도입:** 텍스트, 음성, 음악, 비디오, 이미지 API를 하나의 정액제 구독으로 제공하며, 예측 가능한 청구 및 타사 하네스와의 호환성을 강조합니다.
*   **TRL v1.0.0, 긴 시퀀스 학습에서 VRAM 최대 44배 절약:** AsyncGRPO 출시를 앞두고 긴 시퀀스 학습에서 최대 44배의 VRAM 절약을 주장하는 TRL v1.0.0이 출시되었습니다.
*   **AI2, VLM 기반 GUI 자동화 도구 MolmoPoint GUI 공개:** 좌표 회귀 대신 그라운딩 토큰을 사용하여 VLM 기반 GUI 자동화를 목표로 하며, ScreenSpotPro에서 61.1점을 기록했습니다.

### 🔬 연구 & 논문
*   **Meta, 자기 개선 에이전트 연구 발전 (Hyperagents / DGM-H):** 에이전트가 작업 행동뿐만 아니라 미래 개선을 생성하는 절차까지 개선할 수 있도록 Darwin Gödel Machine 아이디어를 확장했습니다.
*   **Meta, RLLM = RL + LM-as-RM을 통한 RL 후속 학습 통합:** 정책 자체의 출력에서 온-폴리시(on-policy)로 언어 모델 보상 모델을 학습시켜, 다양한 작업 전반에 걸쳐 후속 학습을 통합하는 것을 목표로 합니다.
*   **JEPA 기반 LeWorldModel, 월드 모델 학습 간소화:** 15M 파라미터, 1 GPU로 1초 미만의 플래닝이 가능하며, 기존 월드 모델 대비 약 48~50배 빠른 플래닝 속도를 보입니다.
*   **Anthropic, LLM의 생물학적 해석 가능성 연구:** "On the Biology of a Large Language Model" 요약 스레드는 기계적 해석 가능성이 회로와 내부 특징을 구체적인 수준으로 밝혀내고 있음을 설명했습니다.
*   **학습 이론 및 옵티마이저 스케일링 연구:** Antonio Orvieto의 스레드는 적응형 방법론을 위한 최적화 이론이 알려진 LLM 하이퍼파라미터 스케일링의 많은 부분을 설명하며, 무차별 대입 탐색 없이 전이 규칙을 제안할 수 있다고 주장했습니다.
*   **후기 상호작용 / 다중 벡터 리트리벌 연구 주목:** Weaviate/LightOn 논의는 토큰 수준의 다중 벡터 표현을 사용하는 후기 상호작용 시스템이 코드 및 추론 중심 리트리벌에 실용적이며, 리콜 및 랭킹 품질을 향상시킨다고 주장했습니다.

### 💰 산업 동향
*   **Meta, 개인 초지능 에이전트 개발 가속화:** Meta Superintelligence Labs(MSL)가 개인 지능형 에이전트 기술을 보유한 Dreamer를 'execuhire'했습니다. 이는 12월의 Manus 20억 달러 인수 이후 Meta가 소비자 에이전트 역량을 강화하기 위한 전략적 움직임입니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
