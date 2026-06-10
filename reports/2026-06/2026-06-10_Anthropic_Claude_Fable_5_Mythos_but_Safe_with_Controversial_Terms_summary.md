# Anthropic Claude Fable 5 — Mythos but Safe, with Controversial Terms - 요약

**원문 URL**: https://www.latent.space/p/ainews-anthropic-claude-fable-5-mythos
**번역일**: 2026-06-10 06:23
**발행일**: 2026-06-10

---

### 🔥 주요 뉴스
**[Anthropic, Claude Fable 5 및 Mythos 5 출시]** — Claude Fable 5는 Anthropic의 첫 번째 범용 Mythos급 모델로, Opus보다 최소 2배 크며 FrontierCode Diamond 벤치마크에서 29.3%를 기록하는 등 SOTA 성능을 달성했습니다. API 가격은 Opus의 약 2배이며, 1M 토큰 컨텍스트를 지원합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/7af8f73c-7a20-4f7e-ac83-a05cbc892d8b_2318x1684.png)
**[Anthropic, 프론티어 LLM 개발에 대한 '조용한 개입' 정책 도입]** — Claude Fable 5는 프론티어 LLM 개발을 목표로 하는 요청(예: 사전 학습 파이프라인 구축)에 대해 모델 효과를 제한하는 새로운 개입을 구현했습니다. 이는 사용자에게 통지 없이 프롬프트 수정, 스티어링 벡터, PEFT 등을 통해 이루어지며, 약 0.03%의 트래픽에 영향을 미칠 것으로 추정됩니다.
**[Xiaomi, 8-GPU 서버에서 1T MoE 모델로 1,000+ tps 달성 주장]** — Xiaomi MiMo는 TileRT 모델-시스템 공동 설계를 통해 단일 "표준" 8-GPU 서버에서 1T-파라미터 MoE 모델로 1,000+ 토큰/초 디코딩을 달성했다고 주장합니다. 이는 선택적 FP4/MXFP4 퀀타이제이션 및 DFlash 블록 레벨 마스크 추측성 디코딩 기술을 활용하며, 모델 가중치는 Hugging Face에서 공개되었습니다.

### 📊 모델 & 벤치마크
*   Anthropic은 Claude Fable 5 및 제한된 접근의 Mythos 5를 출시했습니다. Fable 5는 CursorBench에서 72.9%, Terminal-Bench 2.1에서 88.0%, Intelligence Index에서 64.9%를 기록하며 여러 벤치마크에서 SOTA 성능을 보였습니다.
*   Cohere는 첫 오픈소스 코딩 모델인 North Mini Code를 출시했습니다. 이 모델은 30B/3B MoE 아키텍처, 256K 컨텍스트, Apache 2.0 라이선스를 가지며 에이전틱 워크플로우에 최적화되었습니다.
*   새로운 벤치마크 Agents’ Last Exam (ALE)이 노동 시장에 맞춰진 에이전트 성능을 테스트하기 위해 출시되었습니다.
*   iOSWorld 벤치마크가 26개의 맞춤형 iOS 앱과 133개의 작업을 통해 개인 지능형 전화 에이전트를 평가하기 위해 도입되었습니다.

### 🛠️ 제품 & 도구
*   Anthropic Claude Fable 5는 사이버 보안, 생물학/화학 및 디스틸레이션 관련 프롬프트에 대해 Claude Opus 4.8로 투명하게 폴백되는 안전 장치를 포함합니다.
*   Anthropic은 Fable 5의 폴백 메커니즘을 Python, TypeScript, Go, Java, C#용 SDK 미들웨어를 통해 제공합니다.
*   Google은 70개 이상의 언어로 실시간 음성-음성 번역을 제공하는 Gemini 3.5 Flash Live Translate를 발표했습니다. 이는 Gemini API, AI Studio, Google Translate에서 사용 가능하며, Google Meet에도 출시될 예정입니다.
*   vLLM은 vLLM 생태계를 위한 RL 사후 학습 프레임워크인 vime을 소개했습니다.
*   OpenAI는 Responses API의 웹 검색 기능에 이미지 결과를 추가했습니다.
*   GitHub Copilot 앱 업데이트에는 병렬 서브 세션 및 동적 인터페이스를 위한 캔버스 UI가 포함되었습니다.
*   Hermes Desktop은 Ollama 지원을 추가하고 자체 학습 Python 기술 및 메시징 앱 통합 기능을 제공합니다.
*   Google의 Gemma 팀은 공식 Gemma 4 챗 템플릿에 `preserve_thinking` 기능을 추가했습니다.

### 🔬 연구 & 논문
*   LCLM(Latent Context Language Models)이 최대 16배의 컨텍스트 압축을 통해 KV-캐시 압축보다 레이턴시/정확도 프론티어를 개선하는 장문 컨텍스트 인퍼런스 방법으로 소개되었습니다.
*   Microsoft Research의 Mirage는 3D 장면을 잠재 토큰으로 저장하여 10.57배 빠른 비디오 생성과 55배 낮은 메모리 사용량을 보고했습니다.
*   Axiom은 Lean 기반 경제학 라이브러리인 EconLib을 발표했으며, Aumann의 "의견 불일치에 동의하기" 정리를 형식화하는 과정에서 숨겨진 가산성 관련 가정이 드러났습니다.
*   "Economy of Minds" 연구는 중앙 집중식 오케스트레이션 대신 경매와 인센티브를 통한 에이전트 조정을 제안하며, 수학 추론 및 금융 연구에서 성능 향상을 보고했습니다.
*   Mayo Clinic의 REDMOD는 CT 스캔에서 진단 최대 3년 전에 췌장암을 감지했으며, 진단 중앙값 475일 전에 숨겨진 암의 73%를 식별했다고 보고되었습니다.

### 💰 산업 동향
*   Anthropic은 Claude Fable 5 사용 시 퍼스트 파티 및 서드 파티 서비스 모두에서 30일 데이터 보존을 요구하는 정책을 도입했습니다. 이 데이터는 새로운 Claude 모델 학습이나 안전성 관련 목적으로만 사용됩니다.
*   Anthropic은 Claude Fable 5를 6월 22일까지 Pro, Max, Team 및 좌석 기반 Enterprise 플랜에 포함한 후, 용량 제약으로 인해 사용 크레딧이 필요할 것이라고 밝혔습니다.
*   Claude Fable 5 및 Mythos 5의 API 가격은 입력 토큰 100만 개당 $10, 출력 토큰 100만 개당 $50로 책정되었습니다.
*   Hugging Face와 Arcee는 모든 Arcee 모델 및 데이터셋(비공개 데이터셋 포함)에 대해 AWS S3를 Hugging Face로 대체하는 파트너십을 발표했습니다.
*   Marks Saroufim은 프론티어 연구실의 제한된 접근에 대응하여 연구자 상호 라이선스(Researcher Reciprocity License)를 제안하고 GPU MODE 데이터셋을 이 라이선스로 이전했습니다.

### ⚡ 인프라 & 하드웨어
*   Xiaomi MiMo는 TileRT 모델-시스템 공동 설계를 통해 단일 "표준" 8-GPU 서버에서 1T-파라미터 MoE 모델로 1,000+ 토큰/초 디코딩을 달성했다고 주장했습니다.
*   Google과 Hugging Face는 단일 A10G에서 Gemma 4 E4B의 품질 저하 없이 속도를 높이는 Fast Gemma Challenge를 시작했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
