# New AI Infra decacorns: Fireworks, Baseten (with OpenRouter on the way) - 요약

**원문 URL**: https://www.latent.space/p/ainews-new-ai-infra-decacorns-fireworks
**번역일**: 2026-05-27 06:19
**발행일**: 2026-05-27

---

### 🔥 주요 뉴스
*   **[AI 인프라 기업 대규모 투자 유치]** — AI 인퍼런스 인프라 기업 Fireworks가 7개월 만에 3.75배 증가한 $15B 가치로 투자 라운드를 논의 중이며, Baseten은 3개월 만에 2.2배 증가한 $11B 가치로 투자를 유치 중입니다. OpenRouter는 $113M 규모의 Series C 투자를 발표하며 6개월 만에 주간 토큰 볼륨이 5배 증가했다고 밝혔습니다.
![[AINews] 새로운 AI 인프라 유니콘: Exa, Modal, TurboPuffer](https://substack-post-media.s3.amazonaws.com/public/images/ab2507aa-955-4e9d-9cbf-4c7f755a8527_1086x280.png)
![@OpenRouter의 X 아바타](https://pbs.substack.com/profile_images/1682268668321726464/NEb6_n7n.jpg)
*   **[Qwen3.7-Max 모델 출시 및 성능]** — Qwen3.7-Max가 에이전틱 코딩, 소프트웨어 엔지니어링 등 여러 벤치마크에서 Claude급 모델과 경쟁하거나 앞서는 성능을 보이며 출시되었습니다. 특히 Code Arena: Frontend에서 4위를 기록하며 Claude Opus 4.6과 거의 동등한 수준을 달성했습니다.
*   **[Huawei의 'τ 스케일링' 이론 발표]** — Huawei가 "A Time Scaling Theory for Multi-Layer Electronic Systems" 논문을 통해 장치, 칩, 데이터센터 규모 전반에 걸쳐 시간 상수 τ를 통합 측정 기준으로 삼는 엔지니어링 로드맵을 제시했습니다. 미래 Kirin 설계에 LogicFolding을 적용하여 고정 노드에서 밀도 +55%, 에너지 효율 +41%, 주파수 +13% 향상을 주장했습니다.

### 📊 모델 & 벤치마크
*   DeepSWE 벤치마크가 에이전틱 코딩을 위한 새로운 벤치마크로 출시되어 실제 개발자 경험에 더 가까운 평가를 제공합니다.
*   Qwen3.7 Max가 Code Arena: Frontend에서 4위로 데뷔하며 에이전틱 웹 개발 작업에서 Claude Opus 4.6과 거의 동등한 성능을 보였습니다.
*   PrismML이 노트북 및 휴대폰에서 로컬 실행을 위해 설계된 1비트 및 3진 변형을 포함하는 Bonsai Image 4B를 출시했습니다.
*   Microsoft의 MAI-Image-2.5가 Image Arena에서 1,254점을 기록하며 3위로 데뷔, 상위 5위 클럽에 진입했습니다.
*   Artificial Analysis는 Gemini 3.5 Flash가 최대 약 280 출력 토큰/초를 기록하며 강력한 에이전틱 성능을 보였으나, Gemini 3 Flash 비용의 약 5배에 달한다고 측정했습니다.
*   Qwen3.6 35B a3 모델이 로컬 에이전트 워크플로우에서 활용되어 VPS DevOps, 코드 티켓 등 다양한 OS 수준 작업을 수행하며, Unsloth Studio를 통해 24GB RTX Pro 4000 Blackwell SFF GPU에서 100 토큰/초 이상의 성능을 보고했습니다.
*   ik_llama.cpp가 RTX 4070 Super 12GB에서 Qwen3.6-35B-A3B MTP를 사용하여 110.24 토큰/초를 기록, 업스트림 llama.cpp 대비 23%의 처리량 향상을 달성했습니다.

### 🛠️ 제품 & 도구
*   DeepSeek은 모델 출력, 런타임 피드백, 검증 및 수정 간의 루프를 닫기 위해 명시적으로 하네스 팀을 구축하고 있습니다.
*   Google은 Gemini Managed Agents 가이드를 통해 에이전트 인프라를 샌드박싱, 영속성, 마운트를 갖춘 관리형 하네스에 대한 단일 API 호출로 구성했습니다.
*   LangChain은 `create_agent` 문서를 업데이트하여 컨텍스트 거버넌스, 신뢰할 수 있는 메모리, 동적 스킬 라우팅을 포함한 에이전트 스택을 공식화했습니다.
*   Anthropic은 Claude Code용 보안 가이드라인 플러그인을 출시하고 내부 사용에서 보안 관련 PR 댓글이 30~40% 감소했다고 보고했습니다.
*   OpenAI는 Databricks에서 Codex 내 GPT-5.5를 강조하여 더 안정적인 문서 파싱을 가능하게 했습니다.
*   vLLM은 Rust 프론트엔드를 Python API 서버의 드롭인 대체품으로 병합하여, 전처리 작업이 많은 워크로드에서 단일 프로세스 기준 약 837 req/s 대 162 req/s의 성능 향상을 보였습니다.
*   W&B는 코딩 에이전트가 실험 및 학습 실행을 검사할 수 있도록 MCP 서버를 출시했으며, 컨텍스트 윈도우 폭발을 방지하기 위한 스키마 우선 재설계를 특징으로 합니다.
*   Unsloth는 로컬 UI 내에서 GPT, Claude 및 기타 API를 실행하는 지원을 추가했으며, 프롬프트 캐싱 및 코드 실행 기능을 포함합니다.
*   Booking.com은 1억 개 이상의 임베딩으로 스케일링하는 방안을 논의하며 필터링된 벡터 검색, 쓰기 중 읽기, 동시성, 파트너 메시징 에이전트를 위한 휴먼 인 더 루프 평가를 강조했습니다.

### 🔬 연구 & 논문
*   dair.ai는 컨텍스트 거버넌스, 신뢰할 수 있는 메모리, 동적 스킬 라우팅을 포함하는 에이전트 스택에 대한 "하네스" 논문 요약을 발표했습니다.
*   Claude Mythos가 Erdős problem #90을 해결했다고 보고되었으며, 이는 적절한 하네스를 통해 모델의 잠재 능력이 크게 발휘될 수 있음을 시사합니다.
*   "Language Models Need Sleep" 논문은 최근 컨텍스트를 영속적인 고속 가중치로 변환하는 수면과 유사한 통합 단계를 제안하여 장기 기억 병목 현상에 대한 대안을 제시했습니다.
*   QUEST는 장기적인 사실 탐색, 인용 근거 마련, 보고서 합성을 위한 2B–35B 규모의 오픈 모델 제품군으로 출시되었습니다.
*   Sakana/Stanford/Oxford/AI2의 CUSP 벤치마크는 현재 모델이 유망한 연구 방향을 식별할 수 있지만, 돌파구가 언제 어떻게 실현될지에 대해서는 어려움을 겪는다는 사실을 발견했습니다.
*   AMUSE는 안정적인 기울기 평가(Stable gradient Evaluation)를 통한 Anytime MUon을 제안하며, LR 감쇠 없이 안정적인 상시 학습을 가능하게 하고 124M/720M/1B 모델에서 성능 향상을 보고했습니다.
*   MiniMax는 새로운 블록 스파스 2단계 어텐션 경로를 제안하는 M3를 오픈소스로 공개할 것을 예고했으며, 1M 토큰에서 M2 대비 9.7배의 프리필링 및 15.6배의 디코딩 속도 향상을 보고했습니다.
*   Huawei는 "A Time Scaling Theory for Multi-Layer Electronic Systems" 논문을 통해 공정 노드가 아닌 시간 상수 τ를 장치, 칩, 데이터센터 규모 전반에 걸친 통합 측정 기준으로 삼는 이론을 제시했습니다.

### 💰 산업 동향
*   AI 인퍼런스 인프라 기업 Fireworks가 $15B 가치로, Baseten이 $11B 가치로 대규모 투자 라운드를 논의/유치 중이며, OpenRouter는 $113M 규모의 Series C 투자를 발표했습니다.
*   Cloudflare는 최대 $350k의 크레딧을 제공하는 스타트업 프로그램을 재출시하여 AI 스타트업 지원을 강화했습니다.

### ⚡ 인프라 & 하드웨어
*   Huawei는 미래 Kirin 설계에 LogicFolding을 적용하여 고정 노드에서 +55% 밀도, +41% 에너지 효율, +13% 주파수 향상을 포함한 구체적인 주장을 제시했습니다.
*   SemiAnalysis는 데이터센터 전력 효율성 향상을 위한 800VDC 전환에 대해 발표했으며, 이는 EV 전력 전자공학의 고전압 SiC 부품과의 교차점을 강조합니다.
*   Epoch AI는 인퍼런스 컴퓨팅 부족 가능성을 추정하며, 특히 긴 컨텍스트 워크로드의 경우 수요가 서비스 용량보다 빠르게 증가하고 있어 공급이 수요를 따라가지 못할 수 있다고 경고했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
