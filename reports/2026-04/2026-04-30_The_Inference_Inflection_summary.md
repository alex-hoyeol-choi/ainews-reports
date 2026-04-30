# The Inference Inflection - 요약

**원문 URL**: https://www.latent.space/p/ainews-the-inference-inflection
**번역일**: 2026-04-30 06:18
**발행일**: 2026-04-30

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 간결한 브리핑입니다.

### 🔥 주요 뉴스
**[AI 인퍼런스 변곡점 도래 및 CPU 수요 급증]** — Intel CEO는 1분기 실적 발표에서 AI 인퍼런스 컴퓨팅을 위한 CPU 수요 증가를 강조했으며, Nvidia CEO는 AI가 생각하고 행동하기 위해 인퍼런스가 필요하며 지난 2년간 컴퓨팅 수요가 10,000배 증가했다고 언급했습니다. 이는 GPU 워크로드의 전례 없는 재편성 및 Groq, Cerebras 등 인퍼런스 최적화 기업에 대한 투자 흐름으로 이어지고 있습니다.
![Image](https://substack-post-media.s3.amazonaws.com/public/images/abf7db12-c072-4887-b686-4de7a38fa84c_680x380.jpeg)
![](https://substack-post-media.s3.amazonaws.com/public/images/ce489d38-e839-4154-b78d-3deb24865002_2018x1072.png)
![](https://substack-post-media.s3.amazonaws.com/public/images/6cc698ab-21d4-4776-acf8-1f3700e0ef3c_1000x1062.png)
**[OpenAI Codex, 코딩 에이전트 플랫폼으로 확장]** — OpenAI는 Codex를 코딩 도구를 넘어 연구 종합, 스프레드시트 등 광범위한 지식 작업에 활용 가능한 일반적인 작업 표면으로 확장하고 있습니다. 6월 말까지 적격 Business/Enterprise 고객을 대상으로 $0 시트 비용의 Codex 전용 시트를 출시했으며, Supabase 및 Figma 플러그인과 같은 통합 기능을 추가했습니다.
**[Mistral Medium 3.5 및 IBM Granite 4.1 모델 출시]** — Mistral은 128K 컨텍스트를 지원하는 밀집형 128B 모델인 Medium 3.5를 출시했습니다. IBM은 Apache 2.0 라이선스의 Granite 4.1 30B, 8B, 3B 오픈 웨이트 모델을 공개하며, 특히 8B 모델이 AA Openness Index에서 61점을 기록하는 등 비용 효율적인 엔터프라이즈/엣지 배포를 목표로 합니다.

### 📊 모델 & 벤치마크
*   Mistral Medium 3.5 모델이 출시되었습니다. 이는 밀집형 128B 모델로, 128K 컨텍스트를 지원하며 GGUF/가이던스가 공개되었습니다.
*   IBM Granite 4.1 모델 패밀리가 Apache 2.0 라이선스의 30B, 8B, 3B 오픈 웨이트 모델을 추가했습니다. Granite 4.1 8B는 Artificial Analysis Intelligence Index에서 Qwen3.5 9B 대비 적은 출력 토큰으로 AA Openness Index 61점을 기록했습니다.
*   Ant OSS의 Ling-2.6-flash는 약 107B MoE 모델로, MIT 라이선스 하에 61.2 SWE-bench Verified 점수와 강력한 수학 점수를 기록했습니다. Ling-2.6-1T도 vLLM 지원과 함께 출시되었습니다.
*   Tencent Hunyuan은 440MB 크기의 완전 오프라인 휴대폰용 번역 모델인 Hy-MT1.5-1.8B-1.25bit를 오픈소스화했습니다. 이 모델은 33개 언어, 1,056개 번역 방향을 지원하며, 1.25비트 양자화를 통해 상용 API 및 235B 스케일 모델과 동등한 성능을 주장합니다.
*   Qwen 3.5 Plus는 $3/M 출력 토큰, MiMo-V2.5 Pro는 Code Arena에서 $1/$3/M 토큰으로 가격이 책정되어 오픈 모델의 가격 경쟁이 심화되고 있음을 보여줍니다.

### 🛠️ 제품 & 도구
*   OpenAI는 Codex를 코딩 도구를 넘어 연구 종합, 스프레드시트, 의사 결정 추적 등 광범위한 지식 작업에 활용 가능한 일반적인 작업 표면으로 확장했습니다.
*   OpenAI는 6월 말까지 적격 Business/Enterprise 고객을 대상으로 $0 시트 비용의 Codex 전용 시트를 출시했습니다.
*   OpenAI는 Supabase 및 Figma 플러그인과 같은 Codex 통합 기능을 추가했습니다.
*   OpenAI Responses API의 WebSocket 모드는 Codex 스타일 워크플로우를 이동하여 도구 호출 전반에 걸쳐 상태를 유지하고 반복 작업을 줄여 최대 40% 더 빠른 에이전틱 워크플로우를 제공합니다.
*   VS Code는 워크스페이스 전반의 의미론적 인덱싱, 크로스-리포 검색, 채팅 세션 인사이트, 스킬 컨텍스트, Copilot CLI용 원격 제어, 프롬프트/에이전트 평가 확장 프로그램 등 병렬적인 하네스 개선 스택을 출시했습니다.
*   Cursor는 새로운 Cursor SDK를 출시하여 Cursor를 구동하는 동일한 런타임, 하네스 및 모델을 CI/CD, 자동화 및 제품 내 임베디드 에이전트에서 사용할 수 있도록 노출했습니다.
*   LangChain은 모델별 프롬프트, 도구 및 미들웨어를 버전 관리할 수 있는 새로운 Harness Profiles를 출시했으며, OpenAI, Anthropic, Google 모델에 대한 내장 프로파일을 제공합니다.
*   LangChain은 소수의 마크다운/설정 파일과 LangSmith 기반 트레이싱을 사용하는 로우코드 배포 경로인 DeepAgents Deploy를 출시했습니다.
*   Cloudflare는 에이전트가 Cloudflare 고객이 될 수 있도록 하는 아이디어(계정 생성, 도메인 등록, 유료 플랜 시작, 배포를 위한 토큰 확보)를 통해 "에이전트를 소프트웨어로" 스택을 구체화했습니다.

### 🔬 연구 & 논문
*   Incompressible Knowledge Probes (IKP) 연구는 1,400개 질문, 188개 모델, 27개 공급업체에 대한 사실적 지식 정확도가 모델 크기(135M에서 1.6T 파라미터)의 강력한 로그 선형 신호(R² = 0.917)를 제공한다고 주장합니다. 이 연구는 사실적 용량이 시간이 지남에 따라 압축되지 않으며, 피팅된 곡선을 사용하여 클로즈드 모델 크기를 추정할 수 있다고 제안합니다.
*   Agentic Harness Engineering 연구는 되돌릴 수 있는 구성 요소, 응축된 실행 증거, 반증 가능한 예측을 통해 하네스 진화를 관찰 가능하게 만듭니다. Terminal-Bench 2 pass@1에서 10번의 반복을 통해 69.7%에서 77.0%로 향상되었으며, SWE-bench Verified에서 토큰 사용량을 12% 감소시켰습니다.
*   HALO에 대한 관련 연구는 트레이스 분석을 사용하여 하네스 실패를 패치하는 재귀적으로 자체 개선하는 에이전트를 설명하며, Sonnet 4.6에서 AppWorld 성능을 73.7에서 89.5로 개선했다고 주장합니다.

### 💰 산업 동향
*   OpenAI는 코딩 에이전트 Codex를 일반적인 작업 표면으로 확장하며, Business/Enterprise 고객 대상 $0 시트 비용의 Codex 전용 시트를 출시하는 등 플랫폼 전략을 강화하고 있습니다.
*   Cursor는 새로운 SDK 출시를 통해 시트 기반 IDE 제품에서 프로그래밍 가능한 에이전트 인프라로 전환하는 명시적인 플랫폼 전략을 펼치고 있습니다.
*   클로즈드 모델이 많은 에이전트 워크로드에 너무 비싸지고 있어 오픈 하네스, 오픈 평가, OSS 친화적인 모델 조합의 중요성이 강조되고 있습니다.
*   인퍼런스 변곡점 도래와 함께 Nvidia의 Groq 인수, Intel-Sambanova, Amazon의 Cerebras 유사 흐름 참여 등 GPU 워크로드 재편성을 위한 산업 움직임이 활발합니다.

### ⚡ 인프라 & 하드웨어
*   Alibaba Qwen은 TileLang 기반 고성능 선형 어텐션 커널인 FlashQLA를 소개했습니다. 이 커널은 작은 모델, 긴 컨텍스트 워크로드, 텐서 병렬 설정에서 순방향 2~3배, 역방향 2배의 속도 향상을 보고했습니다.
*   vLLM은 Artificial Analysis에서 DeepSeek V3.2에 대해 230 tok/s의 출력 속도, 0.96s TTFT를 보고했으며, NVIDIA HGX B300의 DigitalOcean 서버리스 인퍼런스를 사용하는 Qwen 3.5 397B에서도 NVFP4 양자화, EAGLE3 + MTP 추측 디코딩, 모델별 커널 퓨전 등의 최적화를 통해 강력한 결과를 보여주었습니다.
*   SemiAnalysis는 vLLM 0.20.0 및 GB200의 DeepSeek v4 Pro용 MegaMoE 커널에서 얻은 개선 사항을 강조했습니다.
*   Zhipu AI는 GLM-5 서빙 사후 분석을 발표하며 KV 캐시 경쟁 조건, HiCache 동기화 버그, 그리고 긴 컨텍스트 코딩 에이전트 서빙을 위한 프리필 처리량을 최대 132%까지 개선했다고 보고된 LayerSplit에 대해 자세히 설명했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
