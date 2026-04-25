# DeepSeek V4 Pro (1.6T-A49B) and Flash (284B-A13B), Base and Instruct — runnable on Huawei Ascend chips - 요약

**원문 URL**: https://www.latent.space/p/ainews-deepseek-v4-pro-16t-a49b-and
**번역일**: 2026-04-25 06:21
**발행일**: 2026-04-25

---

### 🔥 주요 뉴스
**[DeepSeek V4 Pro 및 Flash 출시]** — DeepSeek이 1M 토큰 컨텍스트를 지원하는 DeepSeek V4 Pro (1.6T, 49B 활성) 및 DeepSeek V4 Flash (284B, 13B 활성) 모델을 MIT 라이선스 하에 출시했습니다. 이 모델들은 Compressed Sparse Attention (CSA) 및 Heavily Compressed Attention (HCA) 기술을 통해 KV 캐시 효율성을 크게 개선했으며, Huawei CANN 호환성을 지원합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/a10f0270-c9c4-481b-962a-fcba50a2418b_1022x1104.png)
**[OpenAI GPT-5.5 및 GPT-5.5 Pro 출시]** — OpenAI가 1M 컨텍스트 윈도우를 갖춘 GPT-5.5 및 GPT-5.5 Pro를 API 및 생태계 제품에 출시했습니다. 이 모델들은 CursorBench 및 Terminal-Bench에서 1위를 기록하는 등 코딩 및 복잡한 작업에서 뛰어난 성능과 토큰 효율성을 보였습니다.
**[Google, Anthropic에 최대 $40B 투자 계획]** — Google이 Anthropic에 최대 $40B를 투자할 계획이라고 보도되었습니다. 이는 AI 산업 내 주요 기업 간의 전략적 제휴 및 자금 조달 규모를 보여주는 중요한 소식입니다.
**[DeepSeek, DeepEP V2 및 TileKernels 공개]** — DeepSeek이 모델 효율성 및 정확성 향상에 중점을 둔 DeepEP V2와 계산 용량에 비례하여 처리 속도가 선형적으로 스케일링되는 새로운 병렬화 기술인 TileKernels를 오픈소스로 공개했습니다.
**[Hugging Face, 오픈소스 CLI 'ML Intern' 출시]** — Hugging Face가 논문 연구, 코드 작성, 실험 실행, GitHub 검색 등 ML 작업을 위한 오픈소스 CLI 'AI 인턴'인 ML Intern을 출시했습니다. 이는 최대 300단계 반복을 수행할 수 있습니다.

### 📊 모델 & 벤치마크
*   DeepSeek V4 Pro (총 1.6T 파라미터, 49B 활성) 및 V4 Flash (총 284B 파라미터, 13B 활성)가 출시되었으며, 두 모델 모두 1M 토큰 컨텍스트 길이를 지원하고 MIT 라이선스 하에 제공됩니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/f028c03e-53a7-4615-af85-fc5e6e11dab0_1226x940.png)
*   DeepSeek V4 Pro는 Artificial Analysis Intelligence Index에서 52점을 기록하여 오픈 웨이트 추론 모델 중 2위를 차지했으며, 에이전틱 실세계 작업(GDPval-AA)에서 1554점으로 오픈 웨이트 모델 중 선두를 기록했습니다.
*   DeepSeek V4 Flash의 공식 API 가격은 1M 입력 토큰당 $0.14, 1M 출력 토큰당 $0.28로 책정되었으며, JSON 출력, 툴 콜, 사고/비사고 모드를 지원합니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/a10f0270-c9c4-481b-962a-fcba50a2418b_1022x1104.png)
*   GPT-5.5는 CursorBench에서 72.8%, Terminal-Bench에서 82.7%로 1위를 기록했으며, Perplexity Computer에서 복잡한 작업에 56% 더 적은 토큰을 사용했습니다.
*   Qwen 3.6 27B는 Artificial Analysis의 에이전틱 인덱스에서 Sonnet 4.6과 동등한 수준을 달성하며 Gemini 3.1 Pro Preview, GPT 5.2 및 5.3, MiniMax 2.7과 같은 모델들을 능가했습니다.
*   DS4-Flash Max는 LiveCodeBench 및 HLE 벤치마크에서 Qwen3.6 모델(35B-A3B 및 27B)을 일반적으로 능가하는 성능을 보였습니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/a10f0270-c9c4-481b-962a-fcba50a2418b_1022x1104.png)
*   Qwen3.6 27B 모델은 MacBook Pro에서 llama.cpp를 통해 로컬 실행이 가능하며, 코딩 작업에서 인상적인 성능을 보였습니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/a10f0270-c9c4-481b-962a-fcba50a2418b_1022x1104.png)

### 🛠️ 제품 & 도구
*   Hugging Face는 논문 연구, 코드 작성, 실험 실행, HF 데이터셋/작업 사용, GitHub 검색 등을 수행할 수 있는 오픈소스 CLI 'AI 인턴'인 ML Intern을 출시했습니다.
*   Nous/Hermes는 재작성된 React TUI, 대시보드 플러그인, 테마, 더 많은 인퍼런스 제공업체, 이미지 백엔드, QQBot 지원을 도입한 Hermes Agent v0.11.0을 출시했습니다.
*   Cursor는 /multitask 비동기 서브에이전트 및 다중 루트 워크스페이스 기능을 출시했습니다.
*   Deep Agents를 위한 bubblewrap + cgroups v2를 사용하는 네이티브 Linux 샌드박스 백엔드가 출시되었습니다.

### 🔬 연구 & 논문
*   DeepSeek은 모델 효율성 및 정확성 향상에 중점을 둔 DeepEP V2와 계산 용량에 비례하여 처리 속도가 선형적으로 스케일링되는 병렬화 기술인 TileKernels를 오픈소스로 공개했습니다.
*   DeepSeek V4는 새로운 Compressed Sparse Attention (CSA) 및 Heavily Compressed Attention (HCA) 기술을 도입하여 1M 토큰 컨텍스트에서 DeepSeek V3.2 대비 FLOPs를 27%, KV 캐시 메모리를 10%만 필요로 합니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/f73b6f70-b4a0-46e8-8452-7cced7481ba9_1156x730.png)
*   온-폴리시 디스틸레이션 토큰 선택에 관한 논문은 일부 토큰(약 50%)만이 대부분의 학습 신호를 전달하며 메모리를 약 47% 절감할 수 있음을 강조했습니다.
*   Google Research는 고정 메모리 하에서 인컨텍스트 학습에 최적화된 트랜스포머 대체/선형 시퀀스 레이어인 MesaNet을 포함한 여러 ICLR 데모를 발표했습니다.
*   MIT Hyperloop Transformers는 루프형 및 일반 트랜스포머 블록을 혼합하여 약 50% 적은 파라미터를 사용하면서 240M/1B/2B에서 일반 트랜스포머를 능가합니다.
*   Tool Attention Is All You Need 논문은 동적 게이팅 및 지연 스키마 로딩을 통해 95%의 도구 토큰 감소(47.3k → 2.4k/턴)를 주장했습니다.

### 💰 산업 동향
*   Google은 Anthropic에 최대 $40B를 투자할 계획이라고 보도되었습니다.
*   Cohere와 Aleph Alpha는 엔터프라이즈급 및 개인 정보 보호/보안에 중점을 둔 캐나다/독일 주권 AI 파트너십을 발표했습니다.
*   ComfyUI는 $500M의 가치로 $30M를 유치했으며, Mechanize는 $500M의 투자 후 가치로 $9.1M를 유치했습니다.
*   OpenAI는 GPT-5.5에 대한 Bio Bug Bounty를 발표했으며, Anthropic은 Claude가 직원들을 대신하여 협상하는 마켓플레이스인 Project Deal을 출시했습니다.

### ⚡ 인프라 & 하드웨어
*   DeepSeek V4는 Huawei CANN 호환성을 지원하여 NVIDIA/CUDA 칩에 대한 의존도를 줄이고 중국의 AI 독립을 위한 중요한 이정표를 마련했습니다.
*   DeepSeek V4 체크포인트는 FP4 + FP8 혼합 정밀도를 사용하며, 전체 모델이 단일 8×B200 노드에 적합합니다.
*   Meta는 수십억 명의 사용자를 위한 Meta AI 및 에이전틱 시스템 확장을 위해 AWS Graviton 코어 수천만 개를 컴퓨팅 포트폴리오에 추가할 것이라고 밝혔습니다.
*   DeepSeek은 H2에 Huawei Ascend 950 슈퍼노드가 대규모로 배포되면 V4 Pro 가격이 급격히 하락할 수 있다고 언급했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
