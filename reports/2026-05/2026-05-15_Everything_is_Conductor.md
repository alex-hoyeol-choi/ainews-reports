# Everything is Conductor

**원문 URL**: https://www.latent.space/p/ainews-everything-is-conductor
**번역일**: 2026-05-15 06:18
**발행일**: 2026-05-15

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 모든 것이 Conductor입니다

### 매우 조용한 날에 작은 트렌드를 강조해 봅니다.
공유하기AI가 헬스케어를 어떻게 개선하고 있는지 궁금하시다면, 오늘 공개된 저희 첫 번째 팟캐스트를 들어보세요. 이 분야의 다른 최고 엔지니어들을 만나고 싶으시다면, 연사로 신청해 주십시오!

---
진화 생물학에는 "모든 것이 게(Crab)다"라는 농담이 있습니다. 게의 폼 팩터(form factor)는 지구상에서 최소 7번 독립적으로 진화했습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/c44b00aa-b057-4696-a9c6-f8e73c7aaaf7_2289x1342.jpeg)
오늘의 사설이 나온 직접적인 이유는 GitHub가 새로운 GitHub App을 발표했기 때문입니다. Oren Melamed가 말했듯이, "만약 코드를 우선시한다면 예전의 VS Code에 머물고 싶을 수도 있지만, 에이전트를 우선시하고 GitHub를 우선시한다면 아주 좋은 경험을 하게 될 것입니다!"

![](https://substack-post-media.s3.amazonaws.com/public/images/cc0e389d-df44-481c-998d-5524cf58e696_1194x1250.png)
음. 익숙한데요…

![](https://substack-post-media.s3.amazonaws.com/public/images/98d6e93c-4e99-4ff0-8a20-74c75f3a54b8_2310x1298.png)
물론 이 폼 팩터를 개척한 Conductor에게는 매우 좋은 소식입니다. 이제 Y Combinator의 AI에 깊이 빠진(AI pilled) CEO인 Garry Tan이 Conductor의 열렬한 팬이 되었습니다:

![X avatar for @garrytan](https://pbs.substack.com/profile_images/1922894268403941377/-dGWAt3N.jpg)
이제 두 가지 중요한 질문입니다:
- 폼 팩터를 개척했다면, 다른 사람들이 이를 복사하는 동안 어떻게 수익을 창출할 수 있을까요?
- 이 다음에는 무엇이 올까요?
대체 역사에 관심 있는 분들을 위해, 작년에 잠시 유행했던 칸반 보드 폼 팩터에 어떤 일이 있었는지 소개합니다:
그리고 여기 Maggie Appleton이 GitHub Ace의 디자인 씽킹을 분석한 내용입니다:
> 2026년 5월 13일~5월 14일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터(X)를 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터(X) 요약
코딩 에이전트 툴링: Codex Mobile, GitHub의 새로운 앱, VS Code 멀티 에이전트 UX, 그리고 Hermes/Codex 상호 운용성
- OpenAI는 Codex를 일상적인 워크플로우에 더욱 깊이 통합했습니다: 이번 제품군 중 가장 큰 출시는 ChatGPT 모바일 앱에 Codex를 탑재한 것으로, 사용자는 노트북, Mac mini 또는 데브박스에서 Codex가 계속 실행되는 동안 원격으로 작업을 시작하고, 출력을 검토하고, 명령을 승인하고, 실행을 지시할 수 있습니다. OpenAI는 또한 Remote SSH가 관리형 원격 환경에서 이제 일반적으로 사용 가능하며, 나중에 Codex 루프를 중심으로 Business/Enterprise 자동화를 위한 훅(hooks)과 프로그래밍 방식 액세스 토큰을 추가했다고 언급했습니다 (OpenAI, OpenAI follow-up, @OpenAIDevs on mobile workflow, @OpenAIDevs on Remote SSH, @OpenAIDevs on hooks/tokens). 별도로, OpenAI는 코딩 에이전트의 유용성과 제한된 머신 액세스 간의 트레이드오프에 초점을 맞춰 Codex용 Windows 샌드박스에 대한 기술 보고서를 발표했습니다 (OpenAI Devs, @gdb).
- 더 넓은 IDE/앱 생태계는 "에이전트 우선(agent-first)" UX로 수렴하고 있습니다: GitHub는 GitHub Copilot App의 기술 프리뷰를 발표했는데, 이는 병렬 워크스트림, 레포/PR 라이프사이클 관리, 그리고 모델 유연성을 위한 데스크톱 환경으로 설명됩니다 (GitHub, @adrianmg, @OrenMe). VS Code는 멀티 에이전트, 멀티 프로젝트 워크플로우를 위한 새로운 Agents 창, vscode.dev/agents를 통한 브라우저/모바일 지원, BYOK 개선 사항, 그리고 압축된 터미널 출력과 같은 토큰 효율성 기능을 출시했습니다 (VS Code, remote/browser support, BYOK updates, terminal compression). 오픈소스 측면에서는 Nous/Hermes Agent가 Codex 런타임 통합을 추가하여, OpenAI 기반의 턴(turns)을 Codex CLI/앱 서버를 통해 효과적으로 라우팅하고 ChatGPT 구독 기반 실행을 Hermes 세션에서 재사용합니다 (Nous Research, @Teknium, @HermesAgentTips). Kimi 또한 Kimi Web Bridge를 출시했는데, 이는 Kimi Code CLI, Claude Code, Cursor, Codex, Hermes 등에게 인간과 유사한 웹 상호 작용을 노출하는 브라우저 확장 프로그램입니다 (Moonshot AI).
에이전트 인프라 및 자체 개선 루프: LangSmith Engine, SmithDB, 샌드박스, 그리고 지속 학습
- LangChain의 런치 스택은 가장 실질적인 에이전트 인프라 릴리스 클러스터였습니다: SmithDB는 에이전트 트레이스 데이터를 위해 특별히 구축된 데이터베이스이며, LangSmith Engine은 트레이스를 소비하고, 실패를 클러스터링하고, 잠재적인 코드 문제를 식별하며, 수정/평가를 제안합니다—이는 관찰 가능성을 수동적인 검사가 아닌 개선 루프로 전환하는 것입니다 (@hwchase17, @caspar_br on Engine, @bentannyhill). 커뮤니티 논평은 SmithDB의 아키텍처가 객체 스토리지와 이러한 워크로드 형태를 위한 맞춤형 스토리지/쿼리 경로로 전환된 점을 강조했습니다 (@caspar_br on SmithDB, @ngates_, Chinese summary).
- LangChain은 또한 에이전트의 지속 학습에 대한 응용 연구 노력인 LangChain Labs를 발표했습니다. 이 연구는 프로덕션 트레이스가 장기적으로 학습 신호, 평가, 그리고 목표 역량 개선으로 이어져야 한다는 가설을 가지고 있습니다 (LangChain, @jakebroekhuizen, @willccbb, Prime Intellect partnership).
- 에이전트의 실행 격리는 계속해서 성숙해지고 있습니다: W&B/CoreWeave는 RL, 도구 사용, 그리고 평가 워크로드에서 격리된 실행을 위한 CoreWeave Sandboxes를 출시했으며, rm -rf /와 같은 파괴적인 명령을 대규모로 명시적으로 테스트했습니다 (Weights & Biases). 비슷한 맥락에서, 에이전트 디버깅을 위한 오픈소스/로컬 개발 툴링이 등장했습니다: @benhylak은 Codex/Claude Code에 트레이스를 노출하여 자동화된 평가 작성을 가능하게 하는 무료 로컬 에이전트 디버깅 스택을 강조했습니다.
Anthropic Claude Code 제한 및 개발자 반발
- 가장 날카로운 생태계 반응은 Anthropic이 Claude Code 사용을 제한/재편한 것에 대한 것이었습니다. 특히 서드파티 래퍼(wrappers)와 대량의 프로그래밍 방식 워크플로우에 대한 제한이었습니다. Theo의 스레드가 논의의 중심이 되었습니다: 그는 T3 Code 사용자들이 공식적으로 지원되는 경로를 통해 통합했음에도 불구하고 극적인 속도 제한(rate-limit) 감소를 겪었다고 주장했으며, 이후 구독을 취소하고 다른 사람들에게 오픈소스 기부를 위한 취소 스크린샷을 게시하도록 독려했습니다 (@theo initial thread, subscription cancellation, donation thread, T3 Code clarification). 다른 저명한 개발자들도 Anthropic이 오픈소스 개발자/앱을 효과적으로 차단하고 claude -p를 중심으로 구축된 하네스(harnesses)를 불안정하게 만들었다는 불만을 표했습니다 (@theo, @andersonbcdefg).
- 또한 더 전략적인 반론도 있었습니다: 일부 사용자들은 Anthropic이 서드파티 앱 개발자들에게 대규모 보조금이 지급되는 정액제 토큰을 제공할 의무가 없으며, 생태계가 더 명시적인 API 경제와 비싸고 저렴한 모델 간의 더 스마트한 라우팅으로 전환될 가능성이 높다고 주장했습니다 (Sentdex, @tadasayy). 그럼에도 불구하고, 눈에 띄는 이탈 신호는 무시할 수 없는 수준이었으며, 일부 사용자들은 답글 스레드 취소만으로도 상당한 ARR 손실을 추정했습니다 (@thegenioo, Uncle Bob Martin, Theo later). 에이전트 엔지니어들에게 실질적인 교훈은 명확합니다: 구독 기반 하네스는 안정적인 플랫폼 프리미티브가 아닙니다; 공급자/모델 추상화 및 BYOK 경로는 점점 더 필수적으로 보입니다.
로봇 공학 및 체화된 AI: Figure의 24/7 분류 스트림과 더 넓은 자동화 신호
- Figure의 라이브스트림이 로봇 공학 논의를 지배했습니다. 이 회사는 처음에는 8시간 동안 완전 자율적이고 무감독 작업을 선보였고, 이후 24/7 라이브스트림으로 확장하여, 결국 24시간 이상 연속 자율 작동에 실패 없이 성공했다고 보고했습니다. 이는 소형 패키지 분류에서 인간과 거의 동등한 처리량(throughput)을 보였으며, OOD(Out-of-Distribution) 사례에 대한 자동 리셋 기능을 갖춘 Helix-02가 전적으로 온보드에서 작동하는 방식이었습니다—명시적으로 원격 조작(teleoperation)이 없다고 주장했습니다 (Figure CEO Brett Adcock, 24h update, detailed technical clarifications, Day 2 livestream). 반복된 "Bob, Frank, and Gary" 업데이트는 다소 부차적이었지만, 핵심 신호는 생산 수준의 가동 시간(uptime)으로 지속된 자율 작동이었습니다.
- 해석은 Figure에 대한 회의론과 로봇 공학 가속화에 대한 더 넓은 확신으로 나뉘었습니다. 일부 논평자들은 비평가들이 이러한 시연이 단기적인 노동 대체에 미치는 영향을 과소평가하고 있다고 주장한 반면, 다른 이들은 회의론이 로봇 공학이라는 범주 자체보다는 Figure에 더 집중되었다고 언급했습니다 (@cloneofsimo, @iScienceLuvr, @kimmonismus). 어느 쪽이든, 이는 이번 배치에서 가장 명확한 "연속 가동 시간(continuous uptime)" 시연 중 하나였습니다.
연구, 벤치마크, 그리고 오픈 모델: Diffusion LM, 시계열 FM, 메커니즘 해석 가능성, 그리고 RL/탐색
- 몇 가지 기술적으로 중요한 모델/연구 릴리스가 눈에 띄었습니다: Zyphra의 ZAYA1-8B-Diffusion-Preview는 제한된 품질 손실로 자기회귀 생성(autoregressive generation) 대비 4.6~7.7배의 디코딩 속도 향상을 주장하며, Diffusion LM이 더 저렴한 롤아웃과 더 풍부한 생성 모드를 가능하게 한다는 일반적인 주장을 뒷받침합니다 (Zyphra). Datadog의 Toto 2.0은 Apache 2.0 라이선스 하에 4M에서 2.5B 파라미터에 이르는 5개의 오픈 웨이트 시계열 예측 모델을 출시했으며, BOOM, GIFT-Eval, TIME에서 1위를 차지했다고 주장합니다. 더 중요하게는, 스케일링 법칙이 TSFM에 대해 마침내 깨끗하게 적용될 수 있다는 증거를 제시했습니다 (Datadog, @atalwalkar, @ClementDelangue). Goodfire의 해석 가능성 게시물은 Llama가 산술 연산을 위해 기하학적인 "모양 회전 계산기" / 푸리에 특징과 유사한 메커니즘을 사용하며, 순수한 사후 설명(post-hoc description)보다는 조향 기반 증거를 제시한다고 주장했습니다 (GoodfireAI, follow-up).
- RL/탐색 및 옵티마이저 스타일의 진전과 관련하여 몇 가지 주목할 만한 스레드가 있었습니다: LLM RL을 단순히 PPO 대 GRPO가 아닌 생성(Generate) / 필터(Filter) / 제어(Control) / 재생(Replay) 전반에 걸친 롤아웃 엔지니어링으로 구성하는 설문조사 (The Turing Post); 특권 정보를 사용하여 유용한 롤아웃을 적극적으로 찾는 교육적 RL (Pedagogical RL) (Souradip Chakraborty, @lateinteraction); 그리고 Prime Intellect의 nanoGPT 스피드런 벤치마크에서의 자율 옵티마이저 탐색으로, Opus 4.7은 2930 스텝, GPT-5.5는 2950 스텝에 도달하여 약 1만 회 실행 / 약 1만 4천 H200 시간 후 2990의 인간 기준선을 넘어섰습니다 (Prime Intellect, @eliebakouch). 또한 주목할 만한 점은 Kimi K2.6이 Finance Agent Benchmark V2에서 1위 오픈 웨이트 모델로 보고되었고 (Moonshot AI), Ring-2.6-1T가 오픈 릴리스로 day-0 vLLM 지원을 받았다는 것입니다 (vLLM).
최고 인기 트윗 (참여도 기준)
- OpenAI의 Codex 모바일 출시는 참여도와 실용적 관련성 면에서 가장 확실한 제품 승자였습니다: ChatGPT 모바일에서 실행 중인 코딩 에이전트 세션을 원격으로 제어/검토할 수 있습니다 (OpenAI).
- Theo의 Claude Code 반발 스레드는 플랫폼 위험과 구독 기반 에이전트 워크플로우를 둘러싼 가장 강력한 개발자 정서 변화를 포착했습니다 (@theo, @theo donations thread).
- Figure의 자율 휴머노이드 분류 라이브스트림은 가장 많이 논의된 체화된 AI 데모 중 하나로 남아있는데, 특히 온보드 정책 실행 및 원격 조작(teleop) 없음이라는 상세한 주장을 통해 24시간을 넘어서면서 더욱 그러했습니다 (Brett Adcock).
- GitHub의 Copilot App과 LangChain의 Engine/SmithDB/Labs는 이번 주기에서 에이전트 엔지니어들에게 가장 중요한 비-OpenAI 툴링 출시였습니다 (GitHub, LangChain, @hwchase17).
- Prime Intellect의 자율 옵티마이저 탐색 결과는 코딩 에이전트가 단순히 앱 개발뿐만 아니라 개방형 ML 최적화에 통합되는 구체적인 사례로서 주목할 만합니다 (Prime Intellect).

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Qwen 3.6 로컬 인퍼런스 속도 향상 및 양자화
- LLaMA.cpp + TurboQuant에서 Qwen용 멀티 토큰 예측(MTP) (활동: 514): 패치된 llama.cpp 포크는 Qwen용 멀티 토큰 예측(MTP) 지원과 TurboQuant를 추가하여, MacBook Pro M5 Max 64GB에서 21 tok/s → 34 tok/s를 보고했으며, 90%의 MTP 수용률을 주장했습니다; 원시 속도 향상은 약 62%이며 40%가 아닙니다. 코드는 AtomicBot-ai/atomic-llama-cpp-turboquant에 게시되었으며, AtomicChat/qwen-36-udt-mtp HF 컬렉션에는 Qwen 3.6 27B/35B용 GGUF MTP 양자화가 포함되어 있습니다. 논평자들은 TurboQuant의 프레이밍에 의문을 제기하며, 종종 f16, q8 또는 q4보다 느리다고 주장했습니다; 한 논평자는 llama.cpp에 대한 TurboQuant PR이 기존 Q4 KV-quant 회전 지원이 대부분의 이점을 이미 커버했기 때문에 거부되었으며, 이점은 품질 저하가 우려되는 Q3에서 주로 나타난다고 언급했습니다. 다른 이들은 더 높은 추측/MTP 수용률과 초당 토큰 수만으로는 출력 동등성을 확립할 수 없으므로 품질/평가 데이터를 요청했습니다. 여러 논평자들은 TurboQuant가 llama.cpp에서 일반적으로 더 빠르지 않으며, f16, q8 또는 q4보다 느릴 수 있다고 언급했습니다. 이전 llama.cpp에 대한 TurboQuant PR은 llama.cpp가 이미 Q4 KV-캐시 양자화를 위한 회전을 구현하고 있어 표준 Q4가 더 빠르고 이점이 거의 없었기 때문에 거부된 것으로 보고되었습니다; TurboQuant는 Q3 주변에서만 도움이 될 수 있지만, 상당한 품질 저하가 동반됩니다. 사용자들은 속도, 품질, 컨텍스트 트레이드오프를 구분했습니다: TurboQuant 없는 MTP는 속도 향상을 위해 제안되었고, 표준 Q4_1 또는 Q4_0 양자화는 더 긴 컨텍스트/품질 유지를 위해 권장되었습니다. 한 논평자는 TurboQuant가 Mac 특정 이점을 가지고 있는지 의문을 제기하며, 이점이 광범위하게 유용하기보다는 하드웨어 또는 워크로드에 따라 달라진다고 암시했습니다. 한 논평자는 내장 MTP 대신 dflash를 사용할 것을 권장하며, 30~40% 더 빠르다고 주장했습니다. 그들은 또한 이에 대한 풀 리퀘스트가 이미 존재한다고 언급하며, 구현 작업이 이전 llama.cpp 통합 노력을 중복할 수 있음을 시사했습니다.

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-everything-is-conductor&utm_source=paywall-free-trial&utm_medium=web&utm_content=197780500&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-everything-is-conductor&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
