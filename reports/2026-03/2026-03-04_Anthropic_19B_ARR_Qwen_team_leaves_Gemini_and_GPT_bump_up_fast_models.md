# Anthropic @ $19B ARR, Qwen team leaves, Gemini and GPT bump up fast models

**원문 URL**: https://www.latent.space/p/ainews-anthropic-19b-arr-qwen-team
**번역일**: 2026-03-04 07:28
**발행일**: 2026-03-04

---

[AINews: 주중 요약](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Anthropic, 190억 달러 ARR 달성, Qwen 팀 이탈, Gemini 및 GPT 고속 모델 강화

### 조용한 하루
공유> 2026년 3월 2일~3월 3일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터, 24개의 디스코드(264개 채널, 12765개 메시지)를 확인했습니다. 예상 절약 독서 시간(200wpm 기준): 1137분입니다. AINews 웹사이트에서 모든 지난 호를 검색할 수 있습니다. 다시 한번 말씀드리지만, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!
아마도 오늘 가장 중요한 뉴스는 Anthropic이 뉴스 및 대중의 의식 속에서 특별한 한 달을 보낸 후 190억 달러 ARR을 달성했다는 확인 소식일 것입니다. 이는 OpenAI가 최근 공개한 200억 달러에 놀랍도록 근접한 수치이며, 2026년 말 목표인 300억 달러가 회고적으로 보면 우스울 정도로 가까워 보입니다. 만약 Anthropic이 OpenAI를 "추월"한다면, ChatGPT 출시 이후 존재해 온 계층 구조에 확실히 지각변동을 일으키는 재편이 될 것입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/b8d40f52-7af5-4969-b941-896fbbd80306_1184x1702.png)
오늘 주목할 만한 작은 소식들이 많습니다. GPT 5.3 Instant 메시징의 전반적인 정렬 초점에 비해 속도를 전달하는 데 더 효과적인 Gemini 3.1 Flash-Lite 데모 비디오의 즐거운 사운드를 추천합니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/5c5846dc-3d68-436a-8549-b9b4dd707c5d_1556x1004.png)
마지막으로, 내부 정치 문제로 보이는 이유로 많은 Qwen 연구원들의 대규모 이탈은 오픈소스에 엄청난, 어쩌면 지속적인 타격이 될 수 있습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/9b9024fe-bb8e-481d-898d-d61a0513b082_1264x856.png)

---

# AI 트위터 요약
Gemini 3.1 Flash‑Lite 출시: "동적 사고 수준" + 공격적인 가격/성능
- Gemini 3.1 Flash‑Lite (Preview)는 Google의 가장 빠르고 비용 효율적인 Gemini 3-시리즈 엔드포인트로 출시되었으며, 고볼륨 워크로드에 대한 레이턴시와 처리량을 강조합니다. DeepMind의 출시 스레드는 이를 조절 가능한 사고 수준(작업 복잡도에 따라 컴퓨팅 조절)을 갖춘 "규모에 따른 지능"으로 포지셔닝하며 @GoogleDeepMind, AI Studio / Vertex를 통해 API가 배포됩니다 @Google. Jeff Dean은 Gemini 2.5 Flash보다 2.5배 빠른 첫 토큰 생성 시간과 함께 0.25달러/M 입력 및 1.50달러/M 출력, LMArena에서 1432 Elo, 86.9% GPQA Diamond를 강조했습니다 @JeffDean; Noam Shazeer는 "최대 지능, 최소 레이턴시"를 위한 제품 조절기로서 "사고 수준" 프레이밍을 반복했습니다 @NoamShazeer; Sundar Pichai도 동일한 속도/비용 메시지를 강조했습니다 @sundarpichai.
- 서드파티 벤치마킹/포지셔닝: Artificial Analysis는 Flash‑Lite가 1M 컨텍스트 윈도우를 유지하고, >360 출력 토큰/초 및 ~5.1초의 평균 답변 레이턴시를 측정하며, 2.5 Flash‑Lite 대비 "Intelligence Index"를 개선했지만, 가격이 인상되었다고(혼합 비용이 상당히 증가) 보고합니다 @ArtificialAnlys. Arena는 Flash‑Lite Preview가 Text Arena에서 #36위(1432)를 기록하고 Code Arena에서 #35위 근처에 랭크되어 비용-성능 프론티어에서 강력한 지점이라고 평가합니다 @arena. 반복되는 커뮤니티 반응은 이름과 빠른 출시 주기 때문에 "Flash‑Lite… 아주 웃기는 Google" @JasonBotterill 이며, "Google은 내가 테스트를 마치기도 전에 모델을 출시한다" @matvelloso 입니다.
- 멀티모달 관점: Google 직원은 텍스트+이미지+비디오+오디오+PDF 수집을 위해 "파서를 작성하는 대신 Flash‑Lite를 사용하라"고 주장하며 @koraykv, Flash‑Lite를 프로덕션 워크플로우를 위한 배관 모델로 강화하고 있습니다.
OpenAI: GPT‑5.3 Instant 배포 + "덜 설교적" + GPT‑5.4 예고
- GPT‑5.3 Instant는 모든 ChatGPT 사용자에게 배포되었으며, 5.2가 "너무 조심스럽다"거나 "너무 많은 단서가 붙는다"는 불만에 명시적으로 응답했습니다. OpenAI는 향상된 대화의 자연스러움, 불필요한 거부/방어적 면책 조항 감소, 더 나은 검색 통합 답변을 주장합니다 @OpenAI, @nickaturley. OpenAI는 또한 환각이 감소했다고 밝히는데, 내부 기여자에 따르면 검색 사용 시 26.8%, 검색 미사용 시 19.7% 개선되었다고 하며 @aidan_mclau, 직원들도 이를 반복했습니다 @christinahkim.
- API/Arena 노출: 커뮤니티 보고에 따르면 "GPT‑5.3‑chat‑latest"가 API에 나타나며 @scaling01, Text Arena에서 병렬 평가에 사용할 수 있습니다 @arena.
- GPT‑5.4는 높은 참여도를 이끌어낸 "생각보다 빨리" 게시물 @OpenAI로 예고되었으며, "5.3 Thinking과 Pro가 곧 뒤따를 것"이라는 이야기 @kimmonismus와 순서에 대한 혼란을 야기했습니다. 여러 트윗은 5.4가 국방부/국가안보국 계약 논란 속에서 뉴스 주기 전환용으로 사용되고 있다고 추측합니다 @kimmonismus.
Alibaba Qwen 충격: 리더십 이탈, "Qwen은 사람이 없으면 아무것도 아니다", 오픈소스 불확실성
- 주요 이탈: 데이터셋 전반의 주요 논의는 Qwen의 기술 리더십과 선임 기여자들의 이탈입니다. Justin Lin의 "사임" 게시물은 광범위한 반응을 불러일으켰고 @JustinLin610, 이어서 높은 신뢰도의 확인/추모와 함께 또 다른 리더("bye qwen, me too") @huybery 및 별도의 작별 인사 @kxli_2000를 포함한 더 많은 이탈이 있었습니다. 외부 관찰자들은 이를 Alibaba Cloud가 Qwen의 기술 리더를 "내쫓았다"고 묘사합니다 @YouJiacheng.
- 기술적으로 중요한 이유: 많은 엔지니어들은 Qwen을 오픈 모델 생태계, 특히 10B 미만 및 "파레토 프론티어" 모델, 그리고 VLM/OCR 파생 모델을 위한 핵심 인프라로 간주합니다. 이는 오픈 웨이트 출시 주기가 느려지거나 라이선싱 입장이 변경될 경우 진정한 생태계 위험으로 프레이밍됩니다 @natolambert, @teortaxesTex, @awnihannun. 또한 "인기 있는 오픈 모델만으로는 충분하지 않았다"는 점을 감안할 때 Qwen의 OSS 입장이 변경될지 여부에 대한 즉각적인 추측도 있습니다 @code_star.
- 조직 진단: 반복되는 해석은 상위 Alibaba 구조(CEO에게 보고) 하의 "통합"이 영향력/가시성에 대한 정치적 압력을 야기했으며 @Xinyu2ML, 외부 신뢰를 구축하는 "다리" 역할을 하는 이들을 빅테크 계층 구조가 처벌한다는 광범위한 논평이 있었습니다 @hxiao.
- 혼란 속에서도 출시는 계속됩니다: Qwen 3.5 LoRA 파인튜닝 가이드와 저-VRAM 학습 레시피가 빠르게 확산되었고(특히 Unsloth) @UnslothAI, vLLM/SGLang 지원이 포함된 GPTQ Int4 가중치가 홍보되었습니다 @Alibaba_Qwen. 커뮤니티는 또한 Qwen3.5에 대한 교육/재구현을 추진했습니다 @rasbt. 긴장은 강력한 출시 속도와 리더십 이탈이 겹치는 상황입니다.
긴 컨텍스트 + 학습 효율성: "불가능했던" 컨텍스트 윈도우를 실용적으로 만들기
- 긴 컨텍스트 학습을 위한 어텐션 메모리 87% 감소: Together 논문은 Context Parallelism과 Sequence Parallel 스타일 헤드 청킹의 하이브리드를 강조하며, 8×H100(단일 노드)에서 5M 컨텍스트 윈도우 8B 모델을 학습하고 어텐션 메모리 사용량을 최대 87%까지 줄였다고 주장합니다 @rronak_. 이 트윗은 또한 실질적인 격차를 지적하는데, 긴 컨텍스트 프론티어 모델에 대한 대부분의 RL 사후 학습은 메모리 비용 때문에 여전히 전체 컨텍스트의 일부에서만 수행된다는 것입니다.
- FlashOptim (Databricks): 메모리를 절감하면서 업데이트 등가성을 유지하는 오픈소스 옵티마이저 구현(AdamW/SGD/Lion)입니다. 트윗 스레드는 pip install flashoptim을 발표했으며 @davisblalock, MosaicAI는 50% 이상의 학습 메모리 감소를 요약합니다. 예를 들어, AdamW 학습 오버헤드를 매개변수당 ~16바이트에서 7바이트(그라디언트 해제 시 5바이트)로 줄이고, 예시 8B 파인튜닝 피크를 175GiB에서 113GiB로 감소시켰습니다 @DbrxMosaicAI.
- RL을 위한 이종 인프라: SkyPilot은 RL 사후 학습이 강력한 GPU(트레이너), 저렴한 GPU(롤아웃), 고메모리 CPU(리플레이 버퍼)에 걸쳐 워크로드를 분할해야 한다고 주장합니다. Job Groups는 조정된 라이프사이클 및 서비스 디스커버리를 갖춘 단일 YAML 오케스트레이션 모델을 제공합니다 @skypilot_org.
- 커널/툴체인 문제점: CuTeDSL + torch.compile 회귀 보고서는 커스텀 옵스를 통해 컴파일 호환 가능하게 만들 때 래핑된 커널(RMSNorm "Quack" 커널 포함)의 속도가 ~2.5배 저하된다고 지적하며, 커널 수준 속도와 그래프 컴파일 요구 사항 사이의 마찰을 강조합니다 @maharshii.
에이전트 엔지니어링 현실 점검: 벤치마크 대 "실제 작업", 합의 실패, 툴링 변화 (MCP, 샌드박스, 관측 가능성)
- 벤치마크가 노동 경제학과 일치하지 않습니다: 새로운 데이터베이스는 에이전트 벤치마크를 실제 작업 분포에 매핑하려는 시도를 하며, 대부분의 노동/자본이 다른 곳에 있음에도 불구하고 현재 평가가 수학/코딩에 과도한 비중을 둔다고 주장합니다 @ZhiruoW. 이 점은 "실제 작업을 위한 AI 벤치마킹의 핵심 문제"로 강조되었습니다 @emollick. Arena의 Document Arena 출시는 직접적인 대응입니다: 실제 PDF 추론 병렬 평가; Claude Opus 4.6이 (Arena에 따르면) 선두를 달립니다 @arena.
- 다중 에이전트 조정은 취약합니다: 비잔틴 합의 게임은 LLM 에이전트 합의가 악의적이지 않을 때도 신뢰할 수 없음을 보여줍니다. 실패는 적대적 손상보다는 정지/타임아웃에서 오는 경우가 많으며, 그룹 크기가 커질수록 악화됩니다 @omarsar0. 마음 이론 + BDI + 기호 검증에 대한 보완적인 연구는 인지적 "ToM 모듈"이 자동으로 도움이 되지 않으며, 이득은 기본 모델의 능력에 크게 의존한다고 제안합니다 @omarsar0.
- MCP "죽었는가?" 대 MCP 확장: DAIR의 Omar @omarsar0로부터 "MCP는 죽었는가?"라는 명시적인 질문이 있었지만, 동일한 데이터셋에서 MCP 채택은 확대됩니다: Notion은 Meeting Notes를 위한 MCP/API 지원을 출시했고(Claude Code를 통한 한 줄 설치) @zachtratar; Cursor는 에이전트가 채팅 내에서 대화형 UI를 렌더링하는 MCP Apps를 출시했습니다 @cursor_ai.
- "코드 리뷰 없애기" 논쟁: swyx는 인간 코드 리뷰 제거를 에이전틱 엔지니어링과 SDLC 역전의 "최종 보스"로 묘사합니다 @swyx. 반론: thdxr은 LLM을 통해 "이렇게 많은 코드를 생성하는" 팀이 LLM을 잘못 사용하고 있을 수 있다고 주장합니다. 대량의 코드는 자멸적인 코드베이스를 만들고, LLM 자체도 결과적인 복잡성에 어려움을 겪는다는 것입니다 @thdxr.
- 샌드박스화된 "컴퓨터 사용" 플랫폼: Perplexity의 "Computer"는 큰 관심을 끌고 있습니다: Srinivas는 기능 요청을 받으며 @AravSrinivas, Perplexity는 자사 제품을 많은 모델을 오케스트레이션하고 관리형 보안 샌드박스(API 키 관리 불필요)를 통해 앱에 직접 임베딩하는 것으로 포지셔닝합니다 @AravSrinivas, @AskPerplexity. Cursor의 클라우드 에이전트도 유사하게 격리된 VM에서 실행되며 아티팩트와 함께 병합 준비된 PR을 출력합니다 @dl_weekly.
인재, 거버넌스, 신뢰: Anthropic 대 국방부, OpenAI 계약 조사, 주목할 만한 움직임
- Max Schwarzer (OpenAI 사후 학습 VP) → Anthropic: 주요 인사이동입니다. Schwarzer는 사후 학습을 이끌고 GPT‑5/5.1/5.2/5.3-Codex를 출시한 후 OpenAI를 떠나 IC RL 연구로 돌아가기 위해 Anthropic에 합류한다고 발표했습니다 @max_a_schwarzer. 이는 "Anthropic의 큰 승리" @kimmonismus 및 광범위한 "전설들이 이탈한다"는 불안감 @yacinelearning 내러티브에 불을 지폈습니다.
- Anthropic 대 펜타곤/팔란티어 긴장: 보도에 따르면 국방부는 Anthropic을 "공급망 위험"으로 분류하겠다고 위협했으며, 이는 연방 업무를 위한 Palantir의 사용에 잠재적으로 영향을 미칠 수 있습니다. Anthropic은 안전 장치(대규모 국내 감시 + 자율 무기)를 원합니다 @srimuppidi, 추가 보도 자료는 @aaronpholmes에서 확인할 수 있습니다.
- OpenAI–국방부 / 국가안보국 신뢰 위기: 여러 트윗은 실제 계약 문구를 요구하며, "우발적" 감시 문구가 역사적으로 영장 없는 국내 감시를 가능하게 했다고 주장합니다. 비평가들은 PRISM/Upstream 및 FISA/EO 12333 맥락을 인용하며 @jeremyphoward, "우리를 믿으라"는 확신보다는 독립적인 법률 레드팀 구성을 요구합니다 @sjgadler. 이는 OpenAI가 모델 출시를 통해 내러티브를 조종할 것이라는 가설과 반복적으로 연결됩니다.
- 시장 점유율 주장: 한 바이럴 주장은 Claude가 1년 이내에 소수 점유율에서 미국 비즈니스 시장 점유율을 ChatGPT 대비 지배하는 수준으로 급증했다고 말합니다 @Yuchenj_UW. 기본 데이터셋을 검증할 수 없다면 방향성으로만 간주해야 하지만, 이는 인지된 모멘텀을 반영합니다: "코딩 + 에이전트가 성과를 냈습니다."

---

### 인기 트윗 (참여도 기준, 기술 중심)
- GPT‑5.4 티저: "5.4 생각보다 빨리." @OpenAI
- Gemini 3.1 Flash‑Lite 출시 스레드 @GoogleDeepMind
- GPT‑5.3 Instant 배포 + "덜 설교적" @OpenAI
- Qwen 리더십 이탈("사임") @JustinLin610 및 후속 작별 인사 @huybery
- Unsloth: Qwen3.5 LoRA, ~5GB VRAM 주장 + 노트북 @UnslothAI
- Cursor: MCP Apps (에이전트 채팅 내 대화형 UI) @cursor_ai
- Together 긴 컨텍스트 학습 메모리 감소 (최대 87%) @rronak_

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Qwen 3.5 모델 출시 및 벤치마크
- Qwen 2.5 -> 3 -> 3.5, 가장 작은 모델들. 세대를 거듭하며 놀라운 개선을 이루었습니다. (활동: 1017): Qwen 3.5는 Qwen 모델 시리즈의 주목할 만한 발전으로, 비전 인코더를 포함하는 0.8B 매개변수 모델을 특징으로 하며, 이는 언어 모델 구성 요소가 훨씬 더 작음을 시사합니다. 이 모델은 현재의 더 작은 MoE(Mixture of Experts) 모델과 같이 더 작고 효율적인 모델로의 추세의 일부이며, 이들은 성능으로 칭찬받고 있습니다. 크기에도 불구하고 Qwen 3.5는 항공기 엔진에 대한 잘못된 정보와 같은 사실적 부정확성으로 비판받았으며, 이는 엄격한 사실 확인의 필요성을 강조합니다. 댓글 작성자들은 Qwen 3.5와 같은 더 작은 모델이 로컬 머신에서 개인 비서를 가능하게 할 잠재력을 강조하며, 제한된 GPU 리소스를 가진 사용자들을 위한 효율성과 접근성을 강조합니다. 그러나 모델이 사실을 환각하는 경향이 있어 신뢰성을 훼손할 수 있다는 우려가 있습니다. 더 작은 Qwen 모델, 특히 MoE(Mixture of Experts) 모델은 이전 세대에 비해 인상적인 성능 향상을 보인 것으로 주목됩니다. 이 모델들은 로컬 머신에서 개인 사용에 점점 더 실현 가능해지고 있으며, 더 작은 규모에서도 효율성과 기능에서 상당한 발전을 제공합니다. 한 사용자는 Qwen 3.5의 환각 문제를 강조하며, 항공기 엔진 유형 및 구성과 관련된 특정 사실적 부정확성을 지적합니다. 이는 AI 모델 출력이 자신 있게 잘못된 정보를 제시할 수 있으므로, AI 모델 출력의 사실 확인 중요성을 강조합니다. 4B 모델과 같은 더 작은 양자화된 모델의 성능은 덜 강력한 하드웨어에서의 효율성으로 칭찬받고 있습니다. 한 사용자는 llama.cpp를 사용하여 128k 컨텍스트로 초당 60 토큰을 달성했다고 보고하며, 이는 이전의 더 큰 모델에 비해 상당한 개선으로 간주됩니다. 이는 로컬의 리소스 제약이 있는 환경에서 고성능 AI의 잠재력을 보여줍니다.

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 동안 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-anthropic-19b-arr-qwen-team&utm_source=paywall-free-trial&utm_medium=web&utm_content=189838139&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-anthropic-19b-arr-qwen-team&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
