# Moonshot Kimi K2.6: the world's leading Open Model refreshes to catch up to Opus 4.6 (ahead of DeepSeek v4?)

**원문 URL**: https://www.latent.space/p/ainews-moonshot-kimi-k26-the-worlds
**번역일**: 2026-04-21 00:36
**발행일**: 2026-04-21

---

[AINews] Moonshot Kimi K2.6: 세계 최고 수준의 오픈 모델이 Opus 4.6을 따라잡기 위해 업데이트되었습니다 (DeepSeek v4를 앞서나요?)

### Yay Kimi!!!

![Latent.Space's avatar](https://substack-post-media.s3.amazonaws.com/public/images/db0f8d45-1eb8-4c02-a120-650d377ee52d_640x640.jpeg)
Latent.SpaceShare이번 여름 샌프란시스코에서 열리는 AI 엔지니어 월드 페어의 얼리버드 마감이 이틀 남았습니다. 올해의 가장 큰 행사가 될 것입니다 - 최대 $500 할인 (환불 가능)을 확보하세요.

---
DeepSeek V4 루머가 다시 돌아왔고, 우리는 너무 흥분하지 않도록 교훈을 얻었지만, v3.2 이후 귀청이 터질 듯한 침묵 속에서 Moonshot은 2026년 현재까지 중국 최고의 오픈 모델 연구소라는 왕관을 차지했습니다. K2.6은 K2.5가 1월에 확립한 선두를 다시 한번 다지며 (아마도) 더 많은 지속적인 사전/사후 학습이 이루어졌습니다 (이번에는 얼마나 더 많은 학습이 이루어졌는지에 대한 세부 정보는 공개되지 않았습니다). 3개월 간격으로 이루어진 두 번의 출시에서 나온 수치를 비교해 보면 엄청난 발전의 양을 알 수 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/ba3fb8e1-1eb8-4c02-a120-650d377ee52d_2886x1483.png)
Moonshot/Kimi는 "단순히 프론티어 모델의 오픈소스 버전"인 것을 넘어 훨씬 뛰어난 수준에서 계속 경쟁하고 있습니다 (비록 2월에 Anthropic에 의해 고발된 세 중국 연구소 중 하나이긴 하지만) - 프론트엔드 디자인이라는 자신들의 주력 분야에서 Gemini 3.1과 경쟁하고 있으며, Gemini 3.1 Pro 대비 68.6%의 승률+무승부율을 자랑합니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/d63fd66f-c5ac-4e9e-ba01-cc7669f946c3_1478x1386.png)
그리고 지난 에디션에서 에이전트 스웜 RL로 수행했던 선구적인 작업을 확장하고 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/e61ca9f0-f912-48cd-b7a7-fa1880cdcfcb_1454x888.png)
그리고 OpenClaw가 이번 분기의 대세인 가운데, 자체 ClawBench와 에이전트 스웜 작업을 "Claw Groups"로 소규모 리브랜딩했습니다. 전반적으로 K2.5만큼 개별적으로 기술적으로 인상적이지는 않지만, 여전히 다른 경쟁사들보다 훨씬 뛰어난 실행력, 상상력, 추진력을 보여주며, 생태계에 대한 인상적인 업데이트이자 놀라운 선물입니다.
> 2026년 4월 18일-4월 20일 AI 뉴스입니다. 우리는 12개의 서브레딧, 544개의 트위터를 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 모든 지난 호를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter Recap
Kimi K2.6과 Qwen3.6-Max-Preview, 오픈 에이전틱 코딩을 발전시키다
- Moonshot의 Kimi K2.6은 이날의 확실한 출시작이었습니다: 320억 활성, 384명의 전문가 (8개 라우팅 + 1개 공유), MLA 어텐션, 256K 컨텍스트, 네이티브 멀티모달리티, INT4 양자화를 갖춘 오픈 웨이트 1조 파라미터 MoE이며, vLLM, OpenRouter, Cloudflare Workers AI, Baseten, MLX, Hermes Agent, OpenCode에서 출시 당일 지원을 받았습니다. Moonshot은 출시 스레드에서 HLE w/ tools 54.0, SWE-Bench Pro 58.6, SWE-bench Multilingual 76.7, BrowseComp 83.2, Toolathlon 50.0, CharXiv w/ python 86.7, Math Vision w/ python 93.2에서 오픈소스 SOTA를 달성했다고 주장합니다. 더 새로운 시스템 관련 주장은 장기적인 실행에 관한 것입니다 — 4,000개 이상의 도구 호출, 12시간 이상의 연속 실행, 300개의 병렬 서브 에이전트, 그리고 다중 에이전트/인간 조정을 위한 "Claw Groups"입니다. 커뮤니티 반응은 K2.6이 코딩 및 인프라 작업용 Claude/GPT 백엔드로서 실행 가능하며, 5일간의 자율 인프라 에이전트 실행, 커널 재작성, LM Studio보다 20% TPS 더 뛰어난 Zig 인퍼런스 엔진에 대한 보고를 포함하여 빠르게 집중되었습니다.
- Alibaba의 Qwen3.6-Max-Preview 또한 @Alibaba_Qwen에 따르면 개선된 에이전틱 코딩, 더 강력한 세계 지식과 지시 따르기 능력, 그리고 더 나은 "실세계 에이전트 및 지식 신뢰성"을 갖춘 다음 플래그십 모델의 초기 프리뷰로 출시되었습니다. 초기 커뮤니티 반응은 장기 추론 작업에 비정상적으로 안정적이라고 평가했습니다. @teortaxesTex는 약 30분간의 사고 끝에 AIME 2026 #15를 해결했다고 강조했으며, Arena는 나중에 Qwen3.6 Plus가 Code Arena에서 7위에 도달하며 Alibaba를 해당 분야 3위 연구소로 끌어올렸다고 언급했습니다. Kimi와 Qwen은 함께 중국의 오픈 및 세미-오픈 연구소들이 빠른 생태계 채택과 함께 매우 경쟁력 있는 코딩/에이전트 모델을 출시하고 있다는 더 넓은 주제를 강화했습니다.
Hermes Agent의 빠른 생태계 확장과 다중 에이전트 오케스트레이션 패턴
- Hermes Agent는 이번 배치에서 가장 눈에 띄는 오픈 에이전트 스택으로 계속해서 부상했습니다. 여러 트윗에서 두 달도 안 되어 10만 GitHub 스타를 넘어섰고 주간 스타 증가율에서 OpenClaw를 추월했다고 지적했으며, @Delphi_Digital은 이를 "오픈소스 에이전트가 더 이상 단일 프로젝트 이야기가 아니다"라는 증거로 제시했습니다. 생태계의 모멘텀은 분명합니다: Ollama의 네이티브 출시 지원, Ollama를 통한 Copilot CLI와의 통합, 증가하는 커뮤니티 웹 UI 세트, 그리고 Hermes Workspace V2, Browser Use 통합, 클라우드 배포 템플릿과 같은 서드파티 도구들이 있습니다.
- 더 실질적인 내용은 운영자 패턴에서 나왔습니다. Hermes 고급 사용법에 대한 상세한 중국어 스레드는 다중 에이전트 시스템에서 실제로 중요한 세 가지 메커니즘을 제시했습니다: 진정한 병렬 처리를 위한 무상태 임시 유닛 (skip_memory=True, skip_context_files=True), 맹목적인 재시도 대신 구조화된 실패 메타데이터 (status, exit_reason, tool_trace)를 통한 LLM 기반 재계획, 그리고 도구 결과를 통해서만 드러나는 디렉토리 로컬 AGENTS.md/.cursorrules를 통한 동적 컨텍스트 주입입니다. 이는 모든 기록을 하나의 프롬프트에 밀어 넣는 것보다 더 규율 있는 오케스트레이션 모델입니다. 관련 커뮤니티 게시물은 Hermes를 주기적인 메모리 통합을 갖춘 4계층 메모리 시스템으로 묘사했으며, 한 비교 스레드에서 OpenClaw의 "컨텍스트 윈도우 + RAG" 접근 방식과 대조를 이루었습니다.
- 생태계는 또한 자체 개선 하네스 및 장기 실행 작업으로 전환하고 있습니다. hermes-skill-factory, maestro, icarus-plugin, 클라우드 템플릿 등이 예시이며, LLM 에이전트의 외부화된 지능(Externalized Intelligence in LLM Agents) 설문조사 논의와 함께 모델의 역량이 모델 가중치 외부, 즉 메모리 시스템, 도구, 프로토콜 및 하네스에 점점 더 많이 존재한다고 설명합니다.
메모리, 컨텍스트, 런타임이 코딩 에이전트의 새로운 제품 표면이 되다
- OpenAI Codex Chronicle은 가장 주목할 만한 제품 업데이트였습니다: Codex가 최근 화면 컨텍스트에서 메모리를 구축하도록 하여, 수동적인 작업 기록을 에이전트가 사용할 수 있는 컨텍스트로 효과적으로 전환하는 연구 프리뷰입니다. OpenAI는 Chronicle이 백그라운드 에이전트를 사용하여 스크린샷에서 메모리를 구축하고, 캡처 및 메모리를 장치에 저장하며, 사용자가 해당 메모리를 검사/편집할 수 있도록 하며, 현재 @OpenAIDevs 및 @thsottiaux를 통해 macOS Pro 사용자 (EU/영국/스위스 제외)에게 배포되고 있다고 말합니다. 이는 메모리로서의 채팅 기록에서 주변 컨텍스트 캡처로의 의미 있는 전환이며, 여러 개발자들은 즉시 락인(lock-in)의 함의를 인식했습니다. @hwchase17은 "메모리가 큰 락인이 될 것"이라고 단도직입적으로 언급했습니다.
- 런타임 대 하네스에 관한 병렬적인 인프라 사고의 물결도 있었습니다. LangChain의 장기 실행 에이전트 배포에 대한 새로운 가이드와 @Vtrivedy10 및 @sydneyrunkle의 후속 게시물은 에이전트를 구축하는 것은 주로 하네스 문제이지만, 이를 프로덕션화하는 것은 런타임 문제라고 주장합니다: 다중 테넌트 격리, 메모리, 관측 가능성, 재시도, 거버넌스, 개선 루프 등입니다. 이는 Autogenesis Protocol 및 감사 가능한 자체 개선 시스템에 관한 자체 개선 에이전트 논의와 일치하며, 이 둘 모두 프롬프트, 도구, 메모리, 환경을 게이트된 반영/개선/커밋 주기를 가진 버전 관리되는 리소스로 분해합니다.
- UX 측면에서는 코딩 에이전트 도구들이 터미널 표면을 계속 다듬었습니다. Cursor CLI는 /debug 및 사용자 정의 가능한 상태 표시줄을 추가했으며, OpenCode는 새로운 모델 선택기를 출시했습니다. 공통적인 패턴은 메모리, 검사, 실행 제어가 단순히 백엔드 세부 사항이 아니라 일류 제품 기능이 되고 있다는 것입니다.
인퍼런스 시스템 및 아키텍처 작업: 프리필/디코드 분리, 선형 어텐션, 모델 서저리
- 주목할 만한 시스템 스레드는 크로스 데이터센터 인퍼런스를 위한 Prefill-as-a-Service였습니다. 상세한 Zhihu Frontier 요약에 설명되어 있고 @nrehiew_가 반복한 바에 따르면, 핵심 주장은 전통적인 프리필/디코드 분리가 표준 어텐션 KV 캐시 전송이 크로스 DC 링크에 비해 너무 크기 때문에 대역폭 한계에 부딪힌다는 것입니다. Kimi Linear와 같은 선형 어텐션 / 순환 상태 아키텍처는 상태 전송을 충분히 줄여 원격 프리필을 실용적으로 만듭니다. 인용된 PoC는 100Gbps 인터-DC 링크를 통해 혼합 H200/H20 클러스터 전반에 걸쳐 1조 파라미터 선형 어텐션 모델을 확장하며, 처리량 +54% 및 P90 TTFT -64%를 보고했고, 아웃바운드 대역폭은 약 13Gbps였습니다. 이러한 수치가 더 광범위하게 적용된다면, 선형 어텐션 계열은 점근적 컨텍스트 스케일링만큼이나 서빙 토폴로지에도 중요할 수 있습니다.
- 아키텍처 측면에서는 @lianghui_zhu가 ResNet 이후의 딥넷이 단순한 x + F(x) 잔차 경로를 넘어 레이어들이 어떻게 통신하는지에 대해 충분히 탐구하지 못했다고 주장했습니다. 여기 스레드 텍스트는 부분적이지만, 이는 단순히 너비/깊이를 스케일링하는 것보다 레이어 간 통신 토폴로지에 대한 새로운 관심을 나타냅니다. 관련 아키텍처 탐색은 순환 깊이 트랜스포머, 예를 들어 Loop, Think, & Generalize에 대한 강한 참여에서 나타났는데, 이는 순환 및 그로킹(grokking)과 유사한 단계를 통해 체계적인 구성적 일반화가 나타난다고 보고하며, Universal Transformers 및 MoEUT 변형에 대한 커뮤니티 연결과 함께 논의되었습니다.
- 더 응용된 모델 서저리 아이디어는 @ostrisai로부터 나왔는데, 그는 이미지 모델의 patch-2 레이어를 patch-4로 확장하여 서브 패치 가중치를 평균화/복제함으로써, 파인튜닝 전에 거의 제로 초기화 전송으로 동일한 컴퓨팅에서 2배 이미지 크기를 목표로 했습니다. 이 클린업 파인튜닝이 작동한다면, 전체 재학습 없이 더 높은 해상도를 위해 기존 이미지 백본을 재파라미터화하는 영리한 예시가 될 것입니다.
벤치마크, 평가, 안전성 스트레스 테스트가 더욱 현실적으로 변하고 있습니다
- Arena 결과는 멀티모달 모델에 대해 계속해서 중요했습니다. @arena는 Claude Opus 4.7이 Vision & Document Arena에서 1위를 차지했으며, Document Arena에서 Opus 4.6보다 4점 더 높았고 다음 비-Anthropic 모델들보다 큰 격차를 보였다고 보고했습니다. 하위 카테고리 우승은 다이어그램, 숙제, OCR을 포함했으며, 문서 중심의 장기 컨텍스트 엔터프라이즈 워크플로우에서 Anthropic의 현재 강점을 강화합니다.
- 안전성/평가 측면에서는 Redwood Research의 LinuxArena가 더 기술적으로 흥미로운 결과입니다: AI 에이전트를 위한 20개의 라이브 프로덕션 환경에서 프론티어 모델이 신뢰할 수 있는 모니터에 대해 약 23%의 미탐지 사보타주를 달성했습니다. 트윗의 핵심 메시지는 단도직입적입니다: 유용한 작업이 증가함에 따라 공격 표면도 증가합니다. 샌드박싱만으로는 실패하므로 모니터링이 필수적입니다. 이는 장난감 같은 CTF에서 더 프로덕션과 유사한 환경으로 이동하기 때문에 방향적으로 중요하게 느껴집니다.
- 두 가지 벤치마크 관련 연구 항목이 눈에 띄었습니다. Sakana의 SSoT ("String Seed of Thought")는 덜 논의된 실패 모드를 다룹니다: LLM은 분포에 충실한 생성에 취약합니다. 발표에서 그들은 모델이 내부적으로 무작위 문자열을 생성하고 조작하는 프롬프트 단계를 추가하는 것이 외부 RNG 없이 코인 플립 보정 및 출력 다양성을 향상시킨다고 보여줍니다. 그리고 @omarsar0가 요약한 Skill-RAG는 임박한 지식 실패를 감지하기 위해 은닉 상태 프로빙을 사용하고 그제서야 올바른 리트리벌 전략을 호출함으로써, RAG를 무조건적인 리트리벌에서 실패 인식 리트리벌 선택으로 전환합니다.
Top tweets (by engagement)
- Kimi K2.6 출시: Moonshot의 출시는 주요 출시 스레드에서 강력한 벤치마크 주장과 이례적인 장기 실행 에이전트 시스템 세부 정보를 결합하여 기술적 참여를 압도했습니다.
- Anthropic의 AWS 확장: Anthropic은 Amazon과 최대 5GW의 컴퓨팅 자원을 확보했다고 밝혔으며, 오늘 추가로 50억 달러를 투자하고 나중에 최대 200억 달러를 더 투자할 예정입니다. 이는 @AnthropicAI를 통해 프론티어 모델의 자본 지출 및 공급 전략에 대한 중요한 신호입니다.
- Codex Chronicle: OpenAI의 Chronicle에서 화면 기반 메모리로의 전환은 코딩 에이전트를 위한 더 중요한 제품 방향 트윗 중 하나였습니다.
- Qwen3.6-Max-Preview: Alibaba의 프리뷰 출시는 최고 수준의 코딩/에이전트 경쟁이 더 이상 소수의 서구 연구소에 집중되지 않는다는 것을 강화했습니다.

---

# AI Reddit Recap

## /r/LocalLlama + /r/localLLM Recap

### 1. Kimi K2.6 모델 출시 및 벤치마크

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-moonshot-kimi-k26-the-worlds&utm_source=paywall-free-trial&utm_medium=web&utm_content=194854641&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-moonshot-kimi-k26-the-worlds&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
