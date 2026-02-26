# [요약] Anthropic accuses DeepSeek, Moonshot, and MiniMax of "industrial-scale distillation attacks". | AINews

**원문 URL**: https://news.smol.ai/issues/2026-02-23-not-much

**요약일**: 2026-02-26 00:56:04

**원본 리포트**: Anthropic_accuses_DeepSeek_Moonshot_and_MiniMax__20260224_173248.md


---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 뉴스 브리핑입니다.

### 🔥 주요 뉴스
*   **Anthropic, DeepSeek 등 3사에 Claude '디스틸레이션 공격' 주장** — Anthropic은 DeepSeek, Moonshot AI, MiniMax가 24,000개 이상의 사기성 계정을 통해 1,600만 건 이상의 Claude 상호작용을 생성하여 모델 기능을 추출하는 산업 규모의 디스틸레이션 공격을 수행했다고 밝혔습니다. 이는 경쟁적 기능 전이 및 안전장치 우회 등 중대한 보안 및 지적 재산권 문제를 제기합니다.
*   **OpenAI Responses API, WebSockets 지원 추가** — OpenAI는 저지연, 장기 실행, 도구 사용이 많은 에이전트를 위해 Responses API에 WebSockets를 추가했습니다. 이를 통해 지속적인 연결과 점진적 입력 전송이 가능해져, 20개 이상의 도구 호출에서 20~40%의 속도 향상을 주장합니다.
*   **OpenAI, SWE-Bench Verified 벤치마크 사용 중단 권고** — OpenAI는 SWE-Bench Verified 벤치마크가 높은 데이터 오염과 결함/해결 불가능한 작업으로 인해 더 이상 프론티어 코딩 기능을 측정하지 못한다고 밝히며, SWE-bench Pro 사용을 권장했습니다. 이는 AI 모델 평가의 무결성에 대한 중요한 변화를 시사합니다.
*   **GPT-5.2-chat-latest, Arena 리더보드 상위권 진입** — LMArena 리더보드에서 GPT-5.2-chat-latest가 1478점으로 상위 5위에 진입했으며, 이는 기존 GPT-5.2 대비 40점 상승한 수치입니다. 특히 다중 턴, 지시 따르기, 어려운 프롬프트, 코딩 분야에서 개선이 두드러졌습니다.
*   **Anthropic, Claude Code Security 툴 출시** — Anthropic은 Claude 4.6 Opus 기반의 코드 보안 툴인 Claude Code Security를 출시했습니다. 이 툴은 오픈소스 프로덕션 코드에서 500개 이상의 오래된 버그를 발견했으며, 현재 연구 미리보기 대기 목록을 통해 접근 가능합니다.

### 📊 모델 & 벤치마크
*   Gemini 3.1 Pro가 WeirdML 점수 72.1%를 기록하며 3.0의 69.9% 대비 상승했으나, 높은 출력 토큰 사용량과 특정 약점이 지적되었습니다.
*   Qwen이 17B 활성 파라미터를 가진 397B 멀티모달 MoE 모델을 출시했으며, GPT5.2/Claude 4.5와 경쟁한다고 주장하는 트윗이 있었습니다.
*   NL2Repo-Bench는 에이전트가 처음부터 완전히 설치 가능한 Python 라이브러리를 생성할 수 있는지 테스트하며, 최고 모델의 통과율은 40% 미만으로 나타났습니다.
*   OlmOCR-Bench가 커뮤니티 평가 제출을 위한 Hugging Face 벤치마크 데이터셋으로 지정되었습니다.
*   약 15만 5천 건의 실제 사용자 요청과 Opus 4.5, Gemini 3 Pro, GPT 5.2의 응답을 포함하는 Real-Slop 데이터셋이 공개되었습니다.

### 🛠️ 제품 & 도구
*   Simon Willison이 Claude Code/Codex와 같은 코딩 에이전트를 위한 'Agentic Engineering Patterns' 가이드의 첫 장을 발표했습니다.
*   WhatsApp I/O, 스웜, 예약된 작업 등을 갖춘 더 작고 컨테이너로 격리된 OpenClaw 유사 어시스턴트인 NanoClaw가 출시되었습니다.
*   Ollama 0.17 버전이 OpenClaw와 함께 오픈 모델을 사용하는 것을 더 간단하게 만들었습니다.
*   스킬 작성, 통합 생성, 워크플로우 복구 등이 가능한 자체 호스팅 지속형 에이전트 런타임인 Opentulpa가 GitHub에 게시되었습니다.
*   개선 루프에서 몇 시간 동안 자율적으로 실행되는 코딩 에이전트 스웜인 Super System이 Hugging Face에서 공유되었습니다.
*   성능과 해커빌리티에 중점을 둔 Python 네이티브 LLM 인퍼런스 라이브러리인 Pyxis가 출시되었으며, OpenAI 호환 SSE 스트리밍 API를 제공합니다.
*   Mojo 26.1의 Thistle Crypto Library가 OpenSSL과 경쟁하는 성능을 보이며, ML-KEM 및 ML-DSA (양자 내성 암호)를 도입하고 약 700개의 CAVP 테스트를 포함했습니다.

### 🔬 연구 & 논문
*   Qwen 팀은 최근 논문에서 GPQA 및 HLE 테스트 세트의 상당한 데이터 품질 문제를 확인했으며, 이는 DeepSeek-Overclock 프로젝트의 이전 발견을 뒷받침합니다.
*   O(T) 메모리 프리미티브로 MHA와 경쟁력 있는 Addressed State Attention (ASA)이 독립 연구원에 의해 소개되었습니다.
*   기존 등변 아키텍처가 물리 시스템의 모든 대칭성을 동시에 존중할 수 없다는 근본적인 한계를 밝히는 새로운 논문이 발표되었습니다.

### 💰 산업 동향
*   OpenAI는 BCG, McKinsey, Accenture, Capgemini와 '프론티어 얼라이언스'를 발표하며 엔터프라이즈 시장 진출을 확대합니다.
*   Google은 학위 수여 기관의 학생 및 교수진을 위해 대학에 일회성 무제한 자금을 '선물'로 제공하고 있습니다.
*   OpenAI, Oracle, SoftBank 간의 대규모 데이터센터 건설 합작 투자인 'Stargate' 벤처가 통제권 충돌과 재정적 어려움으로 인해 중단되었다고 보도되었습니다.

### ⚡ 인프라 & 하드웨어
*   Taalas는 '트랜지스터에 모델 파라미터 각인' 기술을 통해 Llama 3.1 8B에서 초당 18,000 토큰을 달성했다고 주장했습니다.
*   NVIDIA는 Blackwell에 최적화된 Qwen3.5 MoE를 NVFP4로 양자화하여 SGLang을 사용하여 2배 더 빠른 인퍼런스를 제공한다고 발표했습니다.
*   Hazy Research의 ThunderKittens 2.0은 리팩토링, 메모리 명령어 튜닝 등을 통해 GPU 커널 속도를 최대 10% 향상시켰다고 밝혔습니다.
*   RTX 5080 (sm120)에서의 커널 튜닝이 B200 (sm100)으로 안정적으로 이전되지 않을 것이라는 아키텍처적 차이가 지적되었습니다.


---

*이 요약은 Gemini AI를 사용하여 자동 생성되었습니다. 커뮤니티 반응 및 개인 의견은 제외되었습니다.*
