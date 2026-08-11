# Muse Glimmer and Spark: Open Weights return Personal Superintelligence promise - 요약

**원문 URL**: https://www.latent.space/p/ainews-muse-glimmer-and-spark-open
**번역일**: 2026-08-11 06:04
**발행일**: 2026-08-11

---

### 🔥 주요 뉴스
**Meta Muse Glimmer 30B 출시** — Meta는 Apache 2.0 라이선스 기반의 30B 규모 오픈 웨이트 멀티모달 에이전트 모델 Muse Glimmer를 출시했습니다. 이 모델은 로컬 에이전트 워크플로우에 최적화되어 소비자 하드웨어에서 실행 가능하며, 텍스트+이미지 인터리브 입력과 100개 이상의 언어를 지원합니다.
**OpenAI GPT-5.6-Cyber 출시** — OpenAI는 고급 방어 작업에 특화된 GPT-5.6-Cyber 모델을 출시하고 Daybreak 사이버 보안 이니셔티브를 확장했습니다. 이 모델은 오픈소스 소프트웨어 및 Chrome V8에서 알려지지 않은 버그를 발견하는 등 실제 취약점 연구에 활용되었습니다.
**Anthropic Claude 수학 능력 향상** — Anthropic은 미공개 연구용 Claude 변형 모델이 리만 가설 관련 하한을 41.6%에서 67.2%로 개선했다고 보고했습니다. 이 모델은 3,100만 개 이상의 출력 토큰에 걸쳐 반복적인 재시도와 대규모 탐색을 사용했습니다.
**MiniMax H3 오픈 웨이트 비디오 모델 추진** — MiniMax는 오픈 웨이트 비디오 모델 H3의 커뮤니티 채택을 가속화하며, 양자화, 오프로딩, Context-IR, 소비자 GPU 배포 및 LoRA 지원 등 생태계 지원을 강화하고 있습니다.

### 📊 모델 & 벤치마크
*   Meta Muse Glimmer 30B: Apache 2.0 라이선스의 30B 멀티모달 에이전트 모델 Glimmer를 출시했습니다. Artificial Analysis에 따르면 인텔리전스 인덱스 35점, 개방성 인덱스 44점을 기록했으며, 128K 컨텍스트와 4비트 양자화 시 약 18GB 메모리를 사용합니다.
    ![X avatar for @AIatMeta](https://pbs.substack.com/profile_images/1454145678075117568/2qXqM_Cu.png)
*   OpenAI GPT-5.6-Cyber: 고급 방어 작업에 특화된 모델로, 오픈소스 소프트웨어 및 Chrome V8에서 알려지지 않은 버그를 발견하는 등 실제 취약점 연구에 활용되었습니다.
*   Anthropic Claude: 미공개 연구용 Claude 변형 모델이 리만 가설 관련 하한을 41.6%에서 67.2%로 개선했습니다.
*   MiniMax H3: 오픈 웨이트 비디오 모델로, 양자화, 오프로딩, Context-IR, 소비자 GPU 배포 및 LoRA 지원 등 생태계 지원을 강화하고 있습니다.
*   Google Gemini Omni Flash: 다각도 비디오 생성 및 편집을 위한 Gemini Omni Flash 사용 사례를 선보였습니다.
*   Dyna Robotics Dyna-2: 100만 시간의 인간 비디오로 사전 학습된 월드-액션 모델을 소개하며, 인간 비디오에서의 스케일링이 로봇 데이터로 전이되는 새로운 스케일링 법칙을 제시했습니다.
*   Composio 벤치마크: 30개 에이전틱 작업에서 DeepSeek V4 Flash를 4개 하네스로 실행한 결과, Pi Agent가 가장 저렴하고 성능이 우수했습니다.
*   vLLM 추측 디코딩 벤치마크: Qwen3-4B에 대한 DSpark는 기준 처리량 대비 2.45~2.55배, DFlash는 1.96~2.09배의 성능 향상을 보였습니다.
*   QuixiAI SlimServe: 4개의 A100에서 SlimServe를 사용한 DeepSeek V4 Flash가 단일 요청 시 175 tok/s, 64 동시성에서 1k tok/s를 기록했습니다.

### 🛠️ 제품 & 도구
*   Meta Muse Glimmer: 장기 에이전트 루프, 도구 사용 및 로컬 배포에 최적화되었으며, 텍스트+이미지 인터리브 입력과 100개 이상의 언어를 지원합니다.
*   Meta Muse Spark 1.2: 오픈 웨이트 가중치가 "곧" 출시될 예정입니다.
    ![X avatar for @alexandr_wang](https://pbs.substack.com/profile_images/1631421210205749248/uohbT_40.jpg)
*   OpenAI GPT-5.6-Cyber: 접근이 "승인된 방어자"로 제한되며, 고위험 사이버 작업에 대한 추가 제어 및 모니터링 안전 장치가 적용됩니다.
*   Anthropic Claude Sonnet 5: 초기 가격인 입력 $2/M, 출력 $10/M이 영구화될 예정입니다.
*   Teknium Hermes Agent: 브라우저 자동화에서 여러 브라우저 작업을 하나의 CLI 기반 도구 인터페이스로 통합하여 약 60%의 토큰 감소를 달성했습니다.
*   Pi SDK: 코딩 에이전트가 읽기, bash, 편집, 쓰기 네 가지 기본 요소만으로도 유능하게 작동함을 강조했습니다.
*   Jerry Liu LiteParse: 에이전트 루프 내에서 낮은 레이턴시 문서 파싱을 목표로 하며, OCR/VLM 대체 전 휴리스틱 추출을 통해 200페이지를 4ms 만에 처리합니다.
*   fal: MiniMax H3 LoRA 학습 및 Seedance 2.5 엔드포인트를 추가했습니다.

### 🔬 연구 & 논문
*   Meta Muse Glimmer 아키텍처: Gemma 4 스타일의 하이브리드 어텐션과 스케일 프리 QK 노름, 더 큰 비전 깊이, 더 긴 SWA와의 유사성을 특징으로 합니다.
*   Meta Muse Glimmer 학습 방식: Muse Spark에서 로짓 디스틸레이션되었으며, 처음부터 에이전틱 트레이스에서 학습되어 기존의 "기반 모델 학습 후 후속 학습" 방식과 차별화됩니다.
*   프로그래밍 방식 도구 호출 연구: 프로그래밍 방식 도구 호출이 14개 모델 중 11개에서 네이티브 JSON 도구 호출과 같거나 능가하며, GPT-5.6 제품군은 BFCL v4에서 JSON 기준선 대비 10.6% 향상되었다는 연구 결과가 발표되었습니다.
*   Dyna Robotics 스케일링 법칙: 인간 비디오에서의 스케일링이 이전에 보지 못한 로봇 데이터로 전이되며, 객관적인 선택이 교차 구현 전이에 중요하다는 새로운 스케일링 법칙을 주장했습니다.

### 💰 산업 동향
*   Sakana AI: "물리적 AI", 월드 모델 및 실제 에이전트를 위한 재귀적 자기 개선을 중심으로 RSI Lab을 확장했습니다.

### ⚡ 인프라 & 하드웨어
*   Meta Muse Glimmer 최적화: LM을 20GB 미만으로 줄이기 위한 양자화와 온디바이스에서 빠른 생성을 위한 경량 DFlash 드래프터를 포함합니다.
*   추측 디코딩 발전: vLLM에서 DSpark는 반자동 회귀 구조와 하드웨어 인식 접두사 스케줄러를 통해 기준 처리량 대비 2.45~2.55배의 성능 향상을 달성했습니다.
*   NVIDIA GPU 대체 인퍼런스 아키텍처: SemiAnalysis는 NVIDIA GPU의 TileRT / InferenceX가 배치 크기 1, 분리된 서빙, 디코딩/프리필 분리에 중점을 두어 높은 상호작용 특성을 모방하려는 시도라고 강조했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
