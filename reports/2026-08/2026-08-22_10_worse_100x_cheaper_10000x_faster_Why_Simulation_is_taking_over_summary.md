# 10% worse, 100x cheaper, 10000x faster: Why Simulation is taking over - 요약

**원문 URL**: https://www.latent.space/p/ainews-10-worse-100x-cheaper-10000x
**번역일**: 2026-08-22 12:05
**발행일**: 2026-08-22

---

### 🔥 주요 뉴스
**[DeepSeek, 멀티모달 에이전트 모델 'DeepSeek-V4-Flash-Vision-Exp' 출시]** — DeepSeek이 멀티모달 에이전트 성능이 Opus-4.8에 근접한다고 주장하는 'DeepSeek-V4-Flash-Vision-Exp'를 출시했습니다. 이 모델은 기존 V4-Flash의 텍스트 기능에 멀티모달 지원을 추가하며, 혼합 텍스트+이미지 API 및 이미지 재사용을 위한 Files API를 제공합니다.
**[OpenAI, GPT-5.6 Sol 가격 인하 및 Codex 사용자 2천만 명 돌파]** — OpenAI는 GPT-5.6 Sol API 및 크레딧 기반 제품 가격을 3개월간 20% 이상 인하한다고 발표했습니다. 또한, Codex가 2천만 명의 활성 사용자를 달성했으며, 모든 Codex 및 ChatGPT Work 사용자에게 "뱅크드 리셋"을 부여했습니다.
**[미스터리 모델 'Ox Alpha' 등장, 강력한 코딩 및 에이전트 성능 보고]** — 정체가 불분명한 'Ox Alpha' 모델이 이례적으로 강력한 코딩 및 에이전트 성능을 보이며 주목받고 있습니다. DeepSWE 작업에서 80% 이상을 기록하여 Fable(65%) 및 GPT-5.6 Sol(52%)을 능가하는 벤치마크 결과가 보고되었습니다.

### 📊 모델 & 벤치마크
*   **Ox Alpha 모델 성능 보고:** 미스터리 모델 Ox Alpha가 DeepSWE 작업에서 80% 이상을 기록하며 강력한 코딩 및 에이전트 성능을 보였습니다.
*   **DeepSeek-V4-Flash-Vision-Exp 벤치마크:** DeepSeek의 신규 멀티모달 모델은 Terminal Bench 2.1에서 83.9, Toolathlon-Verified에서 75.9, Chartography에서 64.3점을 기록하며 이전 버전에 비해 DeepSWE에서 약 4점 개선되었습니다.
*   **Qwen3.8-27B 로컬 에이전트 성능:** Qwen3.8-27B가 단일 RTX 3090에서 150k 컨텍스트로 로컬에서 실행되며 대학 시스템 탐색, 강의 일정 검색, 소셜 미디어 비디오 처리 등 높은 수준의 자율 에이전트 워크플로우를 수행했습니다.
*   **Qwen3.8-27B 지식 기억력 퇴보 보고:** Qwen3.8-27B가 오프라인, 툴 호출 없는 사실 기억(factual recall)에서 Qwen3.6-27B에 비해 퇴보한 것으로 보고되었으며, Artificial Analysis의 Omniscience 지식 벤치마크에서도 낮은 점수를 받았습니다.
*   **새로운 에이전트 벤치마크 출시:** FACET은 6,078개의 실행 가능한 터미널 작업을, SWE-bench Science는 119개의 과학 소프트웨어 작업을, CADBench는 Fusion 360 작업을, AI4AI-Bench는 10개 연구 리포지토리에서 재귀적 자체 개선을 테스트하는 벤치마크를 도입했습니다.
*   **NVIDIA AVO, ARC-AGI-3 환경 100% 해결:** NVIDIA AVO가 25개의 공개 ARC-AGI-3 환경에서 183개 레벨을 모두 해결했다고 보고되었으나, François Chollet은 이것이 전체 벤치마크가 아닌 공개 데모/튜토리얼 세트라고 언급했습니다.

### 🛠️ 제품 & 도구
*   **DeepSeek-V4-Flash-Vision-Exp API 출시:** DeepSeek-V4-Flash-Vision-Exp가 DeepSeek API를 통해 라이브로 제공되며, Chat Completions, Messages, Responses API를 지원하고 base64, 외부 URL 또는 Files API를 통한 텍스트+이미지 혼합 입력을 받습니다.
*   **DeepSeek Files API 출시:** DeepSeek은 이미지 재사용을 위한 Files API를 출시하여 사용자가 이미지를 한 번 업로드하고 file_id로 참조할 수 있도록 했습니다.
*   **OpenAI 지출 제어 기능 추가:** OpenAI는 API 키별 사용량 및 지출 추적, 월별 조직/프로젝트의 엄격한 한도 설정 기능을 추가했습니다.
*   **GitHub, Slack 및 Teams에 협업 에이전트 워크플로우 출시:** GitHub가 Slack 및 Teams에 협업 에이전트 워크플로우를 출시하여 에이전트가 작업을 선택하고, PR을 열고, 공유 채널 내에서 디자인을 연동하는 흐름을 지원합니다.
*   **nac v0.1.3 업데이트:** nac v0.1.3이 샌드박스형 git 워크트리, 세션 구성, 비전 인식 이미지 읽기 기능을 추가했습니다.
*   **Hermes Agent 업데이트:** Hermes Agent가 Ox Alpha를 제공하고 "Blank Slate 모드"와 자동 스킬 가지치기 기능을 공개했습니다.
*   **OpenHands 모델 전환:** OpenHands가 무료 기본 모델을 Kimi K3로 전환했습니다.
*   **Ollama, Kimi K3 추가 및 AT&T 파트너십:** Ollama는 AT&T를 오픈 모델에 환영하고 Kimi K3를 Pro/Max 구독에 추가했습니다.

### 🔬 연구 & 논문
*   **Google EnvHarness / EnvRigger:** Google의 EnvHarness / EnvRigger는 플러그인 레이어와 정책 진단 리셰이핑을 사용하여 정적 환경을 조정하며, 9.8% 더 적은 실행 단계로 홀드아웃 성능을 최대 9점 향상시킵니다.
*   **vLLM IsoExec 출시:** vLLM의 IsoExec은 부동 소수점 비결합성으로 인한 RL 롤아웃/학습 로그 확률 불일치를 해결하며, 8xH100에서 Qwen3.5-35B-A3B의 로그 확률 차이를 25.3% 오버헤드로 1.6e-2에서 6.7e-7로 감소시켰습니다.
*   **DeepMind Recirculation 논문:** DeepMind의 Recirculation 논문은 재학습 없이 인퍼런스 시 컨텍스트화된 더 깊은 레이어 활성화를 이전 처리 단계로 다시 공급하는 방식으로 컨텍스트화 오류 60% 감소, perplexity 23% 감소, GSM8K 21% 증가 등의 개선을 보고했습니다.
*   **Google DeepMind Pandora’s Router:** Google DeepMind의 Pandora’s Router는 라우팅을 비용이 많이 드는 검사를 수반하는 최적 검색 문제로 정의하는 새로운 접근 방식을 제시했습니다.
*   **Jim Fan, T-Rex 데이터셋 소개:** Jim Fan은 비동기 비전/촉각 전문가와 함께 50시간, 약 5,500 에피소드, 22-DoF 하드웨어로 구성된 가장 큰 오픈 촉각 데이터셋인 T-Rex를 소개했습니다.

### 💰 산업 동향
*   **OpenAI GPT-5.6 Sol 가격 20% 이상 인하:** OpenAI는 API 및 크레딧 기반 제품에서 GPT-5.6 Sol 가격을 3개월 동안 20% 이상 인하한다고 발표했습니다.
*   **Codex 활성 사용자 2천만 명 달성:** OpenAI Codex가 2천만 명의 활성 사용자를 달성했으며, 모든 Codex 및 ChatGPT Work 사용자에게 "뱅크드 리셋"을 부여했습니다.

### ⚡ 인프라 & 하드웨어
*   **UC Berkeley FreeToken 공개:** UC Berkeley의 FreeToken은 단일 RTX PRO 6000에서 14.9 tok/s의 753B GLM-5.2와 8GB RTX 4060 노트북에서 39.3 tok/s의 Qwen3.6-35B를 달성하며 소비자 GPU에서 Ollama 처리량의 2~4배를 주장했습니다.
*   **Deepseek V4 Flash-0731 인퍼런스 리그:** 16× RTX 5060 Ti 16GB GPU와 Broadcom/PLX PEX88096 PCIe 스위치를 사용한 커스텀 인퍼런스 리그가 DeepSeek V4 Flash-0731을 단일 사용자 생성에서 약 100–150 tok/s, 16명 동시 사용자에서 총 727 출력 tok/s로 서빙하는 성능을 시연했습니다.
*   **Marin 535B-A23B 학습 시작:** Percy Liang은 Marin 535B-A23B 모델이 11× GB200 NVL72에서 약 3개월 동안 18.75T 토큰을 목표로 학습을 시작했으며, 학습 과정을 공개한다고 발표했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
