# not much happened today - 요약

**원문 URL**: https://www.latent.space/p/ainews-not-much-happened-today-cee
**번역일**: 2026-10-03 12:30
**발행일**: 2026-10-03

---

### 🔥 주요 뉴스

**[OpenAI, GPT-6.1 Sol 출시 및 가격 경쟁력 강화]** — OpenAI가 새로운 모델 GPT-6.1 Sol을 출시하며, 백만 입력/출력 토큰당 $2/$10의 가격으로 기존 Astra 모델($10/$50) 대비 크게 낮췄습니다. 이 모델은 DeepSWE v1.1에서 6.4점을 기록하고 AutomationBench에서 Opus 5.5를 2.2점 앞서는 등 강력한 성능을 보여주며, "좋고, 저렴하며, 빠르다"는 평가를 받고 있습니다.

**[Anthropic Sonnet 5.5 데뷔 및 Agent Arena 상위권 장악]** — Anthropic의 Sonnet 5.5 [Max]가 Agent Arena에서 3위(+12.5%)로 데뷔하며 Chat 카테고리 1위를 차지했습니다. 이로써 Anthropic 모델들은 Agent Arena 상위 3개 자리를 모두 차지하게 되었으며, Sonnet 5.5는 WebDev 벤치마크에서 GPT-6 Astra [Max]보다 2점 뒤처지지만 80% 더 낮은 비용으로 경쟁력을 확보했습니다.

**[Meta, Muse Gadgets 오픈소스화 및 스마트 홈 브리지 배포]** — Meta는 Muse와 연동되는 하드웨어 구축을 위한 ESP32 펌웨어와 Linux SDK를 오픈소스화했습니다. 또한, 자체 제작한 스마트 홈 브리지 5,000대를 구독자에게 무료로 제공하며, AI 기반 스마트 홈 생태계 확장을 위한 적극적인 움직임을 보이고 있습니다.

**[llama.cpp, 로컬 의사결정 모델 및 Qwen MTP 추측성 디코딩 지원 강화]** — llama.cpp는 로컬 "Jev 스타일" 의사결정 모델 인퍼런스를 위한 `/v1/systemone` 엔드포인트를 추가하고, Qwen3.8-Flash Next에 대한 MTP 추측성 디코딩 지원을 `--spec-type draft-mtp`를 통해 통합했습니다. 이는 로컬 LLM의 기능 확장과 인퍼런스 성능 향상에 기여하며, 특히 Qwen3.8-Flash-Next에서 디코딩 처리량이 1.55배 향상되었습니다.

**[Griffin, 비디오 튜링 테스트 통과 및 NVIDIA 벤치마크 1위 달성]** — Griffin이 비디오 튜링 테스트를 통과한 최초의 "인간 상호작용 모델"로 발표되었으며, 참가자의 44%가 이를 실제 사람으로 판단했습니다. 또한, NVIDIA의 전이중 AI 비디오 벤치마크에서 1위를 차지하여, 다른 시스템의 약 3% 대비 압도적인 성능으로 AI 비디오 분야의 새로운 이정표를 세웠습니다.

### 📊 모델 & 벤치마크

*   OpenAI가 GPT-6.1 Sol을 출시했으며, DeepSWE v1.1에서 6.4점, AutomationBench에서 Opus 5.5를 2.2점 앞섰다고 주장합니다.
*   Anthropic Sonnet 5.5 [Max]가 Agent Arena에서 3위(+12.5%)로 데뷔하며 Chat 카테고리 1위를 기록했습니다.
*   Gemini 4 Argon [High]이 Text Arena에서 1위를 차지했습니다.
*   오픈 모델 중 MiMo-V2.6-Pro와 Flash가 Agent Arena에서 각각 5위와 9위를 기록했습니다.
*   WeirdML v3 평가에서 Sol은 Astra에 근접하지만 더 낮은 피크를 보이는 토큰 효율적인 모델로 평가되었으며, Sonnet 5.5는 Opus 5를, Grok 4.7은 Kimi-K3를 이겼습니다.
*   Design Arena의 추론 스타일 분석 결과, Astra는 Opus 5.5보다 약 20배 자주 모호한 표현을 사용하며, Opus는 5개 요약 중 약 4개에서 일찍 결론을 내리는 경향을 보였습니다.
*   StepFun의 모델이 Vals에서 작업당 $2.54의 비용으로 오픈 웨이트 모델 중 7위를 기록했으며, 1M 토큰 컨텍스트 윈도우를 가집니다.
*   Perplexity는 pplx-decider-v1-27b가 11개 벤치마크에서 평균 85.7%를 기록하여 Jev를 앞섰다고 주장합니다.
*   3.66B 모델인 webAI TwIL-LM3-Pro는 형식 논리에서 Qwen3-8B와 거의 일치하는 성능을 보였으며, Q4 GGUF는 2.09 GiB입니다.
*   LessThanThreeAI가 출시한 Qwen3.8-27B-Humanlike-Chat 2.0은 IFBench, When2Call, BFCL irrelevance 등에서 개선을 보였으나, MMLU-Pro 및 LiveCodeBench에서는 회귀가 관찰되었습니다.
*   1× RTX 4090에서 Qwen3.8-27B GGUF가 DeepSWE 작업에서 40/43개의 숨겨진 테스트와 109/109개의 기존 테스트를 통과하며 프론티어 모델에 근접한 성능을 보였습니다.
*   Griffin이 비디오 튜링 테스트를 통과하여 참가자의 44%가 실제 사람으로 판단했으며, NVIDIA 전이중 AI 비디오 벤치마크에서 1위를 차지했습니다.
*   The Batch 보고서에 따르면 GLM-5.3이 취약점 악용에서 Claude Mythos와 거의 일치하는 성능(12% vs 14%)을 보였습니다.

### 🛠️ 제품 & 도구

*   OpenAI는 Sam Altman이 가장 좋아하는 제품으로 꼽은 'dots'를 출시했으며, 이는 앱 전반에 걸쳐 컨텍스트를 유지하고 Codex 작업을 조정하며 주의가 필요한 항목에 플래그를 지정합니다.
*   Meta는 Muse와 연동되는 하드웨어 구축을 위한 ESP32 펌웨어와 Linux SDK를 오픈소스화했습니다.
*   Meta는 자체 제작한 스마트 홈 브리지 5,000대를 구독자에게 무료로 제공했습니다.
*   DeepSeek Harness가 macOS 및 Windows용 데스크톱 빌드를 출시했으며, Linux 사용자들은 npm에서 `@deepseek-ai/dsh`를 설치할 수 있습니다.
*   Claude Code에 미들웨어와 같은 훅을 제공하는 플러그인과, 중요한 출력을 플래그 지정하는 보조 에이전트 "You should know" 플러그인이 추가되었습니다.
*   Pi 1.0 안정 버전이 출시되었으며, Codemode에 네이티브 MCP 지원, 비-LLM/이미지 모델 지원 등이 포함되었고, Cloudflare Durable Objects에서 실행되는 실험적인 MIT 라이선스 Pi Durable이 도입되었습니다.
*   40만 명의 사용자를 돌파한 T3 Code 오케스트레이터가 재작성되어 Pi 지원, 크로스 프로바이더 delegate_task, ACP 레지스트리, 스레드 포킹, 스레드 중간 모델 전환, 서브 에이전트 계보 보기 및 예약된 작업이 추가되었습니다.
*   OpenAI Agents API에 원콜 브라우저 컴퓨터 사용, Bedrock Managed Agents 및 휴대용 환경이 추가되었으며, 99.97%의 턴 안정성과 20% 더 빠른 도구 호출을 주장합니다.
*   Cursor Rollouts 기능은 회귀 감지 시 문제 PR을 찾아 이슈를 열고 원클릭 클라우드 에이전트 수정 기능을 제공합니다.
*   Cloudflare Sandbox SDK 1.0은 Durable Objects에 샌드박스 컨테이너에 대한 직접 제어 권한을 부여하며, Cloudflare는 request Traces도 출시했습니다.
*   llama.cpp는 로컬 "Jev 스타일" 의사결정 모델 인퍼런스를 위한 `/v1/systemone` 엔드포인트를 추가했습니다.
*   Cloudflare의 오픈 웨이트 결정 모델 Clef가 Ollama에서 사용할 수 있게 되었습니다.
*   llama.cpp PR #29761을 통해 Qwen3.8-Flash Next에 대한 MTP 추측성 디코딩 지원이 추가되었습니다.

### 🔬 연구 & 논문

*   Hugging Face는 동일한 모델 가중치가 다른 하네스에서 상이한 성능을 보이는 현상을 연구했으며, 트레이너, 데이터 및 학습된 7개 모델을 모두 오픈소스로 공개했습니다.
*   ProVer는 심사관이 결정적인 궤적 세그먼트를 찾아 이점을 설정하는 방법으로, GRPO 대비 Qwen3.5-2B에서 +9.91%, Qwen3.5-4B에서 +7.12%의 상대적 이득을 보고했습니다.
*   AC2는 학습된 비평가를 사용하여 토큰 청크에 점수를 매기므로, 학습에 부분 롤아웃만 필요하게 합니다.
*   새로운 논문은 사후 학습 후 pass@K 스케일링 가능성 손실을 정량화하고, 프롬프트당 온도 샘플러인 PTGS를 제안합니다.
*   SFT가 데이터가 오프-정책이기 때문에 일반화 성능이 더 나쁘다는 것을 발견했으며, 기본 모델의 스타일로 전문가 궤적을 다시 작성하면 격차가 줄어든다는 연구 결과가 나왔습니다.
*   Meta Superintelligence Labs는 전용 컨트롤러가 ProgramBench에서 GPT-5.5의 성능을 63.7%에서 71.5%로 향상시켰다고 보고했습니다.
*   Microsoft의 학습 없는 FOCUS는 피크 컨텍스트를 최대 48%까지 줄이고 작업 성공률을 최대 8.9점 높입니다.
*   NVIDIA Long-Transduction 연구는 7개 오픈 모델에서 4K에서 128K 컨텍스트로 전환할 때 정확도가 62.8% 하락하는 것을 측정했습니다.
*   Apple LoopCD는 반복 루프를 절반으로 줄이면서 AIME 2024 pass@1을 61.88%에서 73.33%로 높입니다.
*   Meta는 Muse Spark 1.1 및 1.2를 사용하여 일반 meta.ai 챗을 통해 생성된 미해결 문제에 대한 6편의 논문을 발표했습니다.
*   Google의 Gemini 멀티 에이전트 시스템인 Cogentic이 5개의 미해결 이론 문제에 대한 새로운 결과를 도출했습니다.
*   Arena는 Bradley-Terry 보상 모델을 충실도, 제약 및 보상 해킹 방지 보상과 결합하여 이미지 사후 학습 연구를 진행했습니다.
*   ScholarCatalyst는 에이전트에게 연구 프로젝트 뒤의 "촉매 논문"을 찾도록 요청하는 새로운 벤치마크를 공개했습니다.
*   EurekaBench는 에이전트가 6개 과학 도메인에서 진정으로 새로운 통찰력을 발견할 수 있는지 테스트하는 벤치마크를 출시했습니다.
*   에이전트가 이전 커밋에서 시작하여 이후 커밋에서 수정된 실제 버그에 대해 점수를 매기는 새로운 SWE 버그 찾기 벤치마크가 공개되었습니다.
*   새로운 논문은 학습 중 내부 신호를 사용하여 화이트박스 모니터링을 저하시키지 않으면서 정렬을 개선하는 방법을 제안합니다.
*   "Models That Know How Evaluations Are Designed Score Safer" 논문이 NeurIPS 2026에 채택되었습니다.
*   모델에게 16,200개의 위도/경도 좌표에 대해 "육지 또는 물?"이라고 질문하여 인식 가능한 세계 지도를 생성하는 실험 결과가 공유되었습니다.
*   Reka는 Apache 2.0 라이선스 하에 게임으로 학습되고 실제 비디오로 일반화되며 모터 및 카메라 동작을 추출하는 역동학 모델 RIDM을 출시했습니다.

### 💰 산업 동향

*   NYT는 Chris Olah가 교황의 AI 회칙 발표에서 철수할 것을 제기했으며, Olah 팀이 교황 고문들에게 모델 의식을 진지하게 받아들이도록 로비했다고 보도했습니다.
*   전 백악관 부비서실장이 운영하며 AI 경고를 조직적인 캠페인으로 규정하는 그룹이 최소 $100M를 지출할 계획이라는 보고서가 나왔습니다.
*   Nathan Lambert와 Tom Zick이 오픈 사후 학습 레시피 및 인프라를 위한 비영리 단체인 Trillium Labs를 설립했으며, Halcyon Futures와 Schmidt Sciences로부터 초기 지원을 받았습니다.
*   비공개 온디바이스 AI 스타트업 Underdog이 a16z, Khosla 등으로부터 지원을 발표했습니다.
*   Yoshua Bengio가 캐나다의 새로운 AI 국가 위원회에 합류했습니다.
*   블룸버그는 $150B의 자사주 매입 증가 후 Nvidia의 시가총액이 $5.7T에 육박하는 사상 최고치를 기록했다고 보도했습니다.

### ⚡ 인프라 & 하드웨어

*   DeepSeek의 오픈소스 분석을 통해 Ascend 950 칩의 레이아웃이 추론되었으며, 32개의 AI 코어와 BF16/FP8/FP4에서 약 432/865/1,730 TFLOPS의 예상 피크 성능을 가집니다.
*   Prime Intellect는 MLA 잠재 공간을 NVFP4에 저장하여 행을 576바이트에서 352바이트로 줄이고 FP8보다 약 50% 더 많은 캐시된 토큰을 저장합니다.
*   Stas Bekman은 B200에서 NVFP4가 MXFP4보다 약 9% 더 효율적이며 더 높은 정확도를 보인다고 측정했으며, mamf-finder 도구는 이제 FP8, MXFP8, MXFP4 및 NVFP4를 벤치마크합니다.
*   NVHBM은 메모리 컨트롤러를 맞춤형 베이스 다이로 이동시켜 HBM4E보다 최대 30% 더 높은 대역폭과 15% 더 낮은 전력을 주장합니다.
*   Volantis는 광학 기술을 사용하여 10T개 이상의 파라미터를 가진 모델에서 사용자당 최대 10K 토큰/초를 목표로 하는 스타트업입니다.
*   SemiAnalysis는 Google의 GPU 클러스터를 Gold 티어로 평가했으며, ConnectX NCCL 플러그인이 이제 자동 활성화된다고 언급했습니다.
*   Google Research는 검증 가능한 차등 프라이버시를 갖춘 TEE 기반 연합 학습을 출시했습니다.
*   llama.cpp 포크/분산 인퍼런스 설정을 통해 iPhone 17 Pro Max를 24GB MacBook의 보조 GPU로 활용하여 Qwen 3.8 27B 인퍼런스 성능을 최대 44% 향상시켰습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
