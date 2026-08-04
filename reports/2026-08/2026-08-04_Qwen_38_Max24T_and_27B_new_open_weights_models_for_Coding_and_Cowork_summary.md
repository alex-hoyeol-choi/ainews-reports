# Qwen 3.8 Max(2.4T) and 27B, new open weights models for Coding and Cowork - 요약

**원문 URL**: https://www.latent.space/p/ainews-qwen-38-max24t-and-27b-new
**번역일**: 2026-08-04 06:06
**발행일**: 2026-08-04

---

### 🔥 주요 뉴스
**[Qwen 3.8 Max 및 27B 오픈 웨이트 출시]** — Alibaba가 2.4T 파라미터의 플래그십 모델 Qwen 3.8 Max와 27B 모델을 오픈 웨이트로 출시했습니다. 이 모델은 10일 이상의 자율 코딩, 칩 설계 최적화, 멀티모달 에이전트 등에서 뛰어난 성능을 시연했으며, API 가격은 입력 $2/M, 출력 $6/M 토큰으로 책정되었습니다.
**[OpenAI, 차세대 모델로 수학/TCS 난제 해결]** — OpenAI의 내부 차세대 모델이 수학 및 이론 컴퓨터 과학 분야의 오랜 미해결 문제 10가지에 대해 새로운 결과를 도출했습니다. 이는 약 $2,000 상당의 GPT-5.6 Sol 토큰 비용으로 달성되었습니다.
**[MiniMax H3, 비디오 생성 분야 SOTA 달성]** — MiniMax가 텍스트/이미지/비디오/오디오 레퍼런스를 처리하는 33B 비디오 모델 H3를 출시했습니다. Video Arena에서 오픈 모델 중 1위, 이미지-투-비디오 부문에서는 전체 1위와 거의 동률을 기록했습니다.
**[OpenAI GPT-Live 아키텍처 재설계]** — OpenAI가 GPT-Live의 기술적 심층 분석을 공개하며, 전용 저지연 오디오 경로와 비동기 추론/툴 사용을 통해 세션 시작 시간을 6번의 왕복에서 1번으로 단축했다고 밝혔습니다.
**[화이트하우스, AI 프레임워크 및 사이버 보안 벤치마크 확정]** — 백악관이 OpenAI, Anthropic, Google, Meta를 초청하여 새로운 자발적 AI 프레임워크를 검토하고 새로운 사이버 보안 테스트 및 해킹 벤치마크를 확정했습니다.

### 📊 모델 & 벤치마크
*   **Qwen 3.8 Max (2.4T) 및 27B:** Alibaba가 2.4T 파라미터의 Qwen 3.8 Max와 27B 모델을 오픈 웨이트로 출시했습니다. 이 모델은 1M 토큰 컨텍스트와 128k 최대 출력 토큰을 지원하며, Frontend Code Arena에서 4위 (1,668 ELO), Vision Arena에서 2위 (1,305점), Vals Index에서 오픈 웨이트 모델 중 2위 (66.1점)를 기록했습니다.
    ![X avatar for @Alibaba_Qwen](https://pbs.substack.com/profile_images/2064231947149377536/Ab70PxT5.jpg)
*   **MiniMax H3 (33B):** 텍스트/이미지/비디오/오디오 레퍼런스를 처리하는 33B 비디오 모델 H3가 출시되었으며, Video Arena에서 오픈 모델 중 1위, 이미지-투-비디오 부문에서 전체 1위와 거의 동률을 기록했습니다.
*   **Kimi K3 + Kimi Code:** RSIBench-Data에서 SWE-bench Verified 50%, SWE-bench Pro 17%를 포함한 6개 벤치마크에서 27.317%의 가중치 점수를 기록했습니다.
*   **DeepSeek V4 Flash (0731):** Vals Index에서 60점 이상 모델 중 가장 저렴하며, 코딩 및 에이전틱 태스크에서 강점을 보였습니다.
*   **GLM-5.2 Max:** Frontend Code Arena에서 전체 2위, 오픈 모델 중 1위를 차지했습니다.
*   **jina-reranker-v3.5 (0.6B):** Jina AI가 0.6B 리스트와이즈 리랭커를 출시하며 BEIR에서 63.20 nDCG@10을 기록, Qwen3-Reranker-4B를 약 7배 적은 파라미터로 능가한다고 주장했습니다.
*   **새로운 벤치마크 아티팩트:** MerchantBench (365일 전자상거래 시뮬레이션), One Layer Deeper (적응형 컴퓨테이션 챌린지), Artifacts Hub / Adoption Dashboard (792개 오픈 모델 추적)가 공개되었습니다.

### 🛠️ 제품 & 도구
*   **Cloudflare @cloudflare/computer:** 각 에이전트가 "자신만의 컴퓨터"를 갖도록 아이솔레이트와 리눅스 컨테이너 사이를 동적으로 라우팅하는 에이전트 런타임을 출시했습니다.
*   **Cursor Google Workspace 플러그인:** Gmail, Drive, Calendar, Docs, Sheets 전반에 걸쳐 Google Workspace 접근을 위한 플러그인을 출시했습니다.
*   **LangChain Deep Agents (Public Beta):** 내장된 평가, 메모리, OAuth 툴 접근, 채널 통합 및 샌드박싱 기능을 갖춘 관리형 Deep Agents가 퍼블릭 베타로 전환될 예정입니다.
*   **DSPy 3.3.0:** 코드 및 프롬프트 최적화를 위한 dspy.Flex, 네이티브/병렬 툴 호출을 지원하는 ReActV2, 타입이 지정된 공급자 중립적 LM 인터페이스가 추가되었습니다.
*   **Google Gemini Spark 자동 브라우징:** Chrome을 사용하여 로그인된 계정에서 사용자의 민감한 단계 확인을 거쳐 작업을 수행할 수 있는 자동 브라우징 기능을 출시했습니다.
*   **Sakana Namazu API:** Kimi를 기반으로 구축되고 일본어/문화/비즈니스에 최적화된 일본 중심 LLM인 Namazu API를 출시했습니다.
*   **LiteParse:** 단순 페이지의 경우 밀리초/페이지 단위로 양식 필드, 체크박스 상태, 주석, 임베디드 이미지, 벡터 그래픽, 태그된 구조, 단어 수준 바운딩 박스를 직접 구조화된 PDF 추출에 추가했습니다.
*   **Hermes Agent "Herald" 릴리스:** 음성 채팅, 플러그인 기반 데스크톱 기능, A2A 프로토콜, 아웃바운드 웹훅, 연구 및 생산성 스킬, 토큰 효율성 개선을 포함하는 업데이트를 출시했습니다.

### 🔬 연구 & 논문
*   **OpenAI 수학/TCS 난제 해결:** OpenAI의 차세대 모델이 수학 및 이론 컴퓨터 과학 분야의 오랜 미해결 문제 10가지에 대해 새로운 결과를 발견했습니다.
*   **Intology Locus 시스템:** 자동화된 AI 연구 시스템 Locus가 PostTrainBench에서 SOTA를 달성했으며, Locus로 사후 학습된 Qwen3 1.7B Base 변형 모델이 인간이 사후 학습한 Qwen3 1.7B 릴리스를 능가했습니다.
*   **에이전트 실패 모드 분류 논문:** 단일 구성 요소가 아닌 상호작용 엣지를 기준으로 41가지 에이전트 실패 모드를 정리한 새로운 논문이 발표되었습니다.
*   **Zero-Mem:** LLM 호출을 메모리 유지 관리에서 제거하고 최종 답변 시에만 LLM을 호출하여, 동일 예산에서 메모리 작업 비용을 57.6% 절감하는 Zero-Mem이 강조되었습니다.

### 💰 산업 동향
*   **화이트하우스, AI 프레임워크 및 사이버 보안 벤치마크 확정:** 백악관이 주요 AI 기업들을 초청하여 새로운 자발적 AI 프레임워크를 검토하고 새로운 사이버 보안 테스트 및 해킹 벤치마크를 확정했습니다.
*   **Epoch, CVE 급증 보고:** 7월에 21개 주요 기술 조직에서 약 2,500개의 높음/심각 CVE가 공개되었으며, 이는 Anthropic의 자율 취약점 발견 공개 이전 월별 기록의 약 5배에 달합니다.

### ⚡ 인프라 & 하드웨어
*   **OpenAI GPT-Live 아키텍처 재설계:** 전용 저지연 오디오 경로와 비동기 추론/툴 사용을 통해 풀 듀플렉스 대화를 지원하고 세션 시작 시간을 6번의 왕복에서 1번으로 단축했습니다.
*   **Vikhyat Photon 2.0:** Moondream, Qwen 3.5, Gemma 4와 같은 모델의 전체 포워드 패스를 단일 GPU 프로그램으로 컴파일하는 메가커널 컴파일러 Photon 2.0을 발표했습니다.
*   **TokTier (스테이트풀 토큰화 서비스):** 에이전트 세션을 위해 토큰화된 프리픽스를 재사용하고 복구하는 스테이트풀 토큰화 서비스 TokTier가 vLLM 환경에서 TTFT를 16–34% 감소시키고, 증분 복구 시나리오에서 표준 Hugging Face 토큰화보다 최대 437배 빠른 속도 향상을 보고했습니다.
*   **Databricks Kimi K3 인퍼런스 속도:** Databricks가 Kimi K3에 대해 239 tok/s의 인퍼런스 속도를 제공하며, Casper Hansen은 단일 B300 노드에서 947 tok/s 배치-32 디코딩 및 152 tok/s 단일 사용자 인퍼런스 속도를 언급했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
