# H100 prices are melting *UP* - 요약

**원문 URL**: https://www.latent.space/p/ainews-h100-prices-are-melting-up
**번역일**: 2026-03-28 07:18
**발행일**: 2026-03-28

---

### 🔥 주요 뉴스
*   **[H100 렌탈 가격 급등]** — 2025년 12월 이후 NVIDIA H100 GPU 렌탈 가격이 크게 상승하여, 전반적인 칩 부족 현상과 추론 모델/에이전트의 가치 증가를 반영합니다. 이는 데이터 센터 및 GPU 비즈니스 모델에 중요한 영향을 미칠 것으로 예상됩니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/efae087a-e8bd-4623-adc9-e8ef80115faa_1096x1122.png)
*   **[Anthropic, Opus 능가하는 'Capybara' 티어 유출]** — Fortune 보고서에 따르면 Anthropic이 Claude Opus 4.6보다 "더 크고 더 지능적인" 새로운 티어인 'Capybara'를 개발 중이며, 코딩, 학술적 추론, 사이버 보안에서 더 나은 성능을 보입니다. 그러나 비용 및 안전성 문제로 출시가 제한되고 있습니다.
*   **[Zhipu, GLM-5.1 출시로 오픈 코딩 모델 격차 축소]** — Zhipu가 모든 코딩 플랜 사용자에게 GLM-5.1을 출시하며, 코딩 평가에서 45.3점을 기록하여 이전 GLM-5의 35.4점을 능가했습니다. 이는 오픈/세미-오픈 코딩 모델이 클로즈드 모델과의 격차를 좁히고 있음을 시사합니다.
*   **[RotorQuant, TurboQuant 대비 10-19배 빠른 양자화 기술 공개]** — Clifford 대수를 활용한 새로운 벡터 양자화 방식인 RotorQuant가 TurboQuant보다 10-19배 빠른 속도와 44배 적은 파라미터로 거의 동일한 코사인 유사도(0.990)를 달성했습니다. 이는 퓨즈드 CUDA 커널 및 Metal 셰이더를 활용하여 RTX PRO 4000 및 Apple M4에서 cuBLAS matmul을 크게 능가합니다.

### 📊 모델 & 벤치마크
*   Anthropic의 유출된 'Capybara' 티어는 Claude Opus 4.6을 능가하며 코딩, 학술적 추론, 사이버 보안에서 더 높은 점수를 기록했습니다.
*   Zhipu의 GLM-5.1이 출시되어 코딩 평가에서 45.3점을 기록, GLM-5의 35.4점을 넘어섰으나 Claude Opus 4.6의 47.9점에는 미치지 못했습니다.
*   Artificial Analysis가 실제 코딩 에이전트 궤적, 100K+ 시퀀스 길이, 가속기당/kW당/달러당/랙당 동시 사용자 수로 표현되는 처리량에 중점을 둔 새로운 에이전트 벤치마크 AA-AgentPerf를 도입했습니다.
*   Cohere가 새로운 2B Apache-2.0 Transcribe 모델을 출시했으며, A100에서 12분 만에 33시간의 오디오를 전사하는 등 강력한 성능을 보였습니다.
*   Mistral의 Voxtral TTS 논문이 언급되었으며, 브라우저/로컬 데모가 나타났습니다.

### 🛠️ 제품 & 도구
*   Nous Research의 Hermes Agent가 Hugging Face를 일류 인퍼런스 제공자로 통합하여 28개의 큐레이션된 모델에 대한 접근을 제공하며, 메모리, 영구적인 머신 접근 및 모델 선택 기능을 갖춘 오픈 에이전트를 향한 진전을 보였습니다.
*   OpenAI 개발자들이 Codex 플러그인과 사용 사례 갤러리를 강조했으며, Box는 Box 콘텐츠에 대한 워크플로우 자동화를 위해 Codex 플러그인을 출시했습니다.
*   @ctatedev가 실시간 브라우저 세션 디버깅을 위한 새로운 에이전트 브라우저 대시보드를 출시했습니다.
*   LangChain이 에이전트 평가 준비 체크리스트, Deep Agents IDE 스타일 UI 가이드라인, 프롬프트 프로모션/롤백을 위한 LangSmith Prompt Hub Environments 등 프로덕션 지향 자료들을 공개했습니다.
*   TurboQuant vLLM 포크가 출시되어 Qwen3.5-35B AWQ, 1M 컨텍스트, 4M KV 캐시를 목표로 퓨즈드 Triton KV 쓰기 경로 및 디코드 어텐션을 포함합니다.

### 🔬 연구 & 논문
*   Meta가 SAM 3의 드롭인 업데이트인 SAM 3.1을 출시하여 객체 멀티플렉싱을 통해 단일 포워드 패스에서 최대 16개의 객체를 허용하며, H100 한 대에서 비디오 처리량을 거의 두 배(16FPS에서 32FPS) 증가시켰습니다.
*   LeCun의 LeWorldModel 논문/리포지토리가 강조되었으며, 표현 붕괴를 수학적으로 불가능하게 설계된 작고 오픈된 월드 모델로 48배 빠른 플래닝과 약 200배 적은 토큰을 주장합니다.
*   @UnitreeRobotics가 롤링 업데이트를 위한 실제 휴머노이드 전신 원격 조작 데이터셋인 UnifoLM-WBT-Dataset을 오픈소스화했습니다.
*   AI2가 완전히 시뮬레이션에서 학습된 오픈 로봇 조작 스위트인 MolmoBot을 출시했으며, 코드, 학습 데이터, 생성 파이프라인 및 평가를 제공합니다.
*   RotorQuant가 Clifford 대수를 활용하여 벡터 양자화에 대한 새로운 접근 방식을 도입했으며, TurboQuant보다 10-19배 빠른 속도 향상과 44배 적은 파라미터를 달성했습니다.
*   llama.cpp의 KV 캐시 압축을 위한 TurboQuant 구현 최적화가 논의되었으며, 무시할 수 있는 어텐션 가중치를 가진 위치에 대한 디양자화를 건너뛰어 32K 컨텍스트 길이에서 디코드 성능을 +22.8% 향상시켰습니다.

### 💰 산업 동향
*   Google이 Anthropic의 데이터 센터에 자금을 지원하는 데 근접했다는 Financial Times 보고서가 있었으며, 이는 프론티어 AI 경쟁이 알고리즘보다는 전력 및 Capex에 의해 점점 더 좌우되고 있음을 시사합니다.
*   Anthropic이 공격적인 스케일링 야망과 여전히 타이트한 서빙 환경 사이에서 균형을 맞추고 있는 것으로 보이며, 유출 당일 529s/오류 증가와 같은 광범위한 불만이 있었습니다.

### ⚡ 인프라 & 하드웨어
*   H100 GPU 렌탈 시장이 2025년 12월 이후 크게 상승하여, 전반적인 칩 부족 현상과 추론 모델/에이전트의 변곡점과 관련이 있습니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/efae087a-e8bd-4623-adc9-e8ef80115faa_1096x1122.png)
*   @bnjmn_marie의 벤치마크 결과, RTX Pro 6000급 하드웨어에서 Qwen3.5 27B 포맷에 대해 INT4가 최고의 인퍼런스 옵션으로 나타났습니다.
*   Google의 TurboQuant 압축 방법이 llama.cpp에 적용되어 Qwen 3.5–9B를 표준 MacBook Air (M4, 16 GB)에서 20000 토큰 컨텍스트로 로컬 실행할 수 있게 되었습니다.
*   llama.cpp의 KV 캐시 압축을 위한 TurboQuant 최적화는 무시할 수 있는 어텐션 가중치를 가진 위치에 대한 디양자화를 건너뛰어 M5 Max에서 32K 컨텍스트 길이에서 디코드 속도를 +22.8% 증가시켰습니다.
*   RotorQuant는 퓨즈드 CUDA 커널과 Metal 셰이더를 활용하여 RTX PRO 4000 및 Apple M4에서 cuBLAS matmul을 크게 능가하는 성능을 보였습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
