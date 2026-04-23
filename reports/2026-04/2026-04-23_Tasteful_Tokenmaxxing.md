# Tasteful Tokenmaxxing

**원문 URL**: https://www.latent.space/p/ainews-tasteful-tokenmaxxing
**번역일**: 2026-04-23 06:18
**발행일**: 2026-04-23

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Tasteful Tokenmaxxing

### 조용한 하루를 맞아 AI 리더들이 어디서나 나누는 최고의 대화에 대해 생각해 봅니다.
Share오늘은 Cloud Next가 열리는 날이며, 예상대로 Google TPUv8(학습 및 인퍼런스 이터레이션)이 발표되었습니다. 그 수치들은 놀랍지만, 이는 주로 10년간의 투자가 GDM과 그들이 학습시키고 서비스하는 모든 모델에 제공한 엄청난 하드웨어 이점을 재확인시켜주는 역할을 합니다.
지난 이틀 동안 AIE Miami가 마무리되면서(다음은 싱가포르입니다!), AI 리더십(CTO, VP, 창업자)으로부터 들었던 주요 대화는 모두 "Tokenmaxxing"이라는 개념과, Gergely Orosz가 AIE 기조연설에서 설명했던 종류의 끔찍한 낭비를 조장하는 단점 없이, 리더들이 팀이 AI를 더 많이 사용하도록 만들고 싶어 하는 방식에 집중되었습니다.
Context Engineering과 "the Dumb Zone"이라는 용어를 만든 Dex Horthy는 6개월 전 자신의 극도로 바이브 코딩에 심취했던 주장을 공개적으로 철회하고, Alex Volkov의 AIE Europe에서의 Z/L 연속체를 인용하며 사람들에게 코드를 읽어달라고 권장했습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/cb2b6f77-150d-4fb4-a74a-259318cba0dd_1698x1172.png)
timestamp비공개적으로, 제가 대화하는 많은 고위 리더들은 Z/L 스펙트럼에서 Lopopolo 측면보다는 Zechner 측면에 더 가깝습니다. 이것이 모든 상황에서 모든 사람에게 한쪽이 옳다는 것을 의미하지 않으며, 모델 발전과 함께 계속해서 옳을 것이라는 의미도 아닙니다! 가장 분명한 점을 지적하자면, 엔지니어와 엔지니어링 리더들은 저렴한 코드 생성과 코드 리뷰의 엄청난 양으로 극복될 수 있는 사소한 아키텍처 품질 문제를 크게 부각시키는 경향이 있습니다.
오늘의 LS 게스트인 Shopify의 CTO Mikhail Parakhin은 "tasteful tokenmaxxing"에 대해 또 다른 견해를 제시했습니다. 즉, 폭넓게 접근하기보다는(예: LLM 슬롯 머신의 5개, 10개, 50개, 500개 병렬 실행을 시작하여 문제를 해결하는 것) 깊이 있게 접근하는 것(예: 더 많은 직렬 자동 연구 루프를 수행하는 것)을 목표로 해야 한다는 것입니다. 생각해 볼 가치가 있습니다.
> 2026년 4월 21일~4월 22일 AI 뉴스입니다. 저희는 12개의 subreddit, 544개의 Twitter를 확인했으며, Discord는 더 이상 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter 요약
오픈 모델: Qwen3.6-27B, OpenAI Privacy Filter, 그리고 Xiaomi MiMo-V2.5
- Qwen3.6-27B, 강력한 로컬/오픈 코딩 모델로 등장: @Alibaba_Qwen이 Qwen3.6-27B를 출시했습니다. 이 모델은 dense한 Apache 2.0 모델로, 사고 모드와 비사고 모드를 모두 갖추고 있으며 통합된 멀티모달 체크포인트를 제공합니다. Alibaba는 이 모델이 SWE-bench Verified 77.2 대 76.2, SWE-bench Pro 53.5 대 50.9, Terminal-Bench 2.0 59.3 대 52.5, SkillsBench 48.2 대 30.0을 포함한 주요 코딩 평가에서 훨씬 더 큰 Qwen3.5-397B-A17B를 능가한다고 주장합니다. 또한 이미지와 비디오에 대한 네이티브 시각-언어 추론을 지원합니다. 생태계는 즉시 움직였습니다: vLLM은 day-0 지원을 출시했고, Unsloth는 18GB-RAM 로컬 GGUF를 공개했으며, ggml은 llama.cpp 사용을 추가했고, Ollama는 패키지 릴리스를 추가했습니다. @KyleHessling1과 @simonw의 초기 사용자 보고서에 따르면 로컬 프론트엔드/디자인 및 이미지 작업에서 특히 강력한 성능을 보였습니다.
- OpenAI, 실용적인 프라이버시 모델을 조용히 오픈소스화: 여러 관찰자들이 OpenAI의 새로운 Privacy Filter를 주목했습니다. 이는 PII 감지 및 마스킹을 위한 경량 Apache 2.0 오픈 모델입니다. @altryne, @eliebakouch, @mervenoyann에 따르면, 이 모델은 1.5B 전체 / 50M 활성 MoE 토큰 분류 모델로, 128k 컨텍스트 윈도우를 가지며, 매우 큰 코퍼스 및 로그에 대한 저렴한 수정(redaction)을 목적으로 합니다. 이는 일반적인 "작은 오픈 모델"보다 운영상 더 흥미로운 릴리스입니다. 온디바이스 또는 저비용 전처리가 중요한 엔터프라이즈/에이전트 파이프라인의 구체적인 인프라 문제를 해결합니다.
- Xiaomi, 에이전틱 오픈 모델을 상향 추진: @XiaomiMiMo는 MiMo-V2.5-Pro와 MiMo-V2.5를 발표했습니다. Xiaomi는 V2.5-Pro를 소프트웨어 엔지니어링 및 장기 에이전트 분야의 주요 도약으로 포지셔닝하며, SWE-bench Pro 57.2, Claw-Eval 63.8, τ3-Bench 72.9를 인용하고 1,000개 이상의 자율 도구 호출을 주장합니다. 비 Pro 모델은 네이티브 옴니모달리티와 1M 토큰 컨텍스트 윈도우를 추가합니다. Arena는 MiMo-V2.5를 Text/Vision/Code 평가에 빠르게 등재했으며, @Teknium을 통해 Hermes/Nous 통합이 뒤따랐습니다.

---

Google Cloud Next: TPU v8, Gemini Enterprise Agent Platform, 그리고 Workspace Intelligence
- Google의 인프라 발표는 실질적이었으며, 단순한 외형 개선이 아니었습니다: @Google과 @sundarpichai는 학습용 TPU 8t와 인퍼런스용 TPU 8i로 분할된 8세대 TPU를 소개했습니다. Google은 8t가 Ironwood 대비 pod당 거의 3배의 컴퓨팅 성능을 제공하며, 8i는 pod당 1,152개의 TPU를 연결하여 낮은 레이턴시 인퍼런스와 높은 처리량의 멀티 에이전트 워크로드를 지원한다고 밝혔습니다. @scaling01의 논평은 추가적인 주장을 강조했습니다: Google은 이제 TPU8t를 통해 단일 클러스터에서 백만 개의 TPU로 확장할 수 있습니다. 원시 하드웨어만큼이나 제품화 신호가 중요합니다. Google은 칩, 모델, 에이전트 툴링, 그리고 엔터프라이즈 제어 플레인을 하나의 수직 통합된 제품으로 명확하게 정렬하고 있습니다.
- 엔터프라이즈 에이전트가 Google의 일등 제품 표면으로 부상했습니다: @GoogleDeepMind와 @Google은 Gemini Enterprise Agent Platform을 출시했습니다. 이는 Vertex AI가 대규모 에이전트를 구축, 관리, 최적화하기 위한 플랫폼으로 진화한 것으로 설명됩니다. 이 플랫폼에는 Agent Studio, Model Garden을 통한 200개 이상의 모델 접근, 그리고 Gemini 3.1 Pro, Gemini 3.1 Flash Image, Lyria 3, Gemma 4를 포함한 Google의 현재 스택 지원이 포함됩니다. 관련 출시로는 문서/시트/회의/메일 위에 구축된 시맨틱 레이어인 Workspace Intelligence GA, Gemini Enterprise inbox/canvas/재사용 가능한 스킬, Agentic Data Cloud, Wiz 통합 보안 에이전트, 그리고 텍스트, 이미지, 비디오, 오디오, 문서 전반에 걸친 통합 임베딩 모델인 Gemini Embedding 2 GA가 있었습니다.

---

에이전트, 하네스, 트레이스, 그리고 팀 워크플로우
- "에이전트 하네스" 추상화가 여러 벤더에서 강화되고 있습니다: OpenAI는 ChatGPT에 워크스페이스 에이전트를 도입했으며, 문서, 이메일, 채팅, 코드 및 외부 시스템(Slack 기반 워크플로우 및 예약/백그라운드 작업 포함) 전반에서 작동할 수 있는 팀용 Codex 기반 에이전트를 공유했습니다. Google은 Gemini Enterprise Agent Platform으로 유사한 엔터프라이즈 움직임을 보였고, Cursor는 작업 시작 및 스트리밍 업데이트를 위해 Slack 호출 기능을 추가했습니다. 패턴은 클라우드 호스팅 에이전트, 공유 팀 컨텍스트, 승인, 그리고 단일 사용자 채팅보다는 장기 실행으로 수렴하고 있습니다.
- 하네스/모델 독립성 관련 개발자 인체공학이 개선되었습니다: VS Code/Copilot은 Anthropic, Gemini, OpenAI, OpenRouter, Azure, Ollama 및 로컬 백엔드와 같은 제공업체를 지원하며, 모든 플랜과 비즈니스/엔터프라이즈에 걸쳐 BYOK(bring-your-own-key)/모델 지원을 출시했습니다. @omarsar0가 언급했듯이, 대부분의 모델이 여전히 자체 에이전트 하네스에 과적합된 것처럼 보이기 때문에 이는 전략적으로 중요합니다. Cognition의 Russell Kaplan은 보완적인 비즈니스 사례를 제시했습니다: 엔터프라이즈 구매자들은 특정 연구소에 종속되는 것이 아니라, 전체 SDLC(Software Development Life Cycle)를 아우르는 모델 유연성과 인프라를 원합니다.
- 트레이스/평가/자기 개선이 핵심 에이전트 데이터 프리미티브가 되고 있습니다: 이 부분에서 가장 강력한 흐름은 LangChain 관련 논의에서 나왔습니다. @Vtrivedy10은 트레이스가 에이전트 오류와 비효율성을 포착하며, 더 나은 평가, 스킬, 환경을 생성하기 위해 트레이스를 이해하는 데 컴퓨팅 자원을 집중해야 한다고 주장했습니다. 이 주장은 트레이스 마이닝, 스킬, 컨텍스트 엔지니어링, 서브 에이전트, 온라인 평가를 포함하는 구체적인 루프로 확장되었습니다. @ClementDelangue는 오픈 에이전트 학습을 위한 누락된 데이터 기반으로서 오픈 트레이스를 주장했으며, @gneubig는 ADP / Agent Data Protocol 표준화를 추진했습니다. LangChain은 또한 @hwchase17을 통해 더 강력한 테스트/평가 제품 방향을 예고했습니다.

---

사후 학습, RL, 그리고 인퍼런스 시스템
- Perplexity 및 기타 업체들이 사후 학습 플레이북을 더 많이 공유했습니다: @perplexity_ai는 사실성, 인용 품질, 지시 따르기, 효율성을 개선하는 검색 증강 SFT + RL 파이프라인에 대한 세부 정보를 공개했습니다. 그들은 Qwen 기반 시스템이 더 낮은 비용으로 사실성 측면에서 GPT 계열 모델과 같거나 능가할 수 있다고 말합니다. @AravSrinivas는 Perplexity가 현재 도구 라우팅과 요약을 통합하고 이미 상당한 트래픽을 처리하고 있는 사후 학습된 Qwen 파생 모델을 프로덕션에서 실행하고 있다고 덧붙였습니다. 연구 측면에서는 @michaelyli__가 프록시 목표 없이 추론과 KV-cache 유지/제거를 공동으로 학습하는 RL을 사용하는 Neural Garbage Collection을 소개했습니다. @sirbayes는 ForecastBench에서 인간 슈퍼 예측가와 일치하는 베이시안 언어적 믿음 예측 에이전트를 보고했습니다.
- 코딩 모델의 "최소 편집" 문제가 유용한 벤치마크 처리 방식을 얻었습니다: @nrehiew_는 코딩 모델이 너무 많은 코드를 다시 작성하여 버그를 수정하는 Over-Editing에 대한 작업을 발표했습니다. 이 연구는 최소한으로 손상된 문제를 구성하고 패치 거리와 추가된 Cognitive Complexity로 과도한 편집을 측정합니다. 그 결과 GPT-5.4가 가장 많이 과도하게 편집하고 Opus 4.6이 가장 적게 과도하게 편집하며, RL이 치명적인 망각 없이 일반화 가능한 최소 편집 스타일을 학습하는 데 SFT, DPO, rejection sampling보다 우수하다는 것을 발견했습니다. 이는 엔지니어들이 프로덕션 코드 리뷰에서 실제로 불평하는 실패 모드를 다루기 때문에 이 세트에서 더 실용적인 사후 학습/평가 기여 중 하나입니다.
- 인퍼런스 효율성 작업은 계속해서 활발했습니다: @cohere는 프로덕션 W4A8 인퍼런스를 vLLM에 통합하여 Hopper에서 W4A16 대비 TTFT를 최대 58% 빠르게, TPOT를 45% 빠르게 만들었다고 보고했습니다. 세부 사항에는 채널당 FP8 스케일 양자화 및 CUTLASS LUT 역양자화가 포함됩니다. @WentaoGuo7은 Blackwell에서 SonicMoE의 처리량 증가를 보고했습니다. DeepGEMM 기준선보다 fwd/bwd TFLOPS가 54%/35% 더 높았으며, 동일한 활성 파라미터에 대해 dense 모델과 동등한 활성화 메모리를 유지했습니다. @baseten은 재랭킹에서 공유 접두사 제거를 위한 RadixMLP를 도입하여 1.4~1.6배의 현실적인 속도 향상을 달성했습니다.

---

가장 인기 있는 트윗 (참여도 기준)
- OpenAI 워크스페이스 에이전트: @OpenAI가 Business/Enterprise/Edu/Teachers를 위한 공유 Codex 기반 워크스페이스 에이전트를 출시했습니다.
- Qwen3.6-27B 출시: @Alibaba_Qwen이 강력한 코딩 성능을 주장하며 Apache 2.0 라이선스를 가진 새로운 오픈 27B dense 모델을 발표했습니다.
- Google TPU v8: @sundarpichai가 학습/인퍼런스 특화된 TPU 8t / 8i를 미리 선보였습니다.
- Flipbook / 모델 스트리밍 UI: @zan2434가 기존 UI 스택 대신 모델에서 직접 픽셀로 화면이 렌더링되는 프로토타입을 시연했습니다.
- OpenAI Privacy Filter: @scaling01 및 기타 사용자들이 Hugging Face에 공개된 OpenAI의 새로운 오픈소스 PII 감지/수정 모델을 강조했습니다.

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Qwen 3.6 모델 출시 및 벤치마크
- Qwen 3.6 27B 출시 (활동: 2576): 새로운 언어 모델인 Qwen 3.6 27B가 Hugging Face에 출시되었습니다. 이 모델은 270억 개의 파라미터를 특징으로 하며, 향상된 성능 벤치마크를 통해 이전 버전을 개선하도록 설계되었습니다. 양자화된 버전인 Qwen3.6-27B-FP8도 제공되어, 제한된 컴퓨팅 리소스 환경에서 더 효율적인 배포가 가능합니다. 이번 출시는 다양한 작업에서 모델의 기능을 보여주는 상세한 벤치마크 결과를 포함합니다. 커뮤니티는 이번 출시에 대해 흥분을 표하고 있으며, 일부 사용자들은 모델의 성능 개선과 더 넓은 접근성을 위한 양자화된 버전의 가용성을 강조하고 있습니다.Namra_7은 Qwen 3.6 27B의 벤치마크 이미지를 공유했는데, 이는 인퍼런스 속도, 정확도 또는 기타 관련 통계와 같은 성능 지표를 포함할 가능성이 높습니다. 그러나 벤치마크의 구체적인 세부 사항은 댓글 자체에 설명되어 있지 않습니다.challis88ocarina는 Hugging Face에서 사용할 수 있는 Qwen 3.6 27B의 양자화된 버전을 언급했는데, 특히 FP8 형식입니다. 양자화는 모델 크기를 크게 줄이고 인퍼런스 속도를 향상시켜, 정확도 손실 없이 배포 효율성을 높일 수 있습니다. 제공된 링크는 추가 탐색을 위한 Hugging Face 모델 저장소로 연결됩니다.Eyelbee는 또 다른 이미지 링크를 게시했는데, 이는 Qwen 3.6 27B와 관련된 추가 시각 데이터 또는 성능 지표를 포함할 수 있습니다. 그러나 댓글은 이미지 내용에 대한 구체적인 통찰력이나 세부 정보를 제공하지 않습니다.
- Qwen3.6-27B 출시! (활동: 895): Qwen3.6-27B는 새로 출시된 dense 오픈소스 모델로, 코딩 작업에서 탁월한 성능을 보이며, 주요 코딩 벤치마크에서 이전 모델인 Qwen3.5-397B-A17B를 능가합니다. 이 모델은 텍스트 및 멀티모달 작업 모두에서 강력한 추론 기능을 특징으로 하며, '사고' 및 '비사고' 모드를 통해 유연성을 제공합니다. 이 모델은 Apache 2.0 라이선스 하에 출시되어 완전히 오픈소스이며 커뮤니티에서 사용할 수 있습니다. 더 자세한 내용은 블로그, GitHub, Hugging Face에서 확인할 수 있습니다. 댓글들은 Qwen 팀에 대한 흥분과 감탄을 반영하며, 사용자들은 자신들의 하드웨어에서 모델을 활용하려는 열망을 표현하고 팀의 기여가 기념비적이라고 제안합니다.ResearchCrafty1804는 Qwen3.6-27B의 인상적인 성능을 강조하며, 270억 개의 파라미터만 가지고 있음에도 불구하고 여러 코딩 벤치마크에서 훨씬 더 큰 Qwen3.5-397B-A17B 모델을 능가한다고 언급합니다. 특히, SWE-bench Verified에서 77.2, SWE-bench Pro에서 53.5, Terminal-Bench 2.0에서 59.3, SkillsBench에서 48.2점을 달성하여 각 경우에서 더 큰 모델을 상당한 차이로 앞섰습니다.bwjxjelsbd는 경쟁 환경에 대해 언급하며, META의 인식된 차질 이후 Alibaba가 Qwen 모델로 발전하는 것에 만족감을 표현합니다. 댓글 작성자는 지속적인 경쟁과 투명성을 희망하며, META가 건강한 경쟁 환경을 유지하기 위해 Muse 계열 모델을 오픈소스화해야 한다고 제안합니다.
- Qwen3.6-35B, 적절한 에이전트와 결합 시 클라우드 모델과 경쟁력 확보 (활동: 848): 이 게시물은 Qwen3.6-35B 모델이 little-coder 에이전트와 결합될 때 벤치마크 성능이 크게 향상되어 Polyglot 벤치마크에서 78.7%의 성공률을 달성하며 상위 10위권에 진입했음을 논의합니다. 이러한 개선은 적절한 스캐폴딩 사용의 중요성을 강조하며, 로컬 모델이 하네스 불일치로 인해 성능이 저하될 수 있음을 시사합니다. 저자는 연구 역량을 위해 Terminal Bench 및 GAIA에서 추가 테스트를 계획하고 있습니다. 전체 세부 정보 및 벤치마크는 GitHub 및 Substack에서 확인할 수 있습니다. 댓글 작성자들은 스캐폴딩 변경으로 인한 성능 향상에 놀라움을 표하며, 그러한 요소를 통제하지 않는 벤치마크의 유효성에 의문을 제기합니다. 또한 모델 하네싱의 확장성을 위해 pi.dev 사용에 대한 관심도 있습니다.DependentBat5432는 스캐폴딩 변경 시 Qwen3.6-35B의 상당한 성능 향상을 강조하며, 19%에서 78%로의 도약을 언급합니다. 이는 그러한 변수를 통제하지 않는 벤치마크 비교의 유효성에 대한 우려를 제기하며, 스캐폴딩 선택이 모델 성능에 극적으로 영향을 미칠 수 있음을 시사합니다.Willing-Toe1942는 Qwen3.6이 pi-coding 에이전트와 함께 사용될 때 opencode보다 거의 두 배 더 잘 작동한다고 보고합니다. 이 비교는 HTML 코드 수정 및 문서화를 위한 온라인 리소스 검색과 같은 작업을 포함하며, 에이전트 선택이 실제 코딩 시나리오에서 모델의 효율성을 크게 향상시킬 수 있음을 나타냅니다.kaeptnphlop은 VS Code에서 GitHub Copilot과 결합된 Qwen-Coder-Next의 강력한 성능을 언급하며, little-coder와 같은 다른 도구와의 추가 탐색 가능성을 시사합니다. 이는 Qwen 모델을 인기 있는 코딩 환경과 통합하면 그 강점을 효과적으로 활용할 수 있음을 의미합니다.

---

7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-tasteful-tokenmaxxing&utm_source=paywall-free-trial&utm_medium=web&utm_content=195193203&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-tasteful-tokenmaxxing&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
