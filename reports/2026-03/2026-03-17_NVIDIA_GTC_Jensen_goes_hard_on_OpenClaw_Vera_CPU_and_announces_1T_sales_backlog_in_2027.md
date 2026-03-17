# NVIDIA GTC: Jensen goes hard on OpenClaw, Vera CPU, and announces $1T sales backlog in 2027

**원문 URL**: https://www.latent.space/p/ainews-nvidia-gtc-jensen-goes-hard
**번역일**: 2026-03-17 06:40
**발행일**: 2026-03-17

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] NVIDIA GTC: Jensen이 OpenClaw, Vera CPU를 강력히 언급하고 2027년까지 1조 달러 판매 잔고를 발표했습니다

### 조용한 하루 동안 NVIDIA GTC 2026을 되돌아볼 수 있었습니다
공유다시 NVIDIA GTC의 날이었습니다. Jensen은 그의 시그니처인 2시간짜리 즉흥 기조연설에서 전체 NVIDIA 유니버스 및 생태계에 대한 업데이트를 제공하고 InferenceMAX 챔피언 벨트를 기념했습니다. 예상대로 Blackwell과 Rubin은 매우 잘 팔리고 있으며(일부 회계 처리가 필요합니다), 이제 Vera입니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/3c9e5d8d-2b90-4c27-ab1c-fd67c035acb4_3592x1886.png)
기조연설의 마지막 섹션은 OpenClaw에 초점을 맞췄는데, Jensen은 OpenClaw를 극찬하며 보안 문제를 지적한 다음, 그의 솔루션인 NemoClaw를 제시했습니다:

![Image](https://substack-post-media.s3.amazonaws.com/public/images/cfaddec2-3aea-4fbd-07158c2251d6_2048x945.jpeg)
NVIDIA는 4조 달러 규모의 회사임에도 불구하고 인상적인 속도로 움직이고 있으며, 저희는 그들의 다음 세대 리더들을 팟캐스트에 모셔 NVIDIA가 어떻게 이렇게 빠르게 작동하는지에 대한 더 많은 통찰력을 얻었습니다:
> 2026년 3월 14일~3월 16일 AI 뉴스. 저희는 12개의 서브레딧, 544개의 트위터를 확인했으며 더 이상의 디스코드는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로 AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
아키텍처 연구: Moonshot의 Attention Residuals와 선행 연구를 둘러싼 논쟁
- Moonshot의 Attention Residuals 논문은 피드에서 가장 명확한 기술적 이야기였습니다. @Kimi_Moonshot은 고정된 잔차 누적(fixed residual accumulation)을 이전 레이어에 대한 입력 의존적 어텐션(input-dependent attention)으로 대체하는 방법을 소개했으며, 교차 레이어 어텐션(cross-layer attention)을 실용적으로 유지하기 위한 Block AttnRes도 추가했습니다. 주장된 결과는 1.25배의 컴퓨팅 이점, 2% 미만의 인퍼런스 레이턴시 오버헤드이며, Kimi Linear 48B 전체 / 3B 활성 모델에서 검증되었습니다. 후속 게시물들은 개선된 은닉 상태 크기 제어(hidden-state magnitude control)와 깊이에 걸쳐 더 균일한 그라디언트(gradients)를 강조했습니다 (논문 스레드, 논문 링크). 이 발표는 @Yuchenj_UW, @elonmusk, @nathancgy4를 포함한 실무자와 연구자들, 그리고 @eliebakouch, @tokenbender와 같은 여러 시각적 설명자들로부터 강력한 긍정적인 반응을 이끌어냈습니다.
- 흥미로운 2차 논의는 이것이 새로운 것인지, 아니면 "대규모에서 새로운 것"인지에 대한 것이었습니다. @behrouz_ali는 이 아이디어가 DeepCrossAttention과 같은 선행 연구와 상당히 겹친다고 주장하며 누락된 인용과 전반적인 ML 분야의 참신성 인플레이션(novelty inflation)을 비판했습니다. @cloneofsimo는 Google이 이전에 관련 아이디어를 탐구했었다는 유사한 주장을 했고, 반면 다른 이들은 시스템 작업과 스케일링 증거가 핵심 직관만큼 중요하다고 반박했습니다 (맥락, 더 많은 맥락). 요컨대, 이 논문은 아키텍처 제안으로서뿐만 아니라 아이디어의 참신성, 인용 품질, 그리고 프론티어 스케일 검증(frontier-scale validation) 사이의 분야의 지속적인 긴장을 보여주는 생생한 사례로서 중요했습니다.
코딩 에이전트, 하네스, 그리고 스킬 인프라
- OpenAI의 Codex 모멘텀이 반복적으로 나타났습니다. OpenAI 개발자들은 Codex x Notion 이벤트를 홍보했으며, 회사 게시물과 리더십 논평은 빠른 채택을 강조했습니다. @fidjissimo는 Codex가 주간 활성 사용자 200만 명 이상을 기록하며 연초 대비 거의 4배 증가했다고 말했으며, OpenAI는 또한 기업 출시를 위한 배포 부서(deployment arm)를 구축하고 있습니다. @sama는 "하드코어 빌더들"이 Codex로 전환하고 있다고 덧붙였고, @gdb는 GPT-5.4가 일주일 만에 하루 5조 토큰에 도달했으며, 순 신규 수익(net-new revenue)에서 연간 10억 달러의 실행률(run-rate)을 기록했다고 말했습니다. 제품 측면에서 Codex는 또한 서브에이전트(subagents)를 추가하여 다중 에이전트 코딩 워크플로우(multi-agent coding workflows)로의 전환을 강화했습니다.
- 코딩 에이전트 주변의 인프라 레이어는 빠르게 성숙하고 있습니다. @AndrewYNg는 현재 API 문서용 오픈 CLI인 Context Hub / chub를 확장했으며, 이는 이제 문서에 대한 에이전트 피드백 루프를 지원합니다. @AssemblyAI는 Claude Code, Codex, Cursor 및 호환 에이전트가 오래된 학습 사전 지식(stale training priors) 대신 최신 API 패턴을 사용할 수 있도록 유지 관리되는 스킬을 출시했습니다. @dair_ai는 GitHub 리포지토리에서 에이전트 스킬을 표준화된 SKILL.md로 자동 추출하는 논문을 강조했으며, 40%의 지식 전달 이득(knowledge-transfer gains)을 주장했습니다. 이 모든 것은 스킬 파일, 최신 문서, 피드백 채널, 그리고 리포지토리에서 추출된 절차적 지식(procedural knowledge)으로 구성된 새로운 에이전트 툴링 스택을 향하고 있습니다.
- LangChain은 "에이전트 하네스 엔지니어링" 분야로 더욱 깊이 들어갔습니다. @LangChain은 터미널 기반 배포/개발 흐름을 위한 LangGraph CLI를 출시했으며, 생태계는 @itsafiz와 @simplifyinAI가 최고의 코딩 에이전트 뒤에 있는 워크플로우(계획/할 일, 파일 시스템 작업, 셸 액세스, 서브에이전트, 컨텍스트 관리)를 MIT 라이선스로 재현한 것으로 설명한 Deep Agents를 오픈소스화했습니다. 내부적으로 @Vtrivedy10은 이것이 프로덕션 에이전트 작업 및 평가(evals)의 기반이기도 하다고 말했습니다. 주목할 만한 패턴은 팀들이 더 이상 단순히 모델만 출시하는 것이 아니라, 레퍼런스 하네스(reference harnesses)를 출시하고 있다는 점입니다.
오픈소스 에이전트: Hermes의 돌파, OpenClaw 통합, 그리고 에이전트 UX
- Hermes Agent는 강력한 커뮤니티 사이클을 가졌습니다. 해커톤 프로젝트는 홈 미디어 자동화(@rodmarkun의 애니메이션 서버 도구), 사이버 툴링(@aylacroft), 지정학/OSINT 예측(@WeXBT), 연구 시각화(@t105add4_13)에 걸쳐 있었습니다. 사용자들의 의견은 Hermes가 OpenClaw보다 설정하기 쉽고 더 견고하다는 것이 일관적이었습니다 (예: @Zeneca, @fuckyourputs, @austin_hurwitz, @0xMasonH). @Teknium은 또한 Honcho 메모리 활성화와 같은 설정 가이드를 게시했습니다.
- OpenClaw는 Hermes와의 비교에도 불구하고 여전히 생태계를 확장했습니다. @ollama는 Ollama를 OpenClaw의 공식 제공업체로 발표했습니다. Comet은 호출/도구/비용 추적을 위한 관측성(observability) 플러그인을 출시했으며, NemoClaw와 같은 서드파티 모드(mods)도 있었습니다. 더 넓은 시사점은 "승자 독식"이라기보다는 오픈 에이전트가 고전적인 소프트웨어 생태계(제공업체, 메모리 백엔드, 추적, 온보딩 가이드, 해커톤 주도 확장)와 유사해지기 시작했다는 것입니다.
모델 및 제품 출시: Perplexity Computer, Gemini Embeddings, Mistral/Minimax 시그널
- Perplexity의 Computer 출시는 가장 구체적인 최종 사용자 에이전트 출시였습니다. @AravSrinivas와 @perplexity_ai는 Android용 Computer를 발표했으며, Computer가 커넥터/MCP 없이 Comet을 제어하고 로컬 브라우저를 도구로 사용할 수 있도록 확장했고, 로컬 쿠키가 보존되고 사용자가 작업 내용을 볼 수 있도록 했습니다 (세부 정보, 구현 노트). 이는 에이전틱 실행(agentic execution)을 클라우드 통합에서 허가된 로컬 브라우저 제어로 확장한다는 점에서 주목할 만합니다.
- Google은 기초적인 멀티모달 프리미티브(multimodal primitive)를 추가했습니다. @Google은 Gemini API와 Vertex AI를 통해 Gemini Embedding 2를 공개 프리뷰로 출시했으며, 이는 텍스트, 이미지, 비디오, 오디오 전반에 걸쳐 100개 이상의 언어를 지원하는 단일 임베딩 공간으로 포지셔닝되었습니다. 이러한 출시는 또 다른 프론티어 챗 모델 벤치마크보다 프로덕션 검색/리트리벌 시스템(production search/retrieval systems)에 더 큰 영향을 미칠 수 있습니다.
- 주목할 만한 다른 모델 및 출시 시그널은 다음과 같습니다. @matvelloso는 gemini-3.1-flash-lite-preview를 가격 × 레이턴시 × 지능 측면에서 칭찬했습니다. @QuixiAI는 Qwen 3.5 FP8을 역설계했으며, Qwen3.5-397B-FP8을 8× MI210에서 초당 6 토큰으로 실행했습니다 (실행 노트). @AiBattle_과 @kimmonismus는 MiniMax 2.7이 임박했음을 지적했습니다. @scaling01은 Mistral Small 4의 일부로 Leanstral을 공개했습니다. 그리고 @SeedFold는 확산 기반(diffusion-based)의 de novo 전원자 단백질 설계(all-atom protein design)를 위한 SeedProteo를 출시했습니다.
시스템, 인퍼런스, 그리고 그래픽: GTC, Speculative Decoding, 그리고 DLSS 5
- NVIDIA GTC의 메시지는 명확했습니다. 무게 중심은 인퍼런스에 있습니다. Jensen이 제시한 "인퍼런스 변곡점(inference inflection point)"이라는 프레이밍은 @basetenco의 인용과 함께 @nvidia, @kimmonismus 등의 생태계 포지셔닝 게시물에서 널리 반복되었습니다. 컨퍼런스 주변에서는 여러 인프라 관련 업데이트가 있었습니다. vLLM의 OCI 프로덕션 스택 가이드, 그리고 P-EAGLE의 강력한 시스템 기여가 있었는데, 이는 한 번의 패스(pass)로 K개의 드래프트 토큰(draft tokens)을 생성하여 Speculative Decoding의 순차적 병목 현상을 제거합니다. B200에서 EAGLE-3 대비 최대 1.69배의 속도 향상이 보고되었으며 vLLM v0.16.0에 통합되었습니다.
- 그래픽 측면에서는 DLSS 5가 반응을 압도했습니다. NVIDIA는 DLSS 5를 실시간 레이 트레이싱(real-time ray tracing) 이후 가장 큰 그래픽 도약으로 포지셔닝했으며, @ctnzr, @GeForce_JacobF, 그리고 Digital Foundry 관련 논의에서 강력한 반응이 있었습니다. 핵심 기술 주장은 원본 지오메트리/자산(geometry/assets)을 보존하면서 완전 생성형 신경 렌더링(generative neural rendering) / 리라이팅(relighting)을 통해 실시간으로 시각적 충실도(visual fidelity)를 실질적으로 발전시킨다는 것입니다. 직접적인 LLM 이야기는 아니지만, 신경화된 런타임 시스템(neuralized runtime systems)을 향한 더 넓은 트렌드의 중요한 부분입니다.
과학, 헬스케어, 그리고 보안 분야의 AI
- 가장 실질적인 과학/헬스케어 게시물은 Microsoft의 GigaTIME 스레드였습니다. @AnishA_Moonka는 Microsoft, Providence, UW의 연구를 요약했는데, 이 연구에서는 모델이 5달러짜리 병리 슬라이드(pathology slide)에서 다중 면역형광(multiplex immunofluorescence) 방식의 공간 단백질체학(spatial proteomics)을 예측하며, 4천만 개의 세포로 학습되고 51개 병원의 14,256명 환자에게 적용되어 약 30만 개의 가상 단백질 지도(virtual protein maps)를 생성하고 1,234개의 검증된 연관성(validated associations)을 밝혀냈습니다. 이 스레드는 모델이 오픈소스이며, 이것이 대규모 암 면역 프로파일링(cancer immune profiling)을 민주화할 수 있다고 주장합니다.
- 기술적으로 의미 있는 다른 과학/안전 항목은 다음과 같습니다. @GoogleResearch는 고온 초전도 추론(high-temperature superconductivity reasoning)에 대한 LLM 평가 연구를 설명하며, 큐레이션된 클로즈드 시스템 모델(curated closed-system models)이 과학 작업에서 웹 중심 설정(web-heavy setups)보다 우수하다고 주장했습니다. @AISecurityInst는 사이버 레인지(cyber ranges)에서 자율 공격 능력(autonomous attack capability)에 대해 7개의 프론티어 모델(frontier models)을 평가했습니다. 그리고 @askalphaxiv는 LeCun의 잠재 계획(Latent Planning)을 위한 Temporal Straightening을 강조했는데, 이는 잠재 궤적(latent trajectories)을 곧게 펴서 유클리드 거리(Euclidean distance)가 도달 가능한 진행 상황을 더 잘 추적하도록 함으로써 계획 안정성(planning stability)을 향상시킵니다.
(참여도 기준) 인기 트윗
- 헬스케어 파운데이션 모델 영향: GigaTIME 병리 → 공간 단백질체학 스레드는 가장 신호가 높고 참여도가 높은 기술 게시물이었습니다.
- 아키텍처 혁신: Moonshot의 Attention Residuals 출시는 탁월한 참여와 광범위한 전문가 토론을 이끌어냈습니다.
- 코딩 에이전트 제품 모멘텀: @sama의 Codex 성장 언급과 @gdb의 GPT-5.4 API 사용량 증가는 가장 명확한 수요 측면 시그널이었습니다.
- 오픈 에이전트 생태계: Ollama가 OpenClaw 제공업체가 된 것은 참여도 기준으로 가장 큰 오픈 에이전트 인프라 발표 중 하나였습니다.
- 에이전트 지식 인프라: @AndrewYNg의 Context Hub에 대한 언급은 에이전트 간 문서 공유를 위한 구체적인 제안으로 돋보였습니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽기
이 게시물을 계속 읽으려면 Latent.Space를 구독하고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-nvidia-gtc-jensen-goes-hard&utm_source=paywall-free-trial&utm_medium=web&utm_content=191206166&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-nvidia-gtc-jensen-goes-hard&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
