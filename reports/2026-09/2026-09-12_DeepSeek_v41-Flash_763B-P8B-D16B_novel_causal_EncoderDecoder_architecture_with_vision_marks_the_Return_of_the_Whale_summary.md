# DeepSeek v4.1-Flash: 763B-P8B-D16B novel causal Encoder–Decoder architecture with vision marks the Return of the Whale - 요약

**원문 URL**: https://www.latent.space/p/ainews-deepseek-v41-flash-763b-p8b
**번역일**: 2026-09-12 07:02
**발행일**: 2026-09-12

---

### 🔥 주요 뉴스
**[DeepSeek v4.1-Flash 출시: 새로운 아키텍처와 비전 기능으로 고효율 달성]** — DeepSeek이 새로운 인과적 Encoder–Decoder 아키텍처와 비전 기능을 갖춘 v4.1-Flash 모델(총 763B 파라미터, 활성 입력 8B/출력 16B)을 출시했습니다. 이 모델은 이전 V4 Pro를 능가하며 KV 캐시 풋프린트를 최대 1/8로 줄여 극도의 추론 효율성과 낮은 비용을 제공합니다.
**[OpenAI, GPT-Live-1 API 및 에이전트 API 공개로 실시간 음성 및 엔터프라이즈 기능 강화]** — OpenAI가 전이중 음성 인터페이스인 GPT-Live-1을 API에 출시하고, 코드 실행 및 파일 관리를 위한 호스팅 샌드박스를 포함한 Agents API 공개 베타를 발표했습니다. 또한 기업 데이터 소스에 연결되는 ChatGPT Work 데이터 에이전트를 선보이며 엔터프라이즈 AI 솔루션을 확장합니다.
**[Cognition, SWE-2 및 Devin Voice 출시로 코딩 에이전트 성능 및 비용 효율성 혁신]** — Cognition이 선도적인 코딩 평가에서 최대 70% 낮은 비용으로 동등한 성능을 주장하는 SWE-2 모델을 출시하고, GPT-Live 및 SWE-2 기반의 Devin Voice를 공개했습니다. 이는 RL을 수조 개의 파라미터로 확장하고 개발자 워크플로우 통합을 강화하는 움직임입니다.
**[Anthropic, Claude 오용에 대한 상세 위협 인텔리전스 보고서 발표]** — Anthropic이 사이버 공격, 영향력 작전, 감시, 생물학 및 무기 개발을 위한 Claude 사용 시도에 대한 가장 상세한 오용 보고서를 발표했으며, 설명된 모든 작전을 방해했다고 밝혔습니다.

### 📊 모델 & 벤치마크
*   DeepSeek이 새로운 인과적 Encoder–Decoder 아키텍처와 비전 기능을 갖춘 v4.1-Flash 모델을 출시했습니다. 이 모델은 총 763.21B 파라미터(활성 입력 8B, 활성 출력 16B)를 가지며, 1M 토큰 컨텍스트를 지원합니다.
*   DeepSeek v4.1-Flash는 Artificial Analysis Intelligence Index에서 40점을 기록하여 V4 Pro 0813을 능가하고 GLM-5.3-Flash 바로 아래에 위치했습니다. AutomationBench-AA에서 69%, GDPval-AA v2에서 1632 Elo, AA-LCR v1.1에서 84%를 달성했습니다.
*   Vals Index에서는 테스트당 $0.30으로 #1 오픈 웨이트 모델로 평가되었으며, Artificial Analysis는 Intelligence Index 작업당 $0.27로 이전 모델 대비 약 2.5~7배 낮은 비용을 추정했습니다.
*   DeepSeek은 V4.1-Flash가 성능, 비용, 속도 면에서 V4 Pro를 능가함에 따라 DeepSeek V4 Pro 0813을 사실상 소프트 은퇴시키고, 해당 트래픽을 V4.1-Flash로 라우팅하며 더 저렴한 Flash 가격으로 청구합니다.
*   Cognition이 SWE-2를 출시하며 선도적인 코딩 평가에서 최대 70% 낮은 비용으로 프론티어에 가까운 성능을 주장하고, RL을 수조 개의 파라미터로 스케일링했다고 밝혔습니다.

### 🛠️ 제품 & 도구
*   OpenAI가 전이중 음성 인터페이스인 GPT-Live-1을 API에 출시하여 개발자가 어조, 속도, 표현력, 응답 길이 및 언어를 제어할 수 있도록 했습니다.
*   OpenAI는 코드 실행, 파일 및 아티팩트 관리를 위한 호스팅 샌드박스를 포함한 Agents API 공개 베타와 관리형 클라우드 에이전트를 발표했습니다.
*   ChatGPT Work 데이터 에이전트가 출시되어 연결된 회사 데이터 소스에 대한 대시보드, 답변 및 작업을 제공합니다.
*   Cognition이 GPT-Live 및 SWE-2 기반의 Devin Voice를 출시하여 개발자 워크플로우에 멀티모달 기능을 통합했습니다.
*   Cursor가 코디네이터 에이전트, 공유 메모리 및 동기화된 아티팩트를 갖춘 영구 스레드를 도입하는 새로운 "Projects" 기능을 출시했습니다.
*   Baseten과 Ollama가 DeepSeek v4.1-Flash 출시 당일(day-0) 또는 빠르게 지원을 시작했습니다.
*   vLLM의 새로운 릴리스에 DeepSeek-V4 공유 전문가(experts)가 통합되었으며, Mooncake Store는 디코드 KV를 오프로드할 수 있도록 지원합니다.

### 🔬 연구 & 논문
*   DeepSeek v4.1-Flash 기술 보고서는 프리필(8B) 및 디코드(16B) 파라미터를 분리하는 새로운 인과적 Encoder–Decoder 아키텍처를 상세히 설명합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/149285a5-df59-4df7-8ba9-4653b68c5f0b_2316x1122.png)
*   이 모델은 Sliding-Window Attention Bounded Replay와 같은 새로운 조정과 결합하여 KV 캐시 풋프린트를 V4 Flash의 최대 1/8로 줄이고, 1세대 모델 대비 437배의 KV-캐시/저장 공간 감소를 주장합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/2ecf8d27-1a84-4919-b168-7416a85dad48_1390x684.png)
*   Salesforce 연구는 약한 모델을 강한 전문가 궤적에 학습시킬 때 하네스 진화 후 성능 저하가 발생할 수 있음을 보여주며, 실패한 턴만 다시 작성하여 모델-하네스 적합성을 유지하는 해결책을 제안했습니다.
*   ByteDance의 HarnessDev 연구는 자체 실행 가능한 하네스를 구축하고 반복적으로 개선하는 에이전트를 설명했으며, 혼합된 일반화 결과를 보였습니다.
*   Qwen의 Elastic Horizon 연구는 성공적인 궤적 길이의 90번째 백분위수를 추적하여 최대 상호작용 호라이즌을 조정하는 폐쇄 루프 컨트롤러를 통해 성공률을 높이고 궤적 토큰을 최대 25% 절약합니다.
*   PARSER 연구는 순차적 청크 읽기를 병렬 고정 하위 에이전트와 RL 학습된 리드 에이전트로 대체하여 896K 컨텍스트에서 +12점 향상 및 최대 11배 낮은 레이턴시를 달성했습니다.
*   SkillAdam 연구는 스킬 자기 진화를 이산 최적화 문제로 프레이밍하고 Adam과 유사한 아이디어를 차용하여 업데이트 방향과 편집 크기를 안정화합니다.
*   Google Research의 ToolGrad는 프롬프트 전에 그라운드 트루스 도구 사용 체인을 생성하여 데이터셋 생성 및 다운스트림 도구 사용 이점에서 거의 100%의 통과율을 보고합니다.

### 💰 산업 동향
*   DeepSeek은 V4.1-Flash의 우수한 성능과 비용 효율성으로 인해 DeepSeek V4 Pro 0813을 사실상 소프트 은퇴시키고, 기존 V4 Pro 트래픽을 V4.1-Flash로 자동 라우팅하며 더 저렴한 Flash 가격으로 청구합니다.
*   Dioxus Labs가 Cognition에 합류하여 Devin의 VM, 컴퓨터 사용 및 테스트에 기여하고 Dioxus 및 관련 Rust OSS에 대한 지원을 계속하기로 발표했습니다.
*   OpenAI는 Astra 용량 문제로 새로운 $200 Pro 구독 가입을 일시 중지했습니다.
*   Anthropic이 사이버 공격, 영향력 작전, 감시, 생물학 및 무기 개발을 위한 Claude 오용 시도에 대한 상세한 위협 인텔리전스 보고서를 발표하고 모든 시도가 방해되었음을 밝혔습니다.

### ⚡ 인프라 & 하드웨어
*   DeepSeek v4.1-Flash는 이전 V4 Flash 대비 KV 캐시 풋프린트를 최대 1/8로 줄였으며, 1세대 모델 대비 437배의 KV-캐시/저장 공간 감소를 주장합니다.
*   Fraser Price는 64GB 시스템 RAM과 4개의 Max-Q GPU만으로 풀-프리시전 DeepSeek 4.1 Flash + DSpark를 200 TPS(나중에는 300+ TPS)로 실행했으며, 200GB Engram/해시 테이블을 NVMe로 오프로드했습니다.
*   Antirez는 128GB M5 Max에서 SSD 스트리밍을 통해 DwarfStar가 V4.1 Flash를 예상외로 빠르게 실행하는 것을 시연했습니다.
*   vLLM의 새로운 릴리스는 DeepSeek-V4 공유 전문가(experts)를 통합하고 Mooncake Store를 통해 디코드 KV를 오프로드할 수 있도록 지원하여 오픈 인프라에서 이러한 모델의 서빙을 용이하게 합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
