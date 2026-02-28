# OpenAI closes $110B raise from Amazon, NVIDIA, SoftBank in largest startup fundraise in history @ $840B post-money

**원문 URL**: https://www.latent.space/p/ainews-openai-closes-110b-raise-from
**번역일**: 2026-02-28 11:59
**발행일**: 2026-02-28

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] OpenAI가 Amazon, NVIDIA, SoftBank로부터 1,100억 달러 투자를 유치하며 역사상 최대 스타트업 자금 조달 기록을 세웠습니다 (@8,400억 달러 포스트머니)

### 축하합니다, 가장 큰 숫자를 확보하셨습니다.
공유> 2026년 2월 26일-27일 AI 뉴스. 저희는 여러분을 위해 12개의 서브레딧, 544개의 트위터, 24개의 디스코드(263개 채널, 12529개 메시지)를 확인했습니다. 예상 절약 독서 시간 (200wpm 기준): 1189분. AINews 웹사이트에서 지난 모든 호를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!
국방부(Department of War)와의 끊임없는 포지셔닝(Anthropic은 조건을 거부하고 OpenAI는 거래를 성사시키는 상황)을 배경으로, OpenAI는 12월부터 시작된 많은 논의가 있었던 대규모 투자 라운드를 마침내 마무리했습니다. 해당 게시물에서 그들은 몇 가지 흥미로운 새로운 공개 내용을 발표했습니다:
- Codex 주간 사용자 수가 연초 대비 세 배 이상 증가하여 1.6M에 달했습니다 (2월 4일에는 1M이었습니다 (!!?!?!)
- 9백만 명 이상의 유료 비즈니스 사용자가 업무에 ChatGPT를 활용합니다 (2025년 6월에는 3M이었습니다)
- ChatGPT는 사람들이 AI를 시작하는 곳이며, 주간 활성 사용자가 9억 명 이상이고, 현재 5천만 명 이상의 개인 구독자를 보유하고 있습니다 (1월/2월에도 수익화가 계속 가속화되고 있습니다) (2025년 10월에는 8억 명, 7월에는 유료 구독자 3,500만 명이었습니다)
이 모든 것이 7,300억 달러의 프리머니 가치로 1,100억 달러의 신규 투자를 정당화합니다:
- SoftBank로부터 300억 달러 ("자체 ASI 전략을 발전시키고 있습니다")
- NVIDIA로부터 300억 달러 (3 GW의 전용 인퍼런스 용량 및 Vera Rubin 시스템에서의 2 GW 학습 사용 포함) - "최대 1,000억 달러"에서 하향 조정되었으며, 여전히 순환 자금 조달 우려가 있습니다.
- Amazon으로부터 500억 달러, 강화된 파트너십 (분석) 포함:
  - 초기 150억 달러 투자와 특정 조건 충족 시 향후 몇 달 내 350억 달러 추가 투자 — Amazon이 OpenAI와 Anthropic 모두에 상당한 지분을 갖게 됩니다.
  - Amazon Bedrock에서 OpenAI가 구동하는 "Stateful Runtime Environment"
  - AWS는 OpenAI Frontier를 위한 독점적인 서드파티 클라우드 제공업체가 될 것입니다.
  - AWS 인프라를 통한 기가와트 규모의 Trainium 용량, "8년간 1,000억 달러" 가치, Trainium3 및 차세대 Trainium4 칩 모두 포함
면밀히 지켜본 사람들은 Microsoft의 부재를 알아차릴 수 있을 것입니다. Microsoft는 기존의 축소된 파트너십을 유지하고 스테이트리스 API를 받습니다.
이를 관점에서 보면, 118개 국가/경제의 명목 GDP가 1,000억 달러 미만입니다 — 전 세계 경제의 약 61%에 해당합니다. 연이은 "역사상 최대 규모의 자금 조달"은 인간의 머리로 이해하기에는 너무 크기 때문에, wtfhappened2025.com에 어울리는 차트를 여기에 제시합니다:
그리고 AI 외적으로, 10년간의 역사:
그리고 OpenAI Deep Research + ChatGPT Canvas에서 금액을 내림차순으로 정렬한 결과:
또는 타임라인 관점:

---

# AI Twitter 요약
즉각적인 LoRA "컴파일"을 위한 하이퍼네트워크: Doc-to-LoRA + Text-to-LoRA
- Doc-to-LoRA / Text-to-LoRA (Sakana AI): Sakana는 단일 포워드 패스에서 LoRA 어댑터를 생성하도록 하이퍼네트워크를 학습시켜 커스터마이징 비용을 상각하는 두 가지 관련 방법을 소개합니다. 이는 파인튜닝/디스틸레이션/긴 컨텍스트 프롬프팅이 될 작업을 "즉각적인 가중치 업데이트"로 전환합니다. 핵심 주장은 다음과 같습니다: 비싼 활성 컨텍스트 윈도우에 모든 것을 유지하는 대신, 작업 설명이나 긴 문서를 1초 미만의 레이턴시로 어댑터 가중치로 컴파일하여 빠른 적응과 "영구 메모리"와 같은 동작을 가능하게 합니다 (SakanaAILabs, hardmaru).
  - Text-to-LoRA: 자연어 설명만으로 보지 못한 작업에 특화됩니다 (SakanaAILabs).
  - Doc-to-LoRA: 사실 문서를 내재화합니다. 니들-인-어-헤이스택 벤치마크에서 기본 모델 컨텍스트 윈도우보다 약 5배 긴 시퀀스에서 거의 완벽한 정확도를 보고하며, 심지어 크로스 모달 트릭을 시연합니다: 내재화된 가중치를 통해 VLM에서 텍스트 전용 모델로 시각 정보를 전송합니다 (SakanaAILabs; 요약 스레드 omarsar0).
  - 긴 컨텍스트와의 포지셔닝: 2차 어텐션 비용을 줄이고 매 호출마다 긴 문서를 다시 읽는 것을 피하는 방법으로 명시적으로 제시됩니다—토큰 대신 어댑터에 지식을 저장합니다 (omarsar0).
- 크레딧/선행 연구 논란: 한 연구원은 Hypersteer (텍스트 설명에서 스티어링 벡터를 생성하는 하이퍼네트워크)가 이후 유사한 작업에서 충분한 크레딧을 받지 못했다고 불평합니다 (aryaman2020). 또한 광범위한 커뮤니티의 흥분 / "하이퍼네트워크가 돌아왔다"는 반응이 있습니다 (willdepue, zhansheng).
- 제기된 열린 질문: 왜 매우 긴 KV-cache를 가진 어텐션을 사용하지 않는가—즉, Doc-to-LoRA는 주로 효율성/서빙 비용에 관한 것인가? (hyhieu226)

---
OpenAI 자금 조달 + 배포 투명성 도구
- 1,100억 달러 자금 조달 라운드: OpenAI는 Amazon, NVIDIA, SoftBank의 지원을 받아 1,100억 달러 투자를 유치했다고 발표하며, "모두에게 AI를 제공하기 위한" 인프라 확장으로 프레이밍했습니다 (OpenAI, sama). Epoch AI의 별도 메모는 그 규모를 설명합니다: 이 라운드는 현재까지 조달된 총 자본을 거의 세 배로 늘릴 것이며; The Information은 2028년까지 1,570억 달러의 현금 소진을 예상한다고 보도했으며, 이번 라운드와 기존 현금은 그 예상치와 거의 일치할 것입니다 (EpochAIResearch).
- Deployment Safety Hub: OpenAI는 "시스템 카드"(이전에는 PDF)를 검색할 수 있는 사이트를 출시하여 배포 안전 문서에 대한 더 접근하기 쉬운 인터페이스를 제공합니다 (dgrobinson).

---
미국 국방부("Department of War") 대 Anthropic 사가: 공급망 지정, 반발, 그리고 산업적 함의
- Anthropic이 선을 긋다; 기술 업계 반응: 핵심 쟁점은 Anthropic이 대규모 국내 감시 및 완전 자율 무기 활성화를 공개적으로 거부한 것입니다 (Anthropic의 성명에 반응하는 게시자들이 특징지은 바와 같이). 이는 드물게 경쟁사 간의 칭찬을 이끌어냈고 프론티어 배포에서의 "레드 라인"에 대한 관심을 높였습니다 (mmitchell_ai, ilyasut).
- 지정 충격 + 법적 범위 논쟁: 국방부가 Anthropic을 "국가 안보에 대한 공급망 위험"으로 지정하고 계약업체/파트너에게 압력을 가하려는 움직임이 있었다는 주장이 담긴 게시물들이 유포됩니다—이는 합법성, 선례, 그리고 위축 효과에 대한 논쟁을 촉발했습니다 (kimmonismus, deanwball). 한 가지 법적 명확화: 국방부는 계약업체가 국방부 계약 업무에서 하는 일을 제한할 수 있지만, 계약업체가 사적/상업적 업무에서 Anthropic을 사용하는 것을 법적으로 금지할 수는 없을 것입니다 (petereharrell).
- 경제적/전략적 파급 효과 프레이밍: 가장 날카로운 비판은 이것이 비즈니스 파트너로서 미국의 신뢰도를 손상시키고 잠재적으로 하이퍼스케일러/투자자들을 불가능한 트레이드오프로 몰아넣을 것이라고 주장합니다 (deanwball); 다른 이들은 전체 세부 사항이 알려질 때까지 불확실성을 지적하지만, 여전히 공급망 지정이 부적절하다고 봅니다 (jachiam0).
- 대중 정서 급증: 게시물들은 국방부가 지원하는 국내 감시 프로그램과 거부에 대한 처벌이라는 생각에 대한 강력한 대중적 분노를 강조합니다 (quantian1, janleike). 많은 사용자들이 Claude에 대한 "연대 구독"을 표명합니다 (willdepue, Yuchenj_UW).
- Anthropic 성명 및 소송 의사: Anthropic은 Hegseth 장관의 발언에 대한 공식 성명을 게시합니다 (AnthropicAI). 논평은 "법정에서 모든 공급망 위험 지정에 이의를 제기할 것"이라는 문구를 강조하고 국방부 계약 범위를 벗어난 고객을 제한하는 것에 대한 분쟁을 강조합니다 (iScienceLuvr).
- 메타 포인트: Anthropic의 선택에 대해 어떤 입장을 취하든 상관없이, 많은 게시물들은 이것을 거버넌스 선례의 순간으로 다룹니다: 누가 허용 가능한 사용을 결정하고, 어떤 적법 절차가 존재하며, 계약이 빠르게 변화하는 모델 기능과 어떻게 상호 작용하는지 (kipperrii).

---
모델 + 리더보드: Qwen3.5 확장 및 "오픈 모델" 순위
- Qwen3.5 신규 출시 (Artificial Analysis 요약): Alibaba는 27B 덴스, 122B A10B MoE, 35B A3B MoE로 Qwen3.5를 확장했으며, 모두 Apache 2.0 라이선스이고 262K 컨텍스트를 지원합니다 (게시물에 따르면 YaRN을 통해 1M까지 확장 가능). Artificial Analysis는 인텔리전스 인덱스 점수를 보고합니다: 27B = 42, 122B A10B = 42, 35B A3B = 37이며, 27B 모델의 GDPval-AA 1205와 같은 주목할 만한 에이전틱/작업 지표와 상세한 트레이드오프 (환각/정확도 및 토큰 사용량—27B는 인덱스를 실행하는 데 98M 출력 토큰을 사용했습니다)를 포함합니다 (ArtificialAnlys).
- Arena 리더보드 (2026년 2월): Arena는 텍스트 및 코드 부문 최고 오픈 모델을 게시합니다. 텍스트 상위 3개: GLM-5 (1455), Qwen-3.5 397B A17B (1454), Kimi-K2.5 Thinking (1452) (arena). 코드 Arena 상위권에는 GLM-5 (1451)가 1위, Kimi-K2.5와 MiniMax-M2.5가 공동 2위를 차지했습니다 (arena). Arena는 또한 재현 가능한 리더보드를 위한 오픈소스 랭킹 패키지인 Arena-Rank를 강조합니다 (arena).
- Perplexity가 양방향 임베딩 모델을 오픈소스화했습니다 (주장): 한 스레드는 Perplexity가 양방향 "Qwen3 재학습" 임베딩 모델 (0.6B/4B; 표준 대 컨텍스트 인식 임베딩; MIT 라이선스)을 오픈소스화하여 리트리벌을 위한 문서 수준 이해도를 향상시켰다고 주장합니다; 이는 1차 출시 노트보다는 서드파티 요약으로 간주하십시오 (LiorOnAI).

---
시스템, 인퍼런스, 커널, 그리고 RL 학습: 대역폭, ROCm, 그리고 오프-폴리시 RL
- vLLM ROCm 어텐션 백엔드 (AMD): vLLM은 KV-cache 레이아웃 변경, 배치 트릭, 모델별 커널을 포함한 ROCm용 vLLM의 7가지 어텐션 백엔드를 발표했습니다; 환경 변수 스위치 (VLLM_ROCM_USE_AITER=1)를 통해 AMD GPU에서 최대 4.4배의 디코딩 처리량을 보고했습니다 (vllm_project). 후속 내용은 MLA KV 압축 주장 (예: ~8K → 576 차원) 및 MI300X/MI325X/MI355X에서의 처리량 개선을 상세히 설명합니다 (vllm_project).
- DeepSeek DualPath I/O 논문 (서드파티 설명): ZhihuFrontier 요약은 DeepSeek+THU+PKU 논문이 RDMA를 통해 디코드 노드의 유휴 스토리지 NIC 대역폭을 활용하기 위한 Prefill/Decode의 시스템 수준 재설계를 제안한다고 설명합니다. 이는 에이전틱 긴 컨텍스트 인퍼런스를 위한 KV-cache 이동 병목 현상을 목표로 합니다; 소규모 모델에 대한 주의사항과 함께 주장된 속도 향상 (예: DS-660B에서 1.87배)을 포함합니다 (ZhihuFrontier).
- 커널/인프라 잡담 ("quack", Liger): 한 스레드는 Dao-AILab의 메모리 계층 대역폭에 대한 quack 보고서와, Liger가 xentropy에 클러스터 수준 감소를 사용하지 않는 것이 일부 설정에서 더 느린 성능을 설명할 수 있다는 점을 지적합니다 (fleetwood___).
- 추론을 위한 오프-폴리시 RL (Databricks MosaicAI): Databricks는 OAPL (Optimal Advantage-based Policy Optimization with lagged inference policy)을 GRPO와 동등하거나 능가하면서 약 3배 적은 학습 세대를 사용하는 안정적인 오프-폴리시 대안으로 홍보합니다. 이는 엄격한 온-폴리시 루프보다 운영상 더 간단하다고 포지셔닝됩니다 (DbrxMosaicAI, jefrankle).
- ERL 대 RLVR (Turing Post 설명): 긴 "워크플로우 분석"은 표준 RLVR (스칼라 검증 가능한 보상)과 에피소드 내 성찰/재시도 + 디스틸레이션을 삽입하는 Experiential Reinforcement Learning (ERL)을 대조합니다; 보고된 이득 (예: Sokoban +81%) 및 트레이드오프 (파이프라인 복잡성/연산)를 인용합니다 (TheTuringPost).
- Mamba-2 / GDN 초기화 버그 논의: Albert Gu는 바이럴 플롯 논쟁을 명확히 합니다: 핵심 요점은 초기화 버그가 일부 결과에 실질적으로 영향을 미친다는 것입니다; 또한 하이브리드에서의 미묘한 상호 작용을 언급합니다 (예: "더 강력한" 구성 요소가 다른 구성 요소를 "게으르게" 만들 수 있으며, 관련 참조가 있습니다) (_albertgu, _albertgu).

---
인기 트윗 (참여도, 기술/산업 관련 기준)
- OpenAI가 1,100억 달러를 유치했습니다 (sama, OpenAI)
- Sakana AI Doc-to-LoRA / Text-to-LoRA (SakanaAILabs, hardmaru)
- Anthropic–국방부 공급망 지정 비판 / 거버넌스 선례 (deanwball, quantian1, janleike)
- Karpathy의 코딩 워크플로우 진화에 대한 견해 (탭 → 에이전트 → 병렬 처리) (karpathy)
- Karpathy의 다중 에이전트 워크플로우를 통한 "연구 조직 프로그래밍"에 대한 견해; 관찰된 한계 (karpathy)
- Anthropic 공식 성명 (AnthropicAI)

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-openai-closes-110b-raise-from&utm_source=paywall-free-trial&utm_medium=web&utm_content=189427137&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-openai-closes-110b-raise-from&for_pub=swyx&change_user=false)


---

## 📷 이미지

![Image](https://substackcdn.com/image/fetch/$s_!fhcB!,w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F5dd10ca4-c51f-4905-acbf-c1bc803b5ca7_890x600.png)

![Image](https://substackcdn.com/image/fetch/$s_!ax2C!,w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F89dd9766-2fb1-4d42-86f2-6afd1fdfa06d_1206x1401.webp)

![Image](https://substackcdn.com/image/fetch/$s_!YaNo!,w_5760,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Ff262d5b1-7a48-45f4-ae8c-b2646931577f_2910x514.png)

![Image](https://substackcdn.com/image/fetch/$s_!Xhe0!,w_2400,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F5e25815d-e755-44e5-b77b-81fb495c7821_2564x2006.png)

![Image](https://substackcdn.com/image/fetch/$s_!Iqub!,w_2400,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F93ed2a68-ee2f-4599-b965-d993d697115b_2590x2038.png)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
