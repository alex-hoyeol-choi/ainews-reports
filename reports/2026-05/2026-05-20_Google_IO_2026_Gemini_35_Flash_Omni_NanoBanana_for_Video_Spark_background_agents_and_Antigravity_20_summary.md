# Google I/O 2026: Gemini 3.5 Flash, Omni (NanoBanana for Video), Spark (background agents), and Antigravity 2.0 - 요약

**원문 URL**: https://www.latent.space/p/ainews-google-io-2026-gemini-35-flash
**번역일**: 2026-05-20 06:20
**발행일**: 2026-05-20

---

### 🔥 주요 뉴스
**[Google, Gemini 3.5 Flash 및 Omni 공개]** — Google이 I/O에서 Gemini 3.5 Flash를 즉시 GA하며 에이전트 및 코딩 워크로드에 최적화된 강력한 성능과 빠른 속도를 제공한다고 발표했습니다. 또한 멀티모달 생성/편집을 위한 Gemini Omni를 선보이며 영상 생성 및 편집 기능을 강화했습니다.
**[Google, Antigravity 2.0 에이전트 스택 확장]** — Google은 에이전트 중심의 데스크톱 앱, CLI, SDK를 포함하는 Antigravity 2.0을 출시하여 에이전트 실행 환경을 강화했습니다. Gemini API의 Managed Agents를 통해 호스팅된 Linux 샌드박스에서 에이전트 실행을 지원합니다.
**[Andrej Karpathy, Anthropic 합류]** — AI 분야의 저명한 연구자인 Andrej Karpathy가 Anthropic에 합류하여 R&D 및 새로운 사전 학습(pretraining) 중심 노력에 참여할 예정입니다.
**[OpenAI, Guaranteed Capacity 도입]** — OpenAI는 고객이 중요한 워크로드를 위해 장기적인 컴퓨팅 자원을 확보할 수 있도록 1~3년 약정으로 할인된 토큰을 제공하는 상업적 제안인 Guaranteed Capacity를 발표했습니다.
**[Hugging Face, Carbon DNA 모델 공개]** — Hugging Face는 생성형 DNA 파운데이션 모델 제품군인 Carbon을 출시했습니다. Carbon-3B는 Evo2-7B와 유사한 성능을 보이며 250-275배 빠른 인퍼런스 속도로 단일 GPU에서 이틀 내에 전체 인간 게놈을 처리할 수 있습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/904f7a4e-f945-40e0-b980-024fc220d0b7_1524x912.png)

### 📊 모델 & 벤치마크
*   Google은 Gemini 3.5 Flash를 즉시 GA했으며, 1M 토큰 컨텍스트, 65k 최대 출력 토큰, 4단계 사고 레벨, 다중 턴 대화 전반에 걸친 thought preservation 기능을 제공합니다.
*   Gemini 3.5 Flash는 Terminal-Bench 2.1에서 76.2%, GDPval-AA에서 1656 Elo, MCP Atlas에서 83.6%, MMMU-Pro에서 84%의 성능을 기록했습니다.
*   Google은 Gemini 3.5 Flash가 유사한 프론티어 모델보다 4배 빠르며, Antigravity에서는 최대 12배 빠르다고 밝혔고, Artificial Analysis는 >280 output tok/s를 관찰했습니다.
*   Gemini 3.5 Flash의 가격은 1M 입력 토큰당 $1.50, 1M 출력 토큰당 $9.00이며, 캐시된 입력에 90% 할인이 적용됩니다.
*   Arena 벤치마크에서 Gemini 3.5 Flash는 Text Arena에서 #9위, Code Arena: Frontend에서 #9위를 기록하며 1507점으로 Gemini 3 Flash 대비 +70점 상승했습니다.
*   Hugging Face는 생성형 DNA 파운데이션 모델 Carbon을 출시했으며, Carbon-3B는 Evo2-7B와 유사한 성능을 보이면서 250-275배 빠른 인퍼런스 속도로 단일 GPU에서 이틀 내에 전체 인간 게놈을 처리할 수 있습니다.

### 🛠️ 제품 & 도구
*   Google은 Gemini Omni Flash를 유료 Gemini 사용자에게 Gemini 앱 및 Flow에서 오늘부터 제공하며, YouTube Shorts/Create에서는 이번 주부터 무료로, 몇 주 내로 API를 통해 제공할 예정입니다.
*   Antigravity 2.0 데스크톱 앱, CLI, SDK가 출시되었으며, Gemini API의 Managed Agents는 Bash/Python/Node, 파일, 브라우징, 커스텀 스킬, repo/GCS 마운트를 지원하는 호스팅된 Linux 샌드박스를 제공합니다.
*   Google Search는 AI 기반 Search 박스를 재설계하고 멀티모달 쿼리를 지원하며, Antigravity + Gemini 3.5 Flash를 사용하여 즉석에서 맞춤형 시각 도구 및 시뮬레이션을 생성하는 기능을 선보였습니다.
*   Google Search는 지속적인 모니터링 작업, 웹/뉴스/소셜/실시간 신호를 기반으로 종합 업데이트를 제공하는 정보 에이전트를 올 여름 Pro/Ultra 사용자에게 출시할 예정입니다.
*   Gemini 앱은 새로운 "Neural Expressive" 디자인 언어, 인라인/즉시 Gemini Live 음성, 받은 편지함/캘린더/작업에서 개인화된 Daily Brief 요약 기능을 포함합니다.
*   Gemini Spark는 전용 Google Cloud 가상 머신에서 24시간 내내 작동하여 사용자 장치가 꺼져 있어도 장시간 실행되는 작업을 허용하는 개인 AI 에이전트입니다.
*   Gemini macOS 앱이 출시되었으며, Spark/음성 데스크톱 워크플로우가 곧 제공될 예정입니다.
*   GitHub Copilot에 Gemini 3.5 Flash가 통합 출시되었으며, Cursor는 Jira와의 통합을 출시하여 클라우드 에이전트가 작업 항목을 가져와 병합 준비된 PR을 생성할 수 있도록 했습니다.
*   Code/VS Code 또한 Gemini 3.5 Flash의 가용성을 발표했습니다.

### 🔬 연구 & 논문
*   Google은 연구자들을 위한 프로토타입 스위트인 Gemini for Science를 소개했으며, 이는 Literature Insights, Hypothesis Generation, Computational Discovery (AlphaEvolve 및 ERA 기반)를 포함합니다.
*   Google Research는 ERA가 Nature에 출판되었다고 언급했습니다.
*   Google Project Genie는 Street View 기반 다지기(grounding)를 사용하여 약 20년간의 지도 이미지를 통해 인터랙티브한 실제 위치 시뮬레이션을 생성합니다.
*   METR은 Anthropic, Google, Meta, OpenAI에 대한 접근을 기반으로 한 첫 번째 프론티어 리스크 보고서를 발표했으며, 모델 CoT 및 기능, 정렬, 제어에 대한 비공개 정보를 포함합니다.

### 💰 산업 동향
*   Google은 현재 월 3.2 경(quadrillion) 토큰 이상을 처리하며, 이는 전년 대비 7배 증가한 수치라고 밝혔습니다.
*   Google Gemini 앱은 월 9억 명 이상의 사용자를 보유하고 있으며 230개 이상의 국가와 70개 이상의 언어로 제공됩니다.
*   Google은 새로운 월 $100 요금제를 도입하고, 최고 티어 Ultra의 월 요금을 $250에서 $200로 인하하는 새로운 가격 체계를 발표했습니다.
*   Andrej Karpathy가 Anthropic에 합류하여 R&D 및 새로운 사전 학습(pretraining) 중심 노력에 참여할 예정입니다.
*   OpenAI는 고객이 중요한 워크로드를 위해 장기적인 컴퓨팅 액세스를 확보할 수 있도록 하는 상업적 제안인 Guaranteed Capacity를 발표했습니다.
*   Google은 Search, Gemini, Chrome, 하드웨어/미디어 서비스 전반에 걸쳐 SynthID를 추진하며, OpenAI, NVIDIA, Kakao, ElevenLabs와의 파트너십을 통해 이들의 생성된 콘텐츠에 SynthID를 적용할 예정입니다.
*   OpenAI는 SynthID 워터마크와 C2PA 자격 증명을 통해 OpenAI가 생성한 이미지를 확인하는 지원을 별도로 발표했습니다.
*   Steven Adler와 Page Hedley가 공동 설립한 새로운 AI 안전 표준 조직인 Guidelight가 첫 두 가지 표준을 공개했습니다.

### ⚡ 인프라 & 하드웨어
*   Google은 현재 월 3.2 경(quadrillion) 토큰 이상을 처리하며, 이는 전년 대비 월 480조(trillion) 토큰에서 7배 증가한 수치라고 밝혔습니다.
*   Gemini Spark는 전용 Google Cloud 가상 머신에서 실행되어 사용자 장치가 꺼져 있어도 장시간 실행되는 작업을 허용합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
