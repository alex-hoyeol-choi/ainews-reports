# Andrew Ng gets into AI Engineering - 요약

**원문 URL**: https://www.latent.space/p/ainews-andrew-ng-gets-into-ai-engineering
**번역일**: 2026-08-25 06:05
**발행일**: 2026-08-25

---

### 🔥 주요 뉴스
**[Andrew Ng의 DeepLearning.ai, AI Engineering에 집중]** AI 분야의 선구자인 Andrew Ng가 DeepLearning.ai의 초점을 AI Engineering으로 전환하고 4가지 핵심 기술을 강조했습니다. 이는 10,000개 이상의 채용 공고 분석과 전문가 인터뷰를 기반으로 한 중요한 산업 동향 변화를 반영합니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/3107842a-995c-42c3-a41a-592339e041f8_1002x1182.png)
**[Anthropic, 엔터프라이즈 MCP 관리 인증 출시]** Anthropic이 MCP 커넥터용 엔터프라이즈 관리 인증을 출시하여 조직의 ID 공급자를 통한 권한 부여 중앙 집중화를 가능하게 했습니다. 이를 통해 Asana, Atlassian 등 주요 커넥터에 대한 도구별 OAuth 필요성을 없애 엔터프라이즈 에이전트 배포의 중요한 진전을 이루었습니다.
**[Liquid AI + Artificial Analysis, 온디바이스 AI 벤치마크 스위트 'Pipette' 공개]** Liquid AI와 Artificial Analysis가 온디바이스 인퍼런스 성능 측정을 위한 오픈소스 평가 스위트 Pipette을 출시했습니다. 이 스위트는 35개 모델 클래스, 7개 양자화, llama.cpp 런타임 및 4개 장치에 걸쳐 10,000개 이상의 검증된 결과를 포함하며, iPhone 17 Pro 및 Galaxy S26 Ultra에 대한 독립적인 평가도 제공합니다.
**[NVIDIA Groq 3 LPX, 에이전트별 처리량 경쟁 가속화]** NVIDIA의 Groq 3 LPX는 Vera Rubin에 전용 토큰 생성 가속기를 추가하여 Artificial Analysis 벤치마킹에서 100K 컨텍스트의 Gemma 4 31B에서 3,400 출력 토큰/초를 달성했다고 주장했습니다. 이는 인퍼런스 벤더들이 원시 TPS를 넘어 에이전트별 처리량으로 경쟁하는 새로운 추세를 보여줍니다.
**[OpenAI, GPT-5.6 출시 및 API 가격 인하]** OpenAI가 Kiro에서 GPT-5.6을 출시하고, Kiro의 Terra 변형에서 Terminal-Bench 2.1 작업당 약 82%의 비용 절감을 발표했습니다. 또한 GPT-5.6 Sol API 가격을 입력 토큰당 $4/M, 출력 토큰당 $20/M으로 인하하여 비용 효율성을 개선했습니다.

### 📊 모델 & 벤치마크
*   Qwen3.8-27B 모델이 Code Arena: WebDev에서 1595점으로 전체 9위를 차지하며, 해당 크기 클래스에서 유일한 모델로 뛰어난 성능을 입증했습니다.
*   미출시 프론티어 모델인 "claude-melon-eap", "claude-marshmallow-eap", Ox Alpha, Qwen 4, GPT Astra 등의 징후가 포착되었으며, 3D/RL 스타일 작업에 중점을 둔 EAP 모델이 보고되었습니다.
*   Together AI는 $100 예산으로 GLM-5.3이 DeepSWE에서 Fable 5보다 5배 더 많은 작업을 완료했다고 보고하며, 비용 정규화된 에이전트 벤치마크에서 GLM-5.3의 효율성을 강조했습니다.
*   DeepSWE v1.1 벤치마크에서 GPT-5.6 Sol Max는 작업당 $6.47에 72.7%를 기록한 반면, Fable 5 Max는 69.7%에 작업당 $21.63을 기록하여 GPT-5.6 Sol Max의 비용 효율성이 우수함을 보였습니다.
*   폰 스케일 평가 결과, 8GB 메모리 / 16K 컨텍스트 프레이밍 하에서 Nanbeige4.2-3B와 LFM2.5-2.6B가 평균 점수 63점으로 최고를 기록했으며, LFM2.5-2.6B는 iPhone에서 Nanbeige보다 훨씬 더 효율적이었습니다.

### 🛠️ 제품 & 도구
*   @andykonwinski는 요청 시에만 생각하는 것이 아니라 지속적으로 생각하는 지속형 에이전트를 위한 오픈소스 "마이크로하네스"인 Headlong을 소개했습니다. 이 시스템은 궤적을 jsonl 파일의 DAG로 저장하고 자체 안내 내부 루프를 실행합니다.
*   @omarsar0는 추가 전용 이벤트 로그, 교체 가능한 실행기, 스냅샷/롤백 가능한 샌드박스를 갖춘 재귀적 자체 개선을 위한 하네스 아키텍처인 exo를 설명했습니다. 이는 에이전트가 영구적인 상태를 손상시키지 않고 프롬프트/도구/메모리를 다시 작성할 수 있도록 설계되었습니다.
*   @a1zhang은 코드 생성 중에 안전한 도구 호출을 예측하고 환경 복사본에서 일찍 실행하여 실행이 토큰 생성과 겹치도록 하는 Speculative Programmatic Tool Calling (sPTC)을 소개했습니다.

### 🔬 연구 & 논문
*   NVIDIA의 새로운 평가 연구는 에이전트 "기술"에 대한 구조적 검사가 유용성을 거의 예측하지 못하며, 대신 동일한 조건에서 기술 유무에 따른 작업 완료 차이를 점수화하는 "Skill Lift" 측정을 제안했습니다.
*   @cwolferesearch는 토큰 수준 대 완료 수준 공식화, PPO/GRPO 변형, 액터-크리틱 메서드, 루브릭 기반 RL 및 에이전틱 RL/월드 모델링을 다루는 포괄적인 강화 학습 가이드를 발표했습니다.
*   Meta/USC의 Periodic Row-wise Muon은 값비싼 Newton–Schulz 업데이트를 상각하면서 AdamW에 대한 이득을 유지함으로써 Muon 최적화를 더 큰 확산 트랜스포머로 확장하는 연구를 발표했습니다.
*   Adobe의 Latent Dynamics Reasoning은 직접적인 미래 예측 대신 잠재 상태 진화를 모델링하여 픽셀에서 외삽적 비디오 월드 모델을 학습합니다.
*   Cartwheel은 인간 동작 생성에 대한 컴퓨팅 최적 스케일링 법칙을 보고했으며, 동작이 Chinchilla와 유사한 스케일링 동작을 가진 다섯 번째 양식이 될 수 있다고 주장했습니다.

### 💰 산업 동향
*   Andrew Ng의 DeepLearning.ai가 AI Engineering에 초점을 맞춰 재출시되었습니다. 이는 "AI 애플리케이션 구축 및 배포", "소프트웨어 엔지니어링 기본", "코딩 에이전트 사용", "빌드 형성"의 4가지 핵심 AI 엔지니어링 기술을 강조합니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/be233653-3987-4e57-82c9-d541fb5e3265_1936x774.jpeg)
*   Anthropic은 MCP 커넥터용 엔터프라이즈 관리 인증을 출시하여 조직의 ID 공급자를 통해 권한 부여를 중앙 집중화했습니다.
*   OpenAI는 GPT-5.6 Sol API 가격을 입력 토큰당 $4/M, 출력 토큰당 $20/M으로 인하했습니다.

### ⚡ 인프라 & 하드웨어
*   Liquid AI + Artificial Analysis는 모델 + 양자화 + 런타임 + 장치 조합 전반에 걸쳐 품질, 속도, 레이턴시 및 메모리를 측정하는 온디바이스 인퍼런스용 오픈소스 평가 스위트인 Pipette을 출시했습니다.
*   폰 스케일 평가에서 MoE 설계(LFM2.5-8B-A1B 및 Ling 3.0 Tiny)는 토큰당 약 1B 매개변수를 활성화하여 휴대폰 하드웨어에서 6초 미만의 응답을 가능하게 합니다.
*   NVIDIA의 Groq 3 LPX는 Vera Rubin에 전용 토큰 생성 가속기를 추가했으며, Artificial Analysis 벤치마킹에서 100K 컨텍스트의 Gemma 4 31B에서 3,400 출력 토큰/초를 달성했다고 주장했습니다.
*   vLLM은 실제 다중 턴 코딩 트레이스에 대한 광범위한 AgentX 1.0 결과를 발표하며, 고성능 에이전틱 처리량의 핵심으로 KV 오프로드, 접두사 재사용 및 프리필/디코드 분리를 강조했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
