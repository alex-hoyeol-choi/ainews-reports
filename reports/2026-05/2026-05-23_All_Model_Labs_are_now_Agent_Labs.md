# All Model Labs are now Agent Labs

**원문 URL**: https://www.latent.space/p/ainews-all-model-labs-are-now-agent
**번역일**: 2026-05-23 06:18
**발행일**: 2026-05-23

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 모든 모델 랩이 이제 에이전트 랩입니다

조용한 하루 동안, 모든 모델 랩이 에이전트 랩으로 변모함에 따라 몇 가지 인용문을 연결해 보았습니다.
다음 주 OpenAI의 IPO 신청이 예상되는 가운데, Greg는 모델 랩들이 점점 더 에이전트를 제품으로 구축하고 있다는 일련의 발언 중 최신 내용을 내놓았습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/348d0573-16b0-46d0-a852-ccaae2b6ff4f_1122x534.png)
이 인용문은 그의 전 OpenAI Labs 책임자를 포함하여 Team Big Model에서 일했던 사람들이 거의 한결같이 고수했던 입장과는 크게 달라진 것입니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/f0b62ab4-065e-4317-857e-6483330aeb08_1088x1308.png)
이는 AI21의 모델 팀이 문을 닫고 에이전트로 전환하는 것과 함께 일어났습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/f8ba4c74-81d3-4163-a6c3-752ef8ec9fe6_1076x1362.png)
심지어 유서 깊은 DeepSeek조차 처음으로 "하네스 팀"을 구축하고 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/77b428e9-bb30-464c-8dc2-827ae5accf1f_1084x426.png)
“모델보다 시스템”을 주장하는 사람들은 이를 자신들이 줄곧 말해왔던 것의 유효성을 입증하는 지점으로 받아들일 것입니다… 다만, 하네스와 함께 공동 학습된 모델이 모델에 대한 접근을 더욱 제한할 수 있는 문을 연다는 미묘한 차이가 있습니다. 만약 모델을 효과적으로 사후 학습시켜 클로즈드 소스 에이전트에서만 의미 있게 작동하도록 할 수 있다면, 모델/API 경쟁을 희생시키면서도 대다수의 사용자를 자신의 에이전트로 유도할 수 있게 됩니다.
하지만 그것은 훨씬 더 큰 논의의 주제입니다…
> 2026년 5월 4일-5월 5일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터를 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색하실 수 있습니다. AINews는 이제 Latent Space의 한 섹션임을 알려드립니다. 이메일 수신 빈도를 선택/해제하실 수 있습니다!

---

# AI 트위터 요약
에이전트 제품, 하네스, 그리고 "단순한 모델"을 넘어서는 변화
- 제품 표면이 상위 스택으로 이동하고 있습니다: 반복되는 주제는 모델 품질만으로는 더 이상 해자가 될 수 없다는 것이었습니다. 성공적인 제품은 점점 더 모델 + 하네스 + 워크플로우 + UI + 메모리 + 경제성으로 구성됩니다. @gdb는 "모델 단독으로는 더 이상 제품이 아니다"라고 직설적으로 말했으며, @dzhng는 최고 수준의 제품이 모델 <> 하네스 <> 제품의 공생을 필요로 한다고 주장했습니다. 동일한 패턴이 실제에서도 나타납니다: @signulll은 앰비언트 AI와 에이전틱 AI를 컴퓨팅 인터페이스의 새로운 접점으로 보았고, @teortaxesTex는 하네스 연구가 더 넓은 인터페이스를 탐색하는 대신 "Claude Code 복제"로 수렴될 위험이 여전히 있다고 지적했습니다.
- 코딩 에이전트 제품 차별화가 구체화되고 있습니다: OpenAI는 "codex thursday no. 6"를 통해 Appshots, /goal 개선, 잠금 상태에서의 원격 컴퓨터 사용, 주석 모드, 플러그인 공유, 분석 기능을 포함한 또 다른 중요한 Codex 업데이트를 출시했습니다. @gdb는 Appshots를 별도로 강조했으며, 사용자들은 의미 있는 워크플로우 변화를 보고했습니다: @gdb는 Codex 이전의 코딩을 기억하기 어렵다고 말했고, @reach_vb는 한 달 넘게 IDE를 열지 않았다고 말했습니다. 하지만 제품의 미흡한 부분은 여전히 남아있습니다: @theo는 T3 Code의 원격 기능을 다른 대안들보다 앞서 있다고 칭찬한 후, 후속 게시물에서 Codex의 버그가 있는 원격 워크플로우와 대조했습니다. Claude 측에서는 @ClaudeDevs가 자동 모드를 Pro 플랜으로 확장하고 Sonnet 4.6 지원을 추가했습니다; @_mohansolo는 사용자들의 반발 이후 Antigravity 2.0의 IDE 지원을 명확히 하고 패치해야 했습니다.
모델 성능, 비용 곡선, 그리고 프론티어 경쟁
- DeepSeek의 가격 정책 변화는 가장 큰 시장 신호였습니다: @deepseek_ai는 DeepSeek-V4-Pro의 75% 할인을 영구화하여, 비용/성능 프론티어를 실질적으로 변화시켰기 때문에 강한 반응을 불러일으켰습니다. @ArtificialAnlys는 자체 가격을 입력 $0.435/M, 출력 $0.87/M, 캐시된 입력 $0.0036/M으로 수량화했으며, 혼합하여 약 $0.18/M로 추정하고 V4 Pro를 지능 대 실행 비용의 파레토 프론티어에 위치시켰습니다. 그들은 V4 Pro에서 Intelligence Index를 실행하는 비용이 Gemini 3.1 Pro Preview보다 약 3배, GPT-5.5보다 약 12배, Claude Opus 4.7보다 약 19배 저렴하다고 추정합니다. 커뮤니티 반응은 @scaling01이 말했듯이 DeepSeek이 "측정하기에는 너무 저렴한 지능"을 향해 나아가는 것에 집중되었습니다. @Yuchenj_UW와 @kimmonismus는 모두 가격 인하의 규모를 강조했습니다.
- Gemini Flash는 개선되었지만, 사용 피드백은 엇갈렸습니다: @OfficialLoganK는 Gemini 3.5 Flash가 GDPval에서 3.1 Pro 대비 상당한 진전을 이루었으며, Flash가 이제 "프론티어에서 경쟁하고 있다"고 주장했습니다. @Designarena는 Design Arena에서 Gemini 3 Flash Preview보다 16단계 상승한 전체 16위에 올랐습니다. 그러나 여러 빌더들은 벤치마크 개선 대비 유용성에 대해 반론을 제기했습니다: @Alezander907은 더 높은 비용으로 브라우저 에이전트 개선이 미미하다고 보았고, @giffmana는 브랜드가 여전히 저렴함을 의미한다면 이것은 "Flash 발전"이 아니라고 주장했습니다. @jeremyphoward는 모델이 인간과 협력하기보다는 평가를 극대화하도록 최적화된 것 같다고 말했습니다. 이는 현재 도구가 정성적, HITL(Human-in-the-Loop) 판단을 경시한다고 주장한 @HamelHusain의 광범위한 평가 회의론과 일치합니다.
- Qwen과 중국 프론티어 모델들이 경쟁을 압축하고 있습니다: 공식 @Alibaba_Qwen 티저와 @ZhihuFrontier의 긴 서드파티 리뷰는 Qwen3.7-Max가 특히 지시 따르기, 컨텍스트 신뢰성, 안정성 면에서 의미 있는 진전을 보였지만, 여전히 장황함과 높은 토큰 사용량에 시달리고 있다고 묘사했습니다. 다른 곳에서는 @scaling01이 최근 ALE-Bench 실행 결과 Kimi-K2.6, DeepSeek-V4, GLM-5.1과 같은 중국 모델들이 해당 설정에서 여러 서구 모델들을 능가했다고 주장했습니다. @ArtificialAnlys는 또한 Cursor Composer 2.5가 Coding Agent 벤치마크에서 Opus 4.7보다 3~18배, GPT-5.5보다 5~32배 저렴하며, 토큰 사용량이 현저히 낮다고 보고했습니다.
프로토콜, 인프라, 그리고 에이전트 런타임 툴링
- MCP의 새로운 릴리스 후보는 실질적인 프로토콜 단순화입니다: @dsp_는 MCP 2026-07-28 릴리스 후보를 발표했으며, 핵심 변경 사항은 프로토콜이 이제 스테이트리스(stateless)라는 것입니다: 핸드셰이크 없음, 세션 ID 없음, 그리고 어떤 요청이든 어떤 서버 인스턴스에든 도달할 수 있습니다. RC는 또한 MCP Apps 및 Tasks와 같은 일등 확장(first-class extensions), 인증 강화(auth hardening), 그리고 더 명확한 사용 중단 정책(deprecation policy)을 도입합니다. 인프라 팀에게 스테이트리스는 큰 운영상의 변화입니다: 더 쉬운 스케일링, 더 간단한 로드 밸런싱, 더 적은 스티키 세션(sticky-session) 문제.
- 샌드박스와 관리형 실행이 일등 기본 요소(first-class primitives)가 되고 있습니다: @_philschmid는 Gemini Managed Agents + Interactions API를 시연하여 에이전트에게 메모리 및 코드 실행이 가능한 보안 호스팅 Linux 샌드박스를 제공했습니다. @CoreWeave는 RL, 에이전트 도구 사용 및 모델 평가를 위한 CoreWeave Sandboxes를 공개 프리뷰로 출시했으며, @cnakazawa는 토큰을 노출하지 않고 셸, Codex, GitHub 접근이 가능한 작업별 Cloudflare 샌드박스를 위한 Cloudsail을 출시했습니다. 오케스트레이션 계층에서는 @skypilot_org가 현대 RL이 이기종 하드웨어와 복구 요구 사항을 가진 다중 서비스 시스템이기 때문에 Slurm에서 RL이 작동하지 않는다고 주장했습니다.
- 오픈소스 하네스와 메모리 계층이 확산되고 있습니다: @NVIDIAAI는 임의의 하네스에 연결할 수 있는 휴대용 심층 연구 파이프라인을 위한 AI-Q 에이전트 스킬을 오픈소스화했습니다. @Teknium은 Hermes에서 키 관리를 위한 Bitwarden 지원을 추가했으며, 나중에 Hermes에서 Grok Build v0.1의 256K 컨텍스트를 복원했습니다. @shannholmberg는 Hermes 에이전트 아래에 유형화된 폴더와 전문 에이전트를 위한 읽기 우선 접근 권한을 가진 공유 메모리 "gBrain" 계층을 설명했습니다. @aakashadesara는 Devin을 지원하고 에이전트 세션을 나열, 검색 및 종료하는 CLI를 위해 CTOP을 업데이트했습니다.
연구: RL, 디스틸레이션, 아키텍처, 그리고 평가
- RL 사후 학습과 보상 설계가 활발히 재고되고 있습니다: @RyanBoldi는 Vector Policy Optimization (VPO)을 소개하며, RL 중 스칼라 보상 붕괴가 테스트 시간 스케일링을 방해할 수 있다고 주장했습니다. VPO는 대신 벡터 값 보상을 최적화하여, 원래의 스칼라 목표에서도 검색 성능을 향상시킵니다. @lateinteraction은 이를 더 다양한 환경과 목표를 위해 LLM을 학습시키는 방법으로 보았고, @FeiziSoheil은 이를 단일 보상 숫자 대신 구조화된 피드백을 향한 광범위한 움직임과 연결했습니다. 별도로, @jsuarez는 극심한 희소성과 관련된 오랜 RL 문제에 대한 해결책을 예고했으며, 초기 실험에서 한 내부 환경에서 SOTA를 보여주었습니다.
- 에이전트 컴파일/디스틸레이션이 진지한 경제적 아이디어로 부상하고 있습니다: @dair_ai는 완전한 에이전틱 워크플로우—다단계 호출, 도구 사용, 스크래치패드, 의사결정 구조—가 가중치로 디스틸레이션되어 거의 프론티어 품질을 유지하면서 약 100배 낮은 인퍼런스 비용으로 실행될 수 있음을 보여주는 논문을 강조했습니다. 이는 비용이 많이 드는 런타임 에이전트 루프를 더 저렴하게 배포 가능한 모델로 컴파일하는 가장 명확한 기술적 주장 중 하나입니다.
- 바닐라 트랜스포머를 넘어선 아키텍처 연구는 여전히 활발합니다: @ChunyuanDeng은 희소 및 선형 어텐션을 결합하여 루핑을 실용적으로 만드는 선형 시간 루프 트랜스포머인 LT2와 디스틸레이션된 Ouro-hybrid-1.4B를 소개했습니다. @ZyphraAI는 에너지 기반 모델을 넘어 생물학적으로 현실적인 뉴런으로 평형 전파(Equilibrium Propagation)를 확장하는 작업을 공유했습니다. MoE에 대해서는 @Jianlin_S가 손실 페널티 없이 시퀀스 수준 로드 밸런싱을 위한 Moving Quantile Balancing을 제안했습니다. 한편 @allen_ai는 ArtifactLinker를 출시했는데, 이는 모델이 어떤 벤치마크에서 SOTA를 달성할 가능성이 있는지 실행 전에 예측하는 도구로, 증가하는 벤치마크 확산 속에서 유용한 메타 평가 도구입니다.
- 수학 및 추론 능력 담론이 다시 변화했습니다: @cozyblaze265065는 gpt-5.5를 사용하여 중간 수준의 추론과 도구 없이 다중 자릿수 곱셈 실험에서 99.46%를 보고했으며, @teortaxesTex는 현대 LLM이 이제 도구 없이 100자릿수 곱셈을 할 수 있다고 언급했습니다. 이는 완전한 추론 이론은 아니지만, "자동 회귀는 산술을 할 수 없다"는 오래된 논점을 더욱 약화시킵니다.
멀티모달 시스템: 비디오, 음성, 월드 모델, 그리고 이미징
- Google의 I/O 스택은 영구 에이전트와 월드 시뮬레이터 방향으로 나아갔습니다: @Google은 반복적인 작업, 스킬, 워크플로우를 위한 24시간 연중무휴 개인 AI 에이전트인 Gemini Spark를 소개했습니다. @GoogleDeepMind는 또한 사용자가 실제 미국 위치를 인터랙티브한 세계로 바꿀 수 있게 해주는 Project Genie + Street View를 출시했습니다; 후속 게시물은 Google Labs를 통해 Google AI Ultra 구독자에게 출시될 것임을 확인했습니다. 멀티모달 측면은 @Google이 대화형 비디오 생성/편집 및 맞춤형 아바타를 위한 Gemini Omni를 발표하면서 강화되었으며, @emollick은 비디오를 기본적으로 편집할 수 있는 완전한 멀티모달 시스템의 중요성을 강조했습니다.
- Runway와 이미지/비디오 툴링은 편집 가능성을 계속 높이고 있습니다: @runwayml은 Aleph 2.0을 출시했으며, 장면의 나머지 부분을 보존하는 타겟 편집 기능을 통해 1080p 해상도로 최대 30초 길이의 멀티샷 시퀀스를 지원합니다. @CuriousRefuge는 Omni 생성 연속물을 사용하여 AI 생성 시네마틱 클립을 원활하게 확장하는 SeeDance 2 Stitcher를 강조했습니다.
- 음성 및 이미지 생성에서 주목할 만한 발전이 있었습니다: @ArtificialAnlys는 Cartesia Sonic-3.5를 Speech Arena에서 새로운 #1 TTS 모델로 선정했으며, Elo 1218점, 42개 언어 지원, 강력한 자연스러움/스크립트 따르기 능력을 언급했습니다. Cartesia는 여기에서 프로덕션 환경에서 82ms의 엔드투엔드 첫 오디오를 제공한다고 주장합니다. 이미지 생성에서는 @wildmindai가 VAE 없이 1K 해상도를 지원하고 Flux/SD 모델 변환을 위한 전송 프레임워크를 갖춘 픽셀 공간 생성기인 Tencent의 Z-Image 6B를 주목했습니다; 관련 생태계 작업에는 @victormustar의 Pixal3D 데모와 @ostrisai의 AI Toolkit에서 Z-Image L2P 1k 학습 지원이 포함되었습니다.
보안, 사이버, 그리고 정책 압력
- 사이버보안은 고급 에이전트의 시험장이 빠르게 되고 있습니다: @AnthropicAI는 Project Glasswing과 파트너들이 한 달 안에 필수 소프트웨어에서 만 개 이상의 높은 또는 치명적인 심각도 취약점을 발견했으며, Claude Mythos Preview와 같은 모델이 찾아낼 수 있는 취약점의 양에 업계가 적응해야 할 것이라고 명시적으로 경고했습니다. 보안 제품화가 뒤따르고 있습니다: @perplexity_ai는 macOS/Linux용 읽기 전용 스캐너인 Bumblebee를 오픈소스화하여 위험한 패키지, 확장 기능 및 AI 도구 구성을 탐지합니다; @AravSrinivas는 엔터프라이즈 배포에는 에이전틱 샌드박스와 지속적인 보안 엔지니어링이 필요할 것이라고 말했습니다.
- 미국 이민 정책 변화가 AI 리더들로부터 강한 반발을 불러일으켰습니다: 여러 높은 참여도의 게시물들은 영주권 신청자들이 미국 밖에서 신청하도록 강제하는 제안된 규칙이 AI 인재 파이프라인에 직접적인 손상을 입힐 것이라고 주장했습니다. @Nick_Davidov, @AndrewYNg, @theo, @garrytan, @togelius의 게시물을 참조하십시오. 공통된 주장은 다음과 같습니다: 이 규칙은 합법적인 고숙련 이민자들을 처벌하고, 스타트업과 연구를 약화시키며, AI 분야에서 미국의 경쟁력을 해친다는 것입니다.
가장 많이 참여한 트윗 (참여도 기준)
- @deepseek_ai의 V4-Pro 할인 영구화에 대한 내용 — 이번 배치에서 LLM 인퍼런스 경제학에 대한 가장 명확한 단일 시장 신호입니다.
- @gdb의 "모델 단독으로는 더 이상 제품이 아니다"에 대한 내용 — 현재 에이전트/하네스 제품 논지를 간결하게 표현한 것입니다.
- @AnthropicAI의 Glasswing이 10,000개 이상의 치명적인 취약점을 발견했다는 내용 — AI 기반 사이버 역량이 프로덕션으로 이동하고 있음을 보여주는 가장 강력한 데이터 포인트 중 하나입니다.
- @dsp_의 MCP 2026-07-28 RC에 대한 내용 — 중요한 프로토콜 업데이트: 스테이트리스 MCP 및 일등 확장.
- @GoogleDeepMind의 Project Genie + Street View에 대한 내용 — 소비자 지향 월드 모델을 향한 주목할 만한 진전입니다.
- @cursor_ai의 커스텀 에이전트를 위한 Cursor SDK 공개에 대한 내용 — 코딩 에이전트 인프라 위에 구축하는 팀들에게 관련성이 높습니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[Start trial](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-all-model-labs-are-now-agent&utm_source=paywall-free-trial&utm_medium=web&utm_content=198927453&coupon=5fe099d9)[Already a paid subscriber? Sign in](https://substack.com/sign-in?redirect=%2Fp%2Fainews-all-model-labs-are-now-agent&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
