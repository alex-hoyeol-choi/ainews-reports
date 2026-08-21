# Poolside gets $12B reverse-execuhire to NVIDIA; founders stay for $1B, employees go for $6B, Infraco scaling to 7GW neocloud - 요약

**원문 URL**: https://www.latent.space/p/ainews-poolside-gets-12b-reverse
**번역일**: 2026-08-21 06:05
**발행일**: 2026-08-21

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식 요약 브리핑입니다.

### 🔥 주요 뉴스
**[Poolside, NVIDIA에 120억 달러 규모의 리버스 엑시큐하이어]** — Poolside의 기술직 직원 109명이 NVIDIA로 이직하고, NVIDIA는 Poolside의 Model Factory를 라이선스했습니다. 창업자들은 10억 달러에 잔류하며 회사를 피벗하고, 직원들은 60억 달러에 이직하는 새로운 형태의 거래가 성사되었습니다. Poolside에서 분사한 PIC infraco는 7GW 규모의 네오클라우드 구축을 목표로 합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/1a668ad4-aca6-4c1c-ac78-5131b8f3d7a8_834x844.png)

### 📊 모델 & 벤치마크
*   **Meta Muse Spark 1.2 벤치마크 공개:** Meta의 Muse Spark 1.2가 시각 코딩, 로봇 공학 계획 및 시청각 이해를 아우르는 데모와 함께 강력한 멀티모달/에이전틱 벤치마크 결과를 보였습니다. Agent Arena에서 순 개선율이 v1.1의 0.9%에서 +2.1%로 증가했으며, DesignArena에서는 Video-to-Website 1위, Image-to-HTML 2위, Image-to-Frontend 3위를 기록했습니다.
*   **Zhipu GLM-5.3 에이전틱/코드 평가:** Zhipu의 GLM-5.3이 Z.ai의 작업 에이전트 AutoClaw에 통합되었으며, Code Arena: WebDev 파레토 프론티어에서 오픈 모델 중 2위, 전체 8위(1597점, 3.65달러/M)를 기록할 것으로 예상됩니다. SAO (Single-Rollout Asynchronous Optimization)가 GLM-5.2/5.3 RL의 핵심 발전으로 재조명되었습니다.
*   **Gemini 3.7 Flash 성능 입증:** Gemini 3.7 Flash가 ARC-AGI-2에서 작업당 0.25달러에 84.6%, ARC-AGI-1에서 작업당 0.12달러에 95.5%를 기록하며 비용 조정 추론 성능에서 두각을 나타냈습니다.
*   **Qwen3.8-27B Dynamic v3 Unsloth GGUF 출시:** Unsloth Dynamic v3.0 GGUF 양자화가 발표되었으며, 동일 모델 크기에서 다른 양자화 제공업체 대비 10% 이상 더 나은 top-1 정확도를 주장합니다. 약 8GB RAM에서 BF16까지 실행 가능한 1비트 양자화를 목표로 합니다.
*   **Qwen3.8-27B의 지식 측면 트레이드오프:** Qwen3.8-27B가 오프라인/가중치 전용 사실 회상에서 Qwen3.6-27B 대비 퇴보했으나, 도구 호출, 코딩 및 에이전틱 워크플로우에는 더 강력한 의도적인 전문화 트레이드오프로 해석됩니다.
*   **Qwen3.8-27B 코딩 벤치마크 결과:** 자체 구축 코딩 평가 벤치마크에서 GPT-5.6-sol이 전반적으로 선두를 달리는 가운데, Qwen3.8-27B xhigh는 어려운 알고리즘에서 강력한 점수를 얻었으며 DS4 0731은 2비트 로컬 양자화임에도 높은 성능을 보였습니다.
*   **Gemma 10억 다운로드 돌파:** Google의 Gemma 모델이 10억 다운로드를 돌파하며 오픈 웨이트 모델의 광범위한 채택을 보여주었습니다.
*   **Kimi K3 출시 확대:** ollama를 통해 Kimi K3가 미국/EU 호스팅 및 제로 데이터 보존으로 구독자 기반의 절반 이상에 출시되었습니다.

### 🛠️ 제품 & 도구
*   **OpenAI ChatGPT 데스크톱 기능 확장:** Mac용 ChatGPT Work/Codex를 위한 Apple Messages 플러그인을 출시하여 데스크톱 앱에서 메시지 검색, 작성 및 전송을 가능하게 했습니다.
*   **OpenAI ChatGPT Sites 협업 편집 기능 추가:** ChatGPT Sites에 협업 편집 기능이 추가되어 팀원들이 프로젝트를 공유하는 동안 Codex가 git/CI를 관리할 수 있게 되었습니다.
*   **OpenAI GPT-Image-2 투명 배경 기능 미리 보기:** GPT-Image-2의 투명 배경 기능이 재사용 가능한 디자인 자산을 위해 현재 미리 보기로 제공됩니다.
*   **OpenAI 데스크톱 메모리/워크플로우 기능 지역 확대:** 컴퓨터 기록 및 앱 간 메모리 기능, Record & Replay 기능이 EEA, 영국, 스위스 Pro/Business/Enterprise Mac 사용자에게 제공됩니다.
*   **Anthropic Claude Platform 에이전트 기능 GA:** Claude Platform에서 컴퓨터 사용, 브라우저 도구, Skills API 및 Files API의 일반 가용성(GA)을 발표했습니다.
*   **Anthropic Skills API 및 Files API 개선:** Skills API는 버전 관리되는 재사용 가능한 절차를 추가하며, Files API는 만료 제어, 5배 높은 속도 제한(500 RPM), 조직당 1TB를 지원합니다.
*   **Anthropic Claude Managed Agents용 AG-UI 어댑터:** Claude Managed Agents를 위한 AG-UI 어댑터를 발행하여 채팅 스레드를 관리 세션에 매핑하고 사용자 정의 UI로 스트리밍합니다.
*   **Awesome Gemma 레포 출시:** _philschmid가 Gemma의 변형, 배포 가이드 및 파인튜닝 레시피를 집계하는 Awesome Gemma 레포를 출시했습니다.

### 🔬 연구 & 논문
*   **Chroma의 자체 개선 메모리 'Foundation' 연구 미리 보기:** Chroma가 이전 에이전트 세션에서 구축된 에이전트 메모리 접근 방식인 Foundation의 연구 미리 보기를 출시했습니다.
*   **하네스 지속 학습 연구 강조:** 프롬프트, 메모리, 스킬 및 라우팅 규칙이 모델과 독립적으로 진화하는 하네스 지속 학습에 대한 논문이 강조되었습니다. 보호된 하네스 진화는 텍스트, 멀티모달 및 오픈 월드 작업 전반에서 10% 이상의 개선을 보고했습니다.
*   **메모리 기반 자체 개선 에이전트의 한계 연구:** 메모리 기반 자체 개선 에이전트가 작업 순서 효과 및 평가 분산을 제어하면 성능이 저하될 수 있다는 연구 결과가 나왔습니다.
*   **에이전트의 초기 전략 고착 경향 논문:** 학습 후 에이전트가 초기 전략에 일찍 고착되어 전략적 선택 자체를 재검토하기보다는 지역적 개선에 집중하는 경향이 있다는 논문이 요약되었습니다.

### 💰 산업 동향
*   **Poolside의 NVIDIA "리버스 엑시큐하이어":** Poolside의 기술직 직원 109명이 NVIDIA로 이직하고, NVIDIA는 Poolside의 Model Factory를 라이선스했습니다. 창업자들은 10억 달러에 잔류하며 회사를 피벗하고, 직원들은 60억 달러에 이직했습니다.
*   **AT&T의 하이브리드 AI 라우팅 사례:** AT&T는 직원 AI 사용량의 40%를 오픈 모델로 라우팅하고 있으며, 목표는 60~70%입니다. 이를 통해 코딩 비용을 2% 품질 저하만으로 56% 절감하고 하루 450억 토큰을 처리합니다.
*   **클로즈드 모델 가격 압력 심화:** Router를 통해 GPT-5.6 Sol이 50% 할인 발표되었고, GitHub Copilot / VS Code 사용자 대상 임시 할인도 확대되었습니다.

### ⚡ 인프라 & 하드웨어
*   **OpenAI의 NVIDIA Vera Rubin 랙 설치:** OpenAI의 첫 번째 NVIDIA Vera Rubin 랙이 설치되어 학습 스택을 실행 중이며, 이는 차세대 프론티어 사전 학습과 연결됩니다.
*   **Cerebras CS-4 인퍼런스 스케일링 성능 향상:** Cerebras의 CS-4는 재설계된 전력 공급 및 냉각을 통해 동일한 5nm 웨이퍼에서 성능을 두 배로 늘렸습니다. WSE-3 Turbo당 250 PFLOPs, 43.2 PB/s 메모리 대역폭을 제공하며, GPT-OSS-120B에서 GPU 기반 시스템보다 최대 30배 빠른 사용자당 4,400+ 토큰/초를 달성합니다.
*   **Linux의 에이전트 워크로드 성능 우위:** Linux가 파일 시스템 사용량이 많은 에이전트 워크로드에서 macOS보다 실질적으로 우수한 성능을 보인다고 주장되었습니다.
*   **Qdrant_engine의 시맨틱 캐싱 보고서:** Qdrant_engine이 57.1%의 적중률, 55.7% 적은 토큰 사용량, 약 15ms의 적중 레이턴시를 보여주는 실용적인 시맨틱 캐싱 보고서를 공유했습니다.
*   **Gisting 기술의 효율성:** Gisting이 약 40% 낮은 엔드투엔드 레이턴시와 약 15% 높은 처리량으로 더 나은 결과를 얻을 수 있는 활용도가 낮은 프로덕션 기술로 추진되고 있습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
