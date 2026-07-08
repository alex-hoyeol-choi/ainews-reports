# Lilian Weng summarizes 35 papers on Harness Engineering for RSI - 요약

**원문 URL**: https://www.latent.space/p/ainews-lilian-weng-summarizes-35
**번역일**: 2026-07-08 06:53
**발행일**: 2026-07-08

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식에 대한 브리핑입니다.

### 🔥 주요 뉴스
**[Meta Muse Image/Video 출시 및 성능]** — Meta Superintelligence Labs가 Muse Image를 출시하고 Muse Video를 미리 공개했습니다. 이 모델들은 계획, 웹 검색, 도구 사용, 코드 실행 및 자체 개선을 포함하는 에이전틱 생성 루프를 특징으로 하며, Muse Image는 Arena에서 GPT Image 2에 이어 2위, Muse Video는 Video Arena 3위를 기록했습니다.
**[Tencent Hy3 모델 Apache 2.0 라이선스 출시]** — Tencent가 총 295B 파라미터, 활성 21B MoE 모델인 Hy3의 오픈 모델 컬렉션을 Hugging Face에 출시했습니다. 이전의 제한적인 커뮤니티 라이선스와 달리 Apache 2.0 라이선스를 채택하여 한국, 영국, EU 등 이전 사용이 제한되었던 지역에서도 상업적 활용이 가능해졌습니다.
**[Liquid AI의 Antidoom 학습 방법 공개]** — Liquid AI가 작은 추론 모델의 컨텍스트 고갈로 인한 둠 루프를 줄이는 오픈소스 학습 방법인 Antidoom을 발표했습니다. 이 방법(FTPO)은 루프를 유발하는 토큰을 재라벨링하고 확률을 재분배하여 LFM2.5-2.6B에서 둠 루프를 10.2%에서 1.4%로, Qwen3.5-4B에서 22.9%에서 1%로 크게 감소시켰습니다.
**[Norm Ai, 1.2억 달러 Series C 투자 유치]** — 에이전틱 법률 시스템을 개발하는 Norm Ai가 12억 달러 가치로 1억 2천만 달러 규모의 Series C 투자를 유치했습니다. 이 회사는 소프트웨어와 AI 네이티브 로펌을 아우르는 풀스택 법률 AI 시스템을 구축하고 있습니다.

### 📊 모델 & 벤치마크
*   Meta Superintelligence Labs가 Muse Image를 출시하고 Muse Video를 미리 공개했습니다. Muse Image는 Arena에서 GPT Image 2에 이어 Image Arena 2위를, Muse Video는 Video Arena 3위를 기록했습니다.
*   NVIDIA가 통합 텍스트+오디오 작업을 위한 1M 컨텍스트를 가진 30B 파라미터 / 3B 활성 MoE 모델인 Audex를 출시했습니다. 이 모델은 단일 MoE 백본을 통해 텍스트 지능을 보존하며 광범위한 오디오 생성 및 이해 기능을 추가합니다.
*   Cohere가 Apache 2.0 라이선스 하에 가장 정확한 오픈소스 아랍어 ASR 모델인 Cohere Transcribe Arabic을 출시했습니다. 이 모델은 방언, 코드 스위칭 및 아랍어 억양의 영어에 중점을 둡니다.
*   Tencent가 총 295B 파라미터, 활성 21B MoE 모델인 Hy3의 오픈 모델 컬렉션을 Apache 2.0 라이선스 하에 Hugging Face에 출시했습니다.
*   Agent Arena 벤치마크에서 Claude Sonnet 5 (Thinking)가 6위에 올랐으며, 확인된 작업 성공 및 bash 사용에서 강력한 신호를 보였습니다.
*   Artificial Analysis가 24개 법률 분야에 걸쳐 120개 비공개 법률 작업을 대상으로 하는 법률 에이전트 벤치마크인 Harvey LAB-AA를 출시했습니다. Claude Fable 5가 14.2%의 전체 통과율로 선두를 차지했습니다.

### 🛠️ 제품 & 도구
*   Anthropic이 Claude를 전면 채팅 UI가 아닌 작업을 실행하는 백그라운드 팀원으로 포지셔닝한 Claude Cowork를 모바일 및 웹에 출시했습니다.
*   LangChain이 새로운 Deep Agents 강좌와 오픈소스 하네스 프로젝트를 통해 에이전트 설계의 변화를 반영했습니다.
*   Google Gemini API Managed Agents에 백그라운드 실행, 원격 MCP 서버, 커스텀 함수 호출 및 자격 증명 새로 고침 기능이 추가되었습니다.
*   Codex Mobile iOS에 작업 관리, 필터링된 diff, SSH 키 로그인, 브랜치 비교 및 첨부 파일 흐름 기능이 추가되었습니다.
*   Hermes Agent에 플러그형 시크릿 관리자, 기본 1Password 통합, 비공개 Hugging Face 리포지토리를 포함한 세션/데이터셋 내보내기 기능이 추가되었습니다.
*   Weaviate 1.38이 런타임으로 게이트된 쓰기 접근을 통해 MCP 서버를 GA(General Availability)로 출시했으며, MCP_SERVER_WRITE_ACCESS_ENABLED를 재시작 없이 실시간으로 전환할 수 있습니다.
*   NVIDIA가 GR00T 1.7과 Isaac Teleop을 LeRobot에 통합하여 Hugging Face 생태계로 로봇 공학 스택을 확장했습니다.
*   Nsight Python 1.0이 출시되어 Python으로 GPU 성능 분석을 스크립트화할 수 있게 되었습니다.
*   Unsloth가 DeepSeek-V4-Flash용 GGUF를 출시했으며, NVFP4/FP8로의 내보내기 및 GRPO와 MoE에 대한 속도 향상을 제공합니다.
*   Anthropic과 Neuronpedia가 오픈 모델용 J-렌즈 가중치를 출시했습니다.
*   DeepMind가 Gemini를 기반으로 평이한 영어 상호작용을 통해 그리스/라틴 역사 분석을 수행하는 Predicting the Past를 출시했습니다.

### 🔬 연구 & 논문
*   Lilian Weng이 에이전트/하네스 엔지니어링에 관한 35편의 논문을 요약한 새로운 게시물을 발표하며, 하네스 개선 사항이 코어 모델에 내재화되더라도 목표와 컨텍스트 지정의 필요성은 사라지지 않을 것이라고 강조했습니다.
    ![X avatar for @lilianweng](https://pbs.substack.com/profile_images/1923619459643711488/qmXOBh1.jpg)
    ![](https://substack-post-media.s3.amazonaws.com/public/images/5005c722-fdff-4ea8-aee0-6b37e44da978_1512x886.png)
    ![](https://substack-post-media.s3.amazonaws.com/public/images/603a46c6-cedc-4b38-a660-2fa1d4b3f4ba_1626x1146.png)
*   Liquid AI가 작은 추론 모델의 둠 루프를 줄이기 위한 오픈소스 학습 방법인 Antidoom (Final Token Preference Optimization, FTPO)을 발표했습니다. 이 방법은 루프를 유발하는 토큰을 재라벨링하고 대안으로 확률을 재분배합니다.
*   NVIDIA가 하이브리드 MoE 상위 모델을 압축하면서 추론, 코딩, 긴 컨텍스트 및 에이전틱 품질을 보존하는 Puzzle-75B-A9B 압축 작업을 공개했습니다.
*   Stanford/NVIDIA/Berkeley 연구진이 스코어링 토큰 로짓에서 보정된 연속 점수를 읽어내는 학습 없는 검증기 논문을 발표했습니다. 이 검증기는 Terminal-Bench V2, SWE-Bench Verified 등에서 강력한 수치를 보여주었습니다.
*   @eliebakouch가 38개 오픈 모델에서 J-렌즈 기하학에 대한 CKA 유사성을 계산하여 Llama 및 OLMo와 같이 관련 없는 계열에서도 보편적인 레이어/깊이 구성을 발견했습니다.
*   Goodfire가 활성화에서 다차원 개념을 위한 Block-Sparse Featurizers를 도입하며, 많은 비전 개념이 단일 방향이 아닌 본질적으로 2-4차원 블록이라고 주장했습니다.
*   Google이 엔드투엔드 과학 워크플로우를 위한 다중 에이전트 시스템인 Experience AI Scientist를 홍보했습니다.

### 💰 산업 동향
*   에이전틱 법률 시스템을 개발하는 Norm Ai가 12억 달러 가치로 1억 2천만 달러 규모의 Series C 투자를 유치했습니다.
*   Tencent Hy3 모델이 Apache 2.0 라이선스로 전환되어, 이전 라이선스에서 제한되었던 한국, 영국, EU 등에서의 상업적 사용이 가능해졌습니다.

### ⚡ 인프라 & 하드웨어
*   NVIDIA의 Puzzle-75B-A9B 압축 작업은 H100에서 약 2배의 서버 처리량과 1개 요청에서 8개로 증가한 1M 컨텍스트 동시성을 제공합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
