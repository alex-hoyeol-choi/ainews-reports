# GPT 5.5 and OpenAI Codex Superapp 

**원문 URL**: https://www.latent.space/p/ainews-gpt-55-and-openai-codex-superapp
**번역일**: 2026-04-24 06:18
**발행일**: 2026-04-24

---

[AINews: 주중 요약](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] GPT 5.5 및 OpenAI Codex 슈퍼앱

### Spud가 살아있습니다!
Opus 4.7 출시 일주일 후, OpenAI는 GPT 5.5에 대해 매우 유사한 파레토 프론티어 개선 차트를 공개하며 반격에 나섰습니다 (Noam Brown이 선호하듯이 — 원시적인 1차원 지능 측정 방식이 2차원 달러당 지능 차트로 대체되고 있습니다). 4.7 대 5.5 경쟁에서 언급되지 않은 것(코딩)을 행간에서 읽어야 하지만, 전반적인 지능 면에서 AA는 이 모델을 세계 최고의 독립적으로 검증된 모델로 평가했으며, 또한…

![](https://substack-post-media.s3.amazonaws.com/public/images/2f9f5845-e1e6-497a-9bed-f645719247c_2048x684.png)
AA 차트… 달러당 지능 ("GPT-5.5 (medium)은 저희 Intelligence Index에서 Claude Opus 4.7 (max)과 동일한 점수를 기록하면서도 4분의 1의 비용(약 $1,200 대 $4,800)으로 제공됩니다. 다만 Gemini 3.1 Pro Preview는 약 $900의 비용으로 동일한 점수를 기록했습니다.")

![](https://substack-post-media.s3.amazonaws.com/public/images/39e50c45-bc8a-4f60-a562-026d1c7bd14d_1026x662.png)
aa 2D
몇 가지 학습 하드웨어에 대한 흥미로운 정보와 긍정적인 RSI 바이브, 그리고 멋진 대안 벤치마크가 있습니다.
하지만 오늘을 단순한 포인트 업데이트 모델 출시(일부는 5.9라고 부르고 싶어 할 것입니다)로만 여긴다면 오산입니다. 오늘은 또한 대규모 Codex 출시일이기도 합니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/ec7c1f27-a6ba-40a7-ba86-24eb303591c8_1030x1254.png)
트위터
내장된 브라우저 제어 기능과 이 대규모 업데이트의 다른 기능들, 그리고 이제는 없어진 Prism (RIP)을 통합함으로써, OpenAI는 Codex를 슈퍼앱 전략의 기반으로 삼는 중요하고 돌이켜보면 당연한 선택을 한 것으로 보입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/cabd0f35-0766-4080-82b3-c90f52faa849_954x1416.png)
> 2026년 4월 22일~23일 AI 뉴스입니다. 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 더 이상의 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
OpenAI의 GPT-5.5 출시: 더 강력한 에이전틱 코딩, 더 넓은 컴퓨터 사용, 토큰 효율성 강조
- GPT-5.5는 오늘날의 지배적인 출시입니다: OpenAI는 "실제 작업을 위한 새로운 차원의 지능"으로 포지셔닝된 GPT-5.5를 출시했으며, ChatGPT와 Codex 전반에 걸쳐 배포되고 추가 안전 장치가 마련될 때까지 API 접근은 지연됩니다. OpenAI와 커뮤니티 벤치마크 게시물들은 전반적인 벤치마크 압도보다는 더 나은 장기 실행, 더 강력한 컴퓨터 사용 행동, 그리고 실질적으로 개선된 토큰 효율성이라는 프로필에 수렴했습니다. 보고된 수치에는 @reach_vb를 통해 Terminal-Bench 2.0 82.7%, SWE-Bench Pro 58.6%, GDPval 84.9%, OSWorld-Verified 78.7%, CyberGym 81.8%, BrowseComp 84.4%, FrontierMath Tier 1–3 51.7%가 포함되며, Artificial Analysis는 GPT-5.5가 더 높은 토큰당 가격에도 불구하고 이제 여러 주요 평가에서 선두를 달리거나 동률을 이루고 새로운 비용/성능 프론티어에 위치한다고 말했습니다 @ArtificialAnlys, @scaling01. OpenAI는 또한 ChatGPT에서 스택 수준 인퍼런스 개선이 GPT-5.5 Pro를 까다로운 작업에 더 실용적으로 만들었다고 강조했습니다 @OpenAI.
- 가격 책정, 컨텍스트, 인프라 및 실제 동작: API 가격은 GPT-5.5의 경우 1M 입력/출력 토큰당 $5/$30, Pro의 경우 $30/$180로 보고되었습니다 @scaling01. Sam Altman은 API에서 1M 컨텍스트 윈도우와 5.4보다 작업당 더 낮은 토큰 사용량을 언급했습니다. 여러 초기 사용자들은 이 모델이 이전 GPT들보다 더 "인간적"이고 덜 형식적이며, 특히 Codex 내부에서 지속적인 에이전트 워크플로우에 더 적합하다고 설명했습니다 @MatthewBerman, @danshipper, @omarsar0. OpenAI는 이 모델이 NVIDIA GB200/300 시스템을 위해 공동 설계되었으며 모델 자체가 자체 인퍼런스 스택을 개선하는 데 도움이 되었다고 주장했습니다 @scaling01. 한편 @sama는 회사가 점점 더 AI 인퍼런스 회사로 변모하고 있다고 언급했습니다. 사용자들로부터 반복되는 주제는 GPT-5.5가 종종 자율성 면에서 계단 함수적 업그레이드처럼 느껴지지만, 탐색적일 수도 있고 제대로 작동하려면 더 엄격한 지시가 필요할 수 있다는 것입니다 @theo.
- Codex가 더 완벽한 에이전트 작업 공간이 되다: 동시에 OpenAI는 상당한 Codex 업그레이드를 출시했습니다: 브라우저 제어, Sheets/Slides, Docs/PDFs, OS 전반의 받아쓰기, 그리고 자동 검토 모드 @ajambrosino. OpenAI는 이제 Codex가 웹 앱과 상호 작용하고, 흐름을 클릭하고, 스크린샷을 캡처하고, 작업 완료까지 반복할 수 있다고 말합니다 @OpenAIDevs. 자동 검토는 보조 "가디언" 에이전트를 사용하여 장기 실행 시 승인 횟수를 줄입니다 @OpenAIDevs, @gdb. 사용자 보고서에 따르면 이는 Codex를 코딩 도구에서 QA, 스프레드시트, 프레젠테이션, 앱 구축, 연구 루프, 야간 실험 실행에 이르는 더 광범위한 컴퓨터 작업 에이전트로 확장하고 있음을 시사합니다 @gdb, @tszzl, @aidan_mclau.
DeepSeek-V4 Preview: 1.6T MIT 라이선스 오픈 모델, 1M 컨텍스트, 공격적인 가격 책정
- DeepSeek은 몇 시간 내에 GPT-5.5에 응답했습니다: DeepSeek은 DeepSeek-V4 Preview를 출시하며 V4-Pro와 V4-Flash를 MIT 라이선스 하에 오픈소스화했습니다. 주요 사양은 이례적으로 공격적입니다: V4-Pro: 총 1.6T 파라미터 / 49B 활성, V4-Flash: 284B / 13B 활성, 둘 다 1M 토큰 컨텍스트와 사고/비사고 모드를 지원합니다 @deepseek_ai, @Yuchenj_UW. 커뮤니티 반응은 빠르게 이를 새로운 오픈 모델 플래그십으로 평가했으며, 이전 세대의 최고 클로즈드 모델과 경쟁하고 DeepSeek V3.x를 크게 뛰어넘는다고 보았습니다 @arena, @scaling01, @kimmonismus.
- 기술 보고서 하이라이트: 긴 컨텍스트 효율성, 하이브리드 어텐션, Muon: 이번 출시는 가중치뿐만 아니라 당일 기술 보고서 @scaling01로도 주목할 만했습니다. 커뮤니티 요약은 두 가지 새로운 압축/하이브리드 어텐션 메커니즘, mHC, Muon 기반 학습, FP4 양자화 인식 학습, 그리고 약 32T 토큰에 대한 사전 학습을 지적합니다 @scaling01, @iScienceLuvr, @eliebakouch. 가장 강력한 기술 논의는 1M 컨텍스트를 실용적으로 만드는 데 중점을 두었으며, 이전 DeepSeek 스타일 스택에 비해 약 4배의 컴퓨팅 효율성 개선과 자릿수 KV-캐시 감소가 보고되었습니다 @Hangsiin. 빠른 인프라 반응 또한 주목할 만했습니다: vLLM은 출시 당일 지원을 발표하고 새로운 어텐션 스택을 어떻게 구현했는지 상세히 설명했습니다. SGLang은 출시 당일 최적화와 RL 파이프라인 지원을 제공했습니다.
- 가격 책정은 모델만큼 중요할 수 있습니다: DeepSeek이 게시한 가격은 매우 공격적입니다: V4-Flash는 1M 입력/출력 토큰당 $0.14/$0.28, V4-Pro는 $1.74/$3.48입니다 @scaling01, @teortaxesTex. 여러 평론가들은 서비스 품질이 유지된다면 V4-Flash가 매우 낮은 비용, 1M 컨텍스트, 오픈 웨이트의 조합을 고려할 때 잠재적으로 더 파괴적인 SKU가 될 수 있다고 강조했습니다 @Hangsiin, @arena. DeepSeek의 주요 주의사항: V4-Pro 처리량은 현재 고성능 컴퓨팅 제약으로 인해 제한되며, 회사는 가격 인하를 위해 향후 Ascend 950 가용성을 명시적으로 언급했습니다 @teortaxesTex.
에이전트 인프라 및 도구: 메모리, 오케스트레이션, 브라우저, 엔터프라이즈 플러밍
- 에이전트는 모델 문제뿐만 아니라 시스템 문제로 변모하고 있습니다: 여러 게시물은 프로덕션 에이전트 작업이 점점 더 하네스, 평가, 메모리 및 오케스트레이션에 관한 것임을 강조했습니다. 유용한 예시는 엔터프라이즈 에이전트를 위한 상태 비저장 의사결정 메모리에 대한 글이었습니다. 이는 변경 가능한 에이전트별 상태를 불변의 의사결정 로그/이벤트 소싱으로 대체하여 수평 확장성, 감사 가능성 및 내결함성을 개선합니다 @omarsar0. 비슷한 맥락에서 @Vtrivedy10은 추적 데이터 → 평가/환경 → 하네스 엔지니어링/SFT-RL이 프로덕션 에이전트를 개선하기 위한 핵심 플라이휠이며, 나중에 Anthropic의 Claude Code 회귀를 오픈 하네스와 오픈 평가가 왜 중요한지에 대한 사례 연구로 사용했습니다 @Vtrivedy10.
- 제어 표면 주변의 새로운 도구: Cua는 에이전트가 멀티플레이어/멀티커서 지원을 통해 백그라운드에서 임의의 앱을 제어할 수 있도록 하는 macOS 드라이버인 Cua Driver를 오픈소스화했습니다. Cognition은 클라우드 에이전트 인프라를 구축하는 데 필요한 것에 대한 게시물을 발표하며, VM 격리, 세션 지속성, 환경 프로비저닝, 오케스트레이션 및 통합과 같은 실제 스택을 언급했습니다. LangChain은 파일 편집, 웹페이지/프레젠테이션 생성 및 슬래시 커맨드 스킬로 LangSmith Fleet을 계속 확장했습니다 @LangChain. 여러 사용자들은 Fleet의 프레젠테이션 렌더러/뷰어가 놀랍도록 유용한 에이전트 네이티브 아티팩트 형식이라고 강조했습니다 @BraceSproul.
- 다중 에이전트 오케스트레이션이 제품으로 이동하고 있습니다: Sakana AI는 동적으로 프론티어 모델을 선택하고 조정하는 다중 에이전트 오케스트레이션 API인 Fugu의 베타 버전을 출시했습니다. SWE-Pro, GPQA-D 및 ALE-Bench에서 SOTA를 달성하고 자체 호출을 통한 재귀적 테스트 시간 스케일링까지 주장했습니다 @SakanaAILabs, @hardmaru. Hermes Agent는 대규모 기여자 릴리스, 확장된 공급자, 이미지 생성 지원, 그리고 효과적으로 즉각적인 GPT-5.5 지원과 함께 v0.11.0을 출시했습니다 @Teknium. 방향은 일관적입니다: 에이전트는 단일 모델 루프가 아니라 이기종 도구 및 모델 위에 있는 오케스트레이션 레이어가 되고 있습니다.
비전, 비디오 및 멀티모달 시스템: Vision Banana, Sapiens2, HDR 비디오 및 옴니 모델
- Google DeepMind의 Vision Banana는 CV를 생성으로 재구성합니다: 기술적으로 더 흥미로운 연구 출시 중 하나는 Vision Banana였습니다. 이는 2D/3D 비전 작업을 이미지 생성으로 처리하는 통합 비전 모델로, 여러 비전 작업에서 전문 SOTA 시스템을 능가하는 것으로 보고되었습니다. 컴퓨터 비전 연구자들의 반응은 이것이 향후 세분화, 깊이, 법선 및 관련 작업에 접근하는 방식의 더 광범위한 변화를 시사한다는 것이었습니다 @sainingxie. 오픈 측면에서는 Meta도 인간 중심 지각 작업을 위해 10억 개의 인간 이미지로 학습된 고해상도 비전 트랜스포머 세트인 Sapiens2를 출시했습니다 @HuggingPapers.
- 비디오 스택 업데이트는 원본 해상도를 넘어 프로덕션 형식으로 이동하고 있습니다: Kling의 "네이티브 4K" 출시는 여러 플랫폼에 걸쳐 확산되었지만, 기술적으로 더 새로운 출시는 LTX HDR 베타일 수 있습니다. 이는 프로덕션에서 AI 비디오의 진정한 병목 현상이 해상도뿐만 아니라 다이내믹 레인지에 있었다고 주장하며, 8비트 SDR을 넘어 그레이딩 및 합성을 견딜 수 있는 영상으로 나아가고 있습니다 @ltx_model. 이는 일반적인 "4K" 마케팅만으로는 얻을 수 없는 더 실질적인 개선입니다. 별도로, World Labs는 Marble 1.1 + Spark LoD를 중심으로 인터랙티브 3D 생성을 위한 World Jam을 출시했습니다 @theworldlabs.
- 더 광범위한 멀티모달 트렌드: 명시적인 교차 모달 추론을 가진 통합 모델: 새로 공유된 Context Unrolling in Omni Models는 텍스트, 이미지, 비디오, 3D 기하학 및 숨겨진 표현 전반에 걸쳐 학습된 통합 모델을 제안하며, 출력을 생성하기 전에 모달리티 전반에 걸쳐 추론을 명시적으로 전개합니다 @arankomatsuzaki. Vision Banana와 함께, 이는 반복되는 모티프를 지적합니다: 이질적인 지각/생성 작업을 더 적은 일반 멀티모달 백본으로 통합한 다음, 인퍼런스 시간 추론이 모달리티를 연결하도록 하는 것입니다.
학습, 스케일링 및 연구 방법: 전역 분산 사전 학습, 셀프 플레이 및 긴 컨텍스트 내부
- Google의 Decoupled DiLoCo는 탄력적인 전역 사전 학습을 다룹니다: Google DeepMind와 Google Research는 분산 저통신 학습을 분리하여 전 세계 데이터센터 학습, 이기종 하드웨어, 그리고 작업을 중단시키지 않고 하드웨어 장애에 대한 내성을 가능하게 하는 Decoupled DiLoCo를 소개했습니다. 이는 거대한 학습 실행을 결함이 있는 지리적으로 분산된 인프라 전반에서 효율적으로 유지하는 실제 프론티어 학습 병목 현상을 목표로 하기 때문에 의미 있는 시스템 결과입니다. 깨끗한 동종 클러스터를 가정하는 것이 아닙니다.
- 무차별 샘플링을 넘어선 알고리즘 스케일링: @LukeBailey181이 강조한 셀프 플레이 논문은 LLM의 장기 셀프 플레이가 왜 정체되는지 연구하고, 7B 모델이 100배 더 큰 모델의 pass@4만큼 많은 문제를 해결할 수 있도록 하는 알고리즘을 제안합니다. 또 다른 반복되는 주제는 실제 프론티어 지표로서의 토큰/계산 효율성이었습니다. 여러 게시물은 노력 수준과 인퍼런스 예산이 역량을 실질적으로 재구성하는 세상에서 단일 숫자 지능 비교가 점점 더 구식이라고 주장했습니다 @polynoamial. 관련하여, Neural Garbage Collection에 대한 스레드는 고정된 휴리스틱 대신 RL을 통해 자체 KV 캐시를 관리하도록 모델을 학습시키는 것을 설명했으며, 이는 장기 에이전트에게 잠재적으로 중요한 방향입니다 @cwolferesearch.
- 인프라 채택 신호: Together AI는 전년 대비 월 30B에서 300T 토큰으로 성장했다고 보고했습니다 @vipulved. 이는 인퍼런스 수요 확장의 대규모 지표입니다. 한편 Epoch AI는 Stargate Abilene의 운영 전력 추정치를 현재 약 0.3 GW로 하향 조정하고 전체 1.2 GW 이정표를 2026년 4분기로 연기하여, 프론티어 컴퓨팅 배포 추적의 지속적인 불확실성을 강조했습니다 @EpochAIResearch.
인기 트윗 (참여도 기준)
- OpenAI GPT-5.5 출시: 가장 높은 참여도를 보인 기술 게시물은 OpenAI의 GPT-5.5 발표였으며, 이어서 @sama의 출시 게시물과 OpenAI DevRel이 GPT-5.5를 지금까지 가장 똑똑한 프론티어 모델로 설명한 것이 뒤를 이었습니다 @OpenAIDevs.
- Claude Code 회귀 사후 분석: Anthropic이 Claude Code 품질이 세 가지 문제로 인해 저하되었으며 v2.1.116+에서 수정되었음을 인정한 것은 그날 가장 높은 참여도를 보인 엔지니어링-제품 게시물 중 하나였으며, 하네스 민감도와 회귀 테스트에 대한 상당한 논의를 촉발했습니다.
- DeepSeek-V4 Preview 출시: DeepSeek의 공식 V4 Preview 출시는 MIT 라이선스, 1M 컨텍스트, 공격적인 가격 책정의 조합을 고려할 때 빠르게 또 다른 주요 높은 참여도를 보인 기술 이벤트가 되었습니다.
- Vision Banana: Google DeepMind의 Vision Banana 발표는 뛰어난 순수 연구 비전 게시물이었습니다.
- ML-Intern 및 자율 연구 워크플로우: Hugging Face 관련 ml-intern이 15분 만에 인턴십 스타일 테스트를 통과하고 이후 보고된 매우 높은 토큰 소비량은 단순한 데모가 아닌 개별 제품으로서 자율 코딩/연구 하네스에 대한 강한 관심을 시사합니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-gpt-55-and-openai-codex-superapp&utm_source=paywall-free-trial&utm_medium=web&utm_content=195312492&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-gpt-55-and-openai-codex-superapp&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
