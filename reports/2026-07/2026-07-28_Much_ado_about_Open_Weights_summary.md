# Much ado about Open Weights - 요약

**원문 URL**: https://www.latent.space/p/ainews-much-ado-about-open-weights
**번역일**: 2026-07-28 06:35
**발행일**: 2026-07-28

---

### 🔥 주요 뉴스
**[Moonshot AI, Kimi K3 오픈 웨이트 모델 출시]** — Moonshot AI가 세계 최고 성능의 오픈 웨이트 모델 Kimi K3를 출시했습니다. 이 모델은 2.8T 파라미터 MoE, 104B 활성 파라미터, 1M 토큰 컨텍스트 및 네이티브 시각 이해 기능을 갖추고 있으며, Opus 4.8을 능가하는 것으로 검증되었습니다. FlashKDA, MoonEP, AgentENV 등 대규모 에이전트 학습 및 서빙을 위한 인프라도 함께 오픈소스화했습니다.

**[NVIDIA, Open Secure AI Alliance 공식 출범]** — NVIDIA가 Microsoft, Hugging Face 등과 협력하여 Open Secure AI Alliance를 공식 출범했습니다. 이 연합은 공격자들이 이미 강력한 AI를 보유하고 있으므로, 방어자들은 오픈 및 클로즈드 프론티어 모델을 아우르는 공유 툴링 및 연구 생태계가 필요하다는 점을 강조합니다.

**[미국 정부, 프론티어 AI 모델 사전 출시 검토 요구 가능성]** — 미국 정부가 NSA 및 CAISI와 같은 기관의 평가를 위해 프론티어 시스템에 대한 최대 30일간의 사전 출시 액세스를 요구할 수 있다는 보도가 나왔습니다. 이는 프론티어 모델 출시가 단순한 제품 출시를 넘어 거버넌스 인터페이스가 되고 있음을 시사합니다.

**[Anthropic, 오픈 웨이트 모델에 대한 입장 명확화]** — Anthropic이 오픈 웨이트 모델 금지를 옹호한 적이 없다고 공식적으로 밝혔습니다. 대신 중국에 대한 칩 통제, 산업 규모 디스틸레이션 방지 조치, 그리고 충분히 유능한 모델에 대한 의무적인 안전성 테스트를 지지한다고 발표했습니다.

### 📊 모델 & 벤치마크
*   Moonshot AI는 Kimi K3의 웨이트, 보고서 및 지원 인프라를 오픈 웨이트 패키지로 출시했습니다. Kimi K3는 2.8T 파라미터 MoE, 104B 활성 파라미터, 토큰당 896명의 전문가 / 16명 활성, 1M 토큰 컨텍스트, 네이티브 시각 이해 기능을 갖추고 있습니다.
*   Kimi K3는 K2 대비 약 2.5배의 스케일링 효율성 개선을 보고했으며, MXFP4 웨이트 / MXFP8 활성화 및 안정성을 위한 비전 인코더의 처음부터 공동 학습에 중점을 둔 아키텍처를 특징으로 합니다.
*   Kimi K3 Max는 Agent Arena에서 오픈 웨이트 모델 중 넷 개선율 +9.75%로 1위를 차지했으며, Frontend Code Arena에서도 모든 모델 중 전체 1위를 기록했습니다.
*   Cognition은 Kimi K3가 FrontierCode 1.1에서 58.2%의 점수와 63.6%의 통과율을 기록하며 "프론티어 수준의 성능에 근접하는" 첫 번째 오픈소스 모델이라고 밝혔습니다.
*   Arena는 Claude Opus 5 Max가 Frontend Code Arena와 Text Arena에서 사실성 부문 1위를 차지했다고 보고했으며, WeirdML 수치에서 Opus 5 high/max는 91.6% / 91.8%를 기록했습니다.
*   _philschmid는 에이전트가 이전 동작을 손상시키지 않고 진화하는 요구 사항을 따를 수 있는지 측정하는 평가 도구인 EvoCode를 강조했습니다.
*   omarsar0는 에이전트 스킬이 이점을 생성하지만, 이 스킬 없이 이전에 해결되었던 많은 작업을 망가뜨리는 "회귀세(regression tax)"를 보여주는 논문을 요약했습니다.
*   omarsar0의 또 다른 논문 요약은 다중 모듈 RL 시스템에서 엔드투엔드 RL이 파이프라인 정확도를 향상시키면서도 모듈이 의도된 책임을 조용히 포기하게 만들 수 있는 "역할 표류(role drift)" 현상을 설명했습니다.

![moonshotai/Kimi-K3의 Hugging Face 페이지 모바일 스크린샷](https://substack-post-media.s3.amazonaws.com/public/images/db0f8d45-1eb8-4c02-a120-650d377ee52d_640x640.jpeg)

### 🛠️ 제품 & 도구
*   Moonshot AI는 Kimi K3와 함께 FlashKDA (Kimi Delta Attention 커널), MoonEP (MoE 통신 라이브러리), AgentENV (분산 에이전트 환경 인프라)를 오픈소스화했습니다.
*   Microsoft는 라이브 이벤트 이해를 위한 코덱-네이티브 스트리밍 VLM인 Mage-VL 4B를 출시했습니다.
*   NVIDIA 연구팀은 인간과 AI 코딩 어시스턴트가 엔드투엔드로 추론할 수 있을 만큼 작게 설계된 PyTorch-네이티브 에이전틱 RL 프레임워크인 Molt를 공개했습니다.
*   Cohere는 보안 에이전트 플랫폼 위에 구축된 평이한 언어 워크플로우 레이어인 North Automations를 발표했습니다.

### 🔬 연구 & 논문
*   EvoCode는 영구 컨테이너에서 26개의 작업 / 227개의 순차 라운드를 중심으로 구축된 평가 도구로, 에이전트가 이전 동작을 손상시키지 않고 진화하는 요구 사항을 따를 수 있는지 측정합니다.
*   에이전트 스킬로 인한 "회귀세(regression tax)"는 스킬이 이점을 생성하지만, 이 스킬 없이 이전에 해결되었던 많은 작업을 망가뜨릴 수 있음을 보여줍니다.
*   다중 모듈 RL 시스템에서 "역할 표류(role drift)"는 엔드투엔드 RL이 파이프라인 정확도를 향상시키면서도 모듈이 의도된 책임을 조용히 포기하게 만들 수 있음을 설명합니다.

### 💰 산업 동향
*   NVIDIA는 Microsoft, Hugging Face, LangChain, Nous Research 등과 함께 Open Secure AI Alliance를 공식 출범했습니다.
*   Anthropic은 오픈 웨이트 모델 금지를 옹호한 적이 없으며, 대신 중국에 대한 칩 통제, 산업 규모 디스틸레이션 방지 조치, 의무적 안전성 테스트를 지지한다고 입장을 명확히 했습니다.
*   미국 정부는 NSA 및 CAISI와 같은 기관의 평가를 위해 프론티어 시스템에 대한 최대 30일간의 사전 출시 액세스를 요구할 수 있다는 보도가 나왔습니다.
*   NYT는 OpenAI와 Anthropic이 미국 규제 당국에 오픈/오픈 웨이트 AI 모델, 특히 프론티어 미국 모델 능력에 근접하는 중국 출시 모델에 대한 제한을 위해 로비해왔다고 보도했습니다.
*   Ilya Sutskever의 "SSI를 확장할 시간"이라는 발언과 후속 보도는 Vera Rubin에서 Safe Superintelligence를 위한 대규모 컴퓨팅 확장을 시사합니다.
*   LangChain은 기업이 모델 액세스를 임대하는 것뿐만 아니라 도구, 프롬프트, 컨텍스트, 메모리를 소유해야 한다고 강조하며 "하네스를 소유하라"는 방향으로의 전환을 지속적으로 주장했습니다.
*   OpenAI는 업무용 연구와 클라우드 에이전트 / Work mode를 둘러싼 광범위한 추진을 통해 챗봇 UX에서 임베디드 개인 및 엔터프라이즈 자동화로의 전환을 시사하고 있습니다.

![Jensen Huang이 Hugging Face 보안 사건 동안 클로즈드 AI 시스템이 필수적인 포렌식 분석을 방해한 반면, 오픈 웨이트 프론티어 모델은 방어자들이 침입을 억제하는 데 도움이 되었다고 주장하는 스크린샷](https://substack-post-media.s3.amazonaws.com/public/images/db0f8d45-1eb8-4c02-a120-650d377ee52d_640x640.jpeg)
![NYT는 OpenAI와 Anthropic이 미국 규제 당국에 오픈/오픈 웨이트 AI 모델, 특히 프론티어 미국 모델 능력에 근접하는 Z.ai 및 Moonshot AI의 중국 출시 모델에 대한 제한을 위해 로비해왔다고 보도했습니다.](https://substack-post-media.s3.amazonaws.com/public/images/db0f8d45-1eb8-4c02-a120-650d377ee52d_640x640.jpeg)

### ⚡ 인프라 & 하드웨어
*   Kimi K3는 8×A100 80GB로는 멀티 노드 샤딩 없이 웨이트를 담을 수 없으며, 8×H200 (~1.13TB)도 최소 두 개의 노드가 필요하고, 8×B300 (~2.3TB)이 웨이트와 긴 컨텍스트 KV 캐시 및 네이티브 FP4를 위한 공간을 갖춘 유일한 단일 노드 구성으로 언급되었습니다.
*   AMD는 MI300X/MI325X에서 학습된 첫 번째 완전 오픈 MoE LM인 Instella-MoE (총 16B / 활성 2.8B 파라미터)를 출시했습니다. 이는 사전 학습부터 RL까지의 체크포인트, 구성, 데이터 혼합 및 코드를 포함하는 풀스택 연구 아티팩트입니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
