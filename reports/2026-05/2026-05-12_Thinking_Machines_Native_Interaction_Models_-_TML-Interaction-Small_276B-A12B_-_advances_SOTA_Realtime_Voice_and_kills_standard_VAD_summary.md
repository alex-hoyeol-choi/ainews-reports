# Thinking Machines' Native Interaction Models - TML-Interaction-Small 276B-A12B - advances SOTA Realtime Voice and kills standard VAD - 요약

**원문 URL**: https://www.latent.space/p/ainews-thinking-machines-native-interaction
**번역일**: 2026-05-12 06:19
**발행일**: 2026-05-12

---

### 🔥 주요 뉴스
**Thinking Machines, 실시간 상호작용 모델 'TML-Interaction-Small' 공개** — 276B 파라미터 MoE 모델인 TML-Interaction-Small은 12B 활성 파라미터로 실시간 음성 모델의 SOTA를 발전시켰습니다. 이 모델은 GPT 4o, GPT-Realtime-2, Gemini 3.1-Flash를 주요 벤치마크에서 능가하며, 200ms 미만의 이미지 및 오디오 처리를 위한 인코더 없는 초기 퓨전을 사용합니다.
![Thinking Machines Interaction Model](https://substack-post-media.s3.amazonaws.com/public/images/02190942-3f50-4067-ae03-97c6b504b3a3_1490x1592.png)
![Thinking Machines Encoder-less Early Fusion](https://substack-post-media.s3.amazonaws.com/public/images/68576e99-b00a-4069-b93f-bbe904ddd810_1336x1602.png)
![Thinking Machines AGI Demo](https://substack-post-media.s3.amazonaws.com/public/images/0bfcadcb-b746-4875-aed4-95f19f5897_1478x1676.png)
**OpenAI, 기업용 배포 및 보안 강화 전략 발표** — 기업 고객의 프론티어 모델 배포를 지원하는 'OpenAI Deployment Company'를 설립하고, Tomoro 인수를 통해 150명의 전문 인력을 확보했습니다. 또한, 사이버 보안 강화를 위한 'Daybreak'를 출시하여 GPT-5.5, Codex 등을 활용한 방어적 사이버 작전 및 소프트웨어 공급망 보안 기능을 제공합니다.

### 📊 모델 & 벤치마크
*   **Thinking Machines, TML-Interaction-Small 모델 출시 및 신규 벤치마크 도입** — 276B 파라미터 MoE 모델인 TML-Interaction-Small은 BigBench Audio, IFEval, FD-bench에서 기존 모델들을 능가했습니다. 시간 인식, 동시 번역, 시각적 주도성을 측정하는 TimeSpeak, CueSpeak, RepCount-A, ProactiveVideoQA 등 2개의 새로운 내부 벤치마크를 만들었습니다.
*   **Artificial Analysis, 코딩 에이전트 벤치마크 'Coding Agent Index' 공개** — SWE-Bench-Pro-Hard-AA, Terminal-Bench v2, SWE-Atlas-QnA를 포함하는 Coding Agent Index를 출시하여 모델과 하네스 조합을 평가합니다. Cursor CLI의 Opus 4.7이 61점으로 선두를 차지했으며, Claude Code의 GLM-5.1, Kimi K2.6, DeepSeek V4 Pro가 오픈 웨이트 모델 중 상위권에 올랐습니다.
*   **OpenHands 및 Claw-Eval, 에이전트 벤치마크 업데이트** — OpenHands는 소프트웨어 엔지니어링 벤치마크를 업데이트했으며, Claw-Eval은 사무, 금융, 터미널, 웹 작업을 아우르는 에이전트 작업을 평가하여 MiMo-V2.5-Pro가 선두를 차지했습니다.
*   **Unsloth, Qwen 3.6 MTP 보존 GGUF 빌드 공개** — Unsloth는 Qwen3.6-27B-GGUF-MTP 및 Qwen3.6-35B-A3B-GGUF-MTP를 출시하여 MTP(다음 토큰 예측) 레이어를 유지하지만, 특정 llama.cpp MTP PR 빌드가 필요합니다.

### 🛠️ 제품 & 도구
*   **OpenAI Deployment Company 설립** — 기업 고객의 프론티어 모델 배포를 돕기 위해 Tomoro 인수를 통해 150명의 Forward Deployed Engineers 및 Deployment Specialists를 확보했습니다.
*   **OpenAI Daybreak 출시** — GPT-5.5, Codex 등을 결합하여 방어적 사이버 작전 및 소프트웨어 공급망 보안을 위한 포괄적인 노력을 제공하며, GPT-5.5-Cyber와 같은 전문화된 접근 계층을 포함합니다.
*   **aggit 출시** — 로컬/원격, S3 기반 에이전트 아티팩트 저장을 위한 Rust CLI로, Git 기록 외부에서 stash/branch/restore 시맨틱을 가능하게 합니다.
*   **Claude agents 터미널 제어 플레인 도입** — 여러 Claude Code 에이전트를 관리하기 위한 새로운 터미널 제어 플레인이 강조되었습니다.
*   **Cursor, Microsoft Teams 통합** — Cursor가 Microsoft Teams에 도입되어 에이전트가 전체 스레드를 읽고 PR을 열 수 있게 되었습니다.
*   **Deep Agents CLI 기능 강화** — 컨텍스트 손실 없이 대화 중에 기본 모델 제공자를 핫스왑할 수 있는 기능을 제공합니다.
*   **LangChain, 제공자/모델 특정 파인튜닝을 위한 하네스 프로필 강조** — 모델 및 제공자별 파인튜닝을 위한 하네스 프로필을 소개했습니다.
*   **Hugging Face, 로컬 앱에 Hermes Agent 지원 및 네이티브 트레이스 시각화 추가** — 로컬 앱에서 Hermes Agent를 지원하고 네이티브 트레이스 시각화 기능을 추가했습니다.

### 🔬 연구 & 논문
*   **AllenAI, 모듈식 MoE 설계 'EMO' 발표** — 문서 수준 라우팅이 공유 전문가 풀을 유도하는 MoE 설계를 제안했으며, 전문가의 25%만 유지해도 표준 MoE 대비 성능 손실이 단 ~1%에 불과하다고 보고되었습니다.
*   **MIND (Monge Inception Distance) 소개** — FID를 대체하는 더 빠르고 샘플 효율적인 생성 평가 방법으로 MIND가 제시되었습니다.
*   **비-AR 언어 모델링을 위한 확산 모델 연구** — 연속 비트스트림 확산이 자기회귀 모델과 거의 일치하는 성능을 보인다는 연구 결과가 나왔습니다.
*   **Fast BLT, 병렬 바이트 디코딩을 위한 확산 모델 활용** — 확산을 사용하여 병렬 바이트 디코딩을 통해 바이트 수준 LM의 인퍼런스 바운드를 줄이는 Fast BLT가 소개되었습니다.
*   **확산 모델의 사후 학습 유용성** — 샘플링이 미분 가능하여 보상 기울기가 표준 LLM 설정보다 파라미터로 더 직접적으로 흐를 수 있다는 확산 모델의 유용한 속성이 언급되었습니다.
*   **"The Memory Curse" 연구** — 긴 이력이 다중 라운드 사회적 딜레마에서 협력을 저하시키며, 명시적인 CoT가 때때로 문제를 증폭시킨다고 주장합니다.
*   **PwC 연구, 명확화의 가치 분석** — 목표 명확화는 실행의 약 10% 이후에 대부분의 가치를 잃는 반면, 입력 명확화는 더 오래 유용하게 유지된다는 연구 결과를 발표했습니다.
*   **Marin의 Delphi 스케일링 작업** — 작은 사전 학습에서 25B / 600B 토큰 실행으로 외삽할 때 0.2%의 예측 오류를 주장합니다.
*   **AutoTTS 연구** — LLM이 테스트 시간 스케일링 컨트롤러 공간을 스스로 검색하여 수동으로 설계된 전략을 능가했다고 보고되었습니다.
*   **TurboQuant에 대한 회의론 증가** — TurboQuant에 대한 최초의 포괄적인 연구에서 정확도, 레이턴시, 처리량 측면에서 "실제로 잘 작동하지 않는다"는 결론이 나왔습니다.

### 💰 산업 동향
*   **OpenAI Deployment Company 설립 및 40억 달러 투자 유치** — 기업 고객을 위한 배포 사업부를 설립하고, 19개 파트너로부터 40억 달러의 초기 투자를 유치했습니다.
*   **Hugging Face, 로컬 에이전트 인체공학 강화** — @onusoz가 Hugging Face에 합류하여 OpenClaw 및 관련 오픈 하네스에서 로컬 모델 개선 작업을 진행합니다.

### ⚡ 인프라 & 하드웨어
*   **로컬/오픈 모델 성능 개선 속도, 무어의 법칙 초과** — 동일한 최고급 MacBook Pro 메모리 한계 내에서 실행 가능한 "가장 똑똑한 오픈 웨이트 모델"의 성능이 24개월 동안 약 4.7배 개선되어, 10.7개월마다 두 배로 증가하는 무어의 법칙보다 빠른 속도를 보였습니다.
*   **Unsloth의 Qwen 3.6 MTP GGUF 빌드** — Unsloth는 Qwen3.6-27B-GGUF-MTP 및 Qwen3.6-35B-A3B-GGUF-MTP를 출시했으나, `llama.cpp` MTP PR 빌드가 필요하며 27B GGUF에서 런타임/어설션 실패가 보고되었습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
