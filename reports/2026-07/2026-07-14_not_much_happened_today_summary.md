# not much happened today - 요약

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-c72
**번역일**: 2026-07-15 00:54
**발행일**: 2026-07-14

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 뉴스 브리핑입니다.

### 🔥 주요 뉴스
**[OpenAI GPT-5.6 Sol, 폭발적 수요로 스케일링 문제 직면]** — OpenAI의 GPT-5.6 Sol 모델이 출시 이후 "엄청난" 수요를 기록하며 인프라 스케일링에 어려움을 겪고 있습니다. Codex + ChatGPT Work의 사용량도 일주일 만에 2.5배 증가했습니다.
**[PrismML, 소비자 기기용 Bonsai 27B 모델 출시]** — PrismML이 Qwen 3.6 27B 기반의 Bonsai 27B 모델을 Ternary(5.9GB) 및 1-bit(3.9GB) 두 가지 컴팩트 변형으로 Apache 2.0 라이선스 하에 공개했습니다. 이 모델은 멀티모달, 도구 사용, 긴 컨텍스트 에이전틱 워크플로우를 로컬에서 지원합니다.
**[Sakana AI, 물리적 자가 수리 시스템 "Smart Cellular Bricks" 발표]** — Sakana AI가 Nature Communications에 "Smart Cellular Bricks" 연구를 게재했습니다. 이 시스템은 중앙 제어 없이 손상을 감지하고 전역적인 모양을 추론하며, 6가지 공간 방향에서 95% 정확도로 누락된 이웃을 감지하고 목표 구조를 재생할 수 있습니다.
**[OpenMOSS, 실시간 비디오 스트림용 MOSS-VL-Realtime 모델 출시]** — OpenMOSS가 연속 비디오 스트림 처리에 특화된 256K 컨텍스트의 11B 비전-언어 모델 MOSS-VL-Realtime을 Apache 2.0 라이선스로 출시했습니다. 이 모델은 생성 중에도 비디오를 계속 시청하고 답변을 수정할 수 있습니다.
**[Perplexity, 에이전틱 연구 벤치마크 WANDR 오픈소스화]** — Perplexity가 500개 작업으로 구성된 광범위하고 심층적인 에이전틱 연구 벤치마크 WANDR을 오픈소스화했습니다. WANDR은 동적인 웹 연구에 맞춰 인용된 페이지를 다시 가져와 증거를 확인하는 방식으로 평가합니다.

### 📊 모델 & 벤치마크
*   PrismML이 Qwen 3.6 27B 기반의 Bonsai 27B 모델(Ternary 및 1-bit 변형)을 Apache 2.0 라이선스로 출시했습니다.
*   Tencent Hunyuan이 1-bit 및 4-bit Hy3 모델(295B 플래그십 규모)을 출시했습니다.
*   OpenMOSS가 연속 비디오 스트림 처리를 위한 256K 컨텍스트의 11B 비전-언어 모델 MOSS-VL-Realtime을 Apache 2.0 라이선스로 출시했습니다.
*   ZhihuFrontier가 Qwen2.5-Omni-7B 기반의 OmniAgent를 공개했으며, 이는 Observation–Thought–Action 루프를 사용하여 필요한 프레임/오디오만 요청합니다.
*   OmniAgent-7B가 LVBench에서 50.5점을 기록하며 Qwen2.5-VL-72B를 능가하고, 훨씬 적은 프레임(203프레임)으로 더 높은 성능을 달성했습니다.
*   LingBot-World 2.0이 시간 단위 규모의 720p/60fps 대화형 생성을 지원하는 최초의 오픈 릴리스 중 하나로 소개되었습니다.
*   Perplexity가 500개 작업으로 구성된 에이전틱 연구 벤치마크 WANDR을 오픈소스화했습니다.
*   Agent Arena가 시스템 비용을 89% 절감하면서도 최고 수준의 정적 구성 정확도를 유지하는 방법을 제시하며, LLM 라우팅 단독보다 전체 시스템 구성이 우월하다고 밝혔습니다.
*   SlopCodeBench가 에이전트가 순차적 작업에서 코드베이스를 어떻게 침식하는지 측정하는 새로운 벤치마크로 소개되었습니다.

### 🛠️ 제품 & 도구
*   JetBrains가 Codex를 권장 에이전트로 지정했습니다.
*   OpenAI 팀이 GPT-5.6으로 처음부터 끝까지 구축된 명령줄 평가 도구를 시연했습니다.
*   LangChain이 Codex에 대한 트레이싱을 추가하고 LangSmith 기능을 Cursor, Copilot, Pi, OpenCode로 확장했습니다.
*   Teknium이 Hermes Agent를 업데이트하여 도구 호출 병렬화 및 뱅크 리셋 기능을 개선했습니다.
*   PixVerse Game이 실시간 대화형 비디오 응답이라는 새로운 애플리케이션 분야를 추구하고 있습니다.
*   Airtap이 SMS를 모바일 앱을 위한 헤드리스 에이전틱 실행 계층으로 전환하는 새로운 서비스를 선보였습니다.

### 🔬 연구 & 논문
*   Sakana AI가 Nature Communications에 "Smart Cellular Bricks" 연구를 발표했습니다. 이 시스템은 중앙 제어 없이 손상을 감지하고 전역적인 모양을 추론할 수 있습니다.
*   Google DeepMind의 모델 라우팅 연구는 라우터 평가 시 정확성/비용 외에 전문가 간 행동 차별화 및 패러프레이즈 하에서의 안정성도 고려해야 한다고 제안했습니다.
*   RekaAILabs가 페타바이트 규모의 비디오와 6단계 파이프라인을 포함하는 옴니 월드 모델의 데이터 스택을 공개했습니다.

### 💰 산업 동향
*   Demis Hassabis의 AGI 거버넌스 제안이 주요 정책 논의의 중심이 되었습니다.

### ⚡ 인프라 & 하드웨어
*   Daniel Hanchen이 Gemma-4 제품군 및 Qwen3.5-122B-A10B, GLM-4.7-Flash 모델에 NVFP4 동적 양자화를 발표했습니다.
*   MiaAI_lab이 1M 컨텍스트 DeepSeek v4 Flash, MiMo-V2.5(2x DGX Sparks), GLM 5.2 NVFP4(4x DGX Sparks)를 포함한 멀티 노드 로컬 배포를 시연했습니다.
*   Alex Toussss가 자율 마이크로 드론이 비행하는 나방을 공중에서 요격하는 데모를 공개했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
