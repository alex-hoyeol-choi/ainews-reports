# It's Meta-Harness Summer

**원문 URL**: https://www.latent.space/p/ainews-its-meta-harness-summer
**번역일**: 2026-06-25 06:50
**발행일**: 2026-06-25

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 메타-하네스 여름이 왔습니다

### 하네스 엔지니어링은 비켜라, 이제 하네스 중의 하네스 시대입니다!
Share메타-하네스의 간략한 역사는 잘 문서화되어 있지 않지만, 대략적으로는 다음과 같습니다: 처음에는 Conductor와 Zed의 ACP가 있었고, 그 다음 OpenInspect, Cloudflare의 Flue, 그리고 Vercel의 Eve와 HarnessAgent, Heypi가 등장했습니다.
오늘 팟캐스트 게스트인 Matei Zaharia, 즉 (LLM 시대 이전 회사로서는) 엄청난 성공을 거둔 Databricks의 CTO가 현재 메타-하네스에 큰 기대를 걸고 있다는 점은 주목할 만합니다. 그가 주력하는 것은 Omnigent로, 모든 코딩 또는 지식 작업 에이전트를 표준화되고 안전하며 신뢰할 수 있고 확장 가능한 시스템으로 통합하기 위한 오픈소스 플러그형 아키텍처입니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/d1a3d909-a54b-4acd-aa2c-33823f9e032e_878x674.png)
omnigentOmnigent가 MCP의 성공을 필연적으로 만들었던 것과 같은 요소들을 가지고 있는지는 불분명합니다. 하지만 아키텍처적 관점에서 볼 때, 이와 유사한 오픈소스 아키텍처가 결국 승리할 것이라는 점은 분명합니다. 왜냐하면 현재 수많은 AI 네이티브 기업에서 독립적으로 재발견되고 있기 때문입니다.
> 2026년 6월 23일~24일 AI 뉴스입니다. 저희는 12개 서브레딧, 544개 트위터(X)를 확인했으며, 추가 디스코드는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
OpenAI의 Jalapeño 칩과 풀스택 AI 인프라를 향한 경쟁
- OpenAI, 하드웨어 분야 심화: OpenAI는 Broadcom과 협력하여 LLM 인퍼런스를 위한 첫 번째 맞춤형 AI 칩인 Jalapeño를 발표했습니다. 이 칩은 ChatGPT, Codex, API 트래픽 및 미래 에이전트 제품에 사용될 예정입니다. 전략적 메시지는 간단합니다. 칩, 커널, 메모리, 네트워킹, 스케줄링, 배포 등 스택의 더 많은 부분을 소유하여 컴퓨팅 경제성과 제품 동작이 상용 GPU 공급에 덜 의존하도록 하는 것입니다. @gdb는 강력한 와트당 성능을 강조했으며, @kimmonismus는 고성능 ASIC으로는 이례적으로 빠른 9개월의 설계-테이프아웃 주기를 언급했습니다. 이는 OpenAI 자체 모델에 의해 가속화된 것으로 알려졌습니다.
- 기술적 분석 및 생태계 영향: 커뮤니티의 역설계에 따르면 Jalapeño는 TPU와 유사한 것으로 보입니다. @scaling01은 거의 레티클 크기의 다이, 약 216GB HBM3E, ~7.1–7.4 TB/s 대역폭, 그리고 ~10 PFLOPS FP4를 추정했습니다. 이러한 수치가 비공식적이라 할지라도, 하이퍼스케일러 스타일의 인퍼런스 실리콘이 이제 프론티어 랩들에게는 필수적인 요소가 되었다는 신호입니다. 같은 날 컴파일러/런타임 환경도 재편되었습니다. Chris Lattner는 Qualcomm이 Modular를 인수한다고 발표했으며, Modular는 Mojo 오픈소스화가 순조롭게 진행 중이라고 밝혔습니다. 이러한 조합은 NVIDIA/CUDA를 넘어 수직 통합된 인퍼런스 스택을 둘러싼 더욱 심각한 경쟁을 예고합니다.
- 서빙 및 처리량은 여전히 활발한 전선: 인프라 측면에서 NVIDIA는 NeMo AutoModel이 Expert Parallelism, DeepEP, TransformerEngine 커널을 통해 MoE 모델의 학습 처리량을 3.4~3.7배 높인다고 밝혔습니다. SkyPilot은 자체 클러스터 전반에 걸쳐 통합 인퍼런스를 위한 Endpoints를 출시했으며, Modal은 오픈소스 인퍼런스 설정이 레이턴시 면에서 독점 제공업체를 능가한다고 주장했습니다. 로컬 최적화를 위해 @jon_durbin은 맞춤형 DFLASH 드래프트/투기 모델 학습을 통해 실제 디코딩 성능이 30~50% 향상되었다고 보고했습니다.
에이전트 UX가 "도구"에서 "동료"로 전환되며 새로운 보안 및 비용 문제 제기
- Anthropic의 Slack 네이티브 에이전트 모델이 주요 UI 이슈: 여러 트윗에서 Slack/팀 워크플로우에 통합된 Claude의 중요성에 대한 의견이 모였습니다. @karpathy는 사람들이 이를 "단순한 기능"이나 Slack 봇이 아니라 조직 수준의 하네스이기 때문에 과소평가하고 있다고 주장했습니다. @gallabytes는 Claude Code가 "페어링 파트너"에서 Tags가 "팀 관리"로 경험적 도약이 이루어졌다고 설명했습니다. @dabit3는 이 아이디어를 더 나아가, 궁극적으로는 에이전트를 명시적으로 태그할 필요조차 없을 수도 있다고 말했습니다.
- 어려운 부분은 ID, 권한, 그리고 락인(lock-in): Anthropic은 이 스레드에서 에이전트 ID 모델을 상세히 설명했습니다. Claude는 자체 자격 증명을 가지며, 모든 행동은 해당 ID로 감사 가능하고, 접근 권한은 중앙에서 철회될 수 있습니다. 이러한 설계는 칭찬과 우려를 동시에 받았습니다. @KentonVarda는 에이전트별 명시적 권한 부여는 확장성이 없다고 주장하며, 세분화되고 작업 범위가 지정된 접근 권한을 가진 역량 기반 보안을 옹호했습니다. @random_walker는 Claude Tag를 "모든 것을 기억하고 생각 단위로 청구하는 동료"로 규정하며, 공유 에이전트가 조직 워크플로우에 깊이 통합되면 암묵적 지식 락인, 프롬프트 인젝션 위험, 예산 불투명성 등의 위험이 있다고 경고했습니다. @JubbaOnJeans도 유사하게 쓰기 작업에 대한 귀속 모호성과 깔끔한 Slack과 같은 경계를 벗어난 미래의 접근 제어 복잡성을 지적했습니다.
- 오픈/DIY 방식의 즉각적인 대응: Hugging Face는 블로그 트윗에서 자체 Slack 기반 코딩 에이전트인 Moon Bot을 설명하며, 셀프 호스팅, 맞춤형 도구, 감사 가능한 세션, 그리고 제로 락인(lock-in)을 강조했습니다. @calebfahlgren의 후속 트윗은 GitHub, Athena, analytics, MongoDB, Elasticsearch, HF Buckets를 아우르는 프로덕션 통합 사례를 나열했습니다. 더 큰 패턴은 다음과 같습니다. 팀들은 에이전트 네이티브 UX를 점점 더 원하지만, 많은 팀은 조직 지능을 벤더에게 아웃소싱하기보다는 하네스와 메모리 레이어를 직접 소유하기를 선호합니다.
Qwen-AgentWorld, OpenThoughts-Agent, 그리고 다음 에이전트 스케일링 축으로서의 메모리
- Qwen-AgentWorld, 에이전트를 위한 "언어 세계 모델" 추진: Alibaba Qwen은 Qwen-AgentWorld를 소개하며, 이를 단일 모델 내에서 7가지 환경(MCP, Search, Terminal, SWE, Web, OS, Android)을 시뮬레이션하는 네이티브 언어 세계 모델로 포지셔닝했습니다. Qwen은 두 가지 경로를 주장합니다. 시뮬레이터 자체를 구축하고, 세계 모델링을 에이전트 사전 학습으로 사용하는 것입니다. 그들은 Qwen-AgentWorld-35B-A3B와 AgentWorldBench를 오픈소스화했으며, 35B MoE / 3B 활성, 256K 컨텍스트 모델을 제공합니다. 한 가지 주목할 만한 결과는 이 후속 요약에서처럼 단일 턴 환경 예측이 인-도메인 및 아웃-오브-도메인 벤치마크 모두에서 이득을 얻으며 다중 턴 에이전트 작업으로 전이된다는 것입니다.
- OpenThoughts-Agent, 진지한 오픈 데이터 레시피 기여: @iScienceLuvr와 @RichardZ412는 100개 이상의 제어된 어블레이션(ablation)을 가진 에이전틱 모델을 위한 오픈 큐레이션/학습 파이프라인인 OpenThoughts-Agent를 강조했습니다. 이 팀은 100K 예제 학습 세트를 구축하고 Qwen3-32B를 파인튜닝하여 7가지 에이전틱 벤치마크에서 평균 44.8%의 정확도를 달성했습니다. 핵심 발견 사항은 실무자들에게 유용합니다. 명령어 선택이 불균형적으로 중요하고, 가장 강력한 벤치마크 티처가 최고의 티처는 아니며, 더 긴 실행 트레이스가 도움이 되고, 규모에서 소스 다양성이 과도한 반복보다 낫다는 것입니다.
- 메모리가 일급 시스템 레이어로 전환 중: 많은 중요한 논의가 에이전트에서 미해결 문제인 메모리에 집중되었습니다. Weaviate의 Engram GA는 모든 것을 컨텍스트에 덤핑하는 대신, 메모리를 추출, 중복 제거, 조정 및 범위 지정하는 비동기 인프라로 정의합니다. @hwchase17은 트레이스가 오프라인으로 분석되어 메모리로 다시 기록되는 "슬립 타임 컴퓨트"를 위한 LangSmith/Context Hub 워크플로우를 보여주었습니다. @dair_ai는 에이전트 메모리가 최종 작업 성공으로만 판단되는 블랙박스가 아니라, 저장, 리트리벌, 업데이트, 통합, 라이프사이클 등 완전한 데이터 관리 레이어로 평가되어야 한다고 주장하는 논문을 지적했습니다. 에이전트 차별화는 점점 이 방향으로 나아가고 있는 것으로 보입니다.
중국 오픈 모델, 격차 계속 좁혀: GLM-5.2, Kimi 배포, 그리고 컴퓨팅 스케일
- GLM-5.2, 오픈 모델 논의 계속 지배: 여러 트윗에서 GLM-5.2를 현재 가장 강력한 오픈 웨이트 경쟁자로 평가했습니다. CoreWeave는 Artificial Analysis와 Agent Arena의 오픈 모델 순위에서 GLM-5.2가 1위를 차지했다고 밝혔으며, Baseten과 Cursor의 가용성은 빠른 서빙/배포 채택을 보여주었습니다. @nutlope는 웹 작업에서 GLM 5.2를 Opus 4.8과 비교하여 유사한 품질, 약 2배의 토큰 출력, 하지만 여전히 더 빠르고 약 3배 저렴하다고 보고했습니다. Arena는 또한 GLM-5.2 Max가 강력한 경쟁자들 사이에서 Code Arena: Frontend를 선도한다고 말했습니다.
- 벤치마크의 미묘한 차이 중요: GLM-5.2는 ARC-AGI-2에서도 등장했습니다. @fchollet은 이를 오픈소스 모델 중 현재까지 가장 강력한 ARC-AGI-2 결과라고 평가했으며, 다른 이들은 22.8%라는 수치가 서구 프론티어 모델과 비교하여 실제로 무엇을 의미하는지 논의했습니다. 더 넓은 의미의 시사점은 특정 벤치마크 하나보다는, 중국의 오픈 모델들이 코딩, 에이전트, 지식 작업 전반에서 꾸준히 "경쟁에 참여하고 있다"는 것입니다.
- 상업화 및 인프라 가속화: Moonshot의 Kimi API는 이제 AWS Marketplace에서 제공되어, 통합 청구 및 EDP 인출을 통해 기업 조달을 용이하게 합니다. 한편, 중국 국내 컴퓨팅은 여전히 주요 테마입니다. @teortaxesTex는 Huawei가 950 SuperPOD 스케일 시스템을 시연할 수 있다는 보고서를 지적했으며, 이는 상당한 규모의 대규모 국내 NPU 클러스터 생산을 의미합니다. 만약 사실이라면, 이는 중국 모델 서빙 생태계의 경제성과 회복력을 실질적으로 향상시킬 것입니다.
정책, 인재, 그리고 프론티어 랩 전략이 경쟁 환경을 재편하고 있습니다
- Anthropic, 정책 분쟁의 중심에 남아: @kimmonismus는 트럼프 시대 AI 수출 통제에 대한 첫 번째 주요 법적 도전을 보고했습니다. Legion은 호스팅된 모델 접근이 가중치나 기술 데이터 수출과 동일하지 않다고 주장했습니다. 이와 병행하여, 많은 논의가 있었던 Mythos 이야기는 맥락을 얻었습니다. 여기에 요약된 Reuters/AP 세부 정보는 Anthropic의 모델이 제한된 테스트 과정에서 민감한 미국 시스템의 취약점을 발견했음을 시사하지만, 일부 논평가들은 이전 보도가 과장되었다고 경고했습니다.
- 디스틸레이션 및 접근 제어가 지정학적 문제로 부상: @kimmonismus는 또한 Anthropic이 Alibaba와 연계된 운영자들이 약 25,000개의 사기 계정과 2,880만 건의 Claude 교환을 사용하여 프론티어 역량을 Qwen급 시스템으로 디스틸레이션했다고 비난했다고 보고했습니다. 만약 사실이라면, 이는 "적대적 디스틸레이션" 논쟁을 소문에서 집행 및 국가 전략에 더 가까운 수준으로 격상시킬 것입니다.
- 인재 및 신규 랩: 이날은 또한 인재 이동과 새로운 기관 설립 소식도 전해졌습니다. Arthur Conmy가 Anthropic에 합류한 것은 정렬(alignment) 측면에서 주목할 만합니다. Mirendil AI는 2억 달러의 시드 라운드와 과학을 위한 자체 가속 AI R&D에 대한 논문으로 출범했습니다. 영국에서는 BOLD Lab과 SOFAIR가 두 개의 새로운 국립 기초 AI 랩에 총 6천만 파운드의 시드 펀딩을 받았으며, UCL DARK는 BOLD에 합병되었습니다. 그리고 상업적 측면에서는 Bloomberg가 보도한 Google DeepMind에서 Anthropic으로의 이탈은 스타트업의 잠재력이 프론티어 인재를 계속해서 끌어들이고 있음을 강조합니다.
인기 트윗 (참여도 기준)
- OpenAI Jalapeño: OpenAI가 첫 번째 맞춤형 인퍼런스 칩을 발표했습니다. 이는 이번 뉴스에서 가장 중요한 제품/인프라 출시입니다.
- GPT-5.5 Instant 업데이트: OpenAI가 의도 이해, 제약 조건 처리, 대화 스타일이 개선된 GPT-5.5 Instant 개정판을 출시했습니다.
- Qwen-AgentWorld: Alibaba Qwen이 에이전트를 위한 언어 세계 모델을 출시하고 오픈소스화했습니다.
- Anthropic의 에이전트 ID 모델: Slack의 Claude가 이제 자체 자격 증명과 감사 추적을 사용하여, 가장 까다로운 엔터프라이즈 에이전트 설계 문제 중 하나를 명확히 했습니다.
- Cursor x Notion: Cursor 작업이 이제 Notion에서 직접 위임될 수 있습니다. 이는 에이전트 워크플로우가 독립형 채팅 앱에 머무르기보다는 기존 팀 소프트웨어로 이동하고 있다는 또 다른 신호입니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-its-meta-harness-summer&utm_source=paywall-free-trial&utm_medium=web&utm_content=203490377&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-its-meta-harness-summer&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
