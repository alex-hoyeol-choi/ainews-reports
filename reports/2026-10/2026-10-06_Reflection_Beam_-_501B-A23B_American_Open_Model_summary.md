# Reflection Beam - 501B-A23B American Open Model - 요약

**원문 URL**: https://www.latent.space/p/ainews-reflection-beam-501b-a23b
**번역일**: 2026-10-06 12:28
**발행일**: 2026-10-06

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 브리핑입니다.

### 🔥 주요 뉴스
**[Reflection Beam 출시]** — 미국에서 처음부터 학습된 501B-total / 23B-active MoE 모델 Beam을 Apache 2.0 라이선스로 공개했습니다. 코딩, 에이전트, 과학 작업을 위한 모델로, SWE-bench Verified에서 80.9점을 기록하며 GLM 5.2 대비 3~4배의 인퍼런스 효율성을 주장합니다.
![Reflection Beam Model Comparison](https://substack-post-media.s3.amazonaws.com/public/images/92c7acf0-990a-45f0-b3ee-b1d7702184bd_874x894.png)
**[OpenAI 서비스 속도 50% 향상]** — GPT-6 Astra 및 GPT-6.1 Sol의 기본 속도가 약 30 TPS에서 약 50 TPS로 50% 증가했습니다. 이 개선 사항은 모든 구독 서비스와 OpenCode, Pi, Amp, Devin 등 Sign in with ChatGPT 파트너에게 적용됩니다.
**[OpenAI 텍스트 워터마킹 도입]** — EU AI Act 준수를 위해 EU 내 적격 ChatGPT 및 Codex 텍스트에 보이지 않는 통계적 워터마크를 추가하며, 전 세계적으로 API 토글을 제공합니다. 단, 재작성 또는 번역 시 워터마크가 제거될 수 있습니다.
**[Alibaba T-Head Zhenwu V900 가속기 발표]** — 216GB 메모리와 1,200GB/s 인터커넥트를 갖춘 Zhenwu V900을 발표했습니다. M890보다 3배 빠르다고 주장하며, 2027년 1분기 출시 예정입니다.
**[Tencent, Oracle로부터 10만 개 고급 칩 임대]** — FT 보도에 따르면 텐센트가 Oracle의 동남아시아 데이터센터에서 약 10만 개의 고급 칩을 5년간 약 70억 달러에 임대했습니다.

### 📊 모델 & 벤치마크
*   **Reflection Beam:** 501B-total / 23B-active MoE 모델 Beam을 출시했습니다. SWE-bench Verified 80.9점, GLM 5.2 대비 3~4배 인퍼런스 효율성을 주장하며, 23.8T 사전 학습 토큰을 사용했습니다.
*   **Aleph Alpha Kolibri:** 78B total / 3.46B active, Apache 2.0 라이선스의 독일어 및 영어 모델을 공개했습니다. AIME 2025 96.9%, GPQA Diamond 84.3%, SWE-Bench Verified 66.4%의 자체 보고 점수를 기록했습니다.
*   **Reka Rho-1:** 텍스트, 이미지, 비디오, 로봇 동작을 이해하고 생성하는 19B 옴니 모델을 발표했습니다. 320개의 H100s에서 약 3개월 동안 처음부터 학습되었습니다.
*   **Command Code Agr & Agr-flash:** 텍스트 생성을 건너뛰고 툴 호출 및 라우팅을 위한 옵션별 확률과 함께 타입이 지정된 값을 반환하는 의사결정 모델 Agr (31B) 및 Agr-flash (360M)를 출시했습니다.
*   **Upstage Solar Mini 4:** 35B / 3B active, 512K 컨텍스트 모델을 Nous Portal에서 2주간 무료로 제공합니다.
*   **Agent Arena 리더보드:** Anthropic이 코드, 작업, 채팅 부문에서 1위를 차지했으며, Fable 5.1이 코드 및 작업을 선도하고 GPT-6 Astra가 코드 부문에서 2위를 기록했습니다.
*   **Design Arena 리더보드:** GPT-6 Astra가 3D 디자인, 프론트엔드, 풀 스택, Image-to-HTML 부문에서 1위를 차지했습니다.
*   **환각 평가 (AA-Omniscience):** Gemini 4 Argon은 모르는 질문의 15%에서 오답을 추측했으며, GPT-6 Astra는 61%로 가장 높은 정확도를 보였습니다.

### 🛠️ 제품 & 도구
*   **Eleven v4 Turbo:** AA의 Provider Voice TTS 아레나에서 v4 가격의 절반으로 최고 성능을 기록했습니다.
*   **OpenAI 서비스 속도 향상:** GPT-6 Astra 및 GPT-6.1 Sol의 기본 속도가 약 50% 증가하여 약 30 TPS에서 약 50 TPS로 상승했습니다.
*   **Pi Durable 하네스:** 장기 실행 멀티플레이어 에이전트가 어디서든 일시 중지하고 재개할 수 있도록 SQLite/JSONL 스토리지를 기반으로 구축된 태스크 기반 워크플로우 엔진을 공개했습니다.
*   **Cognition Devin “Dreaming”:** 밤새 메모리 그래프를 가지치기하고 연결하는 기능을 출시했으며, git 및 마크다운 기반 형식을 Agent Memory Repo로 오픈소스화하고 있습니다.
*   **Cursor SDK 업데이트:** 실행 중 조종, 백그라운드 서브에이전트, 교체 가능한 시스템 프롬프트, 커스텀 툴에 대한 MCP readOnlyHint 및 destructiveHint 어노테이션을 추가했습니다.
*   **DeepSeek Harness v0.2.1-alpha.1:** Claude Code Mods 호환성 레이어를 실험적으로 추가하여 DSH의 플러그인 아키텍처가 Claude Code의 확장 지점의 상위 집합인지 테스트합니다.
*   **Cline (Pareto 26.10 Preview):** 모델 간 라우팅 및 답변 평가 기능을 제공하며, 동일한 DeepSWE 점수에서 태스크당 0.24달러 대 13.41달러의 비용 효율성을 주장합니다.
*   **ChatGPT 커스텀 MCP 서버:** 더 이상 개발자 모드를 요구하지 않습니다.
*   **llama.cpp v0.6.0:** Clef 텍스트 및 비전 지원, Qwen3.8-Flash-Next, 그리고 새로운 llama_batch_ext API를 추가했습니다.

### 🔬 연구 & 논문
*   **Hugging Face 멀티 하네스 RL:** 10개의 수정되지 않은 하네스를 RL 환경으로 활용하는 캡처 프록시를 개발했습니다. LFM2.5-2.6B를 4개 하네스에 걸쳐 학습시켜 첫 시도 해결률을 42%에서 54%로 향상시켰으며, RL 환경은 이제 HF Hub에서 호스팅됩니다.
*   **NVIDIA 미드-하네스 검증:** 후보 셸 명령을 실행 전에 샘플링하고 검증하는 방법을 제시했습니다. GPT-5.6 Sol 검증기가 TerminalBench-Lite Pass@1을 50%에서 68%로 향상시켰습니다.
*   **Google VeriHarness:** 작업 공간 증거에 반하는 불일치를 해결하여 Gemini 3.5 Flash로 +6.2점, Opus 4.8로 +6.4점을 추가하는 방법을 공개했으며, 약 26K개의 롤아웃을 공개했습니다.
*   **UT Austin 컨텍스트 압축 연구:** 약 35K 실행에서 토큰의 1/3을 사용하는 압축이 전체 컨텍스트보다 20~80% 느릴 수 있으며, 최적의 정책은 모델마다 다르다는 것을 발견했습니다.
*   **PAIR (컨텍스트 관리):** 동일한 상태에서 에이전트를 재생하여 유해한 압축을 분리하고, 압축 프롬프트를 다시 작성하여 비압축 성능에 근접하는 방법을 제안했습니다.
*   **CorpusMap (컨텍스트 관리):** 문서 컬렉션을 위한 사전 계산된 엔티티 페이지가 답변 품질을 6.4~11.7점 높이면서 입력 토큰을 34~57% 줄인다는 연구 결과를 발표했습니다.
*   **SelfSearch (자체 개선):** DeepSeek V4 Flash를 사용하여 Terminal-Bench 2.1에서 82.0%를 달성했다고 주장하며, Codex와 일치하고 검색 비용은 4.03달러입니다.
*   **EverMind Raven (자체 개선):** 진화된 연구 하네스가 BrowseComp에서 69.3%를 기록했습니다.
*   **Dust (최적화/아키텍처):** 활성화-섭동 "가상 개체군"을 사용하는 0차 방법이 트랜스포머 사전 학습에서 백프로퍼게이션에 근접하거나 능가하며, EGGROLL보다 1,000~10,000배 더 컴퓨팅 효율적이라고 주장합니다.
*   **LOOM (최적화/아키텍처):** 루프형 MoE가 9~12 루프에서 안정적으로 학습되며, 700M 모델은 iso-FLOP에서 5 루프일 때 가장 좋다는 연구 결과를 발표했습니다.
*   **Vals AI의 과학 AI:** 90개 이상의 Opus 5.5 에이전트가 3일 동안 DFT 시뮬레이션을 실행하여 두 개의 상온 자기 반도체 후보를 식별했으며, 그중 하나는 1999년에 합성된 것이라고 보고했습니다.

### 💰 산업 동향
*   **SemiAnalysis, Claude 구독 가치 평가:** Claude 구독이 OpenAI 플랜보다 5배 이상 API 등가 가치를 제공한다고 보고했습니다.
*   **OpenAI 용량 압박:** 새로운 200달러 가입이 일시 중지되었고, 모든 플랜에서 사용량 제한이 사실상 절반으로 줄었다고 보고되었습니다.
*   **Microsoft의 Anthropic 지출 감소:** The Information은 Microsoft가 예상했던 내부 Anthropic 지출을 1/3 이상 줄였으며, Meta의 Claude Code 사용자 수도 감소했다고 보도했습니다.
*   **OpenAI 텍스트 워터마킹 도입:** EU AI Act 준수를 위해 EU 내 적격 ChatGPT 및 Codex 텍스트에 보이지 않는 통계적 워터마크를 추가하며, 전 세계적으로 선택적 API 토글을 제공합니다.
*   **자율 무기 금지 촉구:** 전 OpenAI 연구원 Joshua Achiam이 화학 무기와 유사한 특정 자율 무기 금지를 촉구했습니다.
*   **전문가 패널의 AI 정책 권고:** 250명 이상의 전문가로 구성된 LEAP 패널은 미국과 중국이 참여하고 사전 출시 승인 권한을 가진 국제 기구를 가장 지지하며, 연방 선점권을 반대했습니다.
*   **Tencent, Oracle로부터 10만 개 고급 칩 임대:** FT 보도에 따르면 텐센트가 Oracle의 동남아시아 데이터센터에서 약 10만 개의 고급 칩을 5년간 약 70억 달러에 임대했습니다.
*   **GPU 서버 밀수 혐의 기소:** 미국 검찰이 캘리포니아의 한 리셀러를 3억 달러 이상의 GPU 서버를 중국으로 밀수한 혐의로 기소했습니다.
*   **AMD, World Labs 인수 보도:** AMD가 World Labs를 82억 달러에 인수했다고 보도되었습니다.

### ⚡ 인프라 & 하드웨어
*   **llama.cpp Metal 추측 디코딩:** 새로운 커널이 M3 Ultra에서 추측 디코딩을 일반 디코딩보다 최대 3.4배 빠르게 만들었습니다 (110 대 32.1 tok/s).
*   **Baseten 에이전틱 커널 작업:** 대부분 자율 에이전트 작업으로 일주일 만에 구축된 엔진이 오픈소스 기준선보다 90% 빠른 디코딩과 57% 낮은 TTFT를 제공한다고 보고했습니다.
*   **NCCL 및 PyTorch 대칭 메모리:** 중소 규모 집합 연산의 속도를 높이는 데 기여합니다.
*   **Alibaba T-Head Zhenwu V900 가속기:** 216GB 메모리와 1,200GB/s 인터커넥트를 갖추고 있으며, M890보다 3배 빠르다고 주장하며 2027년 1분기 출시 예정입니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
