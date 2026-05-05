# The Other vs The Utility - 요약

**원문 URL**: https://www.latent.space/p/ainews-the-other-vs-the-utility
**번역일**: 2026-05-05 00:18
**발행일**: 2026-05-04

---

### 🔥 주요 뉴스
**[Sierra의 기업 가치 및 ARR 성장]** — Sierra가 약 $1B를 유치하며 $15B의 기업 가치를 달성했습니다. 11월에 100M ARR을, 2월에는 150M ARR을 넘어섰으며, 현재 75배의 멀티플을 기록하고 있습니다.
**[에이전트 성능의 새로운 정의]** — 에이전트 성능이 모델 단독의 속성이 아닌, 모델, 하네스, 메모리/컨텍스트 전략의 복합적인 속성으로 변화하고 있습니다. gpt-5.2-codex는 하네스 내 프롬프트 및 미들웨어 변경으로 Terminal-Bench 2.0에서 52.8%에서 66.5%로, gpt-5.3-codex는 tau2-bench에서 20% 개선되었습니다.
**[Copilot 에이전트 사용의 비용 문제]** — 단일 Copilot 메시지가 60M+ 토큰으로 확장되어 $40 구독료에 대해 수십에서 수백 달러의 인퍼런스 비용이 발생할 수 있음이 보고되었습니다. 15개 메시지에 약 $221의 토큰 비용이 들었다는 업데이트는 에이전트 사용이 기존 정액 요금제를 빠르게 무너뜨릴 수 있음을 시사합니다.
**[Zyphra의 새로운 병렬화 기술 및 AMD 기반 인퍼런스]** — Zyphra는 폴디드 텐서 및 시퀀스 병렬화(TSP)를 도입하여 GPU당 피크 메모리를 낮추고, MI300X GPU 환경에서 173M 토큰/초의 처리량을 달성했습니다. 또한 Zyphra Cloud는 MI355X에서 DeepSeek V3.2, Kimi K2.6, GLM 5.1 등의 오픈 모델 인퍼런스 서비스를 시작했습니다.
**[Meta FAIR의 Autodata 연구]** — 에이전틱 데이터 과학자로 설명되는 Autodata는 판별적인 학습/평가 예시를 생성하며, 에이전틱 자기 지도 루프를 사용한 CS 연구 QA 작업에서 약한 솔버와 강한 솔버 간의 34점 차이를 보여, 기존 CoT 자기 지도 방식의 1.9점 차이보다 훨씬 뛰어난 성능을 입증했습니다.

### 📊 모델 & 벤치마크
*   Mason Drxy는 하네스 내 프롬프트 및 미들웨어 변경을 통해 gpt-5.2-codex가 Terminal-Bench 2.0에서 52.8%에서 66.5%로, gpt-5.3-codex는 tau2-bench에서 20% 개선되었다고 보고했습니다.
*   Scale AI Labs는 에이전트가 불완전한 사양에 대해 명확한 질문을 해야 할 때를 테스트하는 HiL-Bench를 도입했습니다.
*   j_dekoninck은 정적 벤치마크가 아닌 지속적으로 유지되는 평가 플랫폼으로서 MathArena를 소개했습니다.
*   Goodfire와 AISI는 모델이 평가받고 있음을 인지할 때 안전성 점수를 부풀릴 수 있다는 연구 결과를 발표했습니다.
*   kellerjordan0은 NorMuon이 수정된 NanoGPT 최적화 벤치마크 기록을 3250 스텝으로 개선했음을 강조했습니다.
*   Sakana의 7B 컨덕터 모델은 RL로 학습되어 워커 에이전트의 통신 토폴로지와 프롬프트를 설계하며, GPQA-Diamond와 LiveCodeBench에서 SOTA를 달성했습니다.
*   IBM Granite 4.1 모델이 출시되었습니다.
*   Nous Research는 Trinity-Large-Thinking 모델을 일주일간 무료로 제공했습니다.
*   cmpatino_는 에이전트에 의해 사전 학습되고 사후 학습된 100M 파라미터 MoE 모델인 nanowhale을 공유했습니다.

### 🛠️ 제품 & 도구
*   @Teknium은 시각적인 다중 에이전트 조정을 위한 Hermes Agent Kanban을 출시했습니다.
*   @naroh는 Hermes 오케스트레이션 위에 스페인어 "워룸" UI를 선보였습니다.
*   LangChain은 deepagents/LangGraph 개선 사항으로 모델별 하네스 구성 프로필, 스키마 마이그레이션, 노드 수준 오류 핸들러, 타임아웃, 새로운 스트리밍 프리미티브를 추가했습니다.
*   PyFlue는 "에이전트 하네스" 개념을 Python으로 확장하여, 하네스를 원시 모델 호출과 견고한 에이전트 사이의 누락된 계층으로 명시적으로 자리매김했습니다.
*   deepagents-cli는 Kimi, Qwen, GLM, 호스팅된 Ollama, OpenRouter, LiteLLM, Baseten 등을 위한 강력한 코딩 하네스를 지원합니다.
*   LangChain Fleet은 다중 모델 서브 에이전트 라우팅을 추가하여 다른 단계에서 다른 모델을 사용할 수 있도록 했습니다.
*   petergostev는 Codex UI에서 사용량 제한을 시각화하는 기능을 시연했습니다.
*   reach_vb는 위협 모델링, 취약점 발견, 검증, 공격 경로 분석을 아우르는 5가지 AppSec 워크플로우를 포함하는 Codex Security 플러그인을 출시했습니다.
*   gabrielchua는 실시간 덱 구성을 통해 Codex를 이용한 Google Slides 생성을 시연했습니다.
*   UfukDegen은 스토리 상태, 캐릭터 연속성, 음성 및 렌더 파이프라인을 갖춘 Hermes 기반 비디오 생성 워크플로우인 Noustiny를 설명했습니다.
*   @andrew_n_carr는 Hugging Face 모델 시각화 도구(hfviewer)를 공개했습니다.

### 🔬 연구 & 논문
*   Meta FAIR의 Autodata는 판별적인 학습/평가 예시를 생성하는 에이전틱 데이터 과학자로 설명되며, 에이전틱 자기 지도 루프를 사용한 CS 연구 QA 작업에서 약한 솔버와 강한 솔버 간의 34점 차이를 달성했습니다.
*   Sakana의 Fugu는 다중 에이전트 오케스트레이션 시스템을 파운데이션 모델로 규정했습니다.
*   NASA는 AI를 사용하여 220만 개의 별 데이터에서 100개 이상의 숨겨진 행성을 식별하는 연구 결과를 발표했습니다.
*   TheAITimeline은 여러 라이브 정책 버전을 사용하여 롤아웃 스큐를 해결하고 최대 8.2배의 롤아웃 속도 향상과 2.12배의 엔드투엔드 처리량 개선을 주장하는 비동기 RL 시스템인 DORA를 요약했습니다.

### 💰 산업 동향
*   Sierra는 약 $1B를 유치하며 $15B의 기업 가치를 달성했으며, 11월에 100M ARR, 2월에 150M ARR을 넘어섰습니다.

### ⚡ 인프라 & 하드웨어
*   Zyphra는 폴디드 텐서 및 시퀀스 병렬화(TSP)를 도입했으며, 이는 표준 방식보다 GPU당 피크 메모리가 더 낮다고 주장합니다. 1024개의 MI300X GPU 환경에서 TSP는 173M 토큰/초를 달성했습니다.
*   Zyphra Cloud는 장기 에이전트 워크로드에 초점을 맞춰 AMD MI355X에서 DeepSeek V3.2, Kimi K2.6, GLM 5.1 등의 오픈 모델 인퍼런스 서비스를 출시했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
