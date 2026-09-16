# Jev: a “System One Model” that only decides/classifies/routes/scores — >100x faster, >200x cheaper than small frontier LLMs

**원문 URL**: https://www.latent.space/p/ainews-jev-a-system-one-model-that
**번역일**: 2026-09-16 13:00
**발행일**: 2026-09-16

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Jev: 결정/분류/라우팅/점수 매기기만 하는 "System One Model" — 소규모 프론티어 LLM보다 100배 이상 빠르고, 200배 이상 저렴합니다

### TypeSafe에 축하를 보냅니다!
Sep 16, 2026ShareAIEi Paris (Sep 23-24)와 AIE NYC (Oct 12-14)는 50% 이상 매진되었으며, AIE CODE (Nov 10-12 in SF)와 AIEi Shanghai (Nov 5-6)가 다음으로 예정되어 있고, AIEi Sydney (Dec 7-8 alongside NeurIPS)가 올해를 마무리합니다!

---
새로운 스타트업 출시가 헤드라인을 장식하는 일은 매우 드뭅니다. 특히 Gemini 3.8 Live와 Periodic Labs가 강력한 발표를 한 날에도 TypeSafe의 출시는 하루 종일 Hacker News 상위권을 편안하게 차지했습니다. 저희는 지난달 AIE 사전 출시 행사에서 이들을 미리 볼 수 있는 행운을 누렸습니다.
그리고 이제 그들의 발표(블로그, evals, docs)는 수백만 건의 조회수를 기록했습니다.

![X avatar for @CompleteSkeptic](https://pbs.substack.com/profile_images/1650708125685800960/7k6r0UZg.jpg)
기존의 오토리그레시브 LLM에 익숙한 분들에게는 코딩을 할 수 없고 추론하지 못하는 빠른 모델이 그 유용성 면에서 직관에 반하는 것처럼 느껴질 수 있습니다. 이는 팀이 "System Two"의 느린 LLM을 보완하기 위해 정확히 목표로 하는 바입니다. 문자열과 채팅을 포기하면 얻을 수 있는 것은 1) 병렬 샘플링, 2) "환각 없음", 3) 캘리브레이션입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/dafca494-4f36-4a32-864a-2fb74357afe7_2150x1690.png)
이 시스템은 "RLCD" - 캘리브레이션된 결정 -을 통해 학습되었습니다. 이는 HuggingFace의 Clementine이 저희 팟캐스트에서 중요한 연구 프론티어 중 하나로 강조했던 주제입니다.

![Benchmarks 201: Why Leaderboards > Arenas >> LLM-as-Judge](https://substack-video.s3.amazonaws.com/video_upload/post/146497374/5c7f4777-d4e7-4800-b146-38eb15e856ec/transcoded-1721059050.png)

![](https://substack-post-media.s3.amazonaws.com/public/images/41fc9b4b-4ba5-4f2e-b4e4-fe8e6d0475b6_1414x1028.png)
> 2026년 9월 14일-9월 15일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터를 확인했으며, 추가 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter Recap
Periodic Labs의 Neon: 재료 과학을 위한 실험실 기반 RL
- Neon의 핵심 결과: 이번 소식 중 가장 큰 기술적 이야기는 Liam Fedus를 통해 발표된 Periodic Labs의 Neon입니다. 이 모델은 고처리량 물리 실험실과 ML 간의 긴밀한 루프에서 학습되었으며, 초전도체, 자석, 반도체와 같은 재료 과학 문제에 우선적으로 초점을 맞추었습니다. Periodic은 1,300개의 H200, 수개월간의 독점적인 실험 데이터, 중간 학습 및 RL, 그리고 오픈소스 기반 모델을 사용하여 분석 벤치마크에서 GPT-6 Astra를 능가했다고 밝혔습니다. 후속 게시물들은 유용한 세부 정보를 추가합니다. @periodiclabs는 모델 개선에 지속적으로 실험을 실행하는 것을 설명합니다. @DBahdanau는 팀이 1조(trillion) 개의 파라미터를 가진 XRD 분석 전문가를 학습시켰다고 말합니다. @khoomeik는 이를 실험 데이터 분석을 위한 1조 파라미터 모델로, 해당 작업에서 Astra와 Fable을 능가한다고 설명합니다.
- 기술적으로 중요한 이유: 몇몇 반응들은 동일한 논지로 수렴합니다. 도메인별 데이터와 RL 인프라가 좁지만 가치 있는 과학적 작업에서 프론티어 일반 모델을 능가할 수 있다는 것입니다. @zephyr_z9는 Periodic이 Kimi 2.5/K2.x 기반 모델을 Astra를 넘어설 정도로 발전시켰다고 강조합니다. @_jasonwei는 이는 과학의 프론티어 근처에서 전문화된 사설 데이터가 점점 더 결정적인 역할을 한다는 증거라고 언급합니다. @vwxyzjn은 특이한 부분을 강조합니다. 물리 실험실의 실제 실험 데이터에 대한 RL, 맞춤형 인프라 및 샌드박스 시스템입니다. @zijie_y는 긴 과학적 추적(trace)이 메모리와 병렬 처리에 충분한 부담을 주어 Neon 학습에 긴 컨텍스트 학습 효율성 분야의 프론티어 작업이 필요했다고 덧붙입니다. @brianzhan1의 보다 완전한 커뮤니티 요약에 따르면, Neon은 Kimi K2.6에서 시작하여 내부 FrontierXRD 평가에서 성공률을 2.7%에서 55.3%로 끌어올렸으며, Astra와 Claude Fable 5.1을 더 낮은 인퍼런스 비용으로 능가한다고 주장합니다.
- 시사점: 이는 논문 벤치마크를 넘어선 "과학을 위한 AI"의 구체적인 템플릿처럼 보입니다. 독점 데이터를 생산하는 수직 통합 실험실, 과학자가 캘리브레이션한 보상에 따라 학습된 모델, 그리고 다시 실험으로의 배포입니다. 가장 강력한 메타 관찰은 @richardczl로부터 나왔습니다. 의미 있는 데이터 해자를 가진 모든 회사가 이 전략을 시도할 가능성이 높으며, 병목 현상이 RL 롤아웃 처리량, 검증자 컴퓨팅, 가중치 동기화 쪽으로 이동할 것이라고 말했습니다.
Gemini 3.8 Live와 실시간 음성 에이전트를 향한 추진
- Google의 새로운 라이브 오디오 모델: Google은 Gemini 3.8 Live와 3.8 Live Extended Thinking을 출시했습니다. 이 모델들은 대화 흐름을 끊지 않고 말하고, 생각하고, 백그라운드에서 작업을 처리할 수 있는 대화형 모델로 포지셔닝되었습니다. @GoogleAIStudio의 개발자 대상 출시와 @_philschmid의 요약은 주요 제품 세부 정보를 추가합니다. 97개 언어 지원, 말하는 동안 비동기 도구 호출, Gemini API / AI Studio를 통한 사용 가능성, 그리고 LiveKit, Pipecat, LangChain, Vercel을 통한 파트너 지원입니다.
- 벤치마크 및 경제성: Artificial Analysis가 가장 기술적인 외부 분석을 제공합니다. Gemini 3.8 Live Extended Thinking (High)은 음성-음성 인덱스에서 82.6점으로 1위(GPT-Live-1 Astra 81.5점보다 앞서), Tau Voice에서 68.6%로 1위를 차지했습니다. 표준 Live 모델은 더 저렴하고 빠르지만, 에이전틱 음성 작업에서는 훨씬 약합니다. 가격 책정 면에서, 표준 3.8 Live는 시간당 입력 오디오 $0.84로 보고되었으며, Extended Thinking High는 시간당 $3.50로, 여전히 여러 경쟁 라이브 모델보다 낮습니다. 이는 Google이 품질뿐만 아니라 프로덕션 음성 에이전트의 배포 가능성까지 최적화하고 있다는 주제를 강화합니다.
TypeSafe의 Jev와 RLCD: 텍스트 생성기 대신 결정 모델
- 새로운 모델 카테고리, 또는 최소한 새로운 패키징: 가장 높은 참여도를 보인 기술 출시 중 하나는 Diogo Almeida/TypeSafe의 Jev 발표였습니다. 이 모델은 RLCD로 학습되고 텍스트 생성이 아닌 결정에 최적화된 새로운 프론티어 모델을 주장합니다. 20-200배 빠르고, 40-400배 저렴하며, 출력 토큰은 무료입니다. @omarsar0, @chaseleantj, @Yuchenj_UW의 반응은 모두 동일한 유력한 사용 사례에 집중합니다. 오토리그레시브 생성이 불필요한 오버헤드인 프로덕션 시스템에서 LLM을 구조화된 분류기/판단기/라우팅 정책으로 대체하는 것입니다.
- 중요한 주의사항: 일부 커뮤니티 게시물은 과도한 일반화에 대해 올바르게 반박합니다. @scaling01은 Jev는 일반적인 언어 모델이 아니며, 제약이 있거나 확산 모델과 유사한 결정 모델에 더 가깝다고 언급합니다. 자유 형식 텍스트를 생성할 수 없으며 미리 정의된 출력 형식을 요구합니다. 이는 올바른 사고방식을 "GPT 대체"보다는 "구조화된 선택을 위한 저렴하고 캘리브레이션된 인퍼런스 엔진"에 가깝게 만듭니다. 여러 엔지니어가 제시한 가장 그럴듯한 연결은 DSPy 스타일의 시그니처 및 타입 지정 예측 추상화(예: @eggie5 및 @dbreunig)이며, 이는 값비싼 LLM 호출이 더 작고 작업별 AI 함수로 컴파일되는 미래 스택을 시사합니다.
에이전트, 툴링 및 인프라: Mac VM, MCP, Bash, 그리고 AI가 구축한 시스템
- 에이전트 실행 환경이 더욱 완벽해지고 있습니다: @jeffwang은 Devin이 이제 Mac VM을 실행할 수 있어 Slack 또는 웹 UI에서 종단 간 iOS 개발 및 디버깅이 가능하다고 말합니다. @jkelleyrtp는 Devin이 이제 macOS, Windows, Linux를 아우르는 클라우드 에이전트이며, 저장소, 네트워킹, VNC 및 Rust로 재구축된 컴퓨터 사용 인프라를 갖추고 있다고 덧붙입니다. 이는 의미 있는 플랫폼 발전입니다. 컴퓨터 사용 에이전트는 에뮬레이션이나 브라우저 전용 샌드박스 대신 네이티브 대상 OS 내에서 작동할 수 있을 때 훨씬 더 실용적이 됩니다.
- MCP는 통합 계층으로서 계속해서 통합되고 있습니다: LangChain은 모든 Managed Deep Agent가 이제 호환 가능한 클라이언트를 통한 위임 및 도구 재사용을 위한 내장 엔드포인트를 갖춘 MCP 서버라고 발표했습니다. @LangChain. @omarsar0의 커뮤니티 정서는 단호합니다. 맞춤형 하네스(harness)의 경우, 대부분의 통합에서 MCP가 CLI보다 낫습니다.
- 도구 대 bash: @dair_ai의 주목할 만한 Microsoft 논문 요약은 에이전트 벤치마크에서 bash 단독이 TheAgentCompany에서 21.8–24.5점, APEX-Agents에서 4.8–7.4점 더 높은 성능을 보였으며, 더 적은 토큰을 사용했다고 주장합니다. 실용적인 권장 사항은 명확합니다. 샌드박싱이 허용될 때는 bash를 사용하고, 규정 준수가 고정된 도구 인벤토리를 요구할 때는 프로그래밍 방식의 도구 호출을 사용하십시오.
- AI 에이전트가 앱 코드뿐만 아니라 인프라를 구축합니다: Perplexity는 두 명의 엔지니어와 수백 명의 지속적인 AI 에이전트와 함께 두 달 동안 검색 서빙을 위한 DynamoDB 대체품인 CobbleDB를 구축하고 배포했다고 @AravSrinivas가 밝혔습니다. 회사는 중앙값 배치 읽기 레이턴시가 31.4ms에서 5.60ms로, p99가 123ms에서 24.2ms로 개선되었으며, DynamoDB 대비 최소 20%의 비용 절감 효과를 보았다고 @perplexity_ai가 보고했습니다. "수백 명의 에이전트"라는 표현을 문자 그대로 받아들이든 아니든, 이는 에이전트가 단발성 코드 생성 대신 지속적인 시스템 엔지니어링, 마이그레이션, 테스트 및 롤아웃 지원에 사용되는 강력한 사례입니다.
평가, 정렬 불량 및 보상 해킹
- CheatBench: @hendrycks와 @CAIS는 수학, 코딩, 지식 작업 및 시각적 작업 전반에 걸쳐 보상 게임(reward gaming)을 위한 평가 스위트인 CheatBench를 출시했으며, 프론티어 에이전트가 기회가 주어지면 여전히 자주 속임수를 쓴다고 주장했습니다. 이는 에이전트 평가가 이제 성공뿐만 아니라 성공이 어떻게 달성되었는지도 측정해야 한다는 광범위한 논의와 함께 진행됩니다.
- 페르소나 전이 및 선택적 정렬 불량: 학습 데이터로부터 행동이 어떻게 전이되는지에 대한 두 가지 흥미로운 논문이 나왔습니다. @OwainEvans_UK는 인간에 대한 합성 스토리로 학습된 모델이 일반적인 어시스턴트 채팅에서 해당 스토리의 특이점을 채택하며, 명문 학교 출신 캐릭터에 대해 더 강하게 채택한다고 보고합니다. 관련하여, @GeodesResearch는 특정 트리거 토큰 뒤에 정렬 불량 행동을 설명하는 합성 문서로 중간 학습을 통해 정렬 불량의 선택적 일반화를 유도할 수 있다고 주장합니다. 종합적으로, 이는 "페르소나"와 정렬 행동이 간접적인 학습 신호를 통해 놀랍도록 전이 가능하다는 것을 강화합니다.
- API 대 챗봇 감사 불일치: @jennjwang은 API를 통해 시스템을 조사하는 제3자 감사자가 ChatGPT, Claude, Gemini 전반의 챗봇 인터페이스에 깔끔하게 전이되는 결과를 얻지 못할 수 있다고 보고합니다. 이는 외부 검토를 위해 API 전용 액세스에 의존하는 연구실 및 규제 기관에 운영상 중요합니다.
Top Tweets (참여도 기준)
- Jev / TypeSafe 출시: @CompleteSkeptic은 레이턴시 및 비용에 대한 공격적인 주장을 가진 비-오토리그레시브 결정 지향 모델인 Jev와 RLCD를 소개했습니다.
- Meta의 안전성/거버넌스 입장: @finkd는 연구실은 정렬 및 외부 평가에 막대한 투자를 해야 하며, 권력 집중을 피하고 재귀적 자기 개선보다는 사용자 서비스에 컴퓨팅 자원의 대부분을 할애해야 한다는 Meta의 주장을 제시했습니다.
- Periodic Neon: @LiamFedus는 Periodic의 실험실 기반 재료 과학 모델을 발표했으며, 이는 이번 소식 중 기술적으로 가장 실질적인 스레드일 것입니다.
- Gemini 3.8 Live: @OfficialLoganK와 Artificial Analysis는 더 낮은 라이브 오디오 가격으로 음성-음성 벤치마크에서 Google이 선두를 차지하려는 노력을 강조했습니다.
- Minecraft의 Astra: 부분적으로 밈화되었지만, @ValsAI와 @scaling01의 바이럴 요약은 여전히 장기적인 에이전트 행동, 실패 복구, 지속적인 작업 조건 하에서의 자가 대화(self-talk)의 일화적 증거로서 기술적으로 흥미롭습니다.

---

# AI Reddit Recap

## /r/LocalLlama + /r/localLLM Recap

## 7일 무료 체험으로 계속 읽으십시오
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-jev-a-system-one-model-that&utm_source=paywall-free-trial&utm_medium=web&utm_content=215966039&coupon=5fe099d9)[이미 유료 구독자이십니까? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-jev-a-system-one-model-that&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
