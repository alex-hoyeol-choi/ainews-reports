# not much happened today

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-f5c
**번역일**: 2026-07-11 06:54
**발행일**: 2026-07-11

---

[AINews: 주중 요약](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 오늘은 별일 없었습니다

### 끊임없는 모델 출시가 이어진 한 주 후의 조용한 하루
Share춤추는 벌레들이 K팝 걸그룹에 밀려 빛을 잃었고, Bun 대 Zig 드라마가 있었으며, 어제의 ChatGPT/Codex 슈퍼앱 출시는 예상보다 매끄럽지 않았고, 이를 보완하기 위해 리셋 버튼이 몇 차례 눌렸습니다.
Statsig를 인수한 후 GPT-5의 라우팅/모델 피커 제거를 크게 다룬 후, 현재 주요 문제는 GPT-5.6의 추가 옵션들이 사람들을 다소 혼란스럽게 한다는 것입니다. 대부분의 사람들은 단일 슬라이더만 가지고 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/780723c6-1158-4a6b-a957-490705fdba08_420x274.png)
하지만 API 사용자들은 현재 말 그대로 36가지의 GPT-5.6 변형을 가지고 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/a462b771-b4e5-4d7a-b815-ac4ca35903f4_1328x982.png)
대부분의 사람들은 대략 3가지 클러스터로 충분히 사용할 수 있습니다

![X avatar for @jumperz](https://pbs.substack.com/profile_images/2066609443194773504/sSlzoKn2.jpg)
그리고 많은 가이드가 나오고 있습니다:

![X avatar for @rasbt](https://pbs.substack.com/profile_images/1661187442043486209/a3E4t1eV.jpg)
이번 주 최고의 AIE 강연은 Theo의 클로징 기조연설이었으며, 온라인 트랙의 마지막 부분은 이번 주말에 공개될 예정입니다.
> 2026년 7월 9일~7월 10일 AI 뉴스입니다. 저희는 12개의 서브레딧과 544개의 트위터 계정을 확인했습니다. AINews 웹사이트에서 지난 모든 호를 검색할 수 있습니다. 참고로 AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
OpenAI의 GPT-5.6 출시: 모델 계층화, 에이전트 UX, 초기 벤치마크 신호
- GPT-5.6은 더 명확한 모델/컴퓨트 계층을 도입했습니다: 사용자들은 이제 Luna / Terra / Sol과 여러 노력 수준을 탐색하고 있으며, 커뮤니티 가이드라인은 “5.5 버전에서 했던 것보다 낮은 수준에서 시작하라”는 방향으로 수렴하고 있습니다. OpenAI 직원들은 Max가 하나의 모델이 어려운 문제에 더 오래 시간을 할애하는 것을 의미하고, Ultra는 서브에이전트 간에 작업을 병렬화한다고 설명했습니다. 또한 5.5→5.6 노력 설정은 직접 비교할 수 없다고 언급했습니다 (@reach_vb의 가이드라인, 후속 조치, 실용적인 기본 설정 제안). 커뮤니티 반응은 엇갈렸습니다: 많은 사람들이 추가된 제어 기능을 칭찬했지만, 다른 이들은 30개 이상의 구성 조합론과 “자동” 라우팅의 부재를 비판했습니다 (@rasbt, @Yuchenj_UW).
- 제품 출시는 실제 UX 회귀를 동반했으며, OpenAI는 공개적으로 빠르게 방향을 수정했습니다: 사용자들은 새로운 ChatGPT Work / Codex 분할이 혼란스럽고, 채팅/프로젝트를 찾기 어려워졌으며, 사용량이 예상보다 빠르게 소진되었다고 불평했습니다 (@scaling01, @simonw, @kimmonismus). OpenAI는 이례적으로 직접적으로 대응했습니다: 여러 차례 사용량 제한 초기화, 기본 설정이 사용자들을 과도하게 비싼 설정으로 유도했음을 인정, 그리고 익숙한 사이드바/탐색 패턴을 복원하고 Work와 Codex 간의 포지셔닝을 명확히 하겠다는 약속을 했습니다 (@thsottiaux 리셋 발표, 두 번째 리셋, 전체 수정 로드맵).
- 초기 평가 현황: GPT-5.6은 에이전틱 코딩 / 프레젠테이션 / 일부 과학 작업에서 가장 강력해 보이지만, 모든 곳에서 명확하게 지배적이지는 않습니다. 예시: Code Arena: Frontend에서 Claude Fable 5와 함께 1위 동점을 기록했으며, 명시된 IO 가격에서 약 2배 저렴합니다 (Arena); AA-Briefcase에서 기록된 최고의 프레젠테이션 Elo는 GPT-5.5보다 약 500점 상승했습니다 (Artificial Analysis); CritPt에서 GPT-5.5보다 향상되었고 Fable 5를 약 4점 차이로 이겼습니다 (Artificial Analysis); 그리고 더 낮은 비용으로 WeirdML에서 강력한 결과를 보였습니다 (@htihle). 동시에 사용자들은 지시 따르기 문제, 실제 토큰 효율성 불균형, 그리고 탈옥 가능성 / 보상 해킹에 대한 일부 우려를 보고했습니다 (@teortaxesTex, @Mononofu, @kimmonismus).
병렬 에이전트 워크플로우, 컴퓨터 사용, 그리고 “하네스가 제품이다”라는 주제
- GPT-5.6의 가장 큰 인지된 도약은 순수한 채팅 품질보다는 오케스트레이션과 컴퓨터 사용일 수 있습니다. 여러 사용자들은 Sol이 플래너 / 검증자 / 오케스트레이터로서 이례적으로 강력하며, 종종 서브에이전트를 자동으로 사용하고 스티어링에 더 빠르게 반응한다고 강조했습니다 (@omarsar0, @Hangsiin). OpenAI는 또한 Sol Ultra를 사용한 컴퓨터 사용을 선보였고, ChatGPT Work를 에이전트를 소비자/모바일 규모로 가져오는 것으로 홍보했습니다 (OpenAI 데모 via @gdb, Work 포지셔닝). 커뮤니티 보고서는 매우 높은 처리량의 GUI 자동화 및 Blender 워크플로우를 설명했습니다 (@mckbrando, @kimmonismus).
- 반복되는 운영 문제는 숨겨진 서브에이전트 비용 폭증입니다: 사용자들은 스폰된 에이전트가 프리미엄 설정을 상속받을 수 있어 예상보다 훨씬 빠르게 할당량을 소진한다는 것을 발견했습니다. 한 가지 구체적인 주장은 `spawn_agent`가 사용자가 모델/노력을 선택할 수 없게 하여, Sol Ultra가 기본적으로 더 많은 Sol Ultra를 스폰한다는 것이었습니다 (@evi77ain). 이는 역량 향상은 좋아하지만 비용 모델이 불투명하다고 생각하는 더 넓은 패턴에 부합합니다.
- 더 넓은 시스템 트렌드는 하네스 중심 경쟁으로 향하고 있습니다. 이는 Perplexity의 Arav Srinivas의 제품 논평 (“진정한 제품은 이제 그 주변의 하네스입니다”), Deep Agents + Nemotron + OpenShell을 중심으로 한 LangChain의 출시 프레이밍, 그리고 OpenWiki 및 OpenSWE와 같은 증가하는 메모리/오케스트레이션 도구 세트에서 드러났습니다 (@dee_bosa가 Arav 인용, @hwchase17, OpenWiki 선제적 메모리, OpenSWE 채택). 핵심 요점은 프론티어 모델 패리티가 강화되고 있으므로, 가치는 점점 더 라우팅, 메모리, 도구 사용, 안전 장치, 엔터프라이즈 컨텍스트로 이동하고 있다는 것입니다.
Meta의 Muse Spark 1.1과 “충분히 좋고, 빠르고, 저렴한” 모델의 넓어지는 프론티어
- Muse Spark 1.1은 그날의 다른 주요 모델 소식이었으며, 많은 실무자들이 이번 주 가장 놀라운 출시라고 불렀습니다. 보고서는 일관되게 강력한 UI/프론트엔드 생성, 빠른 응답, 그리고 이례적으로 공격적인 가격 책정을 강조했으며, 종종 코딩/제품 작업의 상당 부분에서 프론티어에 가까운 품질로 평가했습니다 (@alexandr_wang, @rowancheung, @kimmonismus).
- 벤치마킹은 실제적인 발전이 있음을 시사하지만, 전면적인 프론티어 리더십은 아닙니다. Artificial Analysis는 Muse Spark 1.1에 Intelligence Index에서 51점을 부여했으며, 1.0 버전보다 8점 상승하여 GLM-5.2 / GPT-5.4 / GPT-5.6 Luna와 대략 동점이고 Grok 4.5 / GPT-5.6 Sol / Claude Fable 5에 뒤처집니다. 주목할 만한 세부 사항: 1M 컨텍스트, 중간 속도 약 114 tok/s, 1M 입력/출력 토큰당 $1.25 / $4.25의 가격, 그리고 강력한 토큰 효율성 (Artificial Analysis). Arena는 또한 Code Arena: Frontend에서 9위에 올랐으며, 지시 따르기 및 긴 쿼리 카테고리에서 강력한 향상을 보였습니다 (Arena).
- 많은 사람들이 도출한 전략적 함의는 Meta의 컴퓨트 중심 투자가 단순히 인재 헤드라인만이 아니라 비용 효율적인 인퍼런스 제품으로 나타나기 시작했다는 것입니다. 여러 논평가들은 이것이 OpenAI/Anthropic에 대한 경쟁 압력을 실질적으로 높인다고 주장했으며, 특히 Meta가 배포 및 API 사용성을 개선한다면 더욱 그렇다고 했습니다 (@scaling01이 OpenRouter를 요청, @alexandr_wang, @mweinbach).
오픈 모델, 인프라, 효율성 작업
- 클로즈드 모델에 대한 관심 공백에도 불구하고 오픈 모델 툴링은 계속 출시되었습니다. Unsloth는 Qwen3.6 NVFP4 퀀트를 출시했으며, 2.5배 빠른 인퍼런스를 주장했습니다. 여기에는 24GB VRAM에서 27B 모델과 B200에서 17,561 tok/s를 기록한 35B-A3B 변형이 포함됩니다 (Unsloth, @danielhanchen의 기술 세부 정보). QuixiAI는 듀얼 B60에서 65 tok/s 및 128k 컨텍스트로 Qwen3.6-35B-A3B-NVFP4를 보고했습니다 (QuixiAI).
- 인퍼런스 최적화는 여전히 주요 활발한 연구 분야입니다. Cohere는 vLLM에서 하드웨어 인식 동적 스페큘레이티브 디코딩을 오픈소스화하여, 스페큘레이티브 디코딩이 낮은 배치 사이즈에서는 도움이 되지만 높은 배치 사이즈에서는 해가 되는 익숙한 문제를 해결했습니다 (Cohere/vLLM, vLLM 논평). Google/Hugging Face의 Gemma 챌린지는 단일 A10G 인퍼런스에서 최대 5배 빠른 속도를 보고했으며, 315 TPS 무손실 및 491.8 TPS로 전체에서 가장 빨랐습니다 (Gemma).
- 에이전트 평가/자기 개선 작업이 더욱 구체화되고 있습니다: “LLM-as-a-Verifier”는 반복 샘플링과 점수-로그확률 랭킹을 사용하여 Terminal-Bench V2, SWE-Bench Verified, RoboRewardBench, MedAgentBench에서 SOTA를 보고했습니다 (논문 스레드); Meta 연구원들은 장기 에이전트의 행동 상태 저하를 방지하기 위해 명시적 메모리 에이전트를 제안했습니다 (요약).
과학, 수학, 건강, 모달리티별 시스템
- 수학/과학 역량 주장이 급격히 증가했습니다. OpenAI 직원과 커뮤니티 멤버들은 GPT-5.6 Sol Ultra가 1시간 이내에 64개의 서브에이전트를 사용하여 Cycle Double Cover Conjecture에 대한 주장된 증명을 생성한 사례를 유포했습니다 (@eknight의 주장, @gdb에 의해 확산). 별도로 Bubeck은 GPT-5.6을 사용한 100만 줄의 Lean 형식화 노력을 언급했습니다 (@SebastienBubeck). 이들은 여전히 외부 검토를 기다리는 주장이지만, 연구소들이 내러티브를 어디로 이끌고 싶어 하는지 보여줍니다: 과학 컴퓨트 프리미티브로서 병렬화된 연구 에이전트.
- 건강은 일류 벤치마크이자 제품 버티컬이 되고 있습니다. OpenAI는 GPT-5.6이 헬스 인텔리전스에 있어 큰 진전이라고 말했으며, 가장 낮은 노력 수준의 Luna가 가장 높은 노력 수준의 GPT-5.5를 능가하면서 25배 적은 비용이 든다는 점을 강조했습니다 (OpenAI). Karan Singhal은 20,000개 이상의 축 평가에 대한 블라인드 의사 비교에서, 의사들이 어려운 작업 세트 전반에 걸쳐 의사가 작성한 응답보다 GPT-5.6 응답에서 더 적은 결함을 발견했다고 덧붙였습니다 (세부 정보).
- 오디오/음악 및 창작 툴링도 움직였습니다: Kyutai + Mirelo는 스템이 아닌 풀 믹스에서 다중 악기 오디오-MIDI 전사를 위한 오픈 모델인 MuScriptor를 출시했습니다 (MireloAI, Kyutai). Sakana의 새로운 Picbreeder 스타일 작업은 VLM 에이전트를 사용한 개방형 창의성을 탐구했으며, 다양한 에이전트 집단이 도움이 되지만 여전히 인간의 개방형 탐색에는 미치지 못한다고 결론 내렸습니다 (Sakana).
보안, 안전성, 정책 마찰
- 역량 향상과 함께 보안 우려가 증가했습니다. OpenAI는 바이오 버그 바운티를 비공개 상시 프로그램으로 전환하고 보상을 $50K로 두 배 늘렸으며, 특히 사전 정의된 생체 안전성 과제에 대한 범용 탈옥을 찾고 있습니다 (OpenAI). 별도로 OpenAI는 가장 사이버 역량이 뛰어난 모델에 대한 접근 요구 사항을 강화하여, 9월 1일부터 사이버 멤버를 위한 신뢰할 수 있는 접근에 하드웨어 보안 키를 요구합니다 (@cryps1s).
- 오용 증거는 여전히 두드러집니다: 새로운 연구는 보코하람 구성원들이 폭탄 제조 및 관련 전술적 질의에 프론티어 챗봇을 사용했다고 보고했습니다 (@AntoniaJuelich). 이 스레드는 GPT-5.6이 일부 설정에서 비교적 쉽게 탈옥되거나 보상 해킹될 수 있다는 진행 중인 온라인 토론 옆에 불편하게 놓여 있었습니다 (@Mononofu).
- 정책 담론은 여전히 양극화되어 있고 추측성입니다. “AI 2040 / Plan A” 투명성 및 거버넌스 시나리오는 지지와 조롱을 모두 받았으며, Ajeya Cotra는 전체 연구 투명성의 중요성을 강조한 반면 비평가들은 실현 가능성과 초지능/거버넌스 역량에 대한 가정에 의문을 제기했습니다 (@ajeya_cotra, @binarybits, @banteg satire).
(참여도 기준) 인기 트윗
- OpenAI 출시 및 롤백 관리: OpenAI의 제품 책임자는 출시 혼란을 인정하고, UI 수정을 약속했으며, 사용량을 두 번 초기화하면서 Codex가 계속 유지될 것임을 명확히 했습니다 (전체 스레드).
- Claude Code 데스크톱 브라우저: Anthropic은 Claude Code 데스크톱용 인앱 브라우저를 출시하여 Claude가 앱 내에서 문서/사이트를 탐색할 수 있도록 했습니다 (@ClaudeDevs).
- OpenAI 조직 업데이트: Fidji Simo는 OpenAI의 풀타임 역할에서 물러나 파트타임 고문이 된다고 발표했으며, 만성 질환 회복에 집중해야 할 필요성을 언급하면서 AI 및 건강 관련 작업을 계속할 것이라고 밝혔습니다 (@fidjissimo).
- Perplexity 하네스 확장: Perplexity는 내부 평가에서 Grok 4.5가 Opus 4.8 비용의 대략 절반으로 강력한 WANDR 성능을 보인 후 Computer에 Grok 4.5를 오케스트레이터로 추가했습니다 (Perplexity).

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. GLM-5.2 로컬 인퍼런스 및 보안 검토

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 무료 액세스를 받으세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-not-much-happened-today-f5c&utm_source=paywall-free-trial&utm_medium=web&utm_content=206529076&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-not-much-happened-today-f5c&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
