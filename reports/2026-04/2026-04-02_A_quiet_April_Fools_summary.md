# A quiet April Fools - 요약

**원문 URL**: https://www.latent.space/p/ainews-a-quiet-april-fools
**번역일**: 2026-04-02 07:19
**발행일**: 2026-04-02

---

### 🔥 주요 뉴스
**[Claude Code 소스 코드 유출]** — Anthropic의 Claude Code CLI 소스 코드(50만 라인 이상 TypeScript)가 npm 레지스트리 맵 파일을 통해 유출되었습니다. 이 유출로 멀티 에이전트 오케스트레이션 시스템, 4계층 컨텍스트 압축 스택, 스트리밍 및 병렬 도구 실행, 숨겨진 기능(예: "BUDDY" 펫 시스템, "ULTRAPLAN", "BRIDGE MODE", "KAIROS_DREAM") 등이 드러났습니다. Anthropic은 DMCA를 발행하여 GitHub에서 코드를 삭제하려 했으나, 일부 포크는 복원되었고 오픈소스 클론이 빠르게 확산되었습니다.

**[OpenAI, 1,220억 달러 자금 조달]** — OpenAI가 핵심 AI 인프라 강화를 위해 1,220억 달러를 조달하여 포스트머니 기업 가치 8,520억 달러에 도달했습니다. ChatGPT는 주간 활성 사용자 9억 명, 월 20억 달러의 수익을 보고하며, Amazon, NVIDIA, Microsoft와의 전략적 파트너십을 통해 AI 역량을 발전시키고 있습니다.

**[PrismML, 1-bit Bonsai 모델 출시]** — PrismML이 1-bit Bonsai 8B 모델을 포함한 1-bit Bonsai 모델을 출시했습니다. 이 모델은 1.15GB 메모리에 불과하며, 풀-프리시전 모델보다 14배 작고, 8배 빠르며, 5배 에너지 효율적이어서 엣지 하드웨어에 최적화되었습니다. Apache 2.0 라이선스 하에 오픈소스화되었으며, Llama.cpp 포크를 통해 인퍼런스가 가능합니다.

**[Arcee Trinity-Large-Thinking 오픈 웨이트 모델 출시]** — Arcee가 Apache 2.0 라이선스 하에 오픈 웨이트 모델인 Trinity-Large-Thinking을 출시했습니다. 이 400B 전체 / 13B 활성 모델은 PinchBench에서 #2위, Tau2-Airline에서 SOTA를 달성하는 등 강력한 에이전틱 성능을 주장하며, "미국 오픈소스"의 이정표로 평가받고 있습니다.

### 📊 모델 & 벤치마크
*   **Z.ai GLM-5V-Turbo 출시:** Z.ai가 순수 텍스트 코딩 성능을 유지하면서 이미지, 비디오, 문서 레이아웃 및 디자인 초안을 기본적으로 처리하는 비전 코딩 모델 GLM-5V-Turbo를 발표했습니다. 이 모델은 기본 멀티모달 퓨전, 차세대 CogViT 인코더, 30개 이상의 작업 협업 RL 등을 통해 성능을 향상시켰습니다.
*   **Falcon Perception 및 OCR 모델 출시:** TII가 오픈 보캐블러리 참조 표현 분할 모델인 Falcon Perception과 0.3B OCR 모델을 출시했습니다. OCR 모델은 3~10배 더 큰 모델과 경쟁할 수 있으며, 초기 퓨전 트랜스포머 아키텍처를 특징으로 합니다.
*   **H Company Holo3 출시:** H Company가 GUI-내비게이션 모델 제품군인 Holo3(A3B/35B)를 출시했습니다. Qwen3.5 기반이며 무료 라이선스로 Transformers를 지원합니다.
*   **Qwen3.5 27B 디스틸레이션 모델 성능 주장:** Claude 4.6 Opus 추론 트레이스에서 학습된 Qwen3.5 27B 디스틸레이션 모델이 Claude Sonnet 4.5를 능가하는 SWE-bench 승리, 96.91% HumanEval, 더 낮은 CoT 장황성, 4비트 로컬 사용성, 30만+ HF 다운로드를 주장했습니다.
*   **TurboQuant TQ3_1S 모델 출시:** TurboQuant가 Qwen3.5-27B 모델에 대해 Q4_0에 가까운 품질을 유지하면서 약 10% 더 작은 TQ3_1S 모델을 출시했습니다. 이 모델은 12.9GB 크기로 16GB RTX 5060 Ti에 적합하며, Walsh-Hadamard 회전 및 8-중심 양자화 기술을 사용했습니다.
*   **MemFactory 메모리 증강 에이전트 프레임워크:** MemFactory가 네이티브 GRPO 통합을 통해 메모리 증강 에이전트를 위한 통합 인퍼런스/학습 프레임워크를 제안하며, 기준선 대비 최대 14.8%의 상대적 성능 향상을 보고했습니다.
*   **Baseten KV-cache 압축 퍼시버:** Baseten이 KV-cache를 8배 압축하면서 90% 이상의 사실 유지율을 유지하는 7M-파라미터 퍼시버를 설명했습니다.
*   **DAIR 자기 조직화 에이전트 연구:** DAIR 연구에 따르면 최대 256개 에이전트를 사용하는 25,000개 작업에서 자기 조직화된 역할이 미리 정의된 계층보다 우수하며, 오픈 모델이 더 낮은 비용으로 클로즈드 모델 품질의 95%에 도달했습니다.
*   **새로운 에이전트 벤치마크:** Kaggle Standardized Agent Exams, 1년 스타트업 시뮬레이션 YC-Bench, 187개 조작 작업 및 12개 프론티어 모델을 포함하는 에이전틱 로봇 공학 벤치마크/툴킷 CaP-Gym / CaP-X가 출시되었습니다.
*   **Arena 가격/성능 파레토 프론티어 차트 추가:** Arena가 텍스트, 비전, 검색, 문서 및 코드 전반에 걸친 파레토 프론티어 차트를 추가하여 가격/성능 트레이드오프를 명확히 했습니다.
*   **MLPerf Inference v6.0 강조:** Lambda와 NVIDIA는 MLPerf Inference v6.0이 최고 칩 사양보다 실제 AI 팩토리 생산성을 측정하는 더 나은 렌즈라고 지적했습니다.

### 🛠️ 제품 & 도구
*   **OpenAI Codex 사용량 제한 초기화:** OpenAI가 모든 플랜에서 Codex 사용량 제한을 초기화했습니다. 이는 높은 속도 제한 도달과 동시에 발생한 사기 계정 제거로 인한 컴퓨팅 자원 회수 때문이라고 합니다.
*   **LangChain 문서 채팅 기능 내장:** LangChain이 전체 문서, 지식 기반 및 OSS 코드를 기반으로 하는 채팅 기능을 문서에 내장했습니다.
*   **Together AI 에이전트 스킬 오픈소스화:** Together AI가 Claude Code와 Codex가 올바른 모델 ID 및 SDK 관용구로 API를 호출할 수 있도록 12개의 에이전트 스킬을 오픈소스화했습니다.
*   **OpenAI Devs Linear 통합 강화:** OpenAI Devs가 코드 작업과 티켓을 동기화하기 위해 Codex 앱에서 Linear 통합을 강화했습니다.
*   **SkyPilot VAST Data 지원 추가:** SkyPilot이 이기종 컴퓨팅 백엔드 전반에 걸쳐 고속 데이터셋 마운트를 직접 지원하는 네이티브 VAST Data 지원을 추가했습니다.
*   **Hugging Face Spaces용 영구 Storage Buckets 출시:** Hugging Face가 Spaces용 영구 Storage Buckets를 출시했습니다.
*   **Tinker 컨텍스트 윈도우 확장:** Tinker가 특정 오픈 모델에 대해 최대 256k까지 컨텍스트 윈도우를 확장하여 RL 및 장기 실험에 대한 매력을 높였습니다.
*   **open-multi-agent 프레임워크 출시:** Claude Code 유출된 소스 코드를 기반으로, 멀티 에이전트 오케스트레이션 시스템을 모든 LLM에서 작동하는 오픈소스 프레임워크인 open-multi-agent가 TypeScript로 재구현되어 MIT 라이선스 하에 GitHub에서 사용할 수 있습니다.

### 🔬 연구 & 논문
*   **DeepMind "AI Agent Traps" 논문:** DeepMind의 새로운 논문 "AI Agent Traps"는 에이전트 보안을 모델 탈옥뿐만 아니라 웹페이지/문서의 적대적 콘텐츠 중심으로 재구성합니다. HTML/CSS에 숨겨진 프롬프트 인젝션이 최대 86%의 시나리오에서 성공하고, 잠재적 메모리 오염이 0.1% 미만의 오염으로 80% 이상의 공격 성공률에 도달한다고 언급합니다.
*   **RL 프레임워크 비교 설문조사:** adithya_s_k의 설문조사 스레드는 오케스트레이션, 롤아웃 버퍼링, 가중치 동기화, 지연 처리, 부분 롤아웃 동작, LoRA 지원 및 분산 병렬 처리 측면에서 16개의 RL 프레임워크를 비교했습니다.
*   **리트리벌 후기 상호작용 선호 증거:** 여러 게시물에서 멀티 벡터 / 후기 상호작용 리트리벌이 단일 벡터 임베딩보다 우수하며, 파인튜닝 후에도 치명적인 망각에 대한 더 나은 견고성을 보인다고 재차 강조했습니다.

### 💰 산업 동향
*   **Anthropic DMCA 역풍 및 복원:** Anthropic이 유출된 Claude Code 리포지토리에 대해 지나치게 광범위한 DMCA를 발행했으나, 이후 통신 오류를 인정하고 리포지토리를 복원했습니다.
*   **오픈소스 Claude Code 클론 확산:** 유출된 Claude Code 포크가 하루 만에 110k+ GitHub 스타를 기록하며 오픈소스 생태계 경쟁을 가속화했습니다.
*   **Google Agent Skills 사양 제안:** Google이 기본 컨텍스트를 90% 줄이기 위해 점진적 공개를 제안하는 Agent Skills 사양을 발표했습니다.

### ⚡ 인프라 & 하드웨어
*   **ZINC 인퍼런스 엔진 출시:** ZINC가 ROCm의 복잡성을 우회하고 Vulkan을 통해 AMD GPU와 직접 인터페이스하는 새로운 로컬 인퍼런스 엔진을 출시했습니다. AMD Radeon AI PRO R9700에서 4배의 속도 향상을 달성했으며, Qwen3.5-35B-A3B 및 Qwen3.5-2B 모델을 지원합니다.
*   **Hugging Face TRL v1.0 출시:** Hugging Face의 TRL v1.0이 오픈 사후 학습(SFT, 보상 모델링, DPO, GRPO)을 프로덕션 준비 패키지로 통합했습니다.
*   **HeavyBall 3.0.0 출시:** HeavyBall 3.0.0이 FSDP, DDP, 2.5배 속도 향상을 위한 엔드투엔드 컴파일, 더 빠른 Muon/SOAP 변형, 새로운 옵티마이저와 함께 출시되었습니다.
*   **CuTeDSL 저수준 DSL 출시:** maharshii가 Python에서 PTX를 직접 인라인으로 허용하여 커스텀 커널에 대한 장벽을 낮추는 CuTeDSL을 주장했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
