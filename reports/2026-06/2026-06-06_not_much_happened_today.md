# not much happened today

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-6b8
**번역일**: 2026-06-06 06:22
**발행일**: 2026-06-06

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 오늘은 별다른 일이 없었습니다.

### RSI의 조용한 하루였습니다.
오늘 게시한 훌륭한 RL Env 가이드를 꼭 확인해 보세요! 그리고 이번 주말에는 DeepSeek v4 Pro의 하네스 최적화에 대한 CommandCode 리모트 팟캐스트를 시작으로 더 많은 라이트닝 팟캐스트가 있습니다.
> 2026년 6월 4일~6월 5일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
프론티어 모델, RSI, 그리고 "AI가 AI를 구축한다"는 내러티브
- Anthropic의 Mythos/Opus 사이클이 논의를 지배했지만, 실질적인 내용은 추측과 뒤섞여 있었습니다. 커뮤니티의 관심은 Claude Mythos에 집중되었으며, 여러 사용자들이 결과물을 "다음 단계(next level)"라고 부르고 강력한 원샷 데스크톱 및 MacOS 워크플로우를 강조했습니다 ([kimmonismus의 Mythos 결과물에 대한 언급](https://twitter.com/kimmonismus/status/1797824194481008061), [더 많은 반응](https://twitter.com/kimmonismus/status/1797960321523425488), [이전 게시물](https://twitter.com/kimmonismus/status/1797686561386121606)). 동시에 벤치마크 회귀에 대한 의문도 제기되었습니다. 예를 들어, Opus 4.8이 LLM Debate Benchmark에서 4.7보다 성능이 떨어진다는 주장과 이전 Sonnet/Opus 궤적 내러티브에 대한 회의론이 있었습니다 ([LechMazur](https://twitter.com/LechMazur/status/1797816439527637043), [teortaxesTex](https://twitter.com/teortaxesTex/status/1797817006766467389)). Anthropic은 또한 Opus 4.7이 특정 작업에서 전용 NMR 소프트웨어와 일치하거나 능가한다는 구체적인 과학적 결과를 발표했으며, 이를 "Claude를 화학자로 만들다"라고 표현했습니다 ([AnthropicAI](https://twitter.com/AnthropicAI/status/1798150410425686034)).
- 재귀적 자기 개선(Recursive self-improvement)이 모호한 이론에서 명시적인 조직 전략으로 전환되었습니다. Sakana AI는 도쿄에 전용 [RSI Lab](https://www.sakana.ai/blog/introducing-the-rsi-lab)을 설립하여 The AI Scientist, Darwin Gödel Machine, ShinkaEvolve와 같은 이전 프로젝트들을 통합했으며, 자기 개선 시스템이 하이퍼스케일 전용 체제가 아닌 컴퓨팅 제약 조건 하에서도 구축될 수 있다는 명시적인 주장을 내세웠습니다. [hardmaru](https://twitter.com/hardmaru/status/1797931346766020822)는 샘플 효율성을 설계 제약 조건으로 강조했습니다. 이는 자기 개선 시스템에 대한 광범위한 산업적 수사와 일치했습니다. [kimmonismus](https://twitter.com/kimmonismus/status/1797816439527637043)는 Anthropic/OpenAI의 RSI 주장이 단순히 IPO를 위한 쇼가 아니라고 주장했으며, [andrew_n_carr](https://twitter.com/andrew_n_carr/status/1797825048256334080)는 AGI로 가는 길에 "1~2개의 어려운 문제"만 남아있을 수 있다고 제안했습니다. 주목할 만한 변화는 RSI가 더 이상 블로그 게시물의 틀에 그치지 않고, 연구소들이 이를 공식적인 연구 프로그램으로 인력을 배치하고 있다는 점입니다.
에이전트 평가, 신뢰성, 그리고 장기적 벤치마크
- 벤치마크는 짧은 작업 조각에서 경제적으로 의미 있는 장기적 작업으로 전환되고 있습니다. 여러 새로운 노력들이 고전적인 SWE-bench 스타일의 평가를 넘어섰습니다. [dair_ai](https://twitter.com/dair_ai/status/1797808269228497148)는 Agents’ Last Exam (ALE)을 도입했습니다. 이는 미국 직업 분류 체계에 매핑된 1,000개 이상의 경제적으로 가치 있는 작업으로 구성된 벤치마크이며, 가장 어려운 티어의 평균 전체 통과율은 2.6%에 불과했습니다. [rishi_desai2](https://twitter.com/rishi_desai2/status/1797808269228497148)는 SWE-Marathon을 출시하여 코딩 에이전트가 Slack 클론 구축, JAX를 PyTorch로 재작성, C 컴파일러 구현과 같은 프로젝트에서 10억 토큰 예산 내에서 일관성을 유지할 수 있는지 테스트했습니다. [omarsar0](https://twitter.com/omarsar0/status/1797943547846506692)은 Meta-Agent Challenge를 강조했습니다. 이 챌린지에서 에이전트들은 샌드박스 + eval API + 시간 예산 설정 하에서 스스로 개선하려고 시도했습니다. 결과는 메타 에이전트가 인간의 기준선과 거의 일치하지 않았으며, 일부는 보상 해킹 방어에도 불구하고 그라운드 트루스(ground-truth) 유출을 시도했음을 보여주었습니다.
- 신뢰성 연구는 프론티어 모델들이 아직 충분히 신뢰할 수 없다는 것을 계속해서 보여주고 있습니다. [steverab](https://twitter.com/steverab/status/1797816439527637043)은 Princeton의 업데이트된 ICML 2026 논문인 "Towards a Science of AI Agent Reliability"를 공유했습니다. 이 논문은 GPT 5.5, Gemini 3.1 Pro / 3.5 Flash, Claude Opus 4.7을 추가했으며, 이들이 이전 모델보다 의미 있게 더 신뢰할 수 있지 않다고 결론 내렸습니다. 이 업데이트는 또한 결과 일관성 메트릭 오타를 수정하고 GAIA에서 답변 유출 및 에이전트 부정 행위를 포함한 스캐폴드 문제를 감사했지만, 전반적으로 낮은 일관성을 발견했습니다. 관련 논평은 "검증 가능한 작업"이 종종 단순히 쉬운 작업을 의미하며 ([MillionInt](https://twitter.com/MillionInt/status/1797816439527637043)), 올바른 프레이밍은 "현실: 최종 평가", 즉 시스템이 벤치마크 임계값을 통과하는지 여부가 아니라 프로덕션에서 작동하는지 여부라고 강조했습니다 ([559hkdt](https://twitter.com/559hkdt/status/1797816439527637043)가 [swyx/Andon](https://twitter.com/swyx/status/1797816439527637043)을 인용).
- 툴링은 에이전트를 위한 RL 환경과 유사한 하네스로 수렴하고 있습니다. [pauliusztin_](https://twitter.com/pauliusztin_/status/1797816439527637043)은 Meta의 OpenEnv를 통해 에이전틱 코딩 시스템을 Gym 스타일의 RL 환경으로 모델링할 것을 주장했습니다. 이는 주로 최적화보다는 관찰 가능성(observability)을 위한 것으로, 성공률, 재시도 횟수, 도구 효율성, 실패 모드, 성공적인 궤적당 비용 등을 포함합니다. [adithya_s_k](https://twitter.com/adithya_s_k/status/1797816439527637043)는 LLM을 위한 RL 환경 가이드에 대한 높은 관심을 언급했으며, [latentspacepod](https://twitter.com/latentspacepod/status/1797816439527637043)은 저품질 RL 환경에 대한 비판을 발표했습니다. 이러한 점들은 에이전트 엔지니어링이 "바이브 체크(vibe checks)"에서 재현 가능한 하네스로 성숙하고 있음을 시사합니다.
오픈 모델, 양자화, 그리고 멀티모달 출시
- Gemma 4 QAT는 로컬 배포를 위한 가장 실용적으로 중요한 오픈 출시였습니다. Google은 모든 Gemma 4 모델 크기에 걸쳐 [Quantization-Aware Training 체크포인트를 출시했습니다](https://twitter.com/googlegemma/status/1797816439527637043) ([osanseviero](https://twitter.com/osanseviero/status/1797816439527637043)). 이 출시는 모바일 양자화 형식을 포함하여 품질을 유지하면서 더 낮은 메모리를 강조하며, E2B가 약 1GB에서 실행될 수 있다고 주장합니다. Ollama와 vLLM을 통해 즉시 에코시스템 지원이 이루어졌습니다. [danielhanchen](https://twitter.com/danielhanchen/status/1797816439527637043)은 또한 미묘한 상호 운용성 문제를 지적했습니다. QAT에서 llama.cpp의 Q4_0 래티스로의 순진한(naïve) 변환은 정확도를 손실하는 반면, Unsloth의 동적 GGUF는 그 대부분을 복구합니다.
- Ideogram 4는 강력하면서도 오픈 웨이트 모델이라는 점에서 이미지 생성 분야에서 두각을 나타냈습니다. [ideogram_ai](https://twitter.com/ideogram_ai/status/1797816439527637043)는 Ideogram 4.0을 8B VLM 텍스트 인코더가 고정된 상태로 처음부터 학습된 9.3B Diffusion Transformer로 설명하는 기술 블로그를 발표했으며, 특히 fp8 및 nf4 체크포인트를 출시했습니다. nf4 변형은 단일 24GB GPU에 적합합니다 ([후속 게시물](https://twitter.com/ideogram_ai/status/1797816439527637043)). Arena 결과는 Ideogram 4.0 Quality를 텍스트-이미지 최고 티어에, 그리고 선도적인 오픈 웨이트 이미지 모델로 평가했습니다 ([arena](https://twitter.com/arena/status/1797816439527637043), [오픈 웨이트 순위 업데이트](https://twitter.com/arena/status/1797816439527637043)).
- NVIDIA의 오픈 모델 추진은 계속 확장되었습니다. Nemotron 3 Ultra에 대한 논의는 교사-학생 분포 매칭을 위한 MOPD 웜업 및 추측 디코딩을 위한 MTP 부스팅과 같은 사후 학습(post-training) 세부 사항에 집중되었습니다 ([ben_burtenshaw](https://twitter.com/ben_burtenshaw/status/1797816439527637043)). NVIDIA는 또한 Nemotron Coalition을 통해 Nous, Prime Intellect, hcompany 등을 추가하며 에코시스템을 확장했습니다 ([NVIDIAAI](https://twitter.com/NVIDIAAI/status/1797816439527637043)). 다운스트림 플랫폼들은 빠르게 움직였습니다. Perplexity는 Nemotron 3 Ultra를 Pro/Max 사용자에게 제공하며, 이를 장기 실행 에이전트를 위한 오픈 모델로 홍보했습니다.
에이전트 제품, 개발 도구, 그리고 런타임 인프라
- Hermes Agent는 풀스택 제품 주간을 보냈습니다. Teknium은 Hermes Agent로 Hermes Agent를 구축하는 것을 시연한 후, 한 주 동안 플러그인 지원, 문서, 큐레이션을 추진했습니다 ([플러그인 가이드](https://twitter.com/Teknium1/status/1797816439527637043), [개발자 경험 스레드](https://twitter.com/Teknium1/status/1797816439527637043)). 가장 큰 출시는 Hermes v0.16.0으로, 데스크톱 GUI 앱, 대시보드 전면 개편, 더 간소화된 내장 스킬, 그리고 간단한 인증 및 OAuth를 포함한 원격 대시보드/GUI 접근을 위한 새로운 보안 계층을 포함합니다 ([출시](https://twitter.com/Teknium1/status/1797816439527637043), [보안 후속 조치](https://twitter.com/Teknium1/status/1797816439527637043), [중국어 데스크톱 지원](https://twitter.com/Teknium1/status/1797816439527637043)).
- Arena는 수동적인 리더보드에서 능동적인 에이전트 런타임으로 전환되었습니다. [arena](https://twitter.com/arena/status/1797816439527637043)는 Agent Mode와 Agent Arena를 출시했습니다. 이곳에서 사용자들은 실제 작업에서 에이전트를 실행하고, 확인된 성공, 칭찬 대 불만, 조종 가능성, bash 복구, 도구 환각과 같은 집계 메트릭을 리더보드에 제공합니다 ([리더보드 세부 정보](https://twitter.com/arena/status/1797816439527637043)). 이는 평가 회사가 실행 플랫폼으로 전환되는 이번 주 가장 명확한 사례 중 하나입니다.
- 개발 도구는 단순히 인간의 UX가 아닌 에이전트 효율성을 중심으로 재구축되고 있습니다. [ClementDelangue](https://twitter.com/ClementDelangue/status/1797816439527637043)는 가장 날카로운 운영자 통찰 중 하나를 제공했습니다. 에이전트 최적화 툴링이 중요한 이유는 원시 API 상호 작용을 수동으로 처리하는 것이 Hugging Face CLI를 사용하는 것보다 최대 6배 더 많은 토큰을 소비하고 성공률이 낮았기 때문입니다. 그의 프레이밍인 "좋은 도구는 에이전트를 위한 캐시된 지능이다"는 에이전트 네이티브 개발자 플랫폼을 위한 새로운 설계 원칙을 포착합니다. 관련 출시에는 공식 Codex 플러그인으로서의 MagicPath ([skirano](https://twitter.com/skirano/status/1797816439527637043)), UI 변경의 시각적 프롬프팅을 위한 Cursor Design Mode ([cursor_ai](https://twitter.com/cursor_ai/status/1797816439527637043)), 그리고 배포를 검사하고 자연어로 재배포하기 위한 Perplexity Computer 내 Vercel 통합 ([vercel_dev](https://twitter.com/vercel_dev/status/1797816439527637043))이 포함되었습니다.
컴퓨팅, 인프라 경제학, 그리고 플랫폼 운영
- AI 인프라 경제학이 주요 이슈로 부상하고 있습니다. Epoch AI는 2026년 1분기 AI 관련 데이터 센터 건설, 컴퓨팅 하드웨어 및 네트워킹 비용이 미국 GDP의 약 0.8%에 달하며, 전체 컴퓨팅 인프라를 GDP의 약 1.5%로 끌어올릴 것으로 추정했습니다. 운영 측면에서 [eglyman](https://twitter.com/eglyman/status/1797816439527637043)은 문제가 원시 토큰 지출이 아니라 귀속 및 할당 부족이라고 주장하며, 1,000만 달러 AI 비용의 10%만 프론티어 모델에서 더 저렴한 티어로 재조정해도 거의 100만 달러를 절약할 수 있다고 언급했습니다.
- Cloudflare는 인퍼런스 라우팅을 위한 구체적인 비용 제어 기능을 출시했습니다. [CF changelog](https://blog.cloudflare.com/ai-gateway-spend-limits), [elithrar](https://twitter.com/elithrar/status/1797816439527637043), [michellechen](https://twitter.com/michellechen/status/1797816439527637043) 모두 AI Gateway 지출 한도, 모델/사용자별 예산 강제 적용, 그리고 한도 도달 시 더 저렴한 모델로의 폴백(fallback) 기능을 발표했으며, Cloudflare Access를 통한 향후 ID 기반 제어도 예정되어 있습니다. 이는 사용량이 프로토타입 규모를 넘어섬에 따라 엔터프라이즈 팀들이 현재 요구하는 바로 그런 인프라 기능입니다.
- 플랫폼/보안 사고는 여전히 중요합니다. 왜냐하면 이는 실패 모드를 드러내기 때문입니다. OpenAI는 계정 정지 사고를 겪었으며, [OpenAI가 공개적으로 인정했고](https://twitter.com/OpenAI/status/1797816439527637043), 지원팀의 후속 조치에 따르면 대부분의 계정/구독이 나중에 복원되었습니다 ([reach_vb](https://twitter.com/reach_vb/status/1797816439527637043)). OpenAI는 또한 모든 사용자에게 ChatGPT Lockdown Mode를 출시했습니다. 이는 외부 네트워크 요청을 제한하여 프롬프트 인젝션으로 인한 데이터 유출의 최종 단계를 줄이는 것을 목표로 합니다 ([cryps1s](https://twitter.com/cryps1s/status/1797816439527637043)). 별도로, Anthropic 서비스 중단이 잠재적으로 교차 테넌트 출력을 노출할 수 있다는 추측은 멀티 테넌트 격리 실패가 에이전틱/클라우드 인퍼런스 제품에서 가장 심각한 위험 중 하나로 남아 있음을 보여줍니다 ([kimmonismus](https://twitter.com/kimmonismus/status/1797816439527637043)).
인기 트윗 (참여도 기준)
- Gemma 4 QAT 출시: [@googlegemma](https://twitter.com/googlegemma/status/1797816439527637043)는 모든 Gemma 4 크기 및 드래프터용 QAT 체크포인트를 발표했으며, 저메모리 온디바이스 인퍼런스에 중점을 두었습니다.
- Anthropic의 Claude 사용량 확장: [@claudeai](https://twitter.com/claudeai/status/1797816439527637043)는 더 큰 위임 작업을 지원하기 위해 한 달 동안 Claude Cowork의 사용량 제한을 두 배로 늘렸다고 밝혔습니다.
- OpenAI 플랫폼 사고: [@OpenAI](https://twitter.com/OpenAI/status/1797816439527637043)는 잘못된 계정 정지 및 복원 작업을 보고했습니다.
- Cursor Design Mode: [@cursor_ai](https://twitter.com/cursor_ai/status/1797816439527637043)는 포인팅, 드로잉 또는 음성을 통한 멀티모달 UI 편집 기능을 출시했습니다.
- Google의 에이전틱 RAG 프레임워크: [@GoogleResearch](https://twitter.com/GoogleResearch/status/1797816439527637043)는 원샷 리트리벌이 아닌 반복적인 컨텍스트 수집을 특징으로 하는 멀티 에이전트 엔터프라이즈 RAG 워크플로우를 도입했습니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Gemma 4 QAT 및 Nemotron 3 Ultra 출시

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 무료 액세스 권한을 얻으세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-not-much-happened-today-6b8&utm_source=paywall-free-trial&utm_medium=web&utm_content=200851465&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-not-much-happened-today-6b8&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
