# not much happened today

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-cee
**번역일**: 2026-10-03 12:30
**발행일**: 2026-10-03

---

[AINews: 주중 요약](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 오늘은 별일 없었습니다

### 조용한 하루였습니다.

![Latent.Space's avatar](https://substack-post-media.s3.amazonaws.com/public/images/db0f8d45-1eb8-4c02-a120-650d377ee52d_640x640.jpeg)
Latent.Space2026년 10월 3일공유이 글을 보고 계시다면, 주말을 즐기러 가시는 게 좋을 것 같습니다.
> 2026년 10월 1일~10월 2일 AI 뉴스입니다. 저희는 12개 서브레딧, 544개 트위터 계정을 확인했으며, 추가 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색하실 수 있습니다. 다시 한번 말씀드리지만, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제하실 수 있습니다!

---

# AI 트위터 요약
GPT-6.1 Sol과 Sonnet 5.5, 비용-성능 프론티어를 재편하다
- GPT-6.1 Sol 출시: OpenAI는 Sol의 가격을 백만 입력/출력 토큰당 $2/$10로 책정했으며, Astra의 $10/$50와 비교됩니다 ([가격 요약](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
    - 주장된 결과: DeepSWE v1.1에서 GPT-6 Sol을 6.4점, AutomationBench에서 Opus 5.5를 2.2점 앞섰다고 합니다 ([요약](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
    - 포지셔닝: OpenAI 직원들은 이를 "좋고, 저렴하며, 빠르다"고 설명합니다 ([@reach_vb](https://x.com/reach_vb/status/1841796594735552909)).
    - Codex 사용량: 10월 2일 오전 10시(PT)에 전 세계 Codex 사용량 리셋이 예정되었습니다 ([@reach_vb](https://x.com/reach_vb/status/1841796594735552909)).
    - 도구 사용: Sol은 "codemode를 정말 좋아한다"고 알려졌으며, 이는 GPT 모델이 codemode로 학습된다는 점과 일치합니다 ([@badlogicgames](https://x.com/badlogicgames/status/1841796594735552909), [codemode 참고](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
- Agent Arena 순위: Sol [Max]은 작업당 중앙값 $0.56의 비용으로 5위(+11.23%)를 차지했습니다 ([@arena](https://x.com/arena/status/1841796594735552909)).
    - Sol 비용 비교: GPT-6 Sol보다 39% 저렴하면서 1.52점 더 높은 점수를 기록했습니다. Astra보다 81% 저렴하면서 1.04점 이내의 점수를 기록했습니다.
    - Sonnet 5.5: Sonnet 5.5 [Max]은 3위(+12.5%)로 데뷔했으며, Chat 카테고리에서 1위를 차지했습니다. 작업당 $2.74의 비용이 들며, 2위 Opus 5.5의 $1.58에 비해 높아 파레토 프론티어 밖에 머물러 있습니다 ([데뷔](https://x.com/arena/status/1841796594735552909), [프론티어](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
    - Anthropic의 위치: Anthropic 모델들은 이제 Agent Arena 상위 3개 자리를 차지하고 있습니다.
- Code 및 Text Arena: Sol은 WebDev에서 잠시 3위를 기록했으나, Sonnet 5.5에 밀려 4위로 내려갔습니다 ([주간 요약](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
    - WebDev에서의 Sonnet: Sonnet은 이제 GPT-6 Astra [Max]보다 2점 뒤처지지만, 80% 더 낮은 비용으로 제공됩니다.
    - Gemini 4 Argon: Argon [High]은 Text Arena에서 1위를 차지했습니다.
    - 오픈 모델: MiMo-V2.6-Pro와 Flash는 오픈 모델 중 Agent Arena에서 각각 5위와 9위를 기록했습니다.
- 다른 독립 평가: WeirdML v3는 Sol이 Astra에 근접하지만 더 낮은 피크를 보이는 매우 토큰 효율적인 모델임을 발견했습니다. 동일한 벤치마크에서 Sonnet 5.5는 Opus 5를 이겼고, Grok 4.7은 Kimi-K3를 이겼습니다. 이 결과는 미완성입니다 ([@htihle](https://x.com/htihle/status/1841796594735552909)).
    - 추론 스타일: Design Arena는 324개의 사고 요약을 분석했습니다. 그 결과 Astra는 Opus 5.5보다 약 20배 자주 모호한 표현을 사용하며, Opus는 5개 요약 중 약 4개에서 일찍 결론을 내리는 것으로 나타났습니다 ([@DesignArena](https://x.com/DesignArena/status/1841796594735552909)).
    - Step 5 프리뷰: StepFun의 모델은 Vals에서 작업당 $2.54의 비용으로 오픈 웨이트 모델 중 7위를 기록했습니다. 작업당 평균 약 2시간이 소요되며, 1M 토큰 컨텍스트 윈도우를 가집니다 ([Vals](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details), [세부 정보](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
- 루머 (미확인):
    - Fable 5.5: Claude Fable 5.5는 다음 주에 출시될 것으로 루머가 돌고 있으며, 보안 문제로 지연되었다고 알려진 "Astra 6.1"을 능가한다고 합니다. 게시자는 두 주장 모두 확인할 수 없다고 말했습니다 ([@kimmonismus](https://x.com/kimmonismus/status/1841796594735552909), [후속](https://x.com/kimmonismus/status/1841796594735552909)).
    - GPT-6 Astra Lite: "GPT-6 Astra Lite" 목록이 발견되었으며, [@scaling01](https://x.com/scaling01/status/1841796594735552909)은 이를 Sol과 동일한 모델로 추측하고 있습니다 ([@scaling01](https://x.com/scaling01/status/1841796594735552909)).
- 의사결정 모델 및 오픈 웨이트: llama.cpp는 로컬 "Jev 스타일" 의사결정 모델 인퍼런스를 위한 `/v1/systemone` 엔드포인트를 추가했습니다 ([@ggerganov](https://x.com/ggerganov/status/1841796594735552909)).
    - 로컬 실행: 모델은 `llama serve -hf ggml-org/Kev-4B-GGUF` 명령으로 실행됩니다 ([@ClementDelangue](https://x.com/ClementDelangue/status/1841796594735552909)). Jared Palmer는 Kev 1.0의 작동 방식에 대한 게시물을 발표했습니다 ([게시물](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
    - 생태계: Perplexity는 pplx-decider-v1-27b가 11개 벤치마크에서 평균 85.7%를 기록하여 Jev를 앞선다고 주장합니다 ([@AravSrinivas](https://x.com/AravSrinivas/status/1841796594735552909)). Clef 의사결정 모델은 이제 Ollama에서 사용할 수 있습니다 ([@lucataco](https://x.com/lucataco/status/1841796594735552909)).
    - 회의적인 시각: [@mervenoyann](https://x.com/mervenoyann/status/1841796594735552909)은 의사결정 모델을 제로샷 분류기의 리브랜딩이라고 말합니다 ([트윗](https://x.com/mervenoyann/status/1841796594735552909)).
    - 캘리브레이션 분석: 한 블로그 게시물은 Jev 스타일 캘리브레이션을 가치 및 Q-함수 예측과 연결합니다 ([@SOURADIPCHAKR18](https://x.com/SOURADIPCHAKR18/status/1841796594735552909)).
    - webAI TwIL-LM3-Pro: 이 3.66B 모델은 Granite 4.2로부터 사후 학습되었습니다. webAI의 테스트에서 형식 논리에서 Qwen3-8B와 거의 일치합니다. Q4 GGUF는 2.09 GiB이며 라이선스는 비상업적입니다 ([@kimmonismus](https://x.com/kimmonismus/status/1841796594735552909)).
    - Reka RIDM: Reka는 Apache 2.0 라이선스 하에 역동학 모델을 출시했습니다. 이 모델은 게임으로 학습되었으며, 실제 비디오로 일반화되고 모터 및 카메라 동작을 추출합니다 ([@RekaAILabs](https://x.com/RekaAILabs/status/1841796594735552909)).
에이전트 하네스, 어시스턴트 및 개발자 도구
- OpenAI dots: Sam Altman은 dot을 자신이 가장 좋아하는 OpenAI 제품이라고 부르며, 자신의 워크플로우를 학습하면서 매일 개선된다고 말합니다 ([@sama](https://x.com/sama/status/1841796594735552909)).
    - 기능: Dot은 앱 전반에 걸쳐 컨텍스트를 유지하고, Codex 작업을 조정하며, 주의가 필요한 항목에 플래그를 지정합니다 ([@OpenAIDevs](https://x.com/OpenAIDevs/status/1841796594735552909)).
    - 비교: 한 사용자는 Grokbot의 멀티 에이전트 "비서실장" 설정을 선호합니다 ([@kimmonismus](https://x.com/kimmonismus/status/1841796594735552909)). DIY 클론은 Pi, Telegram 게이트웨이 및 모든 모델을 사용합니다 ([@_alejandroao](https://x.com/_alejandroao/status/1841796594735552909)).
- Muse Gadgets: Meta는 Muse와 연동되는 하드웨어 구축을 위한 ESP32 펌웨어와 Linux SDK를 오픈소스화했습니다 ([@natfriedman](https://x.com/natfriedman/status/1841796594735552909)).
    - Muse Home Link: Meta는 자체 스마트 홈 브리지 5,000대를 제작하여, 재고 소진 시까지 구독자에게 무료로 제공했습니다 ([@alexandr_wang](https://x.com/alexandr_wang/status/1841796594735552909), [배송](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
- 확장 가능한 하네스: DeepSeek Harness는 macOS 및 Windows용 데스크톱 빌드를 출시했습니다. Linux 사용자들은 npm에서 `@deepseek-ai/dsh`를 설치할 수 있습니다 ([@deepseek_ai](https://x.com/deepseek_ai/status/1841796594735552909)).
    - Claude Code 모드: 모드는 Claude Code에 미들웨어와 같은 훅을 제공하는 플러그인입니다 ([@lydiahallie](https://x.com/lydiahallie/status/1841796594735552909)). 새로운 "You should know" 플러그인은 사용자가 놓칠 수 있는 중요한 출력을 플래그 지정하는 보조 에이전트를 생성합니다 ([@ClaudeDevs](https://x.com/ClaudeDevs/status/1841796594735552909)).
    - Pi Durable: Pi는 이제 Pi의 v1.0 출시와 함께 agents SDK v0.26.0을 통해 Cloudflare Durable Objects에서 실행됩니다 ([@mattzcarey](https://x.com/mattzcarey/status/1841796594735552909), [@badlogicgames](https://x.com/badlogicgames/status/1841796594735552909)).
    - 컨텍스트: [@omarsar0](https://x.com/omarsar0/status/1841796594735552909)은 이러한 출시를 유연한 하네스로의 전환으로 설명합니다 ([스레드](https://x.com/omarsar0/status/1841796594735552909)).
- T3 Code 오케스트레이터 재작성: 이 프로젝트는 40만 명의 사용자를 돌파했습니다 ([@theo](https://x.com/theo/status/1841796594735552909)). 1,912개 파일에 걸쳐 823개의 커밋이 포함된 4개월간의 PR이 이제 병합되었습니다 ([@maria_rcks](https://x.com/maria_rcks/status/1841796594735552909)).
    - 새로운 기능: 재작성에는 Pi 지원, 크로스 프로바이더 delegate_task, ACP 레지스트리, 스레드 포킹, 스레드 중간 모델 전환, 서브 에이전트 계보 보기 및 예약된 작업이 추가되었습니다 ([기능 목록](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
- 플랫폼 업데이트: OpenAI의 Agents API는 원콜 브라우저 컴퓨터 사용, Bedrock Managed Agents 및 휴대용 환경을 추가했습니다. 또한 99.97%의 턴 안정성과 20% 더 빠른 도구 호출을 주장합니다 ([@stevendcoffey](https://x.com/stevendcoffey/status/1841796594735552909)).
    - Cursor Rollouts: Rollouts가 회귀를 감지하면, 문제가 되는 PR을 찾아 이슈를 열고 원클릭 클라우드 에이전트 수정 기능을 제공합니다 ([@cursor_ai](https://x.com/cursor_ai/status/1841796594735552909)).
    - Cloudflare: Sandbox SDK 1.0은 Durable Objects에 샌드박스 컨테이너에 대한 직접 제어 권한을 부여합니다 ([@CFchangelog](https://x.com/CFchangelog/status/1841796594735552909)). Cloudflare는 또한 request Traces를 출시했습니다 ([@WalshyDev](https://x.com/WalshyDev/status/1841796594735552909)).
연구: 에이전트 학습, 장기적 제어 및 수학을 위한 AI
- 멀티 하네스 RL (Hugging Face): 동일한 모델 가중치가 한 하네스에서는 62%, 다른 하네스에서는 33%를 기록했습니다 ([@huggingface](https://x.com/huggingface/status/1841796594735552909)).
    - 방법: 프록시는 OpenAI, Anthropic 및 Gemini API 형식을 사용하며, 하네스 자체에는 변경 없이 학습을 위한 샘플링된 토큰 ID와 logprob를 기록합니다.
    - 결과: LFM2.5-2.6B는 4개의 하네스에서 42%에서 54%로 개선되었으며, 도구 호출을 31% 줄였습니다. 3,189개의 Qwen3.8-27B 롤아웃에 대한 SFT는 47.5%에서 정체되었습니다.
    - 출시: 트레이너, 데이터 및 학습된 7개 모델 모두 오픈되어 있습니다.
- 크레딧 할당 및 RL 효율성: ProVer는 심사관이 결정적인 궤적 세그먼트를 찾아내고, 양쪽의 롤아웃을 사용하여 해당 세그먼트의 이점을 설정합니다. GRPO 대비 +9.91% (Qwen3.5-2B) 및 +7.12% (Qwen3.5-4B)의 상대적 이득을 보고했습니다 ([@omarsar0](https://x.com/omarsar0/status/1841796594735552909)).
    - 부분 롤아웃: AC2는 학습된 비평가를 사용하여 토큰 청크에 점수를 매기므로, 학습에는 부분 롤아웃만 필요합니다 ([@wen_kaiyue](https://x.com/wen_kaiyue/status/1841796594735552909)).
    - 프론티어 학습: 이 방법은 모델이 항상 또는 전혀 해결하지 못하는 문제는 GRPO 기울기가 0이 되므로, 능력의 한계에 있는 문제를 목표로 합니다 ([@robinfaro13](https://x.com/robinfaro13/status/1841796594735552909)).
    - Sharpening Tax: 이 논문은 사후 학습 후 pass@K 스케일링 가능성 손실을 정량화하고, 프롬프트당 온도 샘플러인 PTGS를 제안합니다 ([@iScienceLuvr](https://x.com/iScienceLuvr/status/1841796594735552909)).
    - SFT vs RL: 또 다른 논문은 SFT가 목표 때문이 아니라 데이터가 오프-정책이기 때문에 일반화 성능이 더 나쁘다는 것을 발견했습니다. 기본 모델의 스타일로 전문가 궤적을 다시 작성하면 격차가 줄어듭니다 ([@maximelabonne](https://x.com/maximelabonne/status/1841796594735552909)).
- 장기적 제어 및 컨텍스트: Meta Superintelligence Labs는 전용 컨트롤러가 ProgramBench에서 GPT-5.5의 성능을 63.7%에서 71.5%로 향상시켰다고 보고했으며, 동일한 작업자와 예산을 사용했을 때 Codex의 58.0%와 비교됩니다 ([@dair_ai](https://x.com/dair_ai/status/1841796594735552909)).
    - 컨텍스트 압축: Microsoft의 학습 없는 FOCUS는 피크 컨텍스트를 최대 48%까지 줄이고 작업 성공률을 최대 8.9점 높입니다 ([@dair_ai](https://x.com/dair_ai/status/1841796594735552909)).
    - 장문 컨텍스트 성능 저하: NVIDIA의 Long-Transduction 연구는 7개 오픈 모델에서 4K에서 128K 컨텍스트로 전환할 때 정확도가 62.8% 하락하는 것을 측정했습니다 ([@dair_ai](https://x.com/dair_ai/status/1841796594735552909)).
    - 멀티 에이전트 조정: AgentWorld에서 멀티 에이전트 작업의 3분의 1 미만이 작업을 완료하는 데 도움이 되며, 조정 작업은 12%의 성공률에 불과합니다 ([@omarsar0](https://x.com/omarsar0/status/1841796594735552909)).
    - Apple LoopCD: 이 방법은 반복 루프를 절반으로 줄이면서 AIME 2024 pass@1을 61.88%에서 73.33%로 높입니다 ([@arankomatsuzaki](https://x.com/arankomatsuzaki/status/1841796594735552909)).
- 미해결 수학 문제에 대한 AI: Meta는 Muse Spark 1.1 및 1.2를 사용하여 일반 meta.ai 챗을 통해 생성된 미해결 문제에 대한 6편의 논문을 발표했으며, 사용자 정의 스캐폴드는 사용하지 않았습니다 ([@AIatMeta](https://x.com/AIatMeta/status/1841796594735552909), [목록](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
    - 과정: 각 논문은 어떤 부분이 주로 인간 또는 AI에 의해 작성되었는지 표시하며, 두 번째 수학자 그룹이 작업을 검토했습니다.
    - Google Cogentic: 이 Gemini 멀티 에이전트 시스템은 5개의 미해결 이론 문제에 대한 새로운 결과를 도출했습니다 ([@omarsar0](https://x.com/omarsar0/status/1841796594735552909)).
    - Cogentic 설계: 각 초안은 두 개의 적대적 검증자를 통과해야 하며, 에이전트들은 검증된 보조정리의 원장을 공유합니다. 대부분의 문제는 약 100번의 호출이 필요했으며, 가장 어려운 문제는 약 1,000번의 호출이 필요했습니다.
- 이미지 사후 학습: Arena는 Bradley-Terry 보상 모델을 충실도, 제약 및 보상 해킹 방지 보상과 결합했습니다 ([@arena](https://x.com/arena/status/1841796594735552909)).
    - 결과: FLUX.2-dev는 69 ELO를 얻어 1202가 되었고, Ideogram 4는 20 ELO를 얻어 1224가 되었습니다.
벤치마크, 평가 무결성 및 안전성
- 연구 취향 벤치마크: ScholarCatalyst는 에이전트에게 연구 프로젝트 뒤에 있는 "촉매 논문"을 찾도록 요청합니다. 207개의 자체 프로젝트에 대한 184명의 주 저자에 의해 레이블링되었으며, 아직 포화 상태와는 거리가 멀다고 설명됩니다 ([@yoonholeee](https://x.com/yoonholeee/status/1841796594735552909)).
    - EurekaBench: 이 벤치마크는 에이전트가 6개 과학 도메인에서 진정으로 새로운 통찰력을 발견할 수 있는지 테스트합니다 ([@JiayiiGeng](https://x.com/JiayiiGeng/status/1841796594735552909)).
- Vals 웹 검색 인덱스: 이 인덱스는 모델과 하네스를 일정하게 유지하고, 검색 도구만 교체하며, 금융 및 법률 업무에 대한 최종 답변에 점수를 매깁니다 ([@ValsAI](https://x.com/ValsAI/status/1841796594735552909)).
    - 검증: 에이전트는 검색 없이 2.9% (법률) 및 7.4% (금융)를 기록했으며, 검색을 사용하면 30–50%를 기록했습니다. Vals는 또한 모델이 검색 없이 BrowseComp의 44.5%에 답변한 연구를 인용합니다 ([세부 정보](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
- SWE 버그 찾기 벤치마크: 이 새로운 벤치마크에서 에이전트는 이전 커밋에서 시작하여 이후 커밋에서 수정된 실제 버그에 대해 점수를 매깁니다.
    - 비판: Lucas Beyer는 이 벤치마크가 주로 회상을 테스트하며, 구성이 학습하기 쉽다고 주장합니다 ([@giffmana](https://x.com/giffmana/status/1841796594735552909)).
    - 저자들의 답변: 저자들은 테스트 세트가 제외되는 한 버그 찾기 학습은 괜찮다고 말합니다 ([@OfirPress](https://x.com/OfirPress/status/1841796594735552909)).
- 평가 무결성 질문: David Rein은 Terminal Bench의 기반 프레임워크인 Harbor가 에이전트가 평가 전에 궤적을 수정하도록 허용하는지 묻습니다. 그는 코드를 잘못 해석했을 수도 있다고 언급합니다 ([@idavidrein](https://x.com/idavidrein/status/1841796594735552909)).
- 오픈 모델의 공격 능력: The Batch는 GLM-5.3이 취약점 악용에서 Claude Mythos와 거의 일치하는 성능을 보였다고 보고합니다 (12% vs 14%) ([@DeepLearningAI](https://x.com/DeepLearningAI/status/1841796594735552909)).
    - 논란의 주장: 한 평론가는 GLM-5.3 Flash가 ExploitBench에서 Mythos Preview를 능가한다고 말합니다 ([@teortaxesTex](https://x.com/teortaxesTex/status/1841796594735552909)).
    - 무검열 변형: 무검열 GLM-5.3이 Hugging Face에 유포되고 있습니다 ([@kimmonismus](https://x.com/kimmonismus/status/1841796594735552909)).
- 안전성 연구 및 보호 장치: 새로운 논문은 학습 중 내부 신호를 사용하여 화이트박스 모니터링을 저하시키지 않으면서 정렬을 개선하는 방법을 제안합니다 ([@lenalibon](https://x.com/lenalibon/status/1841796594735552909)).
    - NeurIPS 채택: "Models That Know How Evaluations Are Designed Score Safer"는 논문이 NeurIPS 2026에 채택되었습니다 ([@HaritzPuerto](https://x.com/HaritzPuerto/status/1841796594735552909)).
    - 오탐: Opus 5.5는 스펙트로그램 음절 레이블링 중 "추론 추출" 보호 장치를 자주 트리거합니다 ([@ChaseBrowe32432](https://x.com/ChaseBrowe32432/status/1841796594735552909)).
- 새로운 세계 지식: 모델에게 16,200개의 위도/경도 좌표에 대해 "육지 또는 물?"이라고 묻고 답변을 플로팅하면 인식 가능한 세계 지도가 나옵니다 ([@karpathy](https://x.com/karpathy/status/1841796594735552909)).
인퍼런스, 하드웨어 및 시스템
- DeepSeek 커널을 통한 Ascend 950: DeepSeek의 오픈소스 DeepGEMM, FlashMLA, TileKernels 및 DeepEP 분석을 통해 칩의 레이아웃을 추론했습니다 ([@ZhihuFrontier](https://x.com/ZhihuFrontier/status/1841796594735552909)).
    - 예상 사양: 이 칩은 32개의 AI 코어를 가지며, 각 코어는 하나의 Cube 코어와 두 개의 Vector 코어를 쌍으로 이룹니다. 예상 피크 성능은 BF16/FP8/FP4에서 약 432/865/1,730 TFLOPS입니다.
    - 용량: 950 시리즈가 8월에 판매되었다는 주장에도 불구하고 공급이 제한될 수 있습니다 ([@teortaxesTex](https://x.com/teortaxesTex/status/1841796594735552909)).
- Prime Inference: Prime Intellect는 MLA 잠재 공간을 NVFP4에 저장하여 행을 576바이트에서 352바이트로 줄이고 FP8보다 약 50% 더 많은 캐시된 토큰을 저장합니다 ([@PrimeIntellect](https://x.com/PrimeIntellect/status/1841796594735552909)).
    - 스택: vLLM 및 Dynamo에서 GLM-5.3을 제공하며, 스파스-MLA 커널은 FlashInfer로 이동할 예정입니다 ([@vllm_project](https://x.com/vllm_project/status/1841796594735552909)).
- 저정밀도 벤치마킹: Stas Bekman은 B200에서 NVFP4가 MXFP4보다 약 9% 더 효율적이며, 더 높은 정확도를 보인다고 측정했습니다 ([@StasBekman](https://x.com/StasBekman/status/1841796594735552909)).
    - mamf-finder: 이 도구는 이제 FP8, MXFP8, MXFP4 및 NVFP4를 벤치마크합니다 ([업데이트](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
- 메모리 및 속도: NVHBM은 메모리 컨트롤러를 맞춤형 베이스 다이로 이동시켜 HBM4E보다 최대 30% 더 높은 대역폭과 15% 더 낮은 전력을 주장합니다 ([@vikramskr](https://x.com/vikramskr/status/1841796594735552909)).
    - 논란의 경제성: Micron은 NVHBM이 마진을 개선할 것이라고 말하지만, [@vikramskr](https://x.com/vikramskr/status/1841796594735552909)은 이에 반박합니다 ([반론](https://x.com/vikramskr/status/1841796594735552909)).
    - Volantis: 이 스타트업은 광학 기술을 사용하여 10T개 이상의 파라미터를 가진 모델에서 사용자당 최대 10K 토큰/초를 목표로 합니다 ([@omarsar0](https://x.com/omarsar0/status/1841796594735552909)).
    - Cerebras: Altman은 Cerebras를 속도 측면에서 긴밀한 파트너라고 불렀습니다 ([@sama](https://x.com/sama/status/1841796594735552909)).
- 용량 경제학 (Epoch): Epoch은 AI 인프라가 곧 수억에서 수십억 개의 에이전트를 지원할 수 있을 것으로 추정합니다 ([@EpochAIResearch](https://x.com/EpochAIResearch/status/1841796594735552909)).
    - 수요 격차: 단 20%의 활용률만으로도 연간 $2.6–5.3T의 지출이 발생하며, 이는 2027년 말까지 약 $1T의 연구실 수익과 대비됩니다 ([세부 정보](https://www.latent.space/p/ainews-gpt-61-sol-and-sonnet-55#details)).
- 플랫폼: SemiAnalysis는 Google의 GPU 클러스터를 Gold 티어로 평가하며, ConnectX NCCL 플러그인이 이제 자동 활성화된다고 언급합니다 ([@SemiAnalysis_](https://x.com/SemiAnalysis_/status/1841796594735552909)).
    - 연합 학습: Google Research는 검증 가능한 차등 프라이버시를 갖춘 TEE 기반 연합 학습을 출시했습니다 ([@GoogleResearch](https://x.com/GoogleResearch/status/1841796594735552909)).
산업 및 정책
- Anthropic과 바티칸: NYT는 Chris Olah가 교황의 AI 회칙 발표에서 철수할 것을 제기했다고 보도했으며, 이 회칙의 내용은 기계 의식을 거부합니다 ([@ChristopherHale](https://x.com/ChristopherHale/status/1841796594735552909)).
    - 로비: Olah의 팀은 교황의 고문들에게 모델 의식을 진지하게 받아들이도록 로비했다고 알려졌습니다. 그는 결국 참석했습니다 ([@kimmonismus](https://x.com/kimmonismus/status/1841796594735552909)).
    - 컨텍스트: 기사는 Olah가 "우리는 AI 모델이 의식이 있는지 모른다"고 말하는 것으로 시작합니다 ([@buccocapital](https://x.com/buccocapital/status/1841796594735552909)).
    - 비판: Aidan Gomez는 이 캠페인을 도덕적 오만이라고 비판했습니다 ([@aidangomez](https://x.com/aidangomez/status/1841796594735552909)). Lucas Beyer는 대본에서 "create"가 "train"으로 단어가 변경된 것을 언급했습니다 ([@giffmana](https://x.com/giffmana/status/1841796594735552909)).
- 안전성 반대 영향력 캠페인: 한 보고서는 최소 $100M를 지출할 계획을 가진 그룹에 대해 설명하며, 이 그룹은 전 백악관 부비서실장이 운영하고 AI 경고를 조직적인 캠페인으로 규정합니다 ([@NeelNanda5](https://x.com/NeelNanda5/status/1841796594735552909)).
- 새로운 조직: Nathan Lambert와 Tom Zick은 오픈 사후 학습 레시피 및 인프라를 위한 비영리 단체인 Trillium Labs를 설립했습니다 ([@natolambert](https://x.com/natolambert/status/1841796594735552909)).
    - 자금 지원: 초기 지원은 Halcyon Futures와 Schmidt Sciences로부터 받았습니다.
    - Underdog: 비공개 온디바이스 AI 스타트업은 a16z, Khosla 등의 지원을 발표했습니다 ([@0xSigil](https://x.com/0xSigil/status/1841796594735552909)).
- 거버넌스 및 시장: Yoshua Bengio는 캐나다의 새로운 AI 국가 위원회에 합류했습니다 ([@Yoshua_Bengio](https://x.com/Yoshua_Bengio/status/1841796594735552909)).
    - Meta: Meta는 Virtue AI와 결별했습니다 ([@AndrewCurran_](https://x.com/AndrewCurran_/status/1841796594735552909)).
    - Nvidia: 블룸버그는 $150B의 자사주 매입 증가 후 Nvidia의 시가총액이 $5.7T에 육박하는 사상 최고치를 기록했다고 보도했습니다 ([@kimmonismus](https://x.com/kimmonismus/status/1841796594735552909)).
인기 트윗 (참여도 기준)
- Olah와 교황의 회칙에 대한 NYT 보도 — 28.7K
- Karpathy의 "육지 또는 물" 평가 — 16.4K
- Claude Code "You should know" 플러그인 — 7.3K
- Altman의 dots 언급 — 6.8K
- Muse Gadgets 발표 — 4.9K
- DeepSeek Harness 데스크톱 빌드 — 4.3K
- Altman의 Cerebras 파트너십 언급 — 4.1K
- Trillium Labs 출시 — 2.6K

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Qwen 로컬 인퍼런스: 27B 벤치마크, 파인튜닝 및 MTP
- 제 iPhone을 24GB MacBook의 보조 GPU로 만들었습니다: Qwen 3.8 27B는 29–44% 더 빠르게 사전 채우기되며, 제 iPhone이 CTX 윈도우의 일부를 유지합니다. (활동: 1192): OP는 backburner를 구축했습니다. 이는 llama.cpp 포크/분산 인퍼런스 설정으로, 24GB M4 Pro MacBook에서 Qwen 3.8 27B IQ4_XS의 일부를 10Gb/s USB-C를 통해 iPhone 17 Pro Max로 오프로드합니다. Mac은 레이어 1-40을 실행하고 활성화(activations)를 스트리밍하며, iPhone은 Metal 4 텐서 연산을 사용하여 레이어 41-64를 실행합니다. Mac 단독 대비 종단간 사전 채우기(prefill) 성능 향상은 8k에서 +35%, 16k에서 +44%, 32k에서 +29%, 48k에서 +30%로 보고되었습니다. 27k 컨텍스트의 콜드 세션은 순정 llama.cpp의 245초 / 포크 Mac 단독의 228초에서 iPhone 사용 시 168초로 개선되었습니다. 64k 컨텍스트 이상에서는 iPhone이 대신 오래된 KV 페이지(약 5.7GB까지)를 호스팅하여 196k–229k 8비트 컨텍스트 할당을 가능하게 하고, 오래된 키 어텐션을 계산합니다. 140k 컨텍스트 테스트에서는 Neural Engine으로 컴파일된 16k 키 페이지를 추가했을 때 생성 레이턴시가 토큰당 279ms에서 176ms로 개선되었습니다.
    - 기술적으로 관련된 후속 질문은 동일한 "iPhone을 보조 GPU로 사용하는" 접근 방식이 iPad, 특히 더 강력한 Apple Silicon과 잠재적으로 더 많은 RAM을 가진 고급 iPad Pro 구성으로 확장될 수 있는지에 대한 것이었습니다. 이는 iPad가 iPhone보다 더 나은 오프로드 성능을 제공하거나 더 큰 컨텍스트 윈도우 부분을 유지하여 로컬 LLM 인퍼런스를 위한 더 강력한 동반 장치가 될 수 있음을 시사합니다.
- Qwen3.8-27B-Humanlike-Chat 2.0: 인간처럼 텍스트를 작성하며, 이제 도구 호출 및 더 나은 지시 따르기 기능 포함 (활동: 805): LessThanThreeAI는 huihui-ai의 abliterated Qwen3.8-27B 위에 병합된 LoRA인 Qwen3.8-27B-Humanlike-Chat 2.0을 출시했습니다. 이 모델은 Hugging Face에서 GGUF/BF16/LoRA로 데모 Space와 함께 제공됩니다. v2는 일반 SFT를 온-정책 디스틸레이션으로 대체합니다. 학생 모델이 답변을 생성하는 동안 두 개의 교사 모델이 토큰에 점수를 매깁니다. 하나는 채팅/캐릭터 행동을 위한 v1 + 숨겨진 "인간처럼 텍스트 작성" 지시이고, 다른 하나는 지시 따르기, 도구 및 코드를 위한 기본 모델입니다. 이는 비공식적인 문자 메시지 스타일을 유지하면서 도구 사용 및 제어 가능성을 향상시킵니다. abliterated 기본 모델 대비 보고된 평가 결과는 다음과 같습니다: IFBench 37.3 → 43.7, When2Call 48 → 58, BFCL irrelevance 60 → 78, IFEval/GSM8K/BFCL simple에서는 동점/약간의 이득 (83.5 / 89.1 / 98)을 보였으나, MMLU-Pro (78.5 → 72.5) 및 LiveCodeBench (56 → 51)에서는 회귀가 있었습니다. 사용자 정의 "ishuman" 심사 벤치마크에서는 abliterated 기본 모델의 0.3% 및 공식 Qwen3.8-27B의 15.1%에 비해 23.5%로 인간이 작성한 것으로 평가되었습니다. 상위 댓글의 기술적 논의는 드물었으며, 유일하게 관련 있는 비판은 모델의 "인간적인" 어조가 광범위한 인간 대화보다는 십대들의 문자 메시지처럼 들릴 수 있다는 것이었습니다.
    - 한 댓글 작성자는 모델 전이 질문을 제기했습니다: Qwen3.8-27B-Humanlike-Chat 2.0에 사용된 동일한 인간적인 채팅 파인튜닝/정렬 방법이 Gemma 4 31B에서도 유사한 결과를 낼 수 있는지에 대한 것이었습니다. 이는 학습 레시피의 아키텍처 간 일반화 및 행동 스타일 튜닝이 더 큰 Gemma 계열 모델로 이어질 수 있는지에 대한 유일한 기술적으로 실질적인 스레드였습니다.
- 격차는 그들이 말한 것보다 작습니다: 로컬 27B가 실제 코드 테스트에서 프론티어 모델과 거의 일치합니다 (활동: 730): OP는 1× RTX 4090 24GB에서 llama.cpp b11115 + llama-swap v257을 통해 Qwen3.8-27B GGUF를 사용하여 단일 작업 DeepSWE/로컬 코드 벤치마크 실행을 보고했습니다. 특히 unsloth/Qwen3.8-27B-GGUF의 Qwen3.8-27B-UD-IQ4_XS.gguf (14.25GB)를 ctx-size 196608, IQ4_XS, q8_0 K/V 캐시, 추측성 MTP 초안 및 DeepSeek 스타일 추론 예산 4096으로 사용했습니다. 측정 결과: 115 tok/s 디코딩, 22,934 MiB 피크 VRAM, 코드 검토 작업에서 12/12, 그리고 한 DeepSWE 작업에서 40/43개의 숨겨진 테스트와 109/109개의 기존 테스트, 즉 부분적으로는 0.980이지만 이진 통과는 0이었습니다. OP는 나중에 비교를 수정했습니다: 인용된 96.6%는 모든 공개된 시험의 평균 부분 점수였으며, 해당 작업의 프론티어 서브셋은 DeepSWE v1.1 원본 데이터에서 99.8% 부분 점수와 85.3% 통과 점수였습니다. 연결된 보고서는 24GB 적합/컨텍스트 설정(컨텍스트 한계)과 작업 수준 DeepSWE 결과(로컬 신뢰도)를 다룹니다. OP는 이것이 작업별 결과이며, 27B 로컬 모델이 113개 작업 벤치마크 전반에 걸쳐 프론티어 모델과 광범위하게 일치한다는 주장이 아님을 강조합니다. 댓글 작성자들은 더 넓은 프레이밍에 회의적이었습니다: "Flash와 27B"를 모두 사용해본 한 사용자는 "격차는 현실"이라고 말했고, 다른 사용자는 프론티어 코딩 모델조차도 고르지 못하며, 약 24–72B 모델은 개별 서브태스크를 처리할 수 있지만, 인간이 더 큰 엔지니어링 작업을 모델 크기의 태스크로 분해해야 할 때 가치를 잃는 경우가 많기 때문에 결론이 틀렸다고 주장했습니다.
    - 여러 댓글 작성자들은 주장된 거의 동등한 성능이 포화된 벤치마크의 결과일 가능성이 높다고 주장했습니다: Q8에서도 로컬 27B 모델은 작고 개별적인 코딩 작업에서는 잘 수행할 수 있지만, Claude Opus와 같은 프론티어 모델이 필요한 더 어려운 실제 작업에서는 여전히 실패합니다.
    - 반복되는 기술적 반론은 코딩 평가가 프로젝트 수준 분해를 종종 과소평가한다는 것이었습니다: 24B–72B 로컬 모델은 개별 티켓을 해결할 수 있지만, 더 큰 작업 항목의 경우 문제를 모델 크기의 서브태스크로 분해하는 데 필요한 인간의 노력이 생산성 향상을 초과할 수 있습니다.
    - Gemini Flash와 로컬 27B 모델을 모두 실행해본 경험이 있는 사용자들은 특히 프론티어 모델이 더 나은 신뢰성과 작업 완료를 제공하는 중요하지 않은 코딩 워크로드의 경우 성능 격차가 여전히 상당하다고 보고했습니다.
- Qwen4Exp: am17an에 의한 MTP 추가 · Pull Request #29761 · ggml-org/llama.cpp (활동: 405): llama.cpp PR #29761은 약 17시간의 개발 끝에 aman/qwen4-opt 브랜치에 병합된 `--spec-type draft-mtp`를 통해 Qwen3.8-Flash Next에 대한 MTP 추측성 디코딩 지원을 추가합니다. Qwen3.8-Flash-Next iq4_xs에 `-np 1 -lzm` 및 `--spec-draft-n-max 3`을 적용한 DGX Spark 벤치마크 결과는 디코딩 처리량이 28.36에서 43.88 tok/s (1.55배)로 향상되었고, 레이턴시 속도 향상이 1.54배, 24개 작업에 걸쳐 평균 추측성 수용률이 0.640임을 보여줍니다. GGUF 양자화 모델은 Hugging Face에서 사용할 수 있습니다. 댓글 작성자들은 이 모델이 여전히 많은 로컬 설정에서 비실용적으로 크다고 지적했습니다: IQ4_NL GGUF는 작은 10.9MB 샤드와 102GB 샤드로 분할되어, Qwen 3.8 27B에서 쉽게 전환할 수 있다는 아이디어를 약화시킵니다. 한 댓글 작성자는 Gufo도 MTP를 지원한다고 언급했습니다.
    - 한 댓글 작성자는 MTP를 활성화하면 테스트에서 인퍼런스가 더 느려졌다고 보고하며, 이는 MTP 헤드의 수용/적중률이 낮은 매우 큰 전체 아키텍처보다 밀집 모델에 더 유용할 수 있다고 주장했습니다. 그들의 가설은 MTP 헤드가 더 큰 모델의 동작을 충분히 효과적으로 예측/압축할 수 없어 추측성 디코딩 이점을 줄인다는 것입니다.
    - 한 사용자는 Gufo가 이미 MTP를 지원한다고 언급하며, 이는 llama.cpp가 Qwen 스타일 실험 모델을 위한 기존 MTP 지원 도구/백엔드를 따라잡고 있음을 시사합니다.
    - 또 다른 댓글 작성자는 llama.cpp GGUF 인퍼런스가 자신의 워크로드에 "훨씬, 훨씬 느렸기" 때문에 tabbyapi를 통해 EXL3 버전을 사용해왔다고 말했습니다. 그들은 이 PR 이후에 다시 테스트할 계획이었지만, 이전 경험에 따르면 EXL3/tabbyapi가 Qwen4Exp/MTP 지원에 대한 성능 기준점으로 여전히 비교될 수 있음을 시사합니다.

### 2. 로컬 에이전트 툴링: 결정 모델 및 MCP
- Pi 1.0 출시 - MCP 지원이 이제 기본적으로 포함되었습니다 (Activity: 679): Earendil은 최소한의 에이전트 하네스인 Pi 1.0의 안정 버전을 출시했으며, Codemode는 이제 기본적으로 네이티브 MCP 지원과 더불어 비-LLM/이미지 모델 지원, 가상 모델 확장, 지연된 툴 로딩, Anthropic 캐시 워밍, 대화 중 시스템 메시지 및 TUI 업데이트를 포함합니다. 이번 릴리스는 또한 터미널/코딩 에이전트 워크플로우를 넘어 장기 실행 에이전틱 애플리케이션을 위한 실험적인 MIT 라이선스 Pi Durable을 도입하면서도, Pi의 최소한의/확장 가능한 아키텍처를 유지합니다. 주요 댓글들은 이름의 모호성—'pi'가 많은 AI/개발 툴과 충돌한다는 점—에 초점을 맞추었으며, Codemode가 무엇인지에 대한 설명을 요청했습니다. 한 댓글 작성자는 Earendil이 MCP 지원에 대해 입장을 번복한 근거를 담은 게시물인 “You said no MCP”를 링크했습니다. 해당 스레드는 프로젝트 정신에 기반한 제작자의 초기 반대에도 불구하고, MCP가 이제 네이티브하게/기본적으로 포함되었으며, 사용자들은 이를 툴/서버 통합 워크플로우를 위한 “필수적인 추가”로 평가하고 있다고 언급합니다.
- Clef: Cloudflare의 오픈 웨이트 결정 모델 (Activity: 619): Cloudflare는 로컬/자체 호스팅 사용을 위한 오픈 웨이트 “결정 모델”인 Clef를 발표했습니다. 한 주요 댓글 작성자는 Clef가 Qwen3.8-27B로 사후 학습되었으며, clef-flash 또한 Qwen3.5-9B로 사후 학습되어 출시되었다고 언급했습니다. 주요 실질적인 반응은 긍정적이었습니다. 댓글 작성자들은 Clef가 로컬 모델 생태계의 공백을 메우고 있다고 보며, 직접 벤치마크하기를 열망했습니다. 댓글 작성자들은 Cloudflare Clef가 Qwen3.8-27B로 사후 학습되었으며, 더 작은 clef-flash 변형은 Qwen3.5-9B로 사후 학습되어 로컬 인퍼런스 사용 사례를 위한 잠재적으로 중요한 오픈 웨이트 “결정 모델”로 평가했습니다. 제기된 기술적 우려는 양자화 후, 특히 Q8 미만에서 Clef의 품질이 어떻게 유지되는지였습니다. 로컬 배포는 낮은 비트 양자화 변형에 의존할 가능성이 높고, 결정 모델의 동작은 공격적인 압축 하에서 비선형적으로 저하될 수 있기 때문입니다. 벤치마크 논의는 Laya, Kev 9B, DiffusionGemma Jev와 같은 모델과의 비교에 초점을 맞추었지만, 한 댓글 작성자는 평가 세트가 너무 약하다고 비판하며 Clef가 약한 오픈 Jev 기준선보다는 jevbench의 선두 모델과 비교되어야 한다고 주장했습니다.
- llama.cpp의 새로운 기능: 결정 모델 (Activity: 574): 이 게시물은 llama.cpp의 결정 모델 지원을 발표합니다. 이는 순전히 자유 형식 생성기라기보다는 컨트롤러/분류기—행동, 연속 또는 행동 선택 중에서 선택하는—처럼 작동하도록 의도된 로컬 “Jev/Jeff-유사” 모델입니다. 제공된 댓글에서는 벤치마크 수치나 저수준 구현 세부 정보는 논의되지 않았습니다. 제기된 주요 구체적인 사용 사례는 로컬 롤플레이 모델을 조종하여 캐릭터가 “장면 중간에 궤도를 벗어나는 것”을 방지하는 것이었습니다. 댓글 작성자들은 Jev가 방어 가능한 제품/카테고리인지에 대해 회의적이었으며, 이 아이디어는 “해자가 없었고” 많은 Jev-유사 모델로 빠르게 복제되었다고 주장했습니다. 다른 이들은 가능한 에이전트/롤플레이 제어 외에는 이 모델들이 실용적으로 어디에 유용한지 여전히 모른다고 말했습니다. 한 댓글 작성자는 결정 모델을 본질적으로 제약된 분류 루프로 설명합니다. 허용된 클래스를 포함하는 JSON 스키마와 구조화된/비구조화된 입력을 제공한 다음, 모델이 항목당 정확히 하나의 카테고리를 선택하도록 하는 방식입니다. 기술적인 질문은 llama.cpp의 새로운 지원이 일반적인 프롬프트 제약 JSON 분류를 넘어 의미 있는 인퍼런스 시간 동작을 추가하는지, 아니면 주로 로컬 모델의 워크플로우를 표준화하는지 여부입니다. 제기된 한 가지 실용적인 사용 사례는 긴 장면 동안 이탈을 줄이기 위해 로컬 롤플레이 에이전트에 결정 모델을 적용하는 것입니다. 즉, 생성 전에 상태/의도 제약을 강제하기 위해 보조 모델 또는 결정 단계를 사용하는 것입니다. 해당 스레드는 벤치마크나 구현 결과를 보고하지는 않지만, 캐릭터 일관성 및 장면 상태 관리를 위한 잠재적인 제어 계층 패턴을 강조합니다.

## 덜 기술적인 AI 서브레딧 요약
> /r/Singularity, /r/Oobabooga, /r/MachineLearning, /r/OpenAI, /r/ClaudeAI, /r/StableDiffusion, /r/ChatGPT, /r/ChatGPTCoding, /r/aivideo, /r/aivideo

### 1. Gemini 4 Argon 접근 제한에 대한 반발
- Google One AI 플랜을 방금 취소했습니다. (Activity: 1838): 원글 작성자는 Google의 유료 Google One AI Pro 티어가 더 이상 프론티어 Gemini 모델에 대한 접근을 제공하지 않는다고 주장합니다. 주장된 Gemini 4 Argon 발표 이후, 접근은 기업 “Fairwind” 파트너, 유료 API 사용자, 그리고 향후 출시될 Google AI Ultra 티어로 제한되며, Pro 사용자들은 Gemini 3.8 Flash에 머물러 있다고 설명합니다. 그들은 이것이 고급 추론 모델과 관대한 제한이 더 광범위하게 제공되었던 Gemini 2.5 Pro 시대에서의 퇴보라고 주장하며, Anthropic/OpenAI 구독이 표준 유료 사용자에게 프론티어 모델을 제공한다고 주장하는 것과 대조합니다. “인상적인 벤치마크 차트”와 1M 토큰 출력 한도에 대한 주장 외에는 구체적인 벤치마크 수치는 제공되지 않습니다. 주요 댓글들은 대부분 불만을 일축했습니다. 한 사용자는 주로 Google 저장 공간 때문에 구독하고 AI는 보너스로 여긴다고 말했으며, 다른 이들은 게시물이 Gemini가 작성했거나 새 계정의 봇/홍보 활동이라고 주장하며 게시물의 진위 여부를 의심했습니다. 한 댓글 작성자는 Google/Anthropic/OpenAI의 월 20달러 AI 구독 티어가 생산 등급 접근보다는 제약된 시험판처럼 기능하며, “Pro” 브랜딩에도 불구하고 지속적인 워크로드에 대한 실질적인 제한이 있음을 암시한다고 주장했습니다. 그들은 또한 기본 인퍼런스 비용을 고려할 때 Google이 Google One AI Pro 구독에 보조금을 지급하거나 손실을 보고 있을 수 있다고 제안했습니다. 출시 관련 설명에서는 Gemini Ultra가 먼저 접근 권한을 받는 것으로 보이지만, Google은 Astra와 같은 기능에 대한 Pro 티어 접근을 명시적으로 배제하지 않았다고 언급했습니다. 댓글 작성자는 이를 확정적인 영구적인 티어 제외라기보다는 일반적인 단계별 소프트웨어 출시로 보았습니다.
- 대중이 아직 사용할 수 없는 모델을 왜 공개적으로 발표하는가?? (Activity: 1624): 해당 이미지는 Google/Gemini의 “Gemini 4 Argon” 발표라고 주장되는 스크린샷으로, 소프트웨어 엔지니어링, 지식 작업 및 사이버 보안 방어 분야에서 프론티어 성능과 극도로 큰 1M 토큰 출력 한도를 주장합니다: image. 이 게시물의 기술적 중요성은 주로 모델 출시 커뮤니케이션에 관한 것이지 평가에 관한 것이 아닙니다. 제목은 Google이 사용자에게 접근 가능하기 전에 모델을 공개적으로 발표하는 이유에 의문을 제기하며, 이미지 자체는 벤치마크, API 세부 정보, 가격 또는 가용성 타임라인을 제공하지 않습니다. 댓글 작성자들은 이를 Anthropic의 “mythos”와 Google의 주장된 “3.5 pro” 처리 방식을 포함한 이전의 “발표되었지만 사용 불가능한” 모델 출시와 비교합니다. 지배적인 견해는 회의적입니다. 사용자들은 좌절할 수 있으며, 한 댓글 작성자는 이 발표가 “순전히 투자자들을 위한 것”이라고 추측합니다.

### 2. Claude Opus 5.5 퇴보 보고
- Opus 5.5 너프 - 측정 방법, 감지 방법, 소송 방법 (Activity: 2722): 게시자는 Anthropic Opus 5.5가 복잡한 C++/3D/물리/Blender MCP 워크로드에서 출시 후 5~6일 만에 급격한 퇴보를 보였다고 주장하며, 비정상적인 문구와 낮은 코드/출력 품질을 언급했습니다. 또한 양자화, 라우팅 또는 부하 시 서빙 최적화와 같은 잠재적 변화를 감지하기 위해 정확한 출시 당일 프롬프트/출력과 레이턴시 측정을 보존할 것을 권장합니다. 그들은 이를 Digital Content Directive 2019/770에 따른 잠재적인 EU 소비자법 문제로 간주하며, 특히 제7-8조의 적합성 기대치와 제19조의 변경/철회 통지 의무를 언급했습니다. 출시 벤치마크와 “가장 유능한 모델” 마케팅이 강제 가능한 기대치를 설정할 수 있다고 주장합니다. 댓글들은 폐쇄형 모델 제공업체가 모델을 조용히 저하시키거나 재라우팅할 수 있으며 독립적인 감사가 필요하다는 점에 대체로 동의했지만, 재현 가능한 벤치마크나 직접적인 증거를 제공하는 댓글 작성자는 없었습니다. 한 댓글 작성자는 Higgsfield 출력에서도 유사하게 인지된 품질 저하를 보고하며, 초기에는 강력한 생성을 보였으나 이후 크레딧이 낭비되었다고 설명했습니다. 댓글 작성자들은 주장된 폐쇄형 모델 저하의 핵심 측정 문제를 제기했습니다. Anthropic의 호스팅 모델 가중치, 프롬프트, 라우팅 및 서빙 구성이 불투명하기 때문에, 사용자들은 독립적인 감사, 고정된 벤치마크 프롬프트, 반복 샘플링 및 과거 기준선 없이는 퇴보 또는 “너프”를 증명하기 어렵다고 주장합니다. 한 사용자는 특히 “효과적인 테스트 또는 신뢰할 수 있는 너프 추적 사이트”를 요청하며, 일화적인 비교보다는 제3자 종단 평가에 대한 수요를 강조했습니다. 여러 사용자가 적용된 워크플로우 전반에서 Opus 5.5 동작의 일화적인 퇴보를 보고했습니다. 한 사용자는 이제 코딩 버그를 잡기 위해 Gemini 3.8 Flash의 도움이 필요하다고 주장했으며, 다른 사용자는 Higgsfield 디자인/렌더 출력이 초기에는 강력한 결과를 보였으나 이후 하락하여 크레딧을 낭비했다고 말했습니다. 이러한 보고서는 통제된 벤치마크는 아니지만, 사용자들은 버그 찾기 정확도, 디자인/렌더 프롬프트 충실도, 그리고 일별 출력 일관성과 같은 종류의 작업을 추적하기를 원한다는 점을 시사합니다.
- 음, 알겠습니다. 처음에는 다른 사람들을 믿지 않았지만, Opus 5.5에 갑자기 뭔가 이상한 점이 있습니다 (Activity: 2045): 한 Claude Code Enterprise PAYG 사용자는 월별 제한 재설정 후 Claude Opus 5.5 Med 동작에서 급격하게 인지된 퇴보를 보고했습니다. 아키텍처 우선, DRY/SOLID, 토큰 효율적인 구현에서 장황한 서문, 중복 코드, “슬롭코드”, 그리고 이전 Opus 5 동작과 유사한 토큰 소모로 바뀌었다는 것입니다. 그들은 사용량이 약 1시간 만에 약 70%에서 90%로 급증했으며, 이는 이전 주에 하루 약 12시간의 O5.5 집중 사용 동안 지출 한도 증가 요청이 없었던 것과 대조된다고 주장하며, 비교를 위해 일일 비용/토큰 데이터를 제공합니다. 한 댓글 작성자는 외부 감성 추적을 인용하며, modelsentiment.com에서 Opus 5.5 Reddit 감성이 9월 25~28일 71~73/100에서 어제 58, 오늘 55로 하락했다고 밝혔습니다. 이는 백엔드 모델 변경보다는 의견을 측정한다는 점을 언급했습니다. 주요 댓글들은 Anthropic이 출시 홍보 이후 컴퓨팅을 줄이거나, 조용히 라우팅을 변경하거나, 토큰 회계를 변경했을 수 있다고 추측하지만, 직접적인 증거는 제공되지 않습니다. 주요 논쟁은 신뢰/신뢰성입니다. 사용자들은 인지된 출시 후 퇴보보다는 안정적인 모델 동작과 투명한 배포/버전 관리를 원합니다. Reddit 감성을 추적하는 한 댓글 작성자는 Claude Opus 5.5의 급격한 하락을 보고하며, modelsentiment.com에서 9월 25~28일 71–73/100으로 안정적이었던 점수가 어제 58, 오늘 55로 떨어졌다고 주장합니다. 그들은 이것이 모델 동작보다는 사용자 의견을 측정하는 것이므로 백엔드 변경을 확인할 수는 없지만, 갑작스러운 인지된 품질 퇴보를 나타낼 수 있다고 언급합니다. 여러 사용자가 Opus 5.5의 의심되는 기능 퇴보를 설명하며, 특히 지시 따르기 및 다중 부분 프롬프트 준수와 관련이 있다고 말했습니다. 한 사용자는 모델이 이제 “3가지를 언급하고 2가지만 인정하며,” 심지어 이의를 제기하면 누락을 인지한다고 말했습니다. 또 다른 사용자는 모든 작업에 대해 “xhigh effort” 모드로 되돌아갔다고 말하며, 이는 일반 설정에서 기본 신뢰도가 낮아지거나 추론/준수 능력이 감소했음을 암시합니다. 제기된 한 가지 기술적 가설은 Anthropic이 출시/벤치마킹 동안 일시적으로 더 많은 컴퓨팅을 할당했다가 나중에 인퍼런스 리소스를 줄이거나 토큰 회계를 변경하여 인지된 품질 저하로 이어졌을 수 있다는 것입니다. 이는 추측성이고 검증되지 않았지만, 불만은 재현성과 신뢰성에 집중됩니다. 사용자들은 동일한 제품명 하에서 조용히 변경되는 것보다는 출시 후 모델 동작이 안정적으로 유지되기를 원합니다.

### 3. AI 비디오 모델 및 모션 제어
- MiniMax에서 오비팅 LoRA + 첫 프레임 및 마지막 프레임이 환상적인 결과를 제공합니다 (Activity: 2263): 한 사용자가 첫/마지막 프레임 컨디셔닝을 통해 고정된 피사체의 360° 궤도 샷을 생성하기 위한 MiniMax-H3 LoRA를 공유했습니다: pablodawson/MiniMax-H3-360-Orbit-LoRA. 프롬프트는 장면을 정지된 순간으로 명시적으로 제약합니다—객체/자세 변형 없음, 드리프트 없음, 연속적인 동작 없음—따라서 카메라 시차만이 유일한 움직임 소스가 되어, 다운스트림 재구성 워크플로우에 적합한 더 깨끗한 의사-볼륨 출력(pseudo-volumetric outputs)을 목표로 합니다. 링크된 Reddit 데모 비디오가 언급되었지만, Reddit이 403 Forbidden을 반환하여 비디오 URL을 확인할 수 없었습니다. 댓글 작성자들은 이 LoRA가 3D 에셋 생성에 특히 유용하다고 평가했습니다. 한 사용자는 생성된 궤도 클립을 Opus에 넣어 3D 모델 생성을 위한 스냅샷을 추출할 것을 제안하며, 이는 스타일 보존을 개선한다고 주장했습니다. 또 다른 댓글 작성자는 이러한 궤도 일관성 비디오 생성이 기존 영화의 소비자 볼륨메트릭/VR 시청을 더 가깝게 만든다고 추론했습니다. 한 댓글 작성자는 궤도/생성된 3D 비디오 스니펫이 Opus에 입력되어 3D 모델 생성을 위한 스냅샷을 추출하도록 지시되는 워크플로우를 설명합니다. 그들은 비디오 참조 없이 모델에 프롬프트를 제공하는 것보다 이것이 스타일 캡처를 상당히 개선한다고 보고하며, 궤도 비디오가 강력한 다중 시점 컨디셔닝 소스 역할을 한다고 제안합니다. 출력에서 발견된 기술적 아티팩트는 일관성 없는 모션 분할입니다. 사람은 효과적으로 정지된 상태를 유지하는 반면, 자동차, 머리카락, 배경 폭발과 같은 보조 요소는 계속 움직입니다. 이는 MiniMax가 첫/마지막 프레임 제약에서 피사체 자세를 보존하면서도 여전히 환경 역학을 합성하여 부분적인 애니메이션 불일치를 초래할 수 있음을 시사합니다.
- Griffin, 비디오 튜링 테스트를 통과한 최초의 인간 상호작용 모델이자 전이중 AI 비디오 부문에서 이미 NVIDIA 벤치마크 1위 - 다른 시스템이 약 3%인 반면, 44%의 사람들이 실제 사람이라고 생각했습니다 (Activity: 2018): 한 Reddit 게시물은 “인간 상호작용 모델”로 설명되는 Griffin이 비디오 튜링 테스트를 통과한 최초의 시스템이며, NVIDIA의 전이중 AI 비디오 벤치마크에서 1위를 차지했다고 주장합니다. 참가자의 44%가 이를 실제 사람으로 판단했으며, 다른 시스템은 약 3%였습니다. 링크된 Reddit 비디오는 403 Forbidden 응답으로 인해 독립적으로 접근할 수 없었으므로, 제공된 출처에서 벤치마크 세부 정보, 방법론 및 모델 아키텍처를 확인할 수 없습니다. 댓글들은 대부분 비기술적이었습니다. 한 사용자는 인간/AI 공개가 뒤바뀌는 것에 대해 농담했으며, 다른 사용자는 이 기술이 불필요하며 약탈적인 애플리케이션에 사용될 가능성이 높다고 주장했습니다. 한 댓글 작성자는 44%의 인간 식별률이 기술적으로 중요하다는 점을 강조했습니다. 인간은 일반적으로 미묘한 얼굴, 타이밍 및 행동 이상에 매우 민감하며, 이는 CGI/애니메트로닉스에서 불쾌한 골짜기 문제의 기반이 되기 때문입니다. 그들은 이것이 Griffin이 이전의 “가짜 인간” 시스템을 상당히 넘어섰음을 시사하며, 특히 다른 시스템이 동일한 비디오 튜링 스타일 벤치마크에서 약 3%를 기록한다는 게시물의 주장과 비교할 때 더욱 그렇다고 주장했습니다. 제기된 한 가지 기술적으로 관련 있는 실제 악용 사례는 AI 생성 구직자였습니다. 합성 후보자들이 지원하고, 비디오 인터뷰를 진행하고, 고용된 다음, 내부 플랫폼 접근 권한을 얻거나 배송된 작업 장비를 훔친다고 주장됩니다. 댓글 작성자는 약한 심사 또는 제한된 배경 조사를 가진 대기업들이 이러한 AI 매개 인터뷰를 감지하지 못할 수 있으며, 이는 전이중 비디오 에이전트가 신원 확인 및 채용 보안 위험을 실질적으로 악화시킬 수 있음을 암시한다고 언급했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
