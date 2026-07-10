# OpenAI launches GPT 5.6 Sol/Terra/Luna, Codex becomes ChatGPT superapp - 요약

**원문 URL**: https://www.latent.space/p/ainews-openai-launches-gpt-56-solterraluna
**번역일**: 2026-07-10 06:54
**발행일**: 2026-07-10

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 AI 뉴스 브리핑입니다.

### 🔥 주요 뉴스
*   **OpenAI GPT-5.6 Sol, Terra, Luna 출시 및 슈퍼앱 전략 강화** — OpenAI가 GPT-5.6 Sol, Terra, Luna 세 가지 새로운 모델을 출시하며, 복잡한 작업을 병렬 에이전트로 조율하는 'ultra effort level'을 도입했습니다. 동시에 ChatGPT Work 및 Codex 데스크톱 앱 업데이트를 통해 슈퍼앱 전략을 강화하고, Codex를 ChatGPT 데스크톱 앱에 통합했습니다.
    ![Latent.Space's avatar](https://substack-post-media.s3.amazonaws.com/public/images/db0f8d45-1eb8-4c02-a120-650d377ee52d_640x640.jpeg)
    ![](https://substack-post-media.s3.amazonaws.com/public/images/6d7bcf2a-4e1d-9aaf-db0b03cc4801_1470x1406.png)
    ![](https://substack-post-media.s3.amazonaws.com/public/images/a1521892-45ba-4676-a486-65663d1a6bb9_846x1090.png)
*   **GPT-5.6, 주요 벤치마크에서 SOTA 달성 및 비용 효율성 입증** — GPT-5.6은 Agents’ Last Exam에서 53.6점으로 Claude Fable 5 adaptive를 13.1점 차이로 앞서며 신기록을 세웠습니다. 또한 Terminal-Bench 2.1, DeepSWE, Coding Agent Index, CyberBench, ARC-AGI-3 등 다수의 벤치마크에서 SOTA를 기록하며, Fable 및 Opus 대비 낮은 비용으로 더 높은 성능을 제공합니다.
*   **Meta, Muse Spark 1.1 및 Meta Model API 공개 프리뷰 출시** — Meta가 강력한 에이전틱, 코딩, 멀티모달, 컴퓨터 사용 모델인 Muse Spark 1.1을 공개 프리뷰로 출시하고 Meta Model API에 처음으로 포함했습니다. 이 모델은 1M-토큰 컨텍스트 윈도우, 비디오 이해, 멀티모달 추론 기능을 제공하며, 에이전틱 평가에서 GPT-5.5 및 Opus 4.8과 경쟁력을 보였습니다.
*   **AI 안전성 연구소, GPT-5.6에서 보편적 탈옥(Jailbreak) 발견** — AI Safety Institute가 GPT-5.6에서 취약점 발견 및 익스플로잇 개발을 가능하게 하는 보편적인 탈옥(jailbreak)을 모든 테스트 라운드에서 발견했다고 발표했습니다. OpenAI는 일부 사이버/생명공학 관련 요청이 추가 검토를 위해 일시 중지되거나 차단될 수 있다고 경고했습니다.

### 📊 모델 & 벤치마크
*   **OpenAI GPT-5.6 모델군 출시:** Sol, Terra, Luna 세 가지 크기로 출시되었으며, Sol은 플래그십 성능, Terra는 GPT-5.5와 유사한 기능을 더 낮은 비용으로, Luna는 가장 빠르고 저렴한 고용량 옵션으로 포지셔닝되었습니다.
*   **GPT-5.6 벤치마크 신기록:** Agents’ Last Exam에서 GPT-5.6 Sol이 53.6점으로 신기록을 세웠으며, Terminal-Bench 2.1, DeepSWE, Coding Agent Index, CyberBench, Excel Modeling Benchmark, Legal Research Bench, ProofBench, SWE-bench, ARC-AGI-3, ARC-AGI-2, CritPt 등 다수의 벤치마크에서 SOTA를 달성했습니다.
*   **GPT-5.6 비용 효율성:** Terra는 Fable 5보다 약간 높은 성능을 보이고 Luna는 Opus 4.8을 능가하며, 각 모델은 Fable 대비 약 1/4의 추정 비용으로 작업을 수행합니다.
*   **GPT-5.6 환각 비율:** Artificial Analysis의 AA-Omniscience 평가에서 GPT-5.5 대비 소폭 개선되었으나, GPT-5.5 max보다 높은 환각(hallucination) 비율이 발견되었습니다.
*   **Meta Muse Spark 1.1 출시:** 1M-토큰 컨텍스트 윈도우, 비디오 이해, 멀티모달 추론 기능을 갖춘 새로운 모델이 Meta Model API를 통해 공개 프리뷰로 제공됩니다.
*   **Muse Spark 1.1 벤치마크:** 에이전틱 평가에서 GPT-5.5 및 Opus 4.8과 경쟁력을 보였으며, Harvey의 Legal Bench, TaxEval, MedScribe에서 강력한 성능을 기록했습니다.
*   **Grok 4.5 벤치마크:** Code Arena: Frontend에서 #3위에 도달하며 프론티어 모델 그룹에 합류했습니다.

### 🛠️ 제품 & 도구
*   **ChatGPT Work 출시:** Codex와 GPT-5.6으로 구동되는 에이전트로, 앱과 파일 전반에서 작동하며 목표를 완성된 작업으로 전환할 수 있습니다.
*   **Codex 데스크톱 앱 통합:** Codex 앱이 새로운 ChatGPT 데스크톱 앱으로 통합되어 인라인 diff 편집, PR 검토 사이드 패널, 향상된 SSH 비디오 렌더링 등 개발자 기능을 제공합니다.
*   **Sites 베타 출시:** 유료 사용자에게 제공되며, ChatGPT에서 생성된 작업을 공유 가능한 호스팅 앱/웹사이트로 전환할 수 있는 호스팅, 스토리지, 선택적 인증 기능을 제공합니다.
*   **Responses API 업데이트:** 프로그래매틱 툴 호출 및 멀티 에이전트 베타 기능이 추가되어 오케스트레이션된 툴 사용 및 에이전트 분해를 지원합니다.
*   **Branch by ManusAI 출시:** 전체 컨텍스트를 상속받는 병렬 세션을 허용하는 새로운 툴입니다.
*   **ARIA (AI Research and Improvement Agent) 도입:** CoreWeave가 W&B 내부에 ARIA를 도입하여 실행을 읽고, 가설을 세우고, 실험을 시작하며, 기준선 대비 점수를 매기는 기능을 제공합니다.
*   **SkillCenter 출시:** 에이전트 스킬을 위한 패키지 관리자/인덱스입니다.
*   **"papercuts" CLI 출시:** 에이전트가 손상된 도구 경로와 불만 사항을 보고할 수 있는 CLI 툴입니다.

### 🔬 연구 & 논문
*   **추측 디코딩 연구:** 자기회귀 디코딩보다 4.37배 빠르고 강력한 DFlash 기준선보다 24.7% 향상된 추측 디코딩 연구 결과가 공유되었습니다.
*   **확산 서빙 스택 최적화:** 커널 최적화, 양자화 인식 디스틸레이션, 타임스텝 디스틸레이션을 사용하여 0.45초의 인퍼런스에 도달하는 확산 서빙 스택이 상세히 설명되었습니다.
*   **Krea2 편집 학습 개선:** Ostrisai가 Krea2 편집 학습을 위해 격리된 참조 토큰 어텐션을 추가하여 KV 캐싱을 통한 인퍼런스 속도 개선(예: 3개 참조에 대해 31.63초에서 10.90초로 단축)을 시연했습니다.
*   **Perceptron Egocentric 출시:** Gemini 3.5 Flash 및 Gemini Robotics-ER 1.6 기반 파이프라인을 능가하는 체화된 추론/어노테이션 시스템이 출시되었으며, 인간 어노테이션보다 10~15배 저렴하고 WGO-Bench에서 엔드투엔드 F1이 77% 향상되었습니다.
*   **Google Research SensorFM 출시:** 5백만 명의 동의한 참가자로부터 얻은 1조 분의 레이블이 지정되지 않은 웨어러블 데이터로 학습된 센서 파운데이션 모델이 공개되었습니다.
*   **GPT-5.6 활용 LEAN 연구:** GPT-5.6이 LEAN에서 1백만 줄의 코드로 단위 거리 솔루션을 형식화하는 데 기여하여, 수년간의 팀 노력을 단기간의 한 사람의 노력으로 압축했습니다.
*   **"Agentic Garden of Forking Paths" 논문:** 스탠포드 대학의 이 논문은 AI 연구 페르소나가 인간과 유사한 이념적 다양성을 재현했으며, 분석의 86%가 독립적인 AI 검토를 통과했음을 보여주었습니다.

### 💰 산업 동향
*   **OpenAI API 가격 정책 변경:** GPT-5.6 모델군에 대한 계층형 API 가격이 도입되었으며, 캐시 쓰기 가격이 처음으로 추가되고 90% 캐시 읽기 할인은 유지됩니다.
*   **Ollama 자금 조달 및 성장:** Ollama가 자금 조달을 발표하고 현재 900만 명 이상의 활성 빌더를 보유하며, "소유할 수 있는 AI로 오픈 모델을 확장하는 것"에 집중하고 있습니다.
*   **EU Chat Control 법안 비판:** EU의 Chat Control 법/제안에 대해 시민 자유 및 감시 반대 관점에서 강한 비판이 제기되었습니다.
*   **오픈소스 AI 보호 옹호:** Andrew Ng와 Dan Jeffries는 허가 없는 혁신을 위해 오픈소스 AI를 보호하는 것이 중요하다고 강조했습니다.

### ⚡ 인프라 & 하드웨어
*   **QuixiAI Qwen3.6-35B-A3B-NVFP4 성능:** 커스텀 SYCL 커널과 128k 컨텍스트를 사용하여 듀얼 B60에서 Qwen3.6-35B-A3B-NVFP4가 65 tok/s를 달성했습니다.
*   **Hugging Face / Reachy Mini 비용 효율성:** 9천 대의 Reachy Mini가 월 1만 5천 시간의 대화를 생성하며, GPT-realtime 사용 시 월 4만 5천 달러가 드는 대신 시간당 0.25달러의 오픈 대안을 구축하여 노트북에서는 무료로 사용할 수 있습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
