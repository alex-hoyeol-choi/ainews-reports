# MiniMax 2.7: GLM-5 at 1/3 cost SOTA Open Model - 요약

**원문 URL**: https://www.latent.space/p/ainews-minimax-27-glm-5-at-13-cost
**번역일**: 2026-03-19 12:41
**발행일**: 2026-03-19

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 핵심 신규 소식 요약 브리핑입니다.

### 🔥 주요 뉴스
*   **MiniMax M2.7 출시** — MiniMax가 새로운 오픈 모델 M2.7을 출시했습니다. 이 모델은 Z.ai의 GLM-5와 필적하는 SOTA 성능을 보이며, GLM-5 대비 1/3 수준의 비용으로 효율성을 극대화했습니다. MiniMax는 M2.7이 "자체 진화에 깊이 참여한 최초의 모델"이라고 주장합니다.
    ![MiniMax M2.7 Performance Chart](https://substack-post-media.s3.amazonaws.com/public/images/0f6a39ab-2a8a-499d-898d-437396bd2f4b_3600x2114.png)
    ![MiniMax M2.7 Self-Evolution Claim](https://substack-post-media.s3.amazonaws.com/public/images/6f79d04e-0fdf-4940-90e0-9a7e5825f934_1280x673.jpeg)
*   **Xiaomi MiMo-V2-Pro 공개** — Xiaomi가 API 전용 추론 모델인 MiMo-V2-Pro를 선보였습니다. 이 모델은 Artificial Analysis Intelligence Index에서 49점을 기록하며, 1M 컨텍스트와 1M 토큰당 $1/$3의 가격으로 강력한 토큰 효율성과 낮은 환각률을 자랑합니다.
*   **Mamba-3 출시** — Cartesia가 인퍼런스 중심 세계에 최적화된 SSM인 Mamba-3를 발표했습니다. 초기 기술 반응은 Mamba-3를 트랜스포머 하이브리드 아키텍처에 통합하여 Gated DeltaNet과 같은 기존 구성 요소를 대체할 가능성에 주목하고 있습니다.
*   **Runway, 실시간 비디오 생성 미리보기 공개** — Runway가 NVIDIA와 공동 개발한 연구 미리보기를 통해 Vera Rubin 하드웨어에서 첫 프레임까지 100ms 미만의 시간으로 HD 비디오를 생성하는 기술을 시연했습니다. 이는 비디오 모델을 위한 질적으로 다른 상호작용 루프를 가능하게 할 잠재력이 있습니다.

### 📊 모델 & 벤치마크
*   MiniMax M2.7은 SWE-Pro에서 56.22%, Terminal Bench 2에서 57.0%의 성능을 달성했으며, OpenClaw에서 Anthropic Sonnet 4.6과 동등한 성능을 보였습니다. Artificial Analysis Intelligence Index에서 50점을 기록하며 GLM-5와 필적하고, GDPval-AA Elo 1494점으로 MiMo-V2-Pro, GLM-5, Kimi K2.5를 앞섰습니다.
*   Xiaomi MiMo-V2-Pro는 Artificial Analysis Intelligence Index에서 49점, GDPval-AA Elo 1426점을 기록했으며, 동급 모델 대비 강력한 토큰 효율성과 낮은 환각률로 AA-Omniscience 점수에서 +5점을 받았습니다.
*   Baidu는 테이블 추출, 수식 인식, 차트 이해 및 KIE를 단일 패스로 통합하는 4B 엔드투엔드 문서 인텔리전스 모델인 Qianfan-OCR을 소개했습니다.
*   Chandra OCR 2가 오픈소스화되었으며, olmOCR 벤치에서 85.9%의 성능을 보이고 90개 이상의 언어를 지원하며, 더 작은 4B 모델에서 강력한 레이아웃, 필기, 수학, 양식 및 테이블 지원을 제공합니다.
*   LLM-as-judge 평가의 재현성 문제가 제기되었습니다. GPT-5.2-as-judge와 GPT-5.1-as-judge 간에 모델 점수가 최대 10%에서 43.5%까지 차이를 보인다는 연구 결과가 발표되었습니다.

### 🛠️ 제품 & 도구
*   MiniMax는 엔터테인먼트 유스케이스를 위한 오픈소스 데모인 OpenRoom을 출시했습니다.
*   LangSmith는 보안 코드 실행을 위한 Sandboxes와 제품 내 디버깅 및 개선 지원을 위한 Polly GA를 출시했습니다.
*   Google Colab은 로컬 에이전트가 Colab GPU 런타임을 구동할 수 있도록 하는 오픈소스 MCP 서버를 공개했습니다.
*   Google Gemini API가 업데이트되어 단일 호출로 내장 도구와 커스텀 함수를 허용합니다.
*   Hugging Face는 커스텀 커널을 더 쉽게 공유하고 Hub를 통해 통합할 수 있도록 하는 새로운 커널 라이브러리를 출시했습니다.
*   Hugging Face는 에이전트에게 마크다운 논문 뷰를 제공하는 새로운 지원과 토큰 효율적으로 논문을 검색하고 읽기 위한 Paper Pages 스킬을 추가했습니다.
*   Microsoft의 최신 VS Code 릴리스는 엔드투엔드 웹 앱 워크플로우를 위한 통합 브라우저 디버깅 기능을 추가했습니다.
*   Hugging Face는 GUI 에이전트를 위한 ScreenSpot-Pro를 출시했습니다.

### 🔬 연구 & 논문
*   MiniMax는 M2.7이 반복 주기를 통해 소프트웨어 엔지니어링 작업을 최적화하고 내부 평가에서 30%의 성능 향상을 이끌어낸 "자율 반복 능력"을 갖춘 "자체 진화에 깊이 참여한 최초의 모델"이라고 주장합니다.
*   ZhihuFrontier는 전체 어텐션 잔차가 비대칭 통신/메모리 패턴으로 인해 파이프라인 병렬 처리에 부담을 주는 이유와 블록 어텐션 잔차 및 교차 스테이지 캐싱이 대칭성을 복원하는 방법을 분석했습니다.
*   MUVERA는 다중 벡터 리트리벌을 고정 차원 인코딩으로 압축하는 기술로, 약 70%의 메모리 감소와 훨씬 더 작은 HNSW 그래프를 달성했습니다.
*   사전 학습 중 SFT 데이터를 혼합하는 것이 표준 사전 학습-후-파인튜닝 파이프라인보다 성능이 우수할 수 있으며, 토큰 예산 내 비율에 대한 스케일링 법칙이 제시되었습니다.
*   Anthropic은 Claude를 사용하여 80,508명의 사용자에게 AI에 대한 희망과 두려움에 대해 인터뷰한 연구를 발표했습니다. 이는 동종 최대 규모의 정성적 연구입니다.

### 💰 산업 동향
*   OpenAI는 8×H100에서 10분 이내에 학습된 16MB 아티팩트에 최고의 LM을 맞추는 학습 챌린지인 Parameter Golf를 출시했으며, 100만 달러의 컴퓨팅 자원을 투입했습니다.
*   Arena는 평가 작업 자금 지원을 위한 학술 파트너십을 발표했습니다.

### ⚡ 인프라 & 하드웨어
*   Mamba-3는 인퍼런스 중심 세계에 최적화된 SSM으로 발표되어, 모델-시스템 공동 설계의 중요성을 강조합니다.
*   Runway의 실시간 비디오 생성 미리보기는 NVIDIA Vera Rubin 하드웨어에서 시연되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
