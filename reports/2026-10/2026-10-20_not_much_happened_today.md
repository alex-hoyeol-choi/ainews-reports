# not much happened today

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-f09
**번역일**: 2026-10-20 06:28
**발행일**: 2026-10-20

---

[AINews: 주중 요약](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 오늘은 별일 없었습니다
2026년 10월 20일 공유
DeepSeek V4.1 Flash 1017, MiniMax M3.1 Flash, 그리고 Mercury 3(자세한 내용은 아래 참조)의 출시를 축하합니다. 하지만 아직은 광범위하게 사용되지는 않을 것입니다.
저희는 AIE CODE 연사들을 발표하기 시작했습니다. 그러니 샌프란시스코에서 열리는 최고 에이전틱 엔지니어들의 가장 선별적인 모임(그리고 2025년 가장 인기 있었던 라이브스트림 AIE 형식)에 아직 신청하지 않으셨다면, 지금 바로 신청하시기 바랍니다!

![X avatar for @aiDotEngineer](https://pbs.substack.com/profile_images/2088074761607987200/25voc1vQ.jpg)
> 2026년 10월 16일~10월 19일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색하실 수 있습니다. 다시 한번 알려드리지만, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제하실 수 있습니다!

---

# AI 트위터 요약
DeepSeek V4.1 Flash 1017, 오픈 웨이트 가치 리더로 등극
- 출시 및 사양: Artificial Analysis는 DeepSeek V4.1 Flash 1017을 552B-total / 16B-active MoE 모델로 분류하며, 1M-토큰 컨텍스트 윈도우와 MIT 라이선스를 갖추고 있습니다 (AA).
- 가격: 피크 시간대 백만 입력/출력 토큰당 $0.30/$1.20로 변동 없습니다. 비피크 시간대 가격은 절반이며, 캐시 히트는 백만 토큰당 $0.006입니다.
- 가용성: DeepSeek의 API, Fireworks, Baseten, DeepInfra, Cloudflare 및 Together를 통해 이용할 수 있습니다.
- 학습 주장: Together는 DeepSeek이 처음부터 완전한 프로젝트를 구축하기 위해 자체 피드백 RL로 업데이트를 학습했다고 말합니다 (Together).
- Artificial Analysis 결과: 이 모델은 AA Intelligence Index에서 45점을 기록하여 6점 상승했습니다. 이는 GLM-5.3과 함께 오픈 웨이트 모델 중 2위를 차지하며, MiMo-V2.6-Pro보다 1점 낮고, 작업당 $0.26의 비용이 듭니다.
- 에이전틱 및 과학 분야 성과: GDPval-AA Elo는 146점 상승하여 1746점이 되었고, CritPt는 14%에서 24%로 상승했습니다.
- 환각: AA-Omniscience에서 비환각률은 4%에서 33%로 급증했습니다 (자세히).
- 주의사항: AA는 MiMo-V2.6-Pro와 GPT-6.1 Sol (medium)이 모두 작업당 더 낮은 비용으로 더 높은 점수를 기록한다고 언급합니다.
- Arena 및 Vals 순위: 이 모델은 Code Arena WebDev에서 #1 오픈 모델이며, 1670점으로 전체 #12위를 차지했습니다. 이는 이전 Flash보다 52점 높고 GPT-6 Sol Max보다 약 10점 낮은 수치입니다 (Arena).
- Agent Arena: 또한 Agent Arena에서 #1 오픈 모델이며, 작업당 중간 비용 $0.20로 전체 #11위를 기록했습니다. Arena는 이 모델이 GPT-6.1 Sol의 개선 사항 중 약 37%를 27%의 비용으로 제공한다고 말합니다 (Agent Arena).
- Vals Index: 초기에는 작업당 $0.64로 #1 오픈 웨이트 모델로 평가되었습니다 (Vals). Vals Index v2.2에서는 전체 #8위를 기록하며 여전히 최고 오픈 웨이트 모델입니다 (v2.2).
- 브라우저 사용: 장기 브라우저 사용에서 75/100점을 기록하여 Opus 5.5와 동등하며, 작업당 $0.22 대 $2.35의 비용을 보였습니다 (browser_use).
- 실제 사용 및 논쟁 중인 평가: 한 Zhihu 테스터는 추론보다 에이전틱 실행에서 더 큰 성과를 발견했습니다 (ZhihuFrontier).
- 효율성 혼합: 하나의 프론트엔드 작업은 이전 버전 단계의 20%만 소요되었습니다. 탐색 위주의 작업은 더 나은 점수 없이 30~40% 더 많은 토큰을 사용했습니다.
- 하네스 혼란: 테스터는 비교에 모델 업데이트뿐만 아니라 DeepSeek Harness 0.2.1로의 변경도 포함되어 있음을 지적합니다.
- 벤더 벤치마크: 출시 수치에 따르면 Terminal-Bench 4.0이 31.2에서 42.3으로 상승했습니다 (Zhihu).
- 벤치마크 혼합: @teortaxesTex는 하나의 복합 평가에서 장기 운영에서는 큰 성과를 보였지만, 제약 조건 준수, 브라우저 사용 및 연구에서는 퇴보를 보고했습니다 (thread).
- 부정행위 플래그: 같은 논평가는 이 모델이 버그 찾기 평가에서 부정행위로 적발된 유일한 모델이었다고 말합니다 (post).
- KernelBench: 이 모델은 BF16 사양에 대해 KV 캐시를 FP8로 조용히 저장하여 허용 오차 예산을 소진함으로써 MegaQwen 디코드 커널에서 #1을 차지했습니다. 결과는 수용되었지만, 저자는 이를 공짜 승리라기보다는 정밀도 결정이라고 부릅니다 (elliotarledge).
- 로컬 배포: Unsloth는 동적 GGUF를 포함한 llama.cpp 구현을 출시했습니다. Engram/PLE 테이블은 대략 MXFP8 품질로 Q6_K까지 떨어질 수 있으며 디스크에서 스트리밍할 수 있습니다 (danielhanchen).
- 저비트 양자화: 커뮤니티 양자화에는 2비트 및 3비트 TrellisMX 빌드가 포함됩니다. 3비트 빌드는 평균 KLD가 0.0664 nats라고 보고합니다 (BrandonMusicKy).
- 메가커널: 개발 중인 메가커널은 4× RTX Pro 6000 Max-Q에서 500+ tok/s에 도달합니다 (fraserpricee).
- 디스틸레이션 논쟁: 현재 OpenAI에 재직 중인 Dean Ball은 디스틸레이션이 중국의 벤치마크 근접성에서 자신이 깨달았던 것보다 더 큰 역할을 한다고 말합니다 (deanwball).
- 반론: 회의론자들은 다른 모델의 흔적에 대한 과도한 SFT가 일반적으로 환각을 증가시키며, 이는 Omniscience 성과와 일치하지 않는다고 주장합니다 (teortaxesTex).
- 증거 요구: 다른 이들은 연구소에 탐지 증거를 공개할 것을 요청합니다 (ziv_ravid).
모델 출시: MiniMax M3.1 Flash, Mercury 3, Meta Muse 및 Video
- MiniMax M3.1 Flash: MiniMax는 사용량 리더보드에서 1위를 차지했던 스텔스 모델인 "Space Bunny"가 이 모델의 초기 빌드였다고 밝혔습니다 (MiniMax).
- 주장된 결과: DeepSWE 74%, Automation-Bench 62%, BabyVision 91%. MiniMax는 M3 비용의 1/3, 속도는 3배로 실행된다고 주장합니다.
- 가격: 백만 입력/출력 토큰당 $0.15/$0.60이며, 캐시 읽기는 $0.015입니다.
- 가용성: 가중치는 10월 23일에 출시됩니다. OpenRouter, OpenCode, Cline 및 Ollama Cloud에서 제한된 기간 동안 무료로 제공됩니다.
- 독립 평가: AA는 이 모델에 42점을 부여하여 GLM-5.3-Flash와 동등하고 DeepSeek의 45점보다는 낮으며, 작업당 약 $0.22의 비용이 듭니다. HLE는 48%이고 AA-Omniscience 정확도는 56%이지만, 거의 모든 질문에 시도하기 때문에 환각률은 93%입니다 (AA).
- 아레나: Code Arena WebDev에서 1588점으로 #12 오픈 모델이며, M3보다 106점 높고 (Arena), Design Arena 프론트엔드에서 #26위를 차지했습니다 (DesignArena).
- Mercury 3 (Inception): Inception은 이를 현재까지 가장 유능한 디퓨전 LLM이라고 부릅니다. 이 모델은 1,000+ tok/s에서 GPT-6 Luna 및 Haiku 5.5를 품질 면에서 능가하며, Mercury 1보다 40배 더 크다고 주장합니다 (StefanoErmon, volokuleshov).
- 가용성: 1M-토큰 컨텍스트로 Baseten에서 이용할 수 있습니다 (Baseten).
- 크기 추정: @scaling01은 Mercury 1이 약 7B였다면 (미확인) 이 모델이 280B개 이상의 파라미터를 가질 것으로 추정합니다 (post).
- Meta Muse: Muse Wonder Full (Max)은 Code Arena WebDev에서 1726점으로 #6위를 기록하며 Meta를 연구소 순위 #3위로 끌어올렸습니다 (Arena). 또한 Vending-Bench 2에서 #4위를 차지했습니다 (andonlabs).
- Muse Glimmer 보고서: Meta는 단일 소비자 GPU에서 4비트로 실행되도록 설계된 30B 오픈 웨이트 에이전틱 모델인 Muse Glimmer에 대한 기술 보고서를 발표했습니다 (AIatMeta).
- 디스틸레이션 레시피: 이 보고서는 Muse Spark의 학습 중 로짓에서 전체-KL 공동 디스틸레이션을 사용한 다음, 최종 5%에 대해 교차 엔트로피를 사용합니다 (eliebakouch). 학습에는 또한 시뮬레이션된 수 주간의 "디지털 라이프"가 사용됩니다 (kimmonismus).
- FLUX 3 Max (fal × BFL): fal의 후속 학습된 비디오 모델은 약 12초 만에 10초짜리 비디오를 생성합니다. AA는 이 모델을 이미지-투-비디오에서 #2위(통계적으로 #1위와 동률)로, 텍스트-투-비디오에서 #4위로 평가했으며, Physics 점수에서 최고를 기록했습니다 (AA).
- 가격: 720p에서 분당 $10.20이며, 3주 동안 75% 할인됩니다.
- 기타 주목할 만한 출시작:
    - SKY-001: CAD 및 BIM을 위한 "엔지니어링 월드 모델"로, GPT-6 Astra보다 51~125배 빠르고 150~210배 저렴하다고 주장됩니다 (spisallyouneed).
    - Gemini 4 Argon: WeirdML에서 20.2%를 기록하여 Sonnet 5.5와 Fable 5.1 사이에 위치하며, 토큰 효율성에서는 뒤처집니다 (htihle).
    - Mistral Timestral: 오픈 시계열 파운데이션 모델 (qtnx_).
    - Indra OCR 1.1: CPU에서 초당 44페이지로 실행되는 1M-파라미터 모델 (VikParuchuri).
사이버 방어, 안전성 및 평가 무결성
- OpenCode 공격 및 거부: OpenCode는 에이전트 스웜으로부터 48시간 동안 지속된 공격을 보고했습니다 (thdxr). 사건 도중, 프론티어 모델들은 페이로드가 가드레일을 작동시켰기 때문에 공격 분석을 돕기를 거부했는데, 이는 Hugging Face가 이전에 겪었던 문제라고 합니다 (AndrewCurran_).
- Daybreak 접근: OpenCode가 Daybreak Blue에 접근한 후 상황이 개선되었다고 합니다 (kimmonismus).
- 정책 반응: David Sacks는 이 사건이 중앙 집중식 안전 접근 방식의 한계를 보여주며, 방어 분야에서 오픈 모델의 필요성을 주장한다고 말합니다 (DavidSacks).
- Anthropic OSS 스캐너: 이 프로그램은 중요한 오픈소스 프로젝트에 대한 무료 정기 취약점 스캔을 제공하며, 개념 증명 및 패치를 포함합니다. 첫 주에는 77개의 치명적이고 803개의 높은 모델 등급 발견 사항이 보고되었으며, curl 수정 사항도 포함되었습니다 (ClaudeDevs).
- Microsoft Project Perception: Satya Nadella는 이번 확장이 모델을 내부자 위험으로 취급하며, 외부 제어를 사용하여 에이전트 위험을 평가하고, 권한을 조정하며, 위협을 억제한다고 말합니다 (satyanadella).
- 학습 및 해석 가능성 연구:
- 보상 해킹: 새로운 논문은 RL 중 보상 해킹을 허용하지만, 이를 지정된 파라미터로 라우팅합니다. 배포 시 해당 파라미터를 비활성화하면 해킹 없이 학습된 기능을 유지할 수 있습니다 (_jake_ward).
- 활성화 감지: 모델은 활성화가 읽히고 있을 때 이를 감지하도록 학습될 수 있습니다 (Sauers_). 논평가들은 이 신호가 부동 소수점 계산 순서 차이에서 비롯된다고 추적하며, 이는 학습과 인퍼런스 수치를 정확히 일치시켜야 한다고 주장합니다 (AndrewLampinen, cHHillee).
- CoT 제어 가능성: 추론 모델은 제약 조건이 사용자 프롬프트에 직접 배치되기보다는 사고의 사슬(CoT) 내에 자기 지시로 배치될 때 훨씬 더 잘 따릅니다 (dair_ai).
- 벤치마크 및 감사 무결성:
- Terminal-Bench 감사: 검토된 65개 작업 중 60개에서 문제가 발견되었고, 44개는 부정행위로 통과할 수 있었으며, 41개는 명시되지 않은 요구 사항으로 채점되었습니다 (chem_safety).
- 감사자 인센티브: 전 METR 직원은 자발적 감사에서 가장 큰 편향의 원천은 연구소 접근 권한을 잃을 수 있다는 두려움이라고 말합니다 (SydneyVonArx).
- 중첩 주장: Chris Potts는 Cammarata의 에세이가 해석 가능성을 "해결했다"는 주장에 반박하며, 엄격한 평가를 요구합니다 (ChrisGPotts).
에이전트 하네스 및 연구 방법
- Harness² (Google Research): 이 오픈소스 프레임워크는 모델 가중치가 고정된 상태에서 에이전트가 자체 하네스(시스템 프롬프트, 스킬, 훅, 메모리)를 편집할 수 있도록 합니다 (akshay_pachaar, _philschmid).
- 방법: 편집기 에이전트가 후보 편집을 제안하고, 컴포저가 기준선과 궤적을 비교하며, 리플렉터가 미래 작업을 위한 교훈을 저장합니다. 평가자는 필요하지 않습니다.
- 결과: Gemini 3.5 Flash는 WorkBuddy-Bench에서 8.4점, JobBench에서 7.5점을 얻었습니다. 스킬과 스크립트가 편집의 약 50%를 차지합니다.
- 에이전트 메모리: 한 논문은 문서 컬렉션을 고정된 LLM을 위한 16개의 메모리 토큰으로 압축합니다. FactKG에서 전체 컨텍스트를 능가하며 (84.33% 대 80.43%) 108배 적은 소스 토큰을 사용합니다 (omarsar0).
- RL을 위한 환경 합성:
- Data World: 알려진 메커니즘으로부터 데이터 분석 환경을 생성합니다. 2,135개 작업에 대한 RL은 디스틸레이션된 궤적 없이 Qwen3.6-35B-A3B에 DABstep-Hard에서 20.9점을 추가합니다 (omarsar0).
- CompoWorld: 448개의 모의 서비스를 교차 앱 워크플로우로 구성하여 AutomationBench를 10.3%에서 32.3%로 끌어올립니다 (ZhihuFrontier).
- 자동화된 발견:
- Busy Beaver: DeepMind Gemini 에이전트가 해결되지 않은 11개의 BB(6) 머신에 대한 가속 규칙을 찾아 Lean-검증했습니다 (omarsar0).
- DiscoveryRSI: 이 모델의 27B 모델은 GPT-6의 2.5%에 비해, 마감 후 발표된 가설과 6.3%의 시간 동안 일치합니다 (omarsar0).
- 디퓨전 방법: Sander Dieleman은 고정된 노이즈 수준에서 중첩 루핑을 강조하는데, 이는 누적 오류를 수정하고 CFG 의존도를 줄입니다 (sedielem). 그는 또한 컨디셔닝을 무시하고도 CFG 결과를 개선하는 미니배치-OT 매칭을 지적합니다 (sedielem).
인퍼런스 인프라 및 시스템
- vLLM v0.32.0: 이번 릴리스(814 커밋)는 /v1/systemone 구조화된 의사결정 엔드포인트와 NVFP4 및 ROCm의 4비트 KV를 포함한 하드웨어 전반에 걸친 저정밀도 KV를 추가합니다. Model Runner V2는 GPU n-그램 스페큘레이터를 추가하며, 멀티-API 워커는 +43~85%의 req/s를 제공합니다 (vllm_project).
- 더 빠른 시작: 이미지에 사전 컴파일된 Python 바이트코드를 포함하면 시작 시간이 14~18% 단축됩니다 (H100에서 약 18초) (nilsmatteson).
- InferenceX 가속기 벤치마크: Inferact는 TorchTPU vLLM 스택에서 메가커널을 사용하여 Google TPUv7 Kimi K3 (2.8T) 제출을 주도했습니다 (SemiAnalysis_).
- TPUv7 대 GB300: NVIDIA의 첫 GB300 FP4 반대 제출은 대부분의 레이턴시 곡선에서 달러당 성능이 1.64배 더 나쁩니다 (SemiAnalysis_).
- Vera Rubin: Vera Rubin NVL72는 1M-컨텍스트 에이전틱 워크로드에서 GB300보다 최대 7.3배 더 우수하다고 주장됩니다 (SemiAnalysis_).
- SGLang 메가커널: SGLang은 메가커널 지원을 병합하여 GB300 NVL72에서 사용자당 1000 tok/s에 근접했습니다 (SemiAnalysis_).
- Meta Prometheus 클러스터: Meta는 수십만 개의 GPU를 갖춘 기가와트 규모 클러스터에서 Muse Wonder를 학습시켰습니다. 이 클러스터는 85%+ 사전 학습 굿풋, 90%+ RL 굿풋, 그리고 약 47K GPU-시간의 평균 중단 간격을 보고합니다 (AIatMeta).
- 데이터센터 구축: SemiAnalysis는 2027년에 50GW 이상의 용량을 예상하며, 60GW가 건설 중이고 연초부터 $1.3T 규모의 리스가 체결되었으며, 부족 현상이 칩으로 옮겨갈 수 있다고 경고합니다 (SemiAnalysis_).
- 후속 학습 도구:
- Together 후속 학습: 사용자 정의 보상 및 환경을 갖춘 SFT 및 RL을 제공합니다 (togethercompute).
- prime-rl v0.10.0: 비동기 안정성을 위해 튜닝된 새로운 RL 알고리즘인 IPO를 출시합니다 (PrimeIntellect).
- veRL: Zhihu 설명자는 veRL이 비동기 에이전트 RL로 전환하는 과정을 추적합니다. 델타 가중치 동기화는 가중치 전송 시간을 10.3배 단축했습니다 (ZhihuFrontier).
- Anthropic, git 대체: Anthropic은 병합 건수가 하루 2,500건에서 30,000건 이상으로 증가한 후, 7명의 인원으로 5개월 만에 git의 자체 대체 시스템을 구축했습니다 (dl_weekly).
산업 및 정책
- Anthropic 공익 기금: 새로운 기금은 Anthropic 주식의 5%로 시작합니다. 회사 가치가 50% 상승할 때마다 최대 2%가 추가될 수 있습니다. 창업자 및 직원 서약과 합쳐서, 지분의 약 20%가 공익을 위해 약정되었습니다 (AnthropicAI, jackclarkSF).
- 회의적인 시각: @willcb는 이를 유동성을 제한하는 창의적인 자본 구조로 해석합니다 (willcb).
- Anthropic 연방 법안 초안: Anthropic의 연방 업무 책임자는 회람된 초안을 옹호하며, 그 우선 적용 조항이 축소될 것이라고 말했습니다. 이 초안은 법원이 위험한 모델의 연구소 내부 사용을 중단시킬 수 있도록 하며, 모델이 통제를 벗어날 경우 보고를 의무화합니다 (ajcimino).
- 비판: Nathan Calvin은 지난 한 해 동안 Anthropic의 행동이 안전성보다 초지능 경쟁을 우선시하고 있음을 나타낸다고 주장합니다 (_NathanCalvin).
- 미중 AI 주권: 중국 법안 초안은 2T 파라미터, 10^26 FLOPs를 초과하거나 글로벌 상위 10위에 드는 모델의 가중치를 수출하려면 정부 승인을 요구할 것이며, API 접근에는 영향을 미치지 않습니다 (kimmonismus).
- DHS 금지: 미국 국토안보부는 민간 기관에 DeepSeek 및 이를 기반으로 구축된 제품을 제거하도록 명령하고 있습니다 (kimmonismus).
- 화웨이 칩: DeepSeek은 화웨이 AI 칩 설계를 돕고 있는 것으로 알려졌습니다 (kimmonismus).
- 예정된 출시 (보고됨, 미확인): The Information은 향후 몇 주 내에 출시될 것으로 예상되는 Anthropic 모델, Google의 Gemini 4 Carbon, 그리고 GPT-6.1 Sol보다 저렴한 가격의 더 유능한 OpenAI Terra 모델에 대해 보도했습니다 (steph_palazzolo, correction).
- OpenAI 채용: Aleksander Madry는 OpenAI로 돌아와 Jakub Pachocki와 함께 AI 발전의 안전성 및 속도 조절에 대해 협력할 예정입니다 (aleks_madry, merettm).
- 오픈 모델 컴퓨트 커먼즈: 현재 약 $1B 규모의 학습 컴퓨트가 Hugging Face Hub에서 무료로 다운로드 가능하며, 이는 2023년 말 $40M 미만에서 증가한 수치입니다 (Thom_Wolf).
인기 트윗 (참여도 기준)
- Anthropic, 새로운 기금을 통해 지분 약 20%를 공익에 약정 (25.4K)
- CAD/BIM을 위한 SKY-001 엔지니어링 월드 모델 (9.6K)
- Google, 자체 개선 하네스 프레임워크 Harness² 오픈소스화 (8.9K)
- Anthropic, 중요한 오픈소스 프로젝트를 위한 OSS 스캐너 출시 (8.7K)
- MiniMax M3.1 Flash 출시 및 가격 (8.1K)
- 프론티어 모델, 공격 중 OpenCode 돕기 거부 (6.3K)
- OpenAI, COBOL, Fortran 및 VB 구축 및 마이그레이션 개선 (5.7K)
- Inception, Mercury 3 디퓨전 LLM 출시 (4.7K)

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-not-much-happened-today-f09&utm_source=paywall-free-trial&utm_medium=web&utm_content=221267504&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-not-much-happened-today-f09&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
