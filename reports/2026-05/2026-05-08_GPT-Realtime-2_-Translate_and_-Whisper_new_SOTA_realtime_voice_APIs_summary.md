# GPT-Realtime-2, -Translate, and -Whisper: new SOTA realtime voice APIs - 요약

**원문 URL**: https://www.latent.space/p/ainews-gpt-realtime-2-translate-and
**번역일**: 2026-05-08 12:18
**발행일**: 2026-05-08

---

### 🔥 주요 뉴스
**[OpenAI, GPT-Realtime-2, -Translate, -Whisper 출시]** — OpenAI가 "GPT-5급 추론"을 제공하는 실시간 음성 AI 모델 3종을 Realtime API에 공개했습니다. GPT-Realtime-2는 128K 컨텍스트 윈도우, 툴 사용, 방해 처리, 조정 가능한 추론 노력을 지원하며, GPT-Realtime-Translate는 70개 이상 언어에서 13개 언어로 실시간 번역을, GPT-Realtime-Whisper는 실시간 스트리밍 전사를 제공합니다.
**[실시간 음성 AI 벤치마크 SOTA 달성]** — GPT-Realtime-2는 Scale AI Audio MultiChallenge S2S 리더보드에서 1위를 차지했으며, Artificial Analysis Big Bench Audio 음성-대-음성 추론에서 96.6%를 기록하여 이전 최고 기록보다 약 13% 향상된 성능을 보였습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/9c9ffc6c-f36-4f23-a2c3-34d5e64955aa_1014x918.png)

### 📊 모델 & 벤치마크
*   **OpenAI, GPT-Realtime-2 출시:** "GPT-5급 추론"을 특징으로 하는 네이티브 음성-대-음성 모델로, 128K 토큰 컨텍스트 윈도우와 32K 토큰 최대 출력을 지원하며, 최소 추론 시 1.12초, 높은 추론 시 2.33초의 첫 오디오 응답 시간을 제공합니다.
*   **OpenAI, GPT-Realtime-Translate 출시:** 70개 이상의 입력 언어에서 13개 출력 언어로의 실시간 스트리밍 음성 번역을 지원합니다.
*   **OpenAI, GPT-Realtime-Whisper 출시:** 실시간 캡션, 메모 및 음성 이해를 위한 낮은 레이턴시의 스트리밍 전사 기능을 제공합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/81d9ff0f-63ea-4b44-85a9-7fcc0d69f75_1716x772.png)
*   **Scale AI Audio MultiChallenge S2S 벤치마크:** GPT-Realtime-2가 1위를 차지하며, GPT-Realtime-1.5 대비 지시 유지율이 36.7%에서 70.8% APR로 크게 향상되었습니다.
*   **Artificial Analysis Big Bench Audio 벤치마크:** GPT-Realtime-2(높음 변형)가 96.6%를 기록하여 Gemini 3.1 Flash Live Preview High와 동등한 수준을 보였으며, 이전 최고 결과보다 약 13% 높은 것으로 보고되었습니다.
*   **Conversational Dynamics 벤치마크:** GPT-Realtime-2(최소 변형)가 96.1%를 기록하며 일시 정지 처리 및 차례 주고받기에서 강점을 보였습니다.

### 🛠️ 제품 & 도구
*   **OpenAI Realtime API 업데이트:** GPT-Realtime-2, -Translate, -Whisper 모델이 Realtime API를 통해 개발자에게 제공되며, 오디오 입력 시간당 $1.15, 오디오 출력 시간당 $4.61의 가격으로 이용할 수 있습니다.
*   **음성 프롬프팅 가이드 공개:** OpenAI는 개발자들이 추론 노력 튜닝, 프리앰블, 툴 동작, 불분명한 오디오 복구, 엔티티 캡처, 긴 세션 상태 관리 등을 다룰 수 있도록 음성 프롬프팅 가이드를 게시했습니다.
*   **Glean, GPT-Realtime-2 기반 실시간 음성 기능 출시:** 조직 컨텍스트에 기반한 실시간 음성 기능을 출시했으며, 내부 평가에서 이전 버전 대비 42.9%의 상대적 유용성 증가를 보였습니다.
*   **Genspark, Call for Me Agent 업그레이드:** 자사의 Call for Me Agent를 GPT-Realtime-2로 업그레이드하여 유효 대화율이 26% 증가하고 통화 끊김이 줄었다고 발표했습니다.
*   **Vimeo, GPT-Realtime-Translate 활용 실시간 더빙 시연:** 미리 로드된 캡션 없이 실시간으로 번역이 생성되는 것을 시연했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
