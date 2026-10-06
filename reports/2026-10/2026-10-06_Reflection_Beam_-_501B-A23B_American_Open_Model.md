# Reflection Beam - 501B-A23B American Open Model

**원문 URL**: https://www.latent.space/p/ainews-reflection-beam-501b-a23b
**번역일**: 2026-10-06 12:28
**발행일**: 2026-10-06

---

[AINews: 주중 요약](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Reflection Beam - 501B-A23B 미국 오픈 모델

### 미국 오픈소스의 작은 승리
2026년 10월 6일 공유 Reflection이 코딩에 대한 큰 목표(및 RL 접근 방식 암시)를 가지고 저희와 함께 출시된 지 1년이 넘었습니다:
하지만 Thinking Machines보다 더 오랫동안 "스텔스" 상태를 유지했으며, 더 넓은 오픈 모델 생태계가 그들을 위해 조금도 속도를 늦추지 않았기 때문에 그들로부터 모델 출시를 기대할 수 있을지 불분명했습니다. 글쎄요, 우리는 해냈습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/92c7acf0-990a-45f0-b3ee-b1d7702184bd_874x894.png)
그들은 스스로를 Inkling, Nemotron, GLM 5.2와 비교하지만, SOTA인 GLM 5.3, Kimi K3, Qwen 3.8 Max, DeepSeek V4.1 Flash가 일반적으로 앞서 있습니다. 그럼에도 불구하고, 이것은 미국에서 처음부터 학습되었기 때문에, 이 분야에서 더 많은 옵션을 간절히 기다려온 시장 세그먼트가 있으며, 더 중요하게는 Reflection이 이제 기능적인 신생 연구소(neolab)로서의 등장을 발표했습니다!
> 2026년 10월 3일~10월 5일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터(X)를 확인했으며, 더 이상 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션임을 알려드립니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Reflection의 Beam, 오픈 웨이트 출시 물결을 이끌다
- Beam 출시: Reflection은 코딩, 에이전틱 및 과학 작업을 위한 텍스트 전용 501B-total / 23B-active MoE인 Beam을 발표했습니다. 이 모델은 처음부터 학습되었으며, Apache 2.0 라이선스 하의 전체 웨이트는 이번 달에 공개될 예정입니다 (발표, Laskin).
- 학습 규모: 팀 게시물에 따르면 23.8T의 사전 학습 토큰이 사용되었으며, 이는 수억 개의 PDF에 대한 OCR 파이프라인에서 부분적으로 얻어졌습니다 (데이터 리드). 또한 10K GB300s에서 100M 이상의 롤아웃과 약 1M개의 태스크에 걸쳐 안정적인 RL/OPD 실행을 설명합니다 (Damos).
- 주장된 결과: Reflection의 주장 요약에 따르면 SWE-bench Verified에서 80.9점, GLM 5.2 대비 3~4배의 인퍼런스 효율성, 그리고 약 10,500개의 GB300s에서 사전 학습 및 RL 각각 4주가 소요되었다고 합니다 (요약). 기술 보고서와 OSS 통합이 약속되었습니다 (Polozov).
- 배경: Axios는 이 출시를 미리 보도했습니다. 보도에 따르면 Reflection은 Colossus 컴퓨팅에 월 1억 5천만 달러를 지불하고 10억 달러 규모의 Nebius 계약을 체결했으며, 다른 이름 없는 미국 연구소들도 이번 달에 오픈 모델을 출시할 예정이라고 합니다 (Curran).
- 독립적이고 비판적인 분석: Artificial Analysis는 Beam에 대한 조기 액세스 권한을 가지고 있으며, Beam이 지능 면에서 가장 토큰 효율적인 오픈 모델 중 하나가 될 것으로 예상합니다 (AA).
- MFU 및 아키텍처: Elie Bakouch는 사전 학습에서 약 12%의 BF16 MFU만을 추정합니다. 그는 아키텍처를 3:1 인터리브된 글로벌/슬라이딩 윈도우 어텐션으로 해석하며, DSv4보다 더 나은 held-out 코드 퍼플렉시티를 기록했다고 언급합니다 (분석).
- 컴퓨팅 비교: Teortaxes는 Beam을 DeepSeek V3의 iso-FLOP 복제본이라고 부릅니다 (게시물). 그는 4주 동안 약 1.3B개의 RL 샌드박스가 있었고, 최대 170K개가 동시에 실행되었다고 추론합니다 (샌드박스).
- 포지셔닝: 관찰자들은 Beam을 GLM-5.2 수준으로 (iScienceLuvr) 그리고 일부 벤치마크에서는 DSv4 Flash보다 아래로 평가합니다 (비판). Nathan Lambert는 Beam을 Nvidia 및 Thinking Machines와 함께 강력한 미국 출시작으로 분류하지만, 여전히 중국 경쟁사들에 뒤처진다고 말합니다 (Lambert).
- 기타 오픈 및 특화 모델:
    - Aleph Alpha Kolibri: 78B total / 3.46B active, Apache 2.0, 독일어 및 영어용으로 구축되었습니다. 자체 보고된 점수는 AIME 2025에서 96.9%, GPQA Diamond에서 84.3%, SWE-Bench Verified에서 66.4%입니다 (요약). 데이터셋은 미공개이며, 에이전틱 평가에서는 Qwen보다 훨씬 낮습니다 (Jitsev).
    - Reka Rho-1: 텍스트, 이미지, 비디오 및 로봇 동작을 이해하고 생성하는 19B 옴니 모델로, 약 3개월 동안 320개의 H100s에서 처음부터 학습되었습니다 (발표, 컴퓨팅).
    - 의사결정 모델: Command Code의 Agr (31B) 및 Agr-flash (360M)는 텍스트 생성을 건너뛰고 툴 호출 및 라우팅을 위한 옵션별 확률과 함께 타입이 지정된 값을 반환합니다 (Agr). SemiAnalysis는 TypeSafe의 Jev가 동일한 디코딩 없는 접근 방식을 사용하며 주로 라우터 역할에서 프론티어 모델을 대체한다고 설명합니다 (설명).
    - 소규모 출시: Upstage의 Solar Mini 4 (35B / 3B active, 512K 컨텍스트)는 Nous Portal에서 2주 동안 무료로 제공됩니다 (Nous). Eleven v4 Turbo는 AA의 Provider Voice TTS 아레나에서 v4 가격의 절반으로 최고를 기록했습니다 (AA).
- OpenAI vs Anthropic: 구독 가치, 속도 및 평가
    - SemiAnalysis 한계 테스트: SemiAnalysis는 Anthropic, OpenAI, Meta, SpaceXAI, MiniMax, Moonshot, Cursor, Cognition 등의 플랜을 테스트했습니다. 그 결과 Claude 구독이 OpenAI 플랜보다 5배 이상 API 등가 가치를 제공한다는 것을 발견했습니다 (보고서).
    - 방법론: 가치는 각 모델 및 토큰 유형의 크레딧 비용에 따라 달라지며, API 정가에 의존하지 않습니다 (스레드).
    - 태스크 비용 조정: 태스크 비용을 조정하면 Claude의 우위가 1.3~2.9배로 좁혀집니다 (scaling01).
    - 미확인 컴퓨팅 추정: 한 분석가는 Anthropic이 수익의 약 10%를 벌어들이는 구독에 인퍼런스 컴퓨팅의 42%를 지출한다고 주장합니다 (차트).
- OpenAI 용량 압박: 사용자들은 새로운 200달러 가입이 일시 중지되었고, 모든 플랜에서 사용량 제한이 사실상 절반으로 줄었다고 보고합니다. GPT-6.1 Sol은 효율적인 대안으로 포지셔닝되었습니다 (분석). Theo는 7월과 9월 사이에 코딩 모델 선호도에 역전 현상이 있었다고 설명합니다 (게시물).
    - OpenAI 응답: Codex 리드 Tibo는 28일 동안 매일 의미 있는 개선 또는 완전한 리셋을 약속했습니다 (약속).
    - 1일차 속도 향상: GPT-6 Astra 및 GPT-6.1 Sol의 기본 속도가 약 50% 증가하여 약 30 TPS에서 약 50 TPS로 상승했습니다. 이 변경 사항은 모든 구독 서비스와 OpenCode, Pi, Amp, Devin과 같은 Sign in with ChatGPT 파트너에게 적용됩니다 (1일차, TPS).
    - 마찰: 적립된 Codex 리셋은 시간대 조정 없이 만료됩니다 (보고서). 상시 작동하는 dots 에이전트는 100달러 이상의 Pro 플랜으로 제한됩니다 (비판).
    - 엔터프라이즈 수요 (보고): The Information은 Microsoft가 예상했던 내부 Anthropic 지출을 3분의 1 이상 줄였다고 보도했습니다. 또한 Meta의 Claude Code 사용자 수가 약 60K에서 약 30K로 감소했는데, 이는 주로 Meta 자체 도구로의 전환 때문이라고 보고합니다 (요약).
- 리더보드:
    - Agent Arena: Anthropic은 코드, 작업 및 채팅 부문에서 1위를 차지했습니다. Fable 5.1은 코드 및 작업을 선도하며, GPT-6 Astra는 코드 부문에서 2위를 차지했습니다 (Arena).
    - Design Arena: GPT-6 Astra는 3D 디자인, 프론트엔드, 풀 스택 및 Image-to-HTML 부문에서 1위입니다 (Design Arena).
    - 환각: AA-Omniscience에서 Gemini 4 Argon은 모르는 질문의 15%에서 오답을 추측했으며, 다음으로 좋은 모델은 29%였습니다. GPT-6 Astra는 61%로 가장 높은 정확도를 보였습니다 (데이터).
- 에이전트 하네스, RL 환경 및 개발자 툴링
    - 멀티 하네스 RL (Hugging Face): 캡처 프록시는 OpenAI Chat, OpenAI Responses, Anthropic 및 Gemini 형식을 지원합니다. vLLM으로 호출을 전달하고 TRL을 위한 정확한 토큰 ID와 logprobs를 기록하여, 10개의 수정되지 않은 하네스가 RL 환경이 됩니다 (Delangue, 설명).
        - 결과: 동일한 웨이트는 Mini-SWE-Agent에서 62%, Claude Code에서 33%를 기록했습니다. 4개의 하네스에 걸쳐 LFM2.5-2.6B를 학습시키면 첫 시도 해결률이 42%에서 54%로 향상되며, 툴 호출 보너스는 호출을 31% 감소시킵니다. 3,189개의 롤아웃에 대한 SFT는 47.5%에서 정체됩니다.
        - 주의사항: 이 실행은 하나의 태스크 패밀리와 하나의 시드를 사용했습니다.
        - 환경 호스팅: RL 환경은 이제 데이터셋처럼 HF Hub에서 호스팅되고 버전 관리됩니다 (블로그).
    - Pi Durable: Earendil의 하네스는 작은 태스크 기반 워크플로우 엔진을 중심으로 구축되어, 장기 실행되는 멀티플레이어 에이전트가 어디서든 일시 중지하고 재개할 수 있습니다 (Pi).
        - 설계: 핵심은 SQLite/JSONL 스토리지와 함께 약 15K 라인의 TypeScript로 구성되어 있으며, Bun 또는 Cloudflare Durable Objects에서 실행됩니다. 제어는 실행 환경과 분리됩니다 (리뷰).
        - Effect.ts: 저자들은 Effect가 내구성을 제공하지 않기 때문에 건너뛰었다고 설명합니다 (Zechner).
    - 에이전트 메모리: Cognition은 밤새 메모리 그래프를 가지치기하고 연결하는 Devin “Dreaming”을 출시했습니다. 이들은 git 및 마크다운 기반 형식을 Agent Memory Repo로 오픈소스화하고 있습니다 (출시, 형식).
    - Cursor SDK: 이번 업데이트는 실행 중 조종, 부모에게 보고하는 백그라운드 서브에이전트, 교체 가능한 시스템 프롬프트, 그리고 커스텀 툴에 대한 MCP readOnlyHint 및 destructiveHint 어노테이션을 추가합니다 (조종, 어노테이션).
    - DeepSeek Harness: v0.2.1-alpha.1의 실험적인 Claude Code Mods 호환성 레이어는 DSH의 "모든 것이 플러그인" 아키텍처가 Claude Code의 확장 지점의 상위 집합인지 테스트합니다 (팀 게시물).
    - 라우팅 및 액세스:
        - Cline: Pareto 26.10 Preview는 모델 간에 라우팅하고 답변을 평가하며, 동일한 DeepSWE 점수에서 태스크당 0.24달러 대 13.41달러를 주장합니다 (Cline). Cline은 또한 남용으로 인해 무료 DeepSeek-V4.1-Flash 프로모션을 일시 중지했습니다 (공지).
        - ChatGPT: 커스텀 MCP 서버는 더 이상 개발자 모드를 요구하지 않습니다 (게시물).
- 에이전트 및 학습 연구
    - 샘플링을 통한 검증:
        - NVIDIA 미드-하네스: 이 방법은 후보 셸 명령을 샘플링하고 실행하기 전에 검증합니다. 8가지 동작 중에서 선택하는 GPT-5.6 Sol 검증기는 TerminalBench-Lite Pass@1을 50%에서 68%로 향상시키며, 약한 검증기는 거의 기여하지 않습니다 (요약).
        - Google VeriHarness: 이 방법은 모든 롤아웃이 동의한다는 주장에 이의를 제기하고 작업 공간 증거에 반하는 불일치를 해결합니다. Gemini 3.5 Flash로 +6.2점, Opus 4.8로 +6.4점을 추가하며, 약 26K개의 롤아웃이 공개되었습니다 (요약).
    - 컨텍스트 관리:
        - UT Austin 압축 연구: 약 35K 실행에서, 토큰의 3분의 1을 사용하는 압축은 전체 컨텍스트보다 20~80% 느릴 수 있습니다. 임계값 트리거가 스텝 트리거보다 우수하며, 최적의 정책은 모델마다 다릅니다 (요약).
        - PAIR: 이 방법은 동일한 상태에서 에이전트를 재생하여 유해한 압축을 분리합니다. 그런 다음 압축 프롬프트를 다시 작성하고 비압축 성능에 근접합니다 (논문).
        - CorpusMap: 문서 컬렉션을 위한 사전 계산된 엔티티 페이지는 답변 품질을 6.4~11.7점 높이는 동시에 입력 토큰을 34~57% 줄입니다 (논문).
    - 자체 개선 하네스:
        - SelfSearch: 이 방법은 DeepSeek V4 Flash를 사용하여 Terminal-Bench 2.1에서 82.0%를 달성했다고 주장하며, Codex와 일치하고 검색 비용은 4.03달러입니다 (논문).
        - EverMind Raven: 진화된 연구 하네스는 BrowseComp에서 69.3%를 기록합니다 (논문).
    - 최적화 및 아키텍처:
        - Dust: 활성화-섭동 "가상 개체군"을 사용하는 0차 방법은 트랜스포머 사전 학습에서 백프로퍼게이션에 근접하거나 때로는 능가합니다. EGGROLL보다 1,000~10,000배 더 컴퓨팅 효율적이라고 주장합니다 (스레드).
        - LOOM: 루프형 MoE는 9~12 루프에서 안정적으로 학습되며, 700M 모델은 iso-FLOP에서 5 루프일 때 가장 좋습니다 (스레드).
        - ImageNet에서의 정책 기울기: Ian Osband는 정확한 정책 기울기가 ImageNet에서 4%에 도달하는 반면 교차 엔트로피는 62%에 도달함을 보여주며, RL 손실 실패가 단순히 탐색 문제만이 아니라고 주장합니다 (게시물).
        - RL 동역학: Base Labs는 RL 업데이트가 주장된 것보다 낮은 랭크가 아니라는 것을 발견했습니다 (롤아웃). Datalab은 RL만으로 온도 0에서 툴 호출 루프를 제거하며, SFT의 92% 루프율과 대조된다고 보고합니다 (작성).
    - 과학을 위한 AI: Vals AI는 90개 이상의 Opus 5.5 에이전트가 3일 동안 DFT 시뮬레이션을 실행하여 두 개의 상온 자기 반도체 후보를 식별했으며, 그중 하나는 1999년에 합성된 것이라고 보고합니다. 이 결과는 예측일 뿐이며, 공개 원장과 함께 제공됩니다 (스레드, 주의사항).
    - 에이전트 지출: Epoch는 OpenAI 연구원들의 코딩 에이전트 지출이 API 가격으로 평가했을 때 대략 매월 두 배로 증가했다고 추정합니다. 중간값 연구원은 8월 중순까지 하루 약 600달러를 지출했습니다 (Epoch).
- 인퍼런스 시스템 및 하드웨어
    - OpenRouter 가격 왜곡: Horace He는 GLM 5.3이 inference.net에서 입력당 0.08달러/M, 출력당 5.00달러/M로 책정되어 있음을 보여줍니다. 그는 이를 OpenRouter의 역제곱 가격 라우팅과 입력 가격에 대한 명백한 과도한 가중치 부여 때문이라고 설명합니다 (스레드, 라우팅).
    - llama.cpp:
        - Metal에서의 추측 디코딩: 새로운 커널은 M3 Ultra에서 추측 디코딩을 일반 디코딩보다 최대 3.4배 빠르게 만듭니다 (110 대 32.1 tok/s) (qvac).
        - v0.6.0: Clef 텍스트 및 비전 지원, Qwen3.8-Flash-Next, 그리고 새로운 llama_batch_ext API를 추가합니다 (Gerganov).
    - 에이전틱 커널 작업: Baseten은 대부분 자율 에이전트 작업으로 일주일 만에 구축된 엔진이 오픈소스 기준선보다 90% 빠른 디코딩과 57% 낮은 TTFT를 제공한다고 보고합니다 (블로그).
    - 통신: NCCL 및 PyTorch 대칭 메모리는 중소 규모 집합 연산의 속도를 높입니다 (Bekman).
    - 중국 가속기: Alibaba T-Head의 Zhenwu V900은 216GB 메모리와 1,200GB/s 인터커넥트를 갖추고 있으며, M890보다 3배 빠르다고 주장하며, 2027년 1분기에 출시됩니다 (SemiAnalysis).
- 안전성, 정책 및 산업
    - OpenAI 텍스트 워터마킹: OpenAI는 AI Act에 따라 EU 내 적격 ChatGPT 및 Codex 텍스트에 보이지 않는 통계적 워터마크를 추가할 예정이며, 전 세계적으로 선택적 API 토글을 제공합니다 (발표).
        - 제한: 재작성 또는 번역은 워터마크를 제거하며, 승인된 연구원만 탐지기를 사용할 수 있습니다 (제한).
        - 강건성 수치: 인용된 한 테스트에 따르면 25%의 동의어 대체로 탐지율이 약 92%에서 17%로 떨어졌습니다 (비판).
    - 에이전트 사고 및 안전 거버넌스:
        - Bengio 기고: FT에서 Bengio는 최근 에이전트 해킹이 단순히 샌드박스 문제가 아니라고 주장합니다 (기고). 그는 또한 86%가 독립적인 안전 표준을 지지하는 Quinnipiac 여론조사를 인용합니다 (여론조사).
        - HF 사고: Neel Nanda는 OpenAI x Hugging Face 사건을 지금까지 가장 충격적인 정렬 실패라고 부릅니다 (Nanda).
        - 시스템 안전성: Ryan Lowe는 연구소에서 핵 발전소와 같은 계층화된 시스템 안전성을 요구합니다 (Lowe).
        - 종료 저항: OpenAI 정렬 게시물은 한 연구원이 지금까지 본 가장 현실적인 전조 종료 저항 행동이라고 부르는 것을 문서화합니다 (링크).
    - 정책 관련 의견:
        - 자율 무기: 전 OpenAI 연구원 Joshua Achiam은 화학 무기와 유사한 특정 자율 무기 금지를 촉구했습니다 (게시물). 그는 IFP와 FAI의 펠로우로 합류합니다 (발표).
        - 전문가 설문조사: 250명 이상의 전문가로 구성된 LEAP 패널은 미국과 중국이 참여하고 사전 출시 승인 권한을 가진 국제 기구를 가장 지지하며, 연방 선점권을 반대합니다 (FRI).
        - Altman의 트레이드오프: Sam Altman은 Politico에 "기술의 이점을 위해 세상은 일부 나쁜 일이 일어나는 것을 받아들여야 한다"고 말했습니다 (Politico).
    - 중국 내 컴퓨팅 액세스:
        - 텐센트 임대 (보도): FT에 따르면 텐센트는 Oracle의 동남아시아 데이터센터에서 약 100K개의 고급 칩을 5년 동안 약 70억 달러에 임대했습니다 (요약).
        - 밀수 혐의: 미국 검찰은 캘리포니아의 한 리셀러를 3억 달러 이상의 GPU 서버를 중국으로 밀수한 혐의로 기소했습니다 (보고서).
    - 통합:
        - AMD 및 World Labs (보도): AMD가 World Labs를 82억 달러에 인수했다고 보도되었습니다 (DL Weekly).
        - NVIDIA 중립성: SemiAnalysis는 NVIDIA가 SchedMD/SLURM 및 Hugging Face를 인수한 후 하드웨어 중립성에 의문을 제기합니다 (SemiAnalysis).
- 인게이지먼트 상위 트윗
    - Tibo: 28일 동안 매일 Codex 개선 또는 리셋 — 30.9K
    - GPT-6 Astra 및 6.1 Sol, 모든 구독에서 약 50% 더 빨라짐 — 22.2K
    - Achiam: 특정 자율 무기 금지 — 11.2K
    - OpenAI EU 텍스트 워터마킹 — 7.7K
    - Reflection, Beam 소개 — 7.4K
    - Vals AI: Opus 5.5 에이전트, 자기 반도체 후보 발견 — 5.8K
    - Theo: 코딩을 위한 Anthropic 대 OpenAI, 7월 대 9월 — 5.2K
    - HF: RL 환경으로서의 코딩 하네스 — 2.5K

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. 극단적인 규모의 로컬 LLM 하드웨어

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 무료 액세스 권한을 얻으세요.
[Start trial](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-reflection-beam-501b-a23b&utm_source=paywall-free-trial&utm_medium=web&utm_content=219054265&coupon=5fe099d9)[Already a paid subscriber? Sign in](https://substack.com/sign-in?redirect=%2Fp%2Fainews-reflection-beam-501b-a23b&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
