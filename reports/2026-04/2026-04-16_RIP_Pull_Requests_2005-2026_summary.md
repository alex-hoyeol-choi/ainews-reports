# RIP Pull Requests (2005-2026) - 요약

**원문 URL**: https://www.latent.space/p/ainews-rip-pull-requests-2005-2026
**번역일**: 2026-04-16 12:36
**발행일**: 2026-04-16

---

### 🔥 주요 뉴스
**[OpenAI Agents SDK 확장 및 하네스 오픈소스화]** — OpenAI는 Agents SDK를 장기 실행 및 내구성 있는 에이전트 방향으로 추진하며, 하네스를 오픈소스화하고 파트너 샌드박스에 실행을 위임할 수 있도록 했습니다. 이는 제3자가 'Codex 스타일' 에이전트를 쉽게 재현하고 오케스트레이션, 상태 관리, 보안 실행에서 차별화할 수 있도록 지원합니다.
**[Google/Gemini의 제품 대거 출시]** — Google은 Mac용 네이티브 Gemini 앱을 출시하고, 개인 인텔리전스를 Gemini 및 Chrome으로 확장했습니다. 또한, Audio Tags, 70개 이상 언어, SynthID 워터마킹을 지원하는 고도로 제어 가능한 Gemini 3.1 Flash TTS 모델과 Apache 2.0 라이선스의 파운데이션 텍스트-이미지 인코더 TIPS v2를 오픈소스화했습니다.
**[Cloudflare의 에이전트 인프라 'Project Think' 및 'Agent Lee' 출시]** — Cloudflare는 내구성 있는 실행, 서브에이전트, 샌드박스 코드 실행 등을 특징으로 하는 차세대 Agents SDK인 Project Think을 소개했습니다. 동시에 Cloudflare UI를 프롬프트 기반 작업으로 전환하는 대시보드 내 에이전트 Agent Lee를 출시하고, 실시간 음성 파이프라인 및 브라우저 자동화 툴링을 핵심 스택으로 통합했습니다.
**[GPT-5.4 Pro의 수학 난제 증명]** — GPT-5.4 Pro가 Erdős 문제 #1196에 대한 새로운 증명을 생성하여 전문가들을 놀라게 했습니다. 이는 AI가 수학 분야에서 비직관적이지만 간결한 해결 경로를 찾아낼 수 있음을 보여주는 중요한 연구 결과로 평가됩니다.
**[NVIDIA의 Nemotron 3 Super 공개]** — NVIDIA는 1200억 파라미터의 오픈 하이브리드 Mamba-Attention MoE 모델인 Nemotron 3 Super를 공개했습니다. 이 모델은 120억 활성 파라미터, 1M 컨텍스트, 25조 토큰으로 학습되었으며, 기존 모델 대비 최대 7.5배 높은 처리량을 제공합니다.

### 📊 모델 & 벤치마크
*   Nucleus-Image가 최초의 스파스 MoE 디퓨전 모델로 발표되었습니다: 170억 파라미터, 20억 활성, Apache 2.0 라이선스로 가중치, 학습 코드, 데이터셋 레시피가 공개되었으며 diffusers에서 출시 당일 지원됩니다.
*   webAI-ColVec1이 OCR이나 전처리 없이 문서 리트리벌에서 ViDoRe V3 최고 성능을 주장하며 오픈소스화되었습니다.
*   Google의 Gemini 3.1 Flash TTS 모델이 Audio Tags, 70개 이상 언어, 인라인 비언어적 단서, 다중 스피커 지원, SynthID 워터마킹을 갖춘 고도로 제어 가능한 TTS 모델로 출시되었습니다. 독립 평가에서 Speech Arena 2위를 차지했습니다.
*   Google은 새로운 사전 학습 레시피를 포함한 Apache 2.0 라이선스의 파운데이션 텍스트-이미지 인코더인 TIPS v2를 오픈소스화했습니다.
*   METR Evals는 Gemini 3.1 Pro (고도 사고)가 소프트웨어 작업에서 약 6.4시간의 50% 시간 지평을 가졌다고 추정했습니다.
*   Document Arena 상위 순위가 Claude Opus 4.6 Thinking이 1위, Kimi-K2.5 Thinking이 최고의 오픈 모델로 변경되었습니다.

### 🛠️ 제품 & 도구
*   GitHub은 오픈소스 레포에서 Pull Request를 비활성화할 수 있도록 허용하기 시작했습니다.
*   OpenAI는 Agents SDK를 파일/컴퓨터 사용, 스킬, 메모리, 컴팩션을 위한 프리미티브를 갖춘 장기 실행 및 내구성 있는 에이전트 방향으로 추진했으며, 하네스를 오픈소스화하고 파트너 샌드박스에 실행을 위임할 수 있도록 했습니다.
*   Cloudflare는 내구성 있는 실행, 서브에이전트, 영구 세션, 샌드박스 코드 실행, 내장 워크스페이스 파일 시스템, 런타임 툴 생성을 특징으로 하는 차세대 Agents SDK인 Project Think을 소개했습니다.
*   Cloudflare는 샌드박스 TypeScript를 사용하여 Cloudflare의 UI를 프롬프트 기반 작업으로 전환하는 대시보드 내 에이전트인 Agent Lee를 출시했습니다.
*   Cloudflare는 연속적인 STT/TTS를 위한 WebSockets를 통한 실험적인 실시간 음성 파이프라인을 출시했으며, 리브랜딩된 Browser Run 스택(Live View, 휴먼-인-더-루프 개입, 세션 기록, CDP 엔드포인트, WebMCP 지원)을 요약했습니다.
*   Hermes Agent는 단순히 툴 사용을 넘어 완료된 워크플로우를 재사용 가능한 스킬로 자동 전환하는 자체 개선 워크플로우를 선보였습니다.
*   Hermes Agent는 /browser connect를 통한 브라우저 제어, QQBot + AWS Bedrock 지원, 네이티브 Swift 데스크톱 앱 알파 버전을 추가했습니다.
*   Google은 Option + Space 활성화, 화면 공유, 로컬 파일 컨텍스트, 네이티브 Swift 구현을 제공하는 Mac용 네이티브 Gemini 앱을 출시했습니다.
*   Google은 개인 인텔리전스를 Gemini에서 전 세계적으로, 그리고 Chrome으로 확장하여 사용자가 Gmail 및 Photos와 같은 제품의 시그널을 연결할 수 있도록 했습니다.
*   Yoonho Lee는 사용자가 새로운 도메인에서 견고한 하네스를 구현하는 데 도움이 되는 레포인 Meta-Harness를 오픈소스화했습니다.

### 🔬 연구 & 논문
*   GPT-5.4 Pro가 Erdős 문제 #1196에 대한 증명을 생성했으며, 이는 오랫동안 가정되었던 증명 전략을 거부하고 폰 망골트 함수를 활용하여 전문가들을 놀라게 했습니다.
*   NVIDIA는 프레임별 3D 지오메트리를 유지하고 자체 증강 학습을 사용하여 시간적 드리프트를 줄이는 영구적이고 탐색 가능한 3D 월드를 생성하기 위한 프레임워크인 Lyra 2.0을 발표했습니다.
*   Hayden Prairie, Dan Fu, Together Compute는 안정화된 레이어 루핑 트랜스포머 공식인 Parcae를 소개했습니다. 이는 고정된 파라미터 예산에서 루핑 블록이 대략 2배 크기의 모델 품질을 회복할 수 있다고 주장합니다.
*   NVIDIA는 1200억 파라미터의 오픈 하이브리드 Mamba-Attention MoE 모델인 Nemotron 3 Super를 공개했습니다. 이 모델은 120억 활성 파라미터, 1M 컨텍스트, 25조 토큰으로 학습되었으며, GPT-OSS-120B 대비 최대 2.2배, Qwen3.5-122B 대비 7.5배의 처리량을 제공합니다.
*   Omar Sar는 얇은 오케스트레이터가 파일-애즈-버스 패턴에서 영구 워크스페이스 아티팩트를 통해 전문 에이전트들을 조율하는 AiScientist를 요약했습니다.
*   Dair.ai는 지속적인 소형 모델 개선 루프를 위한 Pioneer Agent를 강조했습니다.

### 💰 산업 동향
*   Cloudflare, Modal, Daytonaio, E2B, Vercel Dev 모두 OpenAI Agents SDK의 공식 샌드박스 통합을 발표했습니다.
*   TeraflopAI는 430억 토큰의 SEC EDGAR 데이터를 출시하여 오픈 데이터셋 및 오픈 인프라 추진을 강화했습니다.

### ⚡ 인프라 & 하드웨어
*   NVIDIA의 Nemotron 3 Super 모델은 1M 컨텍스트와 25조 토큰으로 학습되었으며, GPT-OSS-120B 대비 최대 2.2배, Qwen3.5-122B 대비 7.5배의 처리량을 제공하여 메모리 대역폭과 긴 컨텍스트 처리 효율성을 강조했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
