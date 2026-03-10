# Autoresearch: Sparks of Recursive Self Improvement

**원문 URL**: https://www.latent.space/p/ainews-autoresearch-sparks-of-recursive
**번역일**: 2026-03-10 07:28
**발행일**: 2026-03-10

---

[AINews] 오토리서치: 재귀적 자기 개선의 불꽃

### AGI가 또 한 걸음 나아갔습니다.
공유2025년에 무슨 일이 일어났는지에 대한 여파가 계속되는 가운데, 이제 LLM이 (더 작은) LLM을 완전히 자율적으로 학습시킬 수 있는 시작점에 도달했습니다.
모든 AI 여름에는 "AutoML 모멘트"가 있습니다. 모델이 모델 학습을 자동으로 개선하여 지능의 무한 재귀를 일으키고, 이는 유토피아나 파멸로 이어질 수 있다는 꿈입니다. 우리는 마지막 여름에 있을지도 모르지만, 방금 우리의 순간을 맞이했습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/029937e5-83d-4302-a39c-d0bdac3f797e_1188x1252.png)
karpathy2025년 12월 Yi Tay와의 대화에서 그는 "바이브 트레이닝"에 대해 이야기했습니다:
> "AI 코딩이 이제는 제가 작업을 실행하다 버그가 생기면, 거의 버그를 보지도 않는 지경에 이르렀다고 생각합니다. Antigravity 같은 곳에 붙여넣고 버그를 고치게 합니다. 그리고 작업을 다시 시작하죠. 이건 바이브 코딩을 넘어선, 바이브 트레이닝, 바이브 ML 같은 겁니다. 대부분의 경우 꽤 잘 작동한다고 말할 수 있습니다. 그리고 사실 특정 종류의 문제들은 일반적으로... 저는 이게 정말 좋다는 걸 알고 있고, 사실 저보다 나을 수도 있습니다. 저는 문제를 파악하는 데 20분을 써야 할 겁니다. 레벨 1 바이브 코딩은 뭘 해야 할지 알지만 그냥 너무 게으른 경우라고 할 수 있습니다. 네, 그냥 '아, 그냥 네가 해줘' 하는 거죠. 이런 걸 천 번은 해봤으니까요. 다음 레벨은 뭘 해야 할지조차 모르는 경우입니다. 에이전트가 당신을 위해 버그를 조사해줍니다. 답이 그럴듯해 보이면 그냥 출시하는 거죠. 처음에는 다 확인하고 살펴봤습니다. 그러다 어느 순간, '어쩌면 모델이 나보다 코드를 더 잘 짤 수도 있겠네' 싶어서 그냥 모델이 알아서 하게 놔둡니다. 그리고 모델이 준 수정사항을 바탕으로 작업을 다시 시작합니다."
그래서 우리는 이것이 대형 연구소에서 일어나고 있다는 것을 알고 있었지만, 이제 GPU를 가진 사람이라면 누구나 집에서 이것을 가지고 놀면서 모델이 모델을 개선하는 것을 볼 수 있습니다.
2026년 3월인 지금, 우리는 Jakub Pachocki의 "자동화된 AI 연구 인턴"이 올해 9월까지 ("단순히 채팅이나 코딩을 넘어 인간 연구자를 의미 있게 가속화할 수 있는 시스템") 목표에 잘 도달하고 있는 것으로 보입니다.

---
> 2026년 3월 5일~3월 9일 AI 뉴스입니다. 저희는 12개 서브레딧, 544개 트위터, 24개 디스코드(264개 채널, 27779개 메시지)를 확인했습니다. 예상 절약 독서 시간(분당 200단어 기준): 2649분. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
코딩 에이전트: 제품화, 하네스(harness) 설계, 그리고 "모든 것이 에이전트"
- 코딩 에이전트가 병목 현상을 구현에서 검토/검증으로 옮기고 있습니다. 여러 논의가 동일한 시스템 지점으로 수렴하고 있습니다. 생성은 저렴해지고 있지만, 판단, 거버넌스, 검증이 새로운 제약이 되고 있습니다. @AstasiaMyers의 "실행은 저렴하고, 판단은 희소하다"는 프레이밍과, @omarsar0 및 후속 @omarsar0에서 생성과 검증이 서로 다른 엔지니어링 문제라는 보안/거버넌스 지향적 관점을 참조하십시오. 이는 실제 PR-리뷰 제품 출시 및 대안으로 강화되고 있습니다.Claude Code "Code Review": Anthropic이 멀티 에이전트 PR 리뷰를 출시했습니다. 에이전트가 병렬로 문제를 찾고, 발견 사항을 검증하며, 심각도를 평가합니다. 내부적으로 의미 있는 댓글이 달린 PR 비율이 16%에서 54%로 증가하고, 잘못된 발견은 1% 미만이라고 주장합니다 (Claude, 관련 스레드 @kimmonismus, 반응 @Yuchenj_UW).OpenAI Codex Review 포지셔닝: 리뷰당 가격보다 실질적으로 저렴한 "사용량 기반" 코드 리뷰를 제안합니다. @rohanvarma를 참조하십시오.Devin Review: Cognition이 URL 대체 방식의 무료 PR 리뷰 도구를 출시했으며, 자동 수정 및 diff 기능도 포함합니다 (Cognition).
- 하네스 엔지니어링이 시스템 엔지니어링이 되고 있습니다. 에이전트 저장소를 에이전트 컴퓨팅과 분리하여 에이전트 팀이 격리된 샌드박스에서 실행되는 동안 공유 리포지토리/파일 시스템을 통해 협업할 수 있도록 하는 실용적인 패턴이 나타나고 있습니다. 이는 @Vtrivedy10에서 명시적으로 나타납니다. 관련 인프라 세부 사항에는 샌드박스에서 파일 접근을 용이하게 하기 위해 docker 볼륨 마운트를 추가하는 Hermes-agent가 포함됩니다 (Teknium).
- Perplexity "Computer"가 실제 툴체인을 갖춘 에이전트 오케스트레이터로 변모하고 있습니다. Perplexity는 "Perplexity Computer" 내부에 Claude Code + GitHub CLI를 추가하고, 리포지토리 포크 → 수정 구현 → PR 제출의 엔드투엔드 과정을 시연합니다 (AskPerplexity, @AravSrinivas). 또한 Google/Meta Ads API 커넥터를 통해 자율적인 광고 캠페인 운영을 주장하며 (Arav), 에이전트를 "코딩 도움"에서 비즈니스 인프라 운영으로 확장하고 있습니다.
- 터미널 UX와 "에이전트 인체공학"은 여전히 중요합니다. 개발자들은 CLI 도구에서 기본적인 여러 줄 입력 인체공학(shift+enter)에 대해 불평합니다 (theo, @QuixiAI, 그리고 CLI 앱 전반의 미학/UX 선호도 @jerryjliu0). 이는 "에이전트 역량"이 상호작용 설계에 의해 크게 좌우된다는 점을 상기시켜 줍니다.

---
오토리서치 및 자기 개선 루프: ML 학습 및 에이전트 코드를 최적화하는 에이전트
- Karpathy의 "오토리서치"가 밈에서 측정 가능한 성과로 이어졌습니다. Andrej는 nanochat에서 에이전트 기반 연구 루프를 실행하여, depth=12에서 depth=24로 전이되는 약 20가지 추가적인 변경 사항을 발견하고, 약 700번의 자율적인 변경 후 "Time to GPT-2"를 2.02시간에서 1.80시간으로 (~11%) 개선했다고 보고했습니다 (Karpathy). 엔지니어들을 위한 핵심 요점: "새로운 연구"를 수행하지 않을 때도, 이 루프는 스태킹 가능하고 전이 가능한 학습 레시피 개선 사항(정규화 스케일러, 정규화 격차, 어텐션 튜닝, AdamW 베타, 초기화 등)을 체계적으로 발견할 수 있습니다. 그는 이를 프론티어 연구소의 "최종 보스전"이라고 명시적으로 부릅니다: 스웜 에이전트, 프록시 최적화, 더 큰 규모로 확장.
- 에이전트 루프는 하네스/모델 전반에서 여전히 취약합니다. 반복되는 문제는 장기 실행 루프가 순수한 모델 품질보다 하네스 기능에 더 많이 의존한다는 것입니다. Yuchen은 GPT-5.4 xhigh가 "LOOP FOREVER"를 따르지 못하는 반면, Opus 4.6은 12시간 이상 118개 실험을 실행한다고 언급합니다 (Yuchen). Karpathy는 Codex가 현재 설정에서 오토리서치를 제대로 실행할 수 없으며, 에이전트가 /loop와 같은 특별한 명령을 요구해서는 안 된다고 주장합니다. "만약 제가 영원히 반복하라고 말하면, 그냥 그렇게 해야 합니다" (Karpathy, Yuchen의 의견에 동의). 결론: 에이전트 인프라를 구축하고 있다면, 견고한 루핑 프리미티브, 중단/되감기, 투명한 대화형 세션에 투자하십시오.
- Hermes-agent는 자기 개선 + 논란의 여지가 있는 "스킬" 방향으로 나아가고 있습니다. Nous Research의 Hermes 에이전트가 트렌딩 중인 것으로 강조됩니다 (OpenRouter). Teknium은 Qwen-3B 모델의 신속한 "abliteration"(안전장치 제거)을 주장하고 (Teknium), 나중에 자기 개선 에이전트 코드베이스/GEPA에서 영감을 받은 작업을 언급합니다 (Teknium). 이는 GEPA와 같은 보다 공식적인 "자기 진화 에이전트" 접근 방식과 함께 진행됩니다. 실무자 노트 @myanvoos 및 보고된 성과 언급 (LakshyAAAgrawal)을 참조하십시오.

---
모델 생태계 업데이트: GPT-5.4 담론, 문서 분야 Anthropic의 지배력, 그리고 Gemma/Qwen의 변화
- GPT-5.4: 강력한 사용자 반응, 엇갈리는 벤치마크 논의, 그리고 툴링 제약긍정적인 실제 사용 경험: @Hangsiin은 ChatGPT에서 5.4가 5.2보다 크게 발전했다고 말합니다. @Yampeleg은 이를 "환상적"이라고 부릅니다. @gneubig는 Opus 4.6보다 5.4가 지시 준수 면에서 더 낫다고 선호합니다 (Opus는 더 빠르고 프론트엔드가 더 좋지만).비전/OCR 일화는 어려운 한국어 테이블 OCR에서 큰 개선을 시사하며, 잠재적으로 "에이전틱 비전 + 코드 실행"을 통해 가능하지만 긴 실행 시간(최대 40분)이 소요됩니다 (Hangsiin).일부 벤치마크/메타 코멘터리는 특정 리더보드에서 "high/xhigh" 변형 간의 회귀 또는 순위 차이를 주장하는 반면 (scaling01, scaling01), 다른 이들은 새로운 SOTA 점수를 게시합니다 (예: ZeroBench 델타 JRobertsAI).실용적인 참고: Codex 사용 제한 및 티어링은 스크린샷/요약으로 문서화되어 있으며 (Presidentlin), 실제 워크플로우에서 사람들은 이미 하나의 "최고" 모델을 선택하기보다는 역할(기획자/실행자/편집자)별로 모델을 혼합하고 있음을 강조합니다.
- Anthropic: 문서 분석 리더십 + "펜타곤 블랙리스트" 소송 이야기Document Arena는 문서 분석/장문 추론에서 상위 3개 모델이 Anthropic 모델이라고 보고합니다: Opus 4.6 #1, Sonnet 4.6 #2, Opus 4.5 #3 (arena).제품 성공과 병행하여 주요 정치/법률 뉴스가 돌고 있습니다. 여러 언론 매체/트윗은 Anthropic이 펜타곤에 의해 "공급망 위험"으로 분류된 후 소송을 제기했다고 주장하며, 이는 대량 감시/자율 무기에 대한 안전장치 제거를 거부한 것에 대한 보복으로 해석됩니다 (kimmonismus, TheRundownAI). 엔지니어는 정책 담론을 기술 평가와 분리해야 하지만, 이는 조달 제약 및 기업 채택에 관련이 있습니다.
- Gemma 4 및 Qwen3.5Gemma 4 루머/유출이 돌고 있습니다: "임박했다"는 소문과 함께 120B 전체 / 15B 활성 파라미터 주장을 포함한 파라미터 추측이 있습니다 (scaling01, kimmonismus, 유출 언급 kimmonismus). 공식 출시 전까지는 세부 사항을 미확인으로 간주하십시오.Qwen3.5 로컬 실행 가이드 + 파인튜닝 에이전트 워크플로우가 Unsloth에 의해 게시되었으며, ≤24GB RAM에서 작동하고 Unsloth를 사용하여 모델을 파인튜닝하는 에이전트를 보여준다고 주장합니다 (UnslothAI).Qwen 조직 변화 / 보도 회의론: 한 기자는 익명 소스 "DeepSeek 출시일" 특종과 더 넓은 중국 기술 보도 관행을 비판합니다 (vince_chow1). 또한 Qwen의 기술 리더가 사임했다는 언급도 있습니다 (뉴스레터 요약을 통해, 1차 출처 아님) (ZhihuFrontier).

---
인프라, 성능 및 평가 툴링
- 엣지에서의 vLLM + 라우터 작업 + 디버깅 교훈vLLM은 NVIDIA Jetson에서 MoE (Nemotron 3 Nano 30B)를 "클라우드 API 없이" 온디바이스로 제공하는 완전 로컬 어시스턴트를 실행하는 것을 강조했습니다 (vllm_project).Microsoft 임원이 "vLLM Semantic Router"를 언급한 것이 환영받고 있습니다 (XunzhuoLiu). 시맨틱 라우팅은 프로덕션 스택의 점점 더 중요한 부분이 되고 있습니다.디버깅 노트: DeepGemm 비호환성으로 인한 vLLM 손상; VLLM_USE_DEEP_GEMM=0을 통한 해결책 (TheZachMueller).Claude Code + 로컬 모델 속도 저하: 어트리뷰션 헤더가 KV 캐시를 무효화하여 사실상 O(N²) 동작을 유발하는 것은 "클라우드 에이전트 UX"를 로컬 인퍼런스로 프록시하는 모든 사람에게 구체적인 성능 함정입니다 (danielhanchen).
- 학습 이론 및 처리량웜업/감쇠 이론: "그래디언트 노름이 일찍 떨어질 때 웜업이 필요하다"는 주장과 논문 참조 (aaron_defazio); rosinality는 잔여 브랜치별 스칼라 웜업 패턴을 제안합니다 (rosinality).Hugging Face는 Ulysses 시퀀스 병렬화를 Trainer/Accelerate/TRL에 통합했습니다 (StasBekman).CosNet 아이디어: 선형 레이어에 저랭크 비선형 잔여 함수를 추가하면 사전 학습에서 20% 이상의 실제 시간 속도 향상을 가져온다고 주장합니다 (torchcompiled).
- 평가 및 보안 테스트가 개발 워크플로우의 "초기 단계"로 이동하고 있습니다.OpenAI가 Promptfoo를 인수했습니다. Promptfoo는 오픈소스로 유지되며, "OpenAI Frontier"에서 에이전틱 보안 테스트/평가를 강화할 것입니다 (OpenAI, @snsf의 추가 컨텍스트).LangSmith는 멀티모달 평가자와 병렬 에이전트 작업을 관리하기 위한 Agent Builder 인박스를 추가했습니다 (LangChain, LangChain).Harbor는 대규모로 엔드투엔드 컴퓨터 사용 평가(Windows/Linux)를 통합하여 롤아웃에서 SFT/RL을 위한 궤적을 생성합니다 (Mascobot).Teleport는 "에이전틱 아이덴티티"를 제어 플레인으로 제안합니다: 암호화된 아이덴티티, 최소 권한, MCP/도구 전반의 감사 추적 (TheTuringPost).

---
에이전트에게 더 나은 컨텍스트가 필요합니다: 문서, 리트리벌, 메모리, 그리고 "환경화"
- "도구로서의 문서"(프롬프트 붙여넣기가 아닌)가 표준 프리미티브가 되고 있습니다. Andrew Ng은 Context Hub를 출시했습니다. 이는 최신 API 문서를 가져와 오래된 API 환각을 줄이는 CLI 도구입니다. 또한 영구적인 주석과 궁극적인 커뮤니티 공유를 지원합니다 (AndrewYNg). 이것은 빠르게 변화하는 API에서 에이전트 신뢰성을 실질적으로 변화시키는 종류의 작은 "접착" 도구입니다.
- 리트리벌 및 메모리 연구/벤치마크AgentIR은 에이전트 "추론 토큰"을 신호로 사용하여("에이전트의 마음을 읽는") BrowseComp-Plus에서 기준선 대비 35% → 50% → 67%의 성능 향상을 보고합니다 (zijian42chen).Memex(RL)는 컨텍스트 윈도우를 부풀리지 않고 장기적인 작업을 확장하기 위해 인덱싱된 경험 메모리를 제안합니다 (omarsar0).Databricks/DAIR의 KARL: 엔터프라이즈 검색 에이전트를 위한 멀티태스크 RL 학습; 파레토 최적의 비용/레이턴시 품질 트레이드오프와 단일 벤치마크 최적화를 넘어선 개선된 일반화를 주장합니다 (dair_ai).
- "모든 것을 환경으로 전환": 한 해커톤 회고록은 환경이 "컴퓨팅 없이 지분을 얻을 수 있게" 해주기 때문에 AI를 민주화한다고 주장하며, 코딩 에이전트가 환경 구축을 지배하고 있지만 더 나은 스킬/명령이 필요하다고 말합니다 (ben_burtenshaw). Prime Intellect는 최소한의 설정으로 RL 환경 실행/학습을 위한 인프라 계층으로 반복적으로 포지셔닝됩니다 (willccbb).
- 문서 컨텍스트가 일반 프레임워크보다는 "심층 인프라"가 되고 있습니다.LlamaIndex는 LlamaParse → SurrealDB → MCP 에이전트 인터페이스를 사용하여 슬라이드 덱 파싱 및 리트리벌("Surreal Slides")을 보여줍니다 (llama_index, jerryjliu0). Jerry Liu는 광범위한 RAG 프레임워크에서 문서 OCR 인프라로의 전략적 전환을 지속적인 에이전트 병목 현상으로 명시적으로 제시합니다 (jerryjliu0).

---
로보틱스 및 체화된 AI: 휴머노이드 가정 데모에서 오픈소스 로봇 학습까지
- Figure Helix 02 자율 주택 청소: Brett Adcock은 완전히 자율적인 거실 청소 데모를 게시하고 이를 주요 이정표로 평가합니다 (adcock_brett, 후속 adcock_brett). Kimmonismus는 "2027년까지 가정용 로봇"을 예측합니다 (kimmonismus). 타임라인 추측은 차치하고, 이는 주목할 만한 데모 기준점입니다: 전신, 엔드투엔드 가사 작업.
- LeRobot v0.5.0: Hugging Face의 로보틱스 스택이 주요 업데이트를 출시했습니다: Unitree G1 휴머노이드 지원, 새로운 정책, 실시간 청킹, 더 빠른 데이터셋, EnvHub/Isaac 통합, Python 3.12 + Transformers v5, 플러그인 시스템 (LeRobotHF).
- 로보틱스 분야의 메모리 벤치마크: RoboMME가 로봇 제너럴리스트 정책의 메모리 벤치마크로 등장했습니다 (_akhaliq).

---
인기 트윗 (참여도 기준, 주로 기술/AI 관련)
- Claude Code가 멀티 에이전트 PR "Code Review"를 출시했습니다: @claudeai
- OSINT 파이프라인 게시물 (AI 지원 합성)이 엄청난 참여를 얻었습니다 (지정학적 내용이지만 AI 지원 방법론): @DataRepublican
- Karpathy: 오토리서치가 nanochat 학습을 약 11% 개선했습니다: @karpathy
- Google Earth: 위성 임베딩 데이터셋 업데이트 (AlphaEarth Foundations), 10m 픽셀당 64차원 임베딩: @googleearth
- Andrew Ng이 Context Hub를 출시했습니다 (코딩 에이전트를 위한 실시간 API 문서): @AndrewYNg
- OpenAI가 Promptfoo를 인수했습니다 (에이전틱 보안 테스트/평가; 오픈소스로 유지): @OpenAI

---

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-autoresearch-sparks-of-recursive&utm_source=paywall-free-trial&utm_medium=web&utm_content=190463886&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-autoresearch-sparks-of-recursive&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
