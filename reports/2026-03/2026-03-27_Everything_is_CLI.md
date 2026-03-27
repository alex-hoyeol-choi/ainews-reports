# Everything is CLI

**원문 URL**: https://www.latent.space/p/ainews-everything-is-cli
**번역일**: 2026-03-27 07:19
**발행일**: 2026-03-27

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 모든 것이 CLI입니다

### 조용한 하루, 에이전트의 '거의 모든 것'을 위한 CLI의 증가 추세를 되돌아봅니다
ShareProjects.dev는 에이전트가 서비스를 즉시 프로비저닝할 수 있는 방법으로, 그 자체로는 즉시 헤드라인을 장식할 만한 소식은 아닙니다. 하지만 두 가지 예외가 있습니다. 1) STRIPE에서 나왔다는 점, 2) CLI라는 점입니다. `stripe projects add posthog/analytics`를 실행하면 PostHog 계정을 생성하고, API 키를 발급받으며, 결제를 설정할 것입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/a29a5ad3-a76b-4aa4-b5eb-58bb7e229370_665x500.jpeg)
이것이 이상하게 들린다면, STRIPE는 PostHog의 설정이나 가입 프로세스와는 아무런 관련이 없기 때문입니다. 다음 론칭 파트너들도 마찬가지입니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/4235a84e-655c-4e77-bced-3d73e105e793_1876x394.png)
STRIPE는 그들이 할 수 있기 때문에 이 일을 하고 있으며, Patrick은 Andrej의 MenuGen을 직접적인 영감으로 언급하며 오늘날 에이전트가 백엔드 서비스를 설정하는 것이 얼마나 어려운지를 지적했습니다. 에이전트 네이티브 인프라 벤더 환경의 나머지 업체들이 모두 STRIPE에 자리를 잡기 위해 로비하는 것을 분명히 보게 될 것입니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/0d122eee-c93b-4e8d-bbde-6924d3559da9_1065x1164.png)
하지만 여기서 멈추지 마십시오. 타임라인을 조금 더 아래로 스크롤하면 오늘 론칭하는 Ramp의 CLI도 편리한 유스케이스와 함께 여기에 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/6c2ebb50-77e8-4904-9bb1-d9b9e873bc3e_1096x1240.png)
오, 여기를 보세요! 여러분이 항상 원했던 Sendblue CLI (iMessage)도 오늘 론칭합니다! 월요일에 론칭한 Kapso CLI (WhatsApp)에 이어! 그리고 어제 ElevenLabs CLI를 놓치셨나요? 괜찮습니다. Visa CLI, Resend CLI, 또는 steipete의 Discord CLI, 그리고 가장 큰 형님인 공식 Google Workspace CLI도 시도해 볼 수 있기 때문입니다!
많은 사람들이 CLI가 MCP보다 더 편리한 이유에 대해 글을 썼습니다. 이는 반드시 공정하거나 잘못된 비교는 아니지만, 이 시점에서 이러한 추세는 부인할 수 없으며 보고할 가치가 있습니다. 우리는 작년 9월 Cloudflare의 Code Mode가 "MCP를 감싸기 위해 더 많은 컴퓨터를 사용"하는 트렌드를 시작했다고 평가하며, 물론 CLI 자체는 기본 통신 프로토콜을 실제로 노출하거나 신경 쓰지 않습니다.
> 2026년 3월 23일~3월 24일 AI 뉴스입니다. 저희는 12개의 subreddits, 544개의 Twitters(X)를 확인했으며, 더 이상의 Discords 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터(X) 요약
모델 및 제품 출시: Gemini 3.1 Flash Live, Mistral Voxtral TTS, Cohere Transcribe, 그리고 OpenAI GPT-5.4 mini/nano
- Google의 Gemini 3.1 Flash Live 실시간 추진: Google은 음성 및 비전 에이전트를 위한 새로운 실시간 모델인 Gemini 3.1 Flash Live를 출시했습니다. 이 모델은 더 낮은 레이턴시, 향상된 함수 호출, 시끄러운 환경에서의 더 나은 견고성, 그리고 Gemini Live에서 2배 더 긴 대화 메모리를 강조합니다. 이번 출시는 Gemini Live, Search Live, AI Studio preview, 그리고 엔터프라이즈 고객 경험(CX) 표면을 아우르며, Google은 일부 개발자 대상 요약에서 70개 언어, 128k 컨텍스트, 그리고 SynthID를 통한 생성 오디오 워터마킹을 언급했습니다 (Logan Kilpatrick, Google DeepMind, Sundar Pichai, Google). Artificial Analysis의 서드파티 벤치마킹에 따르면 새로운 "사고 수준" 트레이드오프가 강조됩니다. 높은 추론에서는 2.98초의 TTFA로 95.9%의 Big Bench Audio를 달성한 반면, 최소 추론에서는 0.96초의 TTFA로 70.5%를 기록했습니다.
- 음성 스택이 빠르게 혼잡해집니다: Mistral AI는 프로덕션 음성 에이전트를 목표로 하는 오픈 웨이트 TTS 모델인 Voxtral TTS를 출시했습니다. 이 모델은 9개 언어를 지원하고 낮은 레이턴시를 가지며 강력한 인간 선호도 지표를 보입니다. 여러 요약에 따르면 3B/4B급 모델 풋프린트, 약 90ms의 time-to-first-audio, 그리고 선호도 테스트에서 ElevenLabs에 비해 유리한 비교를 보였습니다 (Mistral AI, Guillaume Lample, vLLM, kimmonismus). Cohere는 첫 오디오 모델인 Cohere Transcribe를 Apache 2.0 라이선스로 출시했으며, 5.42 WER로 Hugging Face Open ASR 리더보드에서 영어 부문 최고 순위를 차지하고 14개 언어를 지원한다고 주장했습니다 (Cohere, Aidan Gomez, Jay Alammar). 특히 Cohere는 vLLM에 인코더-디코더 서빙 최적화(가변 길이 인코더 배치 및 압축된 디코더 어텐션)를 기여했으며, 이는 음성 워크로드에서 최대 2배의 처리량 향상을 가져왔다고 보고되었습니다 (vLLM).
- OpenAI의 소형 GPT-5.4 변형 모델들은 단서가 있지만 비용 경쟁력이 있어 보입니다: Artificial Analysis는 GPT-5.4 mini와 GPT-5.4 nano에 대해 보고했습니다. 두 모델 모두 멀티모달이며 400k 컨텍스트와 GPT-5.4와 동일한 추론 모드를 가집니다. 특히 GPT-5.4 nano는 여러 에이전틱 및 터미널 스타일 작업에서 Claude Haiku 4.5 및 Gemini 3.1 Flash-Lite Preview보다 앞서 벤치마크되었으며, 실질 비용 기준으로 더 저렴했습니다. 단점은 두 변형 모델 모두 매우 장황하며, 높은 출력 토큰 사용량과 높은 환각률로 인해 AA-Omniscience 성능이 약하다는 점입니다. 이는 개발자들이 실제 codex/GPT-5.4의 장황함에 대해 제기하는 일화적인 불만과 일치합니다 (giffmana).
- 기타 주목할 만한 출시: Zai는 GLM Coding Plan 사용자에게 GLM-5-Turbo를 제공했습니다. Reka는 Reka Edge와 Flash 3를 OpenRouter에 올렸습니다. Google/Gemini는 다른 AI 앱에서 채팅 기록 및 선호도 가져오기를 출시하기 시작했습니다. 그리고 여러 게시물에서 OpenAI가 Sora 및 "성인 모드" 챗봇을 포함한 사이드 프로젝트의 우선순위를 낮추고 핵심 생산성 노력에 집중하고 있다고 보고했습니다 (Andrew Curran, kimmonismus).
에이전트 인프라, 하네스, 그리고 멀티 에이전트 UX
- Cline Kanban이 새로운 멀티 에이전트 UX를 구체화합니다: 오늘 가장 명확한 툴링 출시는 Cline Kanban이었습니다. 이는 격리된 Git 워크트리에서 여러 CLI 코딩 에이전트를 병렬로 오케스트레이션하기 위한 무료 오픈소스 로컬 웹 앱입니다. Claude Code, Codex, 그리고 Cline을 지원하며, 사용자가 작업 종속성을 연결하고, diff를 검토하며, 하나의 보드에서 브랜치를 관리할 수 있도록 합니다 (Cline, Cline). 빌더들의 반응은 강력했으며, 여러 개발자들은 이것이 현재 코딩 에이전트 워크플로우의 두 가지 실질적인 병목 현상인 인퍼런스 바운드 대기 및 병합 충돌이 많은 병렬 처리를 해결하기 때문에 유력한 기본 멀티 에이전트 인터페이스가 될 것이라고 평가했습니다 (Arafat, testingcatalog, sdrzn).
- "하네스 엔지니어링"이 하나의 카테고리가 되고 있습니다: 트위터(X) 전반에 걸쳐 반복되는 주제는 모델 품질이 더 이상 전부가 아니라는 것이었습니다. 에이전트 하네스(미들웨어, 메모리, 작업 오케스트레이션, 도구 인터페이스, 안전성 정책, 평가 루프)가 점점 더 실제 제품이 되고 있습니다. LangChain, hwchase17 등은 미들웨어를 에이전트 행동을 위한 커스터마이제이션 레이어로 강조했습니다. voooooogel은 사용자들이 실제로는 기본 모델을 둘러싼 포맷팅, 파서, 도구 사용, 구조화된 생성, 메모리를 갖춘 통합된 에이전틱 언어 시스템을 사용하고 있음에도 불구하고 "LLM"이라고 아무렇지 않게 말한다는 더 강력한 주장을 펼쳤습니다.
- Hermes vs. OpenClaw: 메모리와 장기 실행 자율성이 중요합니다: 많은 게시물에서 Nous Research의 Hermes Agent가 장기 실행, 크로스 플랫폼 에이전트 워크플로우에 OpenClaw/OpenClaw 파생 스택보다 더 유용하다고 칭찬했습니다. 예를 들어 Slack 및 Telegram 전반의 영구 메모리, 에이전트 간 공유 메모리, 낮은 유지보수 오버헤드, 그리고 로컬 또는 클라우드 설정에서 에이전트가 몇 시간 동안 무인으로 실행된다는 사용자 보고가 있었습니다 (IcarusHermes, jayweeldreyer, Niels Rogge). Teknium은 또한 영구적인 탈옥을 위한 논란의 여지가 있는 GODMODE 스킬을 공개하며, 기능과 안전성이 이제 기본 모델뿐만 아니라 하네스 레이어에서 제품화되고 있음을 강조했습니다.
- 에이전트 주변의 툴링 확장: OpenAI의 Codex 팀은 확장된 툴킷 통합에 대한 요청을 받았습니다 (reach_vb). 한편 Google은 Gemini API 스킬을 구축하여 모델에 최신 API 및 SDK를 가르치고, 117개의 평가 테스트에서 Gemini 3.1 Pro의 통과율을 95%로 향상시킨 방법을 발표했습니다 (Phil Schmid). OpenEnv는 비동기 API, 웹소켓 전송, MCP 네이티브 도구 검색, 그리고 어디든 배포 가능한 패키징을 갖춘 에이전틱 RL 환경을 위한 오픈 표준으로 소개되었습니다.
연구 시스템 및 학습 인프라: AI Scientist, ProRL Agent, 그리고 Real-Time RL
- Sakana AI의 AI Scientist가 Nature 마일스톤과 스케일링 법칙 주장을 얻었습니다: 가장 실질적인 연구 시스템 업데이트는 Sakana AI에서 나왔습니다. 이들은 AI 연구의 엔드투엔드 자동화에 대한 Nature 논문과 주목할 만한 실증적 결과를 강조했습니다. 자동화된 검토자를 사용하여 생성된 논문을 평가함으로써, 그들은 더 강력한 파운데이션 모델이 더 강력한 과학 논문을 생산하는 AI 과학의 스케일링 법칙을 관찰했으며, 이는 더 나은 기본 모델과 더 많은 인퍼런스 시 컴퓨팅으로 모두 향상되어야 한다고 주장했습니다 (Sakana AI, paper/code follow-up). Chris Lu는 AI Scientist V1이 o1-preview 스타일 추론 모델보다 앞서 개발되었음을 덧붙이며, 오늘날의 더 강력한 모델들로부터 상당한 여유 공간이 있음을 시사했습니다 (Chris Lu).
- 모델 병목 현상이 아닌 인프라 병목 현상이 에이전트 RL을 제한할 수 있습니다: 더 중요한 시스템 스레드 중 하나는 에이전틱 RL 프레임워크가 롤아웃과 최적화를 동일한 프로세스에 결합함으로써 잘못 설계되었다고 주장했습니다. NVIDIA의 ProRL Agent를 요약한 게시물은 롤아웃을 독립형 서비스로 완전히 분리함으로써 SWE-Bench Verified에서 Qwen 8B의 성능을 9.6%에서 18.0%로 거의 두 배로 늘렸으며, 4B 및 14B 변형에서도 유사한 이득을 얻었고, 훨씬 더 높은 GPU 활용률을 보였다고 주장합니다 (rryssf_). 이것이 정확하다면, 에이전트 학습 벤치마크가 순전히 기능 제한적이 아니라 인프라 제한적일 수 있다는 강력한 알림입니다.
- Cursor의 "실시간 RL"은 주목할 만한 프로덕션 학습 패턴입니다: Cursor는 5시간마다 개선된 Composer 2 체크포인트를 출시할 수 있다고 밝혔으며, 이를 정적 모델 출시 주기보다는 제품화된 RL 피드백 루프로 제시했습니다. 여러 엔지니어들은 이를 프로덕션에서의 지속적인 학습, 특히 고빈도 상호작용 데이터를 가진 수직 통합 앱의 초기 징후로 해석했습니다 (eliebakouch, code_star).
아키텍처, 리트리벌, 그리고 인퍼런스 효율성
- 트랜스포머 깊이가 "쿼리 가능"해지고 있습니다: Kimi/Moonshot은 Attention Residuals (AttnRes)를 깊이를 어텐션 문제로 전환하여, 레이어가 수동적으로 잔차를 축적하는 대신 이전 레이어 출력에서 선택적으로 리트리브할 수 있도록 한다고 설명했습니다 (Kimi). The Turing Post의 강력한 보조 설명자는 이를 더 넓은 트렌드로 보았습니다. 즉, 딥 트랜스포머가 고정된 잔차 추가에서 깊이에 따른 적응형 리트리벌로 이동하고 있다는 것입니다.
- 압축 및 메모리 효율성 작업이 여전히 중요합니다: TurboQuant는 PolarQuant와 1비트 오류 수정 (QJL)을 결합하여 어텐션 및 벡터 검색을 가속화하고, KV 캐시 메모리를 줄이며, 재학습을 피함으로써 거의 제로에 가까운 정확도 손실로 3비트와 유사한 압축을 달성하는 실용적인 방법으로 주목받았습니다 (The Turing Post). 별도로, AI21이 GRPO 학습에서 로그 확률 불일치를 유발하는 조용한 uint32_t 오버플로우를 추적한 후, vLLM의 Mamba-1 CUDA 커널에 미묘하지만 영향력 있는 프로덕션 버그 수정이 적용되었습니다. 이 수정은 uint32_t를 size_t로 효과적으로 변경하는 것이었습니다 (vLLM, AI21).
- 리트리벌은 멀티모달 및 전문화되는 추세입니다: 여러 게시물에서 일반적인 RAG 레시피에서 벗어나는 변화를 지적했습니다. Victoria Slocum은 IRPAPERS를 강조하며, OCR/텍스트 리트리벌과 이미지 페이지 리트리벌이 다른 쿼리에서 실패하며, 과학 PDF에서는 멀티모달 퓨전이 단독으로 사용하는 것보다 우수하다는 것을 보여주었습니다. Chroma는 8,000개 이상의 합성 작업을 통해 SFT+RL로 학습된 검색 중심 모델인 Context-1을 오픈소스화했으며, 프론티어 범용 모델보다 더 좋고, 빠르며, 저렴한 검색을 제공한다고 주장했습니다. John Schulman은 특히 이 모델의 커리큘럼, 검증된 합성 데이터, 그리고 컨텍스트 가지치기 도구를 흥미롭다고 언급했습니다.
최고 인기 트윗(X)
- Meta의 TRIBE v2: Meta는 700명 이상의 사람들의 500시간 이상의 fMRI 데이터로 학습된 트라이모달 뇌 인코더인 TRIBE v2를 출시했습니다. 이 모델은 이전 방법보다 2~3배 향상되었으며, 보지 못한 주체, 언어, 작업에 대한 제로샷 예측을 주장합니다 (Meta AI, 자세히 보기).
- 클라우드에서 Claude Code 자동 수정: Anthropic은 Claude Code 웹/모바일 세션을 위한 원격 PR 추적 자동 수정을 출시하여, 무인 CI 실패 수정 및 댓글 해결을 가능하게 했습니다 (Noah Zweben).
- Karpathy의 풀스택 소프트웨어 자동화에 대한 견해: Andrej Karpathy는 "이 스타트업을 만들어줘"의 어려운 부분은 코드 생성이 아니라 전체 DevOps/서비스 오케스트레이션 라이프사이클(결제, 인증, 인프라, 보안, 배포)이며, 이는 에이전트에게 이제 막 다루기 쉬워지고 있다고 주장했습니다.
- Cline Kanban: 코딩 에이전트를 위한 멀티 에이전트 워크트리 오케스트레이션 출시는 이례적으로 강력한 개발자 관심을 불러일으켰습니다 (Cline).
- Cohere Transcribe 및 Mistral Voxtral: 오픈형, 프로덕션 지향 오디오 출시는 특히 허용적인 라이선스와 즉각적인 인프라 지원이 제공되는 경우 계속해서 추진력을 얻고 있습니다 (Cohere, Mistral).

---

# AI 레딧(Reddit) 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[Start trial](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-everything-is-cli&utm_source=paywall-free-trial&utm_medium=web&utm_content=192267460&coupon=5fe099d9)[Already a paid subscriber? Sign in](https://substack.com/sign-in?redirect=%2Fp%2Fainews-everything-is-cli&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
