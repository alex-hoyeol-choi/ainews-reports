# OpenAI closes $110B raise from Amazon, NVIDIA, SoftBank in largest startup fundraise in history @ $840B post-money

**원문 URL**: https://www.latent.space/p/ainews-openai-closes-110b-raise-from
**번역일**: 2026-02-28 12:35
**발행일**: 2026-02-28

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] OpenAI, Amazon, NVIDIA, SoftBank로부터 $110B 투자 유치, $840B 투자 후 기업 가치로 역사상 최대 스타트업 자금 조달 기록

### 축하합니다, 가장 큰 숫자를 확보하셨습니다.
공유> 2026년 2월 26일~27일 AI 뉴스입니다. 12개 서브레딧, 544개 트위터, 24개 디스코드(263개 채널, 12529개 메시지)를 확인했습니다. 예상 절약 독서 시간(200wpm 기준): 1189분. AINews 웹사이트에서 모든 지난 호를 검색할 수 있습니다. 다시 한번 말씀드리지만, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!
미 국방부(Department of War)와의 끊임없는 입장 표명(Anthropic은 조건 거부 vs OpenAI는 계약 체결)을 배경으로, OpenAI는 12월부터 시작된 많은 논의가 있었던 대규모 투자 라운드를 마침내 마무리했습니다. 게시물에서 그들은 몇 가지 흥미로운 새로운 내용을 공개했습니다:
- Codex 주간 사용자 수는 연초 이후 세 배 이상 증가하여 160만 명을 기록했습니다 (2월 4일에는 100만 명이었음 (!!?!?!)
- 9백만 명 이상의 유료 비즈니스 사용자가 업무에 ChatGPT를 의존하고 있습니다 (2025년 6월에는 3백만 명이었음)
- ChatGPT는 사람들이 AI를 시작하는 곳으로, 주간 활성 사용자 수가 9억 명 이상이며, 현재 5천만 명 이상의 소비자 구독자를 보유하고 있습니다 (1월/2월에 수익화가 계속 가속화되고 있음) (2025년 10월에는 8억 명, 7월에는 유료 구독자 3천5백만 명이었음)
이 모든 것은 $730B의 투자 전 기업 가치에 $110B의 신규 투자를 정당화합니다:
- SoftBank로부터 $30B (“우리의 ASI 전략 발전”),
- NVIDIA로부터 $30B (3 GW의 전용 인퍼런스 용량 및 Vera Rubin 시스템에서의 2 GW 학습 사용 포함) - "최대 $100B"에서 하향 조정되었지만, 여전히 순환 자금 조달 우려가 남아있습니다.
- Amazon으로부터 $50B 및 파트너십 강화 (분석) 포함:초기 $15B 투자 후 특정 조건 충족 시 수개월 내 $35B 추가 투자 — Amazon은 OpenAI와 Anthropic 모두에 상당한 지분을 갖게 됩니다.Amazon Bedrock에서 OpenAI가 구동하는 "Stateful Runtime Environment"AWS는 OpenAI Frontier의 독점적인 서드파티 클라우드 제공업체가 될 것입니다.AWS 인프라를 통해 "8년간 $100B" 가치의 2기가와트 Trainium 용량 (Trainium3 및 차세대 Trainium4 칩 모두 포함)
면밀히 관찰하는 사람들은 Microsoft의 부재를 알아차릴 수 있는데, 이는 기존의 축소된 파트너십을 계속하고 스테이트리스 API를 받습니다.
이를 관점에서 보면, 118개 국가/경제의 명목 GDP가 $100B 미만입니다 — 전 세계 경제의 약 61%에 해당합니다. 연속적인 "역사상 최대 자금 조달"이 너무 커서 인간의 머리에 다 들어가지 않기 때문에, wtfhappened2025.com에 어울리는 차트가 있습니다:
그리고 AI 외적으로, 10년 역사:
그리고 여기 OpenAI Deep Research + ChatGPT Canvas에서 금액 내림차순으로 정렬된 차트:
또는 타임라인 관점:

---

# AI 트위터 요약
즉각적인 LoRA "컴파일"을 위한 하이퍼네트워크: Doc-to-LoRA + Text-to-LoRA
- Doc-to-LoRA / Text-to-LoRA (Sakana AI): Sakana는 단일 포워드 패스로 LoRA 어댑터를 생성하는 하이퍼네트워크를 학습시켜 커스터마이징 비용을 상각하는 두 가지 관련 방법을 소개합니다. 이는 파인튜닝 / 디스틸레이션 / 긴 컨텍스트 프롬프팅을 "즉각적인 가중치 업데이트"로 전환합니다. 핵심 주장은 다음과 같습니다: 비싼 활성 컨텍스트 윈도우에 모든 것을 유지하는 대신, 작업 설명이나 긴 문서를 서브-세컨드 레이턴시로 어댑터 가중치로 컴파일하여 빠른 적응과 "영구적인 메모리"와 유사한 동작을 가능하게 합니다 (SakanaAILabs, hardmaru).Text-to-LoRA: 자연어 설명만으로 미지의 작업에 특화됩니다 (SakanaAILabs).Doc-to-LoRA: 사실적 문서를 내재화합니다; needle-in-a-haystack 벤치마크에서 기반 모델 컨텍스트 윈도우보다 약 5배 긴 시퀀스에서 거의 완벽한 정확도를 보고하며, 심지어 크로스-모달 트릭을 시연합니다: 내재화된 가중치를 통해 VLM의 시각 정보를 텍스트 전용 모델로 전송합니다 (SakanaAILabs; 요약 스레드 omarsar0).긴 컨텍스트와의 포지셔닝: 2차 어텐션 비용을 줄이고 호출할 때마다 긴 문서를 다시 읽는 것을 피하는 방법으로 명시적으로 구성되었습니다—토큰 대신 어댑터에 지식을 저장합니다 (omarsar0).
- 크레딧 / 선행 연구 논란: 한 연구원은 Hypersteer (텍스트 설명에서 스티어링 벡터를 생성하는 하이퍼네트워크)가 이후 유사한 작업에서 충분한 크레딧을 받지 못했다고 불평합니다 (aryaman2020). 또한 광범위한 커뮤니티의 흥분 / "하이퍼네트워크가 돌아왔다"는 반응도 있습니다 (willdepue, zhansheng).
- 제기된 의문: 왜 매우 긴 KV-cache를 가진 어텐션을 사용하지 않는가—즉, Doc-to-LoRA는 주로 효율성/서빙 비용에 관한 것인가? (hyhieu226)

---
OpenAI 자금 조달 + 배포 투명성 툴링
- $110B 자금 조달 라운드: OpenAI는 Amazon, NVIDIA, SoftBank의 지원을 받아 $110B 투자를 유치했다고 발표했으며, 이는 "모두에게 AI를 제공하기 위한" 인프라 확장으로 프레이밍되었습니다 (OpenAI, sama). Epoch AI의 별도 노트는 규모를 맥락화합니다: 이번 라운드는 현재까지 조달된 총 자본을 거의 세 배로 늘릴 것입니다; The Information은 2028년까지 $157B의 현금 소진을 예상하며, 이번 라운드와 기존 현금은 대략 그 예상을 충족할 것입니다 (EpochAIResearch).
- Deployment Safety Hub: OpenAI는 "시스템 카드"(이전에는 PDF)를 검색 가능한 사이트로 출시하여 배포 안전성 문서에 대한 더 접근성 높은 인터페이스를 제공합니다 (dgrobinson).

---
미 국방부("Department of War") vs Anthropic 논란: 공급망 지정, 반발, 그리고 산업적 함의
- Anthropic, 선을 긋다; 기술계 반응: 핵심 쟁점은 Anthropic이 대규모 국내 감시 및 완전 자율 무기(Anthropic의 성명에 반응하는 게시자들이 특징지은 바와 같이)를 가능하게 하는 것을 공개적으로 거부한 것입니다. 이는 경쟁사 간의 이례적인 칭찬을 받았고 프론티어 모델 배포의 "레드라인"에 대한 관심을 높였습니다 (mmitchell_ai, ilyasut).
- 지정 충격 + 법적 범위 논쟁: DoW가 Anthropic을 "국가 안보에 대한 공급망 위험"으로 지정하고 계약자/파트너에게 압력을 가하려는 움직임에 대한 게시물이 유포되면서, 합법성, 선례, 위축 효과에 대한 논쟁이 촉발되었습니다 (kimmonismus, deanwball). 한 가지 법적 해명: 국방부는 계약자가 국방부 계약 업무에서 무엇을 할지 제한할 수 있지만, 계약자가 사적/상업적 업무에서 Anthropic을 사용하는 것을 법적으로 금지할 수는 없을 것입니다 (petereharrell).
- 경제적/전략적 파급 효과 프레이밍: 가장 날카로운 비판은 이것이 사업 파트너로서 미국의 신뢰도를 손상시키고 잠재적으로 하이퍼스케일러/투자자를 불가능한 상충 관계로 몰아넣을 것이라고 주장합니다 (deanwball); 다른 이들은 전체 세부 사항이 알려질 때까지 불확실성을 언급하지만, 여전히 공급망 지정을 부적절하다고 봅니다 (jachiam0).
- 대중 정서 급등: 게시물들은 국방부 지원 국내 감시 프로그램과 거부에 대한 처벌이라는 생각에 대한 강력한 대중의 분노를 강조합니다 (quantian1, janleike). 많은 사용자들이 Claude에 대한 "연대 구독"을 표명합니다 (willdepue, Yuchenj_UW).
- Anthropic 성명 및 소송 의사: Anthropic은 Hegseth 장관의 발언에 대한 공식 성명을 게시합니다 (AnthropicAI). 논평은 "법정에서 모든 공급망 위험 지정에 이의를 제기할 것"이라는 문구를 강조하고 국방부 계약 범위를 벗어난 고객 제한에 대한 분쟁을 강조합니다 (iScienceLuvr).
- 핵심 요점: Anthropic의 선택에 대한 입장이 어떻든 간에, 많은 게시물들은 이것을 거버넌스 선례의 순간으로 다룹니다: 누가 허용 가능한 사용을 결정하고, 어떤 적법 절차가 존재하며, 계약이 빠르게 변화하는 모델 역량과 어떻게 상호작용하는지 (kipperrii).

---
모델 + 리더보드: Qwen3.5 확장 및 "오픈 모델" 순위
- Qwen3.5 신규 릴리스 (Artificial Analysis 요약): Alibaba는 Qwen3.5를 27B dense, 122B A10B MoE, 35B A3B MoE로 확장했으며, 모두 Apache 2.0 라이선스이며 262K 컨텍스트를 지원합니다 (게시물에 따르면 YaRN을 통해 1M까지 확장 가능). Artificial Analysis는 인텔리전스 인덱스 점수를 보고합니다: 27B = 42, 122B A10B = 42, 35B A3B = 37이며, 27B의 GDPval-AA 1205와 같은 주목할 만한 에이전틱/작업 지표와 자세한 상충 관계(환각/정확도 및 토큰 사용량—27B는 인덱스를 실행하는 데 98M 출력 토큰을 사용)를 포함합니다 (ArtificialAnlys).
- Arena 리더보드 (2026년 2월): Arena는 텍스트 및 코드 부문 최고의 오픈 모델을 게시합니다. 텍스트 상위 3개: GLM-5 (1455), Qwen-3.5 397B A17B (1454), Kimi-K2.5 Thinking (1452) (arena). 코드 Arena 상위권에는 GLM-5 (1451)가 1위, Kimi-K2.5와 MiniMax-M2.5가 공동 2위를 차지했습니다 (arena). Arena는 또한 재현 가능한 리더보드를 위한 오픈소스 랭킹 패키지인 Arena-Rank를 강조합니다 (arena).
- Perplexity, 양방향 임베딩 모델 오픈소스화 (주장): 한 스레드는 Perplexity가 양방향 "Qwen3-retrained" 임베딩 모델(0.6B/4B; 표준 vs 컨텍스트 인식 임베딩; MIT 라이선스)을 오픈소스화하여 리트리벌을 위한 문서 수준 이해를 개선했다고 주장합니다; 이는 공식 릴리스 노트라기보다는 서드파티 요약으로 간주됩니다 (LiorOnAI).

---
시스템, 인퍼런스, 커널, 그리고 RL 학습: 대역폭, ROCm, 그리고 오프-폴리시 RL
- vLLM ROCm 어텐션 백엔드 (AMD): vLLM은 KV-cache 레이아웃 변경, 배칭 트릭, 모델별 커널을 포함하는 ROCm용 vLLM의 7가지 어텐션 백엔드를 발표했습니다; 환경 변수 스위치(VLLM_ROCM_USE_AITER=1)를 통해 AMD GPU에서 최대 4.4배의 디코드 처리량 향상을 보고했습니다 (vllm_project). 후속 게시물은 MLA KV 압축 주장(예: ~8K → 576차원)과 MI300X/MI325X/MI355X에서의 처리량 향상을 자세히 설명합니다 (vllm_project).
- DeepSeek DualPath I/O 논문 (서드파티 설명): ZhihuFrontier 요약은 DeepSeek+THU+PKU 논문이 RDMA를 통해 디코드 노드의 유휴 스토리지 NIC 대역폭을 활용하여 에이전틱 긴 컨텍스트 인퍼런스의 KV-cache 이동 병목 현상을 해결하기 위한 Prefill/Decode의 시스템 수준 재설계를 제안한다고 설명합니다; 소규모 모델에 대한 주의사항과 함께 주장된 속도 향상(예: DS-660B에서 1.87배)을 포함합니다 (ZhihuFrontier).
- 커널/인프라 잡담 ("quack", Liger): 한 스레드는 Dao-AILab의 메모리 계층 대역폭에 대한 quack 보고서와, Liger가 xentropy에 클러스터 수준 리덕션을 사용하지 않는 것이 일부 설정에서 느린 성능을 설명할 수 있다는 점을 지적합니다 (fleetwood___).
- 추론을 위한 오프-폴리시 RL (Databricks MosaicAI): Databricks는 OAPL (Optimal Advantage-based Policy Optimization with lagged inference policy)을 GRPO와 같거나 능가하면서 약 3배 적은 학습 세대를 사용하는 안정적인 오프-폴리시 대안으로 홍보하며, 엄격한 온-폴리시 루프보다 운영상 더 간단하다고 포지셔닝합니다 (DbrxMosaicAI, jefrankle).
- ERL vs RLVR (Turing Post 설명): 긴 "워크플로우 분석"은 표준 RLVR (스칼라 검증 가능 보상)과 에피소드 내 반성/재시도 + 디스틸레이션을 삽입하는 경험적 강화 학습(ERL)을 대조합니다; 보고된 성능 향상(예: Sokoban에서 +81%)과 상충 관계(파이프라인 복잡성/연산)를 인용합니다 (TheTuringPost).
- Mamba-2 / GDN 초기화 버그 논의: Albert Gu는 바이럴 플롯 논쟁을 명확히 합니다: 핵심 요점은 초기화 버그가 일부 결과에 실질적인 영향을 미쳤다는 것입니다; 또한 하이브리드에서의 미묘한 상호작용(예: "더 강력한" 구성 요소가 다른 구성 요소를 "게으르게" 만들 수 있으며, 관련 참조도 있음)을 언급합니다 (_albertgu, _albertgu).

---
인게이지먼트 기준 상위 트윗 (기술/산업 관련)
- OpenAI, $110B 투자 유치 (sama, OpenAI)
- Sakana AI Doc-to-LoRA / Text-to-LoRA (SakanaAILabs, hardmaru)
- Anthropic–DoD 공급망 지정 비판 / 거버넌스 선례 (deanwball, quantian1, janleike)
- Karpathy, 코딩 워크플로우 진화에 대해 (탭 → 에이전트 → 병렬 처리) (karpathy)
- Karpathy, 멀티-에이전트 워크플로우를 통한 '연구 조직 프로그래밍'; 관찰된 한계 (karpathy)
- Anthropic 공식 성명 (AnthropicAI)

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-openai-closes-110b-raise-from&utm_source=paywall-free-trial&utm_medium=web&utm_content=189427137&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-openai-closes-110b-raise-from&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
