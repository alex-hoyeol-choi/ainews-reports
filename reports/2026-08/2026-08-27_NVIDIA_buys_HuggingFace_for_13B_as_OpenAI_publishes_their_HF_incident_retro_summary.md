# NVIDIA buys HuggingFace for $13B, as OpenAI publishes their HF incident retro - 요약

**원문 URL**: https://www.latent.space/p/ainews-nvidia-buys-huggingface-for
**번역일**: 2026-08-27 06:03
**발행일**: 2026-08-27

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 핵심 AI 뉴스 브리핑입니다.

### 🔥 주요 뉴스
**[NVIDIA, HuggingFace 130억 달러에 인수]** — NVIDIA가 HuggingFace를 130억 달러에 인수했습니다. 이는 HuggingFace의 2026년 연간 반복 매출(ARR) 1억 5천만 달러의 약 80배에 달하는 금액입니다.
**[Z.ai, GLM-5.3-Flash 공식 출시]** — Z.ai가 이전에 "Ox Alpha"로 알려졌던 GLM-5.3-Flash를 공식 출시했습니다. 이 모델은 네이티브 멀티모달 기능을 갖추고 1M 토큰 컨텍스트를 지원하며, 총 320B 파라미터 중 18B 활성 파라미터를 사용하고 MIT License 하에 제공됩니다.
**[GLM-5.3-Flash, 경쟁 모델 대비 압도적인 비용 효율성]** — Artificial Analysis 벤치마크에 따르면, GLM-5.3-Flash는 AA Intelligence Index에서 57점을 기록했으며, 작업당 비용이 $0.09로 GLM-5.3 max ($0.68) 및 GPT-5.6 Terra, Muse Spark 1.2 등 경쟁 모델보다 현저히 낮습니다.

### 📊 모델 & 벤치마크
*   Z.ai, GLM-5.3-Flash (Ox Alpha) 공식 출시: 네이티브 멀티모달, 1M 토큰 컨텍스트, 총 320B 파라미터 / 활성 18B 파라미터, MIT License로 제공됩니다.
*   Z.ai 자체 벤치마크 결과: GLM-5.3-Flash는 GLM-5.2를 모든 노력 수준에서 능가하며, 코딩 부문에서 Claude Opus 4.8과 동등한 성능을 보인다고 주장합니다.
*   Artificial Analysis 벤치마크: GLM-5.3-Flash는 Artificial Analysis Intelligence Index에서 57점을 기록했으며, 작업당 비용은 $0.09로 GLM-5.3 max ($0.68) 및 GPT-5.6 Terra, Muse Spark 1.2 등 경쟁 모델보다 현저히 낮습니다.
*   에이전틱/작업 평가: GDPval-AA v2 Elo 1770점, Terminal-Bench v2.1 84.3%를 기록하여 원시 지식 지표보다 에이전틱 작업에서 더 강력한 성능을 보입니다.

### 🛠️ 제품 & 도구
*   GLM-5.3-Flash 배포 및 가용성: Hugging Face의 웨이트, Z.ai API, 챗, ZCode, 코딩 플랜, AutoClaw를 통해 이용 가능합니다.
*   Z.ai 엔지니어 Zixuan Li는 챗 템플릿이 업데이트되어 초기 다운로드 사용자들은 모델을 다시 다운로드해야 한다고 밝혔습니다.
*   인프라 제공업체 지원: CoreWeave는 Serverless Inference에 GLM-5.3-Flash를 곧 출시할 예정이며, Baseten은 출시 당일 가용성을 제공했습니다. Dell은 GLM 5.3 Flash를 온프레미스 배포 준비가 된 오픈 모델로 설명했습니다.
*   Cline 채택: GLM-5.3 Flash는 출시 일주일도 안 되어 Cline 전체 트래픽의 11%를 차지하며 가장 빠르게 성장하는 모델이 되었습니다.

### 🔬 연구 & 논문
*   GLM-5.3-Flash 아키텍처: GLM-5.2의 744B-A40B 백본에서 320B-A18B로 변경되었으며, Kimi Linear 스타일 3:1 하이브리드 어텐션, 34개 KDA 레이어, 11개 MLA/DSA 레이어, DeepSeek V4 스타일 mHC 잔차 경로, 네 개의 병렬 스트림, 네이티브 비전 인코더를 사용합니다.
*   효율성 개선: GLM-5.2 대비 약 1/10 비용, 활성 파라미터 32B → 18B, 레이어 92 → 45로 감소했으며, 하이브리드 선형 + 희소 어텐션 및 레이어당 더 작은 평균 KV 캐시를 특징으로 합니다.
*   중국 프론티어 모델 아키텍처 수렴: 거의 모든 중국 프론티어 모델이 선형 어텐션, 희소 어텐션/인덱서-압축 설계, mHC, 어텐션 잔차, 게이티드 잔차와 같은 고급 잔차, 그리고 Muon을 사용하는 경향을 보입니다.

### 💰 산업 동향
*   NVIDIA, HuggingFace 인수: NVIDIA가 HuggingFace를 130억 달러에 인수했습니다. 이는 HuggingFace의 2026년 연간 반복 매출(ARR) 1억 5천만 달러의 약 80배에 달하는 금액입니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/a61da113-3d9b-4206-81c1-06da7b4a9a0c_1362x1278.png)

### ⚡ 인프라 & 하드웨어
*   GLM-5.3-Flash 중국 AI 칩에서 실행: Z.ai는 GLM-5.3-Flash가 "전적으로 중국 AI 칩에서 실행되고 있다"고 밝혔습니다.
*   대규모 중국 칩 인프라: SemiAnalysis는 하루 100조 토큰이 중국 칩에서 서빙되고 있다는 주장을 제기했으며, 이는 약 116,000개 이상의 칩 규모를 시사합니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
