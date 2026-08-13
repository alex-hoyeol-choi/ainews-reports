# SpaceXAI Grok 4.6 and Grok @Bot - 요약

**원문 URL**: https://www.latent.space/p/ainews-spacexai-grok-46-and-grok
**번역일**: 2026-08-13 06:04
**발행일**: 2026-08-13

---

다음은 제공된 AI 뉴스레터 내용에서 추출한 핵심 신규 소식에 대한 간결한 한국어 브리핑입니다.

### 🔥 주요 뉴스
**[Grok 4.6 출시 및 Grok @Bot]** — xAI가 최신 모델 Grok 4.6을 출시했습니다. 이 1.5T 모델은 지식 작업에서 세계 두 번째로 뛰어난 성능을 보이며, 효율성 면에서는 최고 수준입니다. Artificial Analysis에 따르면 Intelligence Index 61점, Terminal-Bench v2.1에서 88.4%를 기록했으며, 1M 토큰당 $2/$6의 저렴한 가격으로 프론티어 모델 중 가격/성능 면에서 경쟁력을 갖추었습니다.
![X avatar for @bot](https://pbs.substack.com/profile_images/2087219239275069440/KW6C403V.jpg)
**[Claude 텍스트 워터마킹 도입]** — Anthropic이 Claude 모델의 모든 텍스트 출력에 보이지 않는 워터마크를 삽입하고, 지원되는 파일(.png, .jpg, .svg)에는 디지털 서명된 C2PA 출처 메타데이터를 추가한다고 발표했습니다. 이는 2026년 8월 2일 이후 출시된 Claude 모델에 적용되며, AI 생성 콘텐츠의 출처를 표시하는 것을 목표로 합니다.
**[Qwen3.8-Max 오픈 웨이트 공개]** — Alibaba가 2.4T 총 / 95B 활성 MoE 규모의 Qwen3.8-Max 모델을 오픈 웨이트로 출시했습니다. vLLM은 NVIDIA B300 및 AMD MI355X용 4비트 체크포인트와 함께 Day-0 지원을 제공하며, Together AI와 Baseten도 즉각적인 지원을 발표했습니다.
**[Microsoft, 추론 모델 MAI-Thinking-1 출시]** — Microsoft가 자체 개발한 첫 번째 추론 모델인 MAI-Thinking-1을 Foundry에서 사용할 수 있도록 발표했습니다. 이 모델은 응용 추론에 중점을 두며, 특히 도구 사용에 대한 피드백을 요청하고 있습니다.

### 📊 모델 & 벤치마크
*   **Grok 4.6 (xAI):** Grok 4.5를 기반으로 장기 실행 에이전트 및 시각 작업에 중점을 둔 1.5T 모델로, 더 긴 보충 학습 실행과 개선된 학습 레시피를 통해 개발되었습니다.
*   **Qwen3.8-Max (Alibaba):** 2.4T 총 / 95B 활성 MoE 규모의 오픈 웨이트 모델로, 긴 컨텍스트 및 에이전트 지향성을 특징으로 합니다. 초기 오픈 웨이트 버전은 텍스트 전용이며 비전 입력은 지원하지 않습니다.
*   **DeepSeek V4 Pro GA (DeepSeek):** 입력 1M당 약 $0.435, 출력 1M당 $0.87의 낮은 가격으로 출시되었으며, Terminal Bench에서 프리뷰 버전 대비 15.8% 성능 향상을 보였습니다.
*   **MAI-Thinking-1 (Microsoft):** Microsoft가 처음부터 구축한 추론 모델로, 현재 Foundry에서 제공되며 도구 사용에 대한 피드백을 수집하고 있습니다.
*   **Solar Pro 4 (Upstage):** Artificial Analysis의 Intelligence Index에서 14위에서 42위로 순위가 상승했으며, 특히 에이전틱 및 긴 컨텍스트 작업에서 큰 개선을 보였습니다.
*   **North Micro Vision (Cohere):** Apache-2.0 오픈소스 소형 VLM으로, 문서 이해를 목표로 하며 Gemma 4 E2B 및 Ministral 3 3B를 능가한다고 주장합니다.
*   **LFM2.5-VL-3B (Liquid AI):** 강력한 소형 비전 모델로 언급되며, 하이브리드 로컬/원격 에이전트 스택에 활용될 수 있습니다.
*   **DiG-bench (Princeton/MIT):** 표준 QA 또는 코드 작업이 아닌 발견을 위한 텍스트 기반 벤치마크입니다.
*   **Conceptual Reasoning Index (Redwood + Anthropic):** AI 위험 관련 논증 및 개념적 추론을 목표로 하는 새로운 벤치마크입니다.
*   **SRE-Bench (Vals):** 소스 레벨 사이버 작업보다는 바이너리 리버스 엔지니어링에 중점을 둔 벤치마크입니다.

### 🛠️ 제품 & 도구
*   **Grok @Bot (xAI):** Grok 4.6 모델에 의해 구동되는 AI 팀메이트/멀티에이전트 분야의 새로운 진입자입니다.
![X avatar for @bot](https://pbs.substack.com/profile_images/2087219239275069440/KW6C403V.jpg)
*   **LTX-2.5 (Lightricks):** Diffusers에 비디오 + 48kHz 오디오 동시 생성, 프롬프트 제어 클립 길이, 2패스 품질 모드, 타일 렌더링 등 로컬 비디오 워크플로우를 위한 실용적인 기능을 추가했습니다.
*   **SL2T (Google DeepMind):** Android/Pixel 11에서 ASL 입력을 지원하는 수화-텍스트 시스템으로, 온디바이스 신체 자세 추적과 서버 측 번역을 결합합니다.
*   **Flux TTS (Deepgram):** 약 80ms의 응답 시간과 통화 중 적응 기능을 갖춘 저지연 대화형 TTS 모델입니다.
*   **LLM Compressor v0.13.0:** MoE 모델을 위한 REAP 전문가 가지치기 및 임의의 3/5/6/7비트 양자화 기능을 추가했습니다.
*   **CuTeDSL 4.7.0:** GPU 커널 개발자가 워프 역할, 리소스, 종속성 및 스케줄을 선언하여 교착 상태, 경쟁 조건 등에 대한 정적 검사를 가능하게 하는 Task Scheduling 커널을 도입했습니다.
*   **Agent Plugins 1.0 (GitHub):** 스킬, MCP 서버 및 AI 확장을 패키징하는 Agent Plugins 1.0을 출시했으며, UX 개선 사항도 포함합니다.
*   **Codex for Linux (OpenAI):** OpenAI/Codex의 모멘텀의 일환으로 Linux용 Codex가 포함되었습니다.
*   **LangSmith 대시보드 (LangChain):** 더 유용한 트레이스 분석 및 보고를 위해 재구축되었습니다.
*   **Hermes Agent 업데이트:** Raspberry Pi 배포, 쉬운 프로필 내보내기/가져오기, 관찰된 웹 트래픽에서 재사용 가능한 API를 생성하는 새로운 스킬 등 여러 생태계 업데이트를 받았습니다.
*   **Managed Deep Agents (LangChain):** 내구성 있는 메모리 및 소셜 미디어 에이전트와 같은 반복적인 워크플로우에 초점을 맞춘 예시를 제공합니다.

### 🔬 연구 & 논문
*   **Direct On-Policy Distillation:** RL을 더 작은 모델에서 수행하고 결과적인 정책 변화를 조밀한 암시적 보상을 사용하여 더 큰 모델로 전이시키는 방식으로, 파이프라인 비용을 거의 절반으로 줄일 수 있습니다.
*   **긴 컨텍스트 연구 (dair.ai):** 정규화, GQA, 사전 학습 컨텍스트 길이, 슬라이딩 윈도우 어텐션이라는 네 가지 아키텍처 선택이 긴 컨텍스트 성능의 최대 47%를 차지할 수 있음을 주장합니다.
*   **ResidencyRL (Google):** Gemini 3.5 Flash를 49,870건의 시뮬레이션된 원격 의료 상담에 대해 학습시킨 결과, 적대적 조건에서 진단 정확도가 81%에서 88%로 증가하고 놓친 위험 신호가 31% 감소했습니다.

### 💰 산업 동향
*   **Claude 텍스트 워터마킹 정책:** Anthropic은 Claude가 생성한 텍스트에 보이지 않는 워터마크를 삽입하고 파일에 디지털 서명된 메타데이터를 추가하여 AI 생성 콘텐츠의 출처를 표시하는 새로운 정책을 도입했습니다.
*   **Expedia의 Keras 3 마이그레이션:** Expedia가 최신 Keras 3 설정으로 마이그레이션하여 랭킹 모델의 학습 속도가 30% 향상되고 인퍼런스 레이턴시가 70% 감소했습니다. Keras의 백엔드에 구애받지 않는 API는 벤더 락인(lock-in)을 줄이는 이점을 제공합니다.
*   **Snowflake SQL 자동 완성 모델 개선:** Snowflake의 새로운 4B SQL 자동 완성 모델이 이전 30B-A3B MoE 모델을 능가하여 사용자 수용도를 높이고 중앙값 레이턴시를 71% 단축했습니다.

### ⚡ 인프라 & 하드웨어
*   **vLLM Azure Blob 지원:** vLLM이 모델 로딩 및 KV 커넥터 모두에 Azure Blob 경로를 지원하여 거대 모델 및 긴 프롬프트 워크로드를 위한 중요한 인프라를 추가했습니다. Microsoft/NVIDIA 레시피를 통해 H100/A100에서 최대 7.3배 빠른 가중치 로딩과 Blob 기반 KV 캐싱이 가능합니다.
*   **Unsloth의 1비트 양자화:** Qwen3.8-2.4T-A95B 모델을 동적 1비트 양자화를 통해 4.9TB에서 397GB로 축소하여 410GB 이상의 RAM/VRAM 시스템에서 로컬 실행을 가능하게 했다고 주장했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
