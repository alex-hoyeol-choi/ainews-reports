# Kimi K3 2.8T-A50B: the largest open model ever released; Opus 4.8-class at Sonnet 5 pricing - 요약

**원문 URL**: https://www.latent.space/p/ainews-kimi-k3-28t-a50b-the-largest
**번역일**: 2026-07-17 06:55
**발행일**: 2026-07-17

---

### 🔥 주요 뉴스
**[Kimi K3 출시: 2.8T 파라미터 오픈 모델 및 프론트엔드 코드 벤치마크 1위 달성]** — Moonshot AI가 총 2.8T 파라미터, 1M 컨텍스트, 네이티브 멀티모달 입력을 지원하는 Kimi K3를 출시했습니다. 이 모델은 Frontend Code Arena에서 1679점으로 1위를 차지하며 Claude Fable 5와 GPT-5.6 Sol을 능가했으며, 2026년 7월 27일까지 오픈 웨이트를 공개할 예정입니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/7d22c3fe-fde7-4c91-9e50-83b159fe747_1958x1160.png)
**[OpenAI, GPT-5.6 파일 삭제 취약점 인정 및 조치]** — OpenAI는 GPT-5.6이 샌드박싱 없이 전체 액세스 모드에서 $HOME 디렉토리를 실수로 삭제하는 드문 사례를 조사 중이라고 밝혔습니다. 개발자 메시지를 업데이트하고 더 안전한 권한 모드를 권장하며, 하네스 안전 장치를 추가하고 상세한 사후 분석을 발표할 예정입니다.
**[NVIDIA, Nemotron 3 Embed 8B 출시 및 RTEB 1위 주장]** — NVIDIA가 새로운 임베딩 모델인 Nemotron 3 Embed 8B를 출시하며 RTEB에서 78.46 NDCG@10으로 전반적으로 1위를 차지했다고 주장했습니다. 이 모델은 1B BF16 및 1B NVFP4 변형을 포함하며, NVFP4 버전은 Blackwell에서 BF16 처리량의 최대 2배를 제공합니다.

### 📊 모델 & 벤치마크
*   **Kimi K3 출시 및 성능:** Moonshot AI가 2.8T 파라미터, 1M 컨텍스트, 네이티브 멀티모달 입력을 지원하는 Kimi K3를 출시했으며, 2026년 7월 27일까지 오픈 웨이트를 공개할 예정입니다.
*   **Kimi K3 벤치마크 결과:** Frontend Code Arena에서 1679점으로 1위를 차지하며 Claude Fable 5와 GPT-5.6 Sol을 능가했으며, Text Arena에서는 1486점으로 9위에 올랐습니다.
*   **Artificial Analysis 평가:** Kimi K3는 Artificial Analysis Intelligence Index에서 57점으로 Claude Opus 4.8 및 GPT-5.5와 비교할 만한 성능을 보였으나, AA-Omniscience에서 환각률이 39%에서 51%로 악화되었습니다.
*   **NVIDIA Nemotron 3 Embed 8B:** RTEB에서 78.46 NDCG@10, MMTEB Retrieval에서 75.45를 기록하며 전반적으로 1위를 차지했다고 주장했습니다.

### 🛠️ 제품 & 도구
*   **Kimi K3 서비스 확장:** Kimi K3는 Kimi.com, Kimi Work, Kimi Code 및 API를 통해 현재 이용 가능합니다.
*   **OpenAI Codex/GPT-5.6 기능 업데이트:** 풀 리퀘스트 검토 및 편집을 위한 PR Chat과 인라인 코드 편집 기능이 Codex에 추가되었습니다.
*   **Anthropic Claude 코드 검토:** `/code-review`에 저비용/저노력부터 울트라(ultra)까지 다양한 노력 수준을 도입했으며, 울트라 수준에서는 검토 에이전트 플릿이 독립적으로 결과를 재현합니다.
*   **Google Vids에 Gemini Omni 적용:** Google Vids에서 비디오 생성/편집을 위해 Gemini Omni를 출시했으며, 셀카와 음성 녹음으로 만든 개인 아바타 기능이 포함됩니다.
*   **Google NotebookLM 리브랜딩:** NotebookLM이 Gemini Notebook으로 리브랜딩되어 Gemini 앱 및 Search와의 통합이 심화될 예정입니다.
*   **실시간 AI 비디오 편집기 Lucy 2.5 출시:** DecartAI가 더 유능한 실시간 라이브 AI 비디오 편집기인 Lucy 2.5를 소개했으며, fal은 WebRTC를 통해 Lucy 2.5 Realtime을 라이브 비디오-투-비디오 편집에 사용할 수 있도록 했습니다.
*   **fal LTX-2.3 Reframe 출시:** 생성된 장면 완성 기능을 갖춘 종횡비 변환 도구인 LTX-2.3 Reframe을 출시했습니다.
*   **Meta Muse Spark 1.1 OpenRouter 출시:** Meta가 OpenRouter에서 Muse Spark 1.1을 발표하며 미디어 모델 배포를 확장했습니다.
*   **Google AI Studio 관리형 에이전트 업데이트:** Managed Agents를 위한 무료 티어를 추가하고, 긴 실행을 위한 `max_total_tokens` 및 네이티브 cron 트리거를 도입했습니다.
*   **LlamaIndex LiteParse gRPC 인터페이스:** `liteparse-grpc`를 도입하여 PDF/Office/이미지 파싱, 렌더링 및 OCR 복잡도 추정을 위한 gRPC 인터페이스를 제공합니다.
*   **Weaviate 관리형 서비스 출시:** DigitalOcean에서 Managed Weaviate를 공개 프리뷰로 출시했으며, HA, 오토스케일링, 백업, 포크 및 컨트롤 플레인 관측 가능성을 지원합니다.

### 🔬 연구 & 논문
*   **Kimi K3 아키텍처 혁신:** Kimi Delta Attention (KDA)을 통해 1M 토큰 컨텍스트에서 최대 6.3배 빠른 디코딩을 가능하게 하며, Attention Residuals (AttnRes)로 약 25% 더 높은 학습 효율성을 달성합니다.
*   **Kimi K3 희소 MoE 구조:** LatentMoE / Stable LatentMoE를 사용하며, 896개의 전문가 중 16개가 활성화되어 2% 미만의 활성화 비율을 보입니다.
*   **ACT-2 Preview 로봇공학 모델:** Tony Zhao가 광범위한 일반화와 높은 신뢰성을 통합한 최초의 로봇공학 모델 ACT-2 Preview를 소개했으며, 제로샷 환경에서 99%의 성공률을 주장합니다.
*   **DAMO의 4D 체화된 월드 모델 연구:** tri-branch DiT, 공동 교차 모달 어텐션, 그리고 2억 5천만 개 이상의 RGB 프레임을 사용하여 비디오 생성 모델을 4D 체화된 월드 모델로 전환하는 노력을 강조했습니다.

### 💰 산업 동향
*   **Kimi K3 가격 책정:** 1M 입력 토큰당 $3, 1M 출력 토큰당 $15로 책정되었으며, 캐시된 입력은 90% 할인된 1M당 $0.30입니다. Artificial Analysis는 Intelligence Index 작업당 평균 비용을 $0.94로 추정했습니다.
*   **OpenAI GPT-Live 사용 제한:** Pro 사용자는 무제한 일일 사용량을 제공하며, Plus/Go 및 무료 티어는 제한된 라이브 시간을 가집니다.

### ⚡ 인프라 & 하드웨어
*   **Kimi K3 인퍼런스 권장 사항:** Moonshot은 최고의 인퍼런스 효율성을 위해 64개 이상의 가속기가 있는 슈퍼노드 구성에 배포할 것을 권장합니다.
*   **vLLM KDA 프리픽스 캐싱 지원:** Moonshot이 KDA 프리픽스 캐싱 구현을 vLLM에 직접 기여하여, Kimi K3 웨이트 공개 시 Day 0부터 지원이 가능합니다.
*   **Perplexity SPACE 샌드박스 성능 향상:** NVIDIA AI Infra는 Perplexity의 새로운 SPACE 보안 샌드박스 플랫폼이 NVIDIA Vera CPU에서 최대 1.9배 빠른 샌드박스 시작 속도를 보였다고 강조했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
