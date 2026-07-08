# Lilian Weng summarizes 35 papers on Harness Engineering for RSI

**원문 URL**: https://www.latent.space/p/ainews-lilian-weng-summarizes-35
**번역일**: 2026-07-08 06:53
**발행일**: 2026-07-08

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Lilian Weng이 RSI를 위한 하네스 엔지니어링에 관한 35편의 논문을 요약했습니다

### 조용한 날에는 응축된 통찰력을 읽을 수 있습니다
ShareMeta Superintelligence가 세계 최고의 이미지/비디오 모델 2/3를 보유하게 된 것을 축하합니다! 이것은 헤드라인 기사 후보였겠지만, 안타깝게도 Muse Image/Video에 대한 기술적 세부 사항이나 논문이 전혀 없다는 것이 거의 모든 정보입니다. 그럼에도 불구하고, 이것은 지난달 Microsoft MAI 모델들을 능가하는 좋은 소식입니다.
저희는 Lilian Weng의 팬이므로, 그녀가 또 다른 연구 요약을 발표할 때마다 주목합니다. 특히 그녀가 Thinky의 공동 창립자가 된 지금은 더욱 드문 일입니다. 오늘 그녀는 하네스와 RSI의 관계에 대해 생각하고 있습니다:

![X avatar for @lilianweng](https://pbs.substack.com/profile_images/1923619459643711488/qmXOBhZ1.jpg)
저희는 Greg Brockman조차도 이제 에이전트/하네스 엔지니어링을 조용히 지지하고 있다는 글을 이전에 썼지만, Lilian과 같이 존경받는 사상가이자 신생 연구소 공동 창립자가 "많은 하네스 개선 사항이 결국 코어 모델에 내재화되더라도, 목표와 컨텍스트를 지정해야 할 필요성은 사라지지 않을 것입니다"라고 동의하는 것은 신선합니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/5005c722-fdff-4ea8-aee0-6b37e44da978_1512x886.png)
그녀의 게시물은 모든 사람이 알아야 할 하네스의 주요 입증된 설계 트렌드를 제시하고, 잘 알려진 ACE paper부터 AINews에서 일화적으로 다루었던 Meta-Harnesses와 같은 최신 트렌드에 이르기까지 하네스 최적화 문헌을 요약합니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/603a46c6-cedc-4b38-a660-2fa1d4b3f4ba_1626x1146.png)
이는 또한 Thinky가 Interaction Models 외에 무엇을 생각하고 있는지에 대한 힌트를 제공할 것입니다.
> 2026년 7월 6일-7월 7일 AI 뉴스입니다. 저희는 12개의 subreddits, 544개의 Twitters를 확인했으며, 추가 Discords는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter Recap
에이전트 제품, 하네스 및 장기 워크플로우
- Anthropic이 Claude 위에 "백그라운드 에이전트" UX를 확장합니다: 가장 많은 참여를 이끌어낸 제품 출시는 Claude Cowork가 모바일 및 웹에 출시된 것으로, Claude를 전면 채팅 UI가 아닌 작업을 실행하는 백그라운드 팀원으로 포지셔닝했습니다. 관련 게시물들은 @mikeyk의 공유 홈 탭과 더욱 긴밀한 Chat/Cowork 통합을 중심으로 한 제품 통합을 보여줍니다. 별도로, Anthropic은 @claudeai의 높은 참여를 이끌어낸 발표를 통해 7월 12일까지 유료 요금제 사용자에게 Claude Fable 5 접근을 연장했지만, @kimmonismus 및 다른 사용자들의 반응에서 많은 사용자들이 주간 제한과 관련된 어색한 타이밍을 지적했습니다.
- 하네스 엔지니어링이 에이전트 설계의 중심으로 떠오르고 있습니다: Lilian Weng의 새 게시물은 재귀적 자기 개선을 직접적인 가중치 자체 수정이 아닌 하네스를 중심으로 재구성하는 것으로 널리 언급되었습니다. Sakana의 요약은 이를 그들의 스레드에서 "The AI Scientist", "ShinkaEvolve", "Darwin Gödel Machine"과 연결합니다. LangChain도 @LangChain 및 @hwchase17의 게시물에서 새로운 Deep Agents 강좌와 오픈소스 하네스 프로젝트를 통해 동일한 변화를 반영했습니다. Google도 이 방향을 제품화하고 있습니다: Gemini API Managed Agents는 @\_philschmid 및 @OfficialLoganK의 게시물에서 백그라운드 실행, 원격 MCP 서버, 커스텀 함수 호출 및 자격 증명 새로 고침 기능을 추가했습니다.
- 실용적인 에이전트 인프라가 더욱 독자적인 방향으로 발전하고 있습니다: 몇 가지 주목할 만한 운영자 대상 업데이트가 있었습니다: Codex Mobile iOS는 @Dimillian 및 @reach_vb의 게시물에서 작업 관리, 필터링된 diff, SSH 키 로그인, 브랜치 비교 및 첨부 파일 흐름을 추가했습니다. Hermes Agent는 @Teknium의 스레드에서 플러그형 시크릿 관리자와 기본 1Password 통합, 그리고 비공개 Hugging Face 리포지토리를 포함한 형식으로 세션/데이터셋 내보내기 기능을 추가했습니다. Weaviate 1.38은 @victorialslocum의 게시물에서 런타임으로 게이트된 쓰기 접근을 통해 MCP 서버를 GA(General Availability)로 출시했으며, 특히 MCP_SERVER_WRITE_ACCESS_ENABLED를 재시작 없이 실시간으로 전환할 수 있도록 했습니다. @omarsar0는 에이전트가 휴먼-인-더-루프 제어를 위해 전화/SMS/iMessage를 통해 의사 결정을 에스컬레이션할 수 있도록 Dial MCP 서버를 사용하는 더욱 실험적인 패턴을 제시했습니다.
모델 및 모달리티 출시: 오디오, 음성, 로봇 공학 및 미디어 생성
- Meta의 Muse Image/Muse Video가 에이전틱 생성 기능을 미디어 분야로 확장합니다: Meta Superintelligence Labs는 @AIatMeta, @alexandr_wang, @\_tim_brooks의 발표에서 Muse Image를 출시하고 Muse Video를 미리 공개했습니다. 주목할 만한 기술적 측면은 단순히 이미지 품질뿐만 아니라, 계획, 웹 검색, 도구 사용, 코드 실행 및 렌더링 전 자체 개선을 포함하는 명시적으로 에이전틱한 생성 루프입니다. Meta는 또한 스케일링된 테스트 시간 컴퓨팅으로 성능이 향상되며, 이 후속 조치에서 자체 개선 동작이 수동으로 스크립팅된 것이 아니라 RL 과정에서 나타났다고 말합니다. 공개 평가에서 Muse Image는 Arena의 순위에서 GPT Image 2에 이어 Image Arena 2위에 빠르게 올랐으며, Muse Video는 또 다른 Arena 게시물에서 Video Arena 3위로 데뷔했습니다.
- NVIDIA와 Cohere 모두 강력한 오디오 릴리스를 출시했습니다: NVIDIA는 통합 텍스트+오디오 작업을 위한 1M 컨텍스트를 가진 30B 파라미터 / 3B 활성 MoE 모델인 Audex를 출시했으며, @HuggingPapers가 요약하고 @\_weiping이 더 자세히 설명했습니다. 이 모델의 핵심 주장은 단일 MoE 백본을 통해 광범위한 오디오 생성 및 이해 기능을 추가하면서 텍스트 지능을 보존하는 것입니다. Cohere는 Apache 2.0 라이선스 하에 가장 정확한 오픈소스 아랍어 ASR 모델로 설명되는 Cohere Transcribe Arabic을 출시했으며, @cohere 및 @JayAlammar의 게시물에서 방언, 코드 스위칭 및 아랍어 억양의 영어에 중점을 두었습니다.
- 오픈 로봇 공학은 Hugging Face + NVIDIA를 중심으로 통합되고 있습니다: NVIDIA는 @NVIDIARobotics의 발표 및 통합 가이드에서 GR00T 1.7과 Isaac Teleop을 LeRobot에 통합하여 HF 생태계로 로봇 공학 스택을 확장했으며, 이는 오픈 휴머노이드 로봇 공학 워크플로우를 목표로 합니다. 체화된 측면에서 UMA는 강력한 풀스택 로봇 공학 내러티브를 보여주었습니다: @RemiCadene는 9개월 만에 소규모 팀이 구축한 프로토타입을 설명했으며, Northstar 공개와 @psermanet의 안전성 관련 언급은 신뢰할 수 있는 로봇을 위한 수직 통합 하드웨어/소프트웨어를 강조했습니다.
학습, 인퍼런스 및 후처리 기술
- Liquid AI의 "Antidoom"은 추론 루프 실패 모드를 직접적으로 겨냥합니다: 그날의 가장 명확한 기술 릴리스 중 하나는 Liquid AI의 Antidoom이었습니다. 이는 작은 추론 모델이 컨텍스트 고갈까지 토큰을 반복하는 둠 루프를 줄이기 위한 오픈소스 학습 방법입니다. 보고된 감소는 상당합니다: 탐욕적 샘플링(greedy sampling) 하에서 LFM2.5-2.6B는 10.2%에서 1.4%로, Qwen3.5-4B는 22.9%에서 1%로 감소했으며, 다운스트림 평가 이득도 있었습니다. 이 방법인 FTPO (Final Token Preference Optimization)는 루프를 유발하는 토큰을 재라벨링하고 대안으로 확률을 재분배하는 것으로, @helloiamleonie 및 @LiorOnAI가 잘 요약했습니다. 이는 단순히 파라미터를 스케일링하는 것이 아니라 특정 실패 모드를 제거하는 최근 분야의 패턴을 잘 보여주는 예시입니다.
- 인퍼런스 효율성과 압축은 여전히 주요 프론티어입니다: NVIDIA의 Puzzle-75B-A9B 압축 작업은 @omarsar0를 통해 큰 주목을 받았습니다. 이는 하이브리드 MoE 상위 모델을 압축하면서 추론, 코딩, 긴 컨텍스트 및 에이전틱 품질을 보존하며, H100에서 약 2배의 서버 처리량과 1개 요청에서 8개로 증가한 1M 컨텍스트 동시성을 제공합니다. 도구 측면에서는 @HagedornBastian의 게시물에서 Nsight Python 1.0이 출시되어 Python으로 GPU 성능 분석을 스크립트화할 수 있게 되었습니다. Unsloth는 또한 @danielhanchen의 업데이트에서 DeepSeek-V4-Flash용 GGUF를 출시했으며, NVFP4/FP8로의 내보내기 및 GRPO와 MoE에 대한 속도 향상을 제공했습니다.
- 에이전트 RL 및 검증이 더욱 전문화되고 있습니다: @cwolferesearch는 GRPO 스타일 정규화가 다중 턴 환경에서 더 높은 보상 분산을 처리하기 위해 작업 또는 환경 수준에서 에이전틱 RL에 맞게 어떻게 조정되고 있는지를 강조했습니다. 별도로, @omarsar0는 Stanford/NVIDIA/Berkeley의 학습 없는 검증기 논문을 지적했습니다. 이 논문은 스코어링 토큰 로짓에서 보정된 연속 점수를 읽어내며, Terminal-Bench V2, SWE-Bench Verified, RoboRewardBench 및 MedAgentBench 전반에 걸쳐 강력한 수치를 보여주어 검증이 독립적인 스케일링 축이 되고 있음을 시사합니다.
해석 가능성, 모델 내부 및 "J-스페이스" 논쟁
- Anthropic의 J-스페이스 연구는 해석 가능성 논의를 지배했지만, 날카로운 비판도 받았습니다: 커뮤니티는 이 작업을 유용한 기계적 분석으로 보는 것과 의식 프레이밍에 반대하는 것으로 나뉘었습니다. @danburonline, @paul_cal, @scaling01은 Jacobian-lens 정의 하에서 벡터가 주로 구성에 의해 인과적이라고 주장하며 강한 비판을 제기했습니다. @jacobandreas는 독자들에게 원래의 Jacobian lenses paper를 다시 참조하도록 지적하며 유용한 역사적 참고 자료를 제공했습니다.
- 더 강력한 기술적 시사점은 의식 수사학이 아닌 교차 모델 구조입니다: @eliebakouch는 38개 오픈 모델에서 J-렌즈 기하학에 대한 CKA 유사성을 계산했으며, Llama 및 OLMo와 같이 관련 없는 계열에서도 놀랍도록 보편적인 레이어/깊이 구성을 발견했습니다. Anthropic과 Neuronpedia도 이 후속 조치에서 오픈 모델용 J-렌즈 가중치를 출시했습니다. 이와 병행하여 Goodfire는 활성화에서 다차원 개념을 위한 Block-Sparse Featurizers를 도입했으며, 그들의 스레드에서 많은 비전 개념이 단일 방향이 아닌 본질적으로 2-4차원 블록이라고 주장했습니다.
벤치마크, 평가 및 도메인별 시스템
- 에이전트 및 법률 벤치마크는 "많은 기준을 통과하는 것"과 "실제 작업을 완전히 해결하는 것" 사이의 격차를 계속 드러냅니다: Agent Arena는 Claude Sonnet 5 (Thinking)를 6위에 올렸으며, 확인된 작업 성공 및 bash 사용에서 가장 강력한 신호를 보였지만, 조종 가능성(steerability)에 대한 불확실성은 여전히 남아있었습니다. Artificial Analysis는 24개 법률 분야에 걸쳐 120개 비공개 법률 작업을 대상으로 하는 법률 에이전트 벤치마크인 Harvey LAB-AA를 출시했습니다. 여기서 Claude Fable 5가 14.2%의 전체 통과율로 선두를 차지했으며, Claude Opus 4.8과 GLM-5.2는 7.5%로 동률을 이루었고, GLM은 Fable의 작업당 비용의 약 6% 수준으로 이를 달성했다고 그들의 릴리스에서 밝혔습니다. 핵심 메시지는 모델이 많은 개별 평가 항목을 충족할 수 있지만, 여전히 허용 가능한 엔드투엔드 결과물을 생성하지 못할 수 있다는 것입니다.
- 연구 자동화 및 전문 도메인 시스템이 확장되고 있습니다: Google은 이 ICML 게시물에서 엔드투엔드 과학 워크플로우를 위한 다중 에이전트 시스템인 Experience AI Scientist를 홍보했습니다. DeepMind는 또한 그들의 스레드에서 Gemini를 Aeneas와 Ithaca에 기반하여 평이한 영어 상호작용을 통해 그리스/라틴 역사 분석을 수행하는 Predicting the Past를 출시했습니다. 법률 AI 상업화 측면에서는 Norm Ai가 12억 달러 가치로 1억 2천만 달러 규모의 Series C 투자를 발표했으며, @johnjnay의 게시물에서 소프트웨어와 AI 네이티브 로펌을 아우르는 풀스택 "에이전틱 법률" 시스템을 설명했습니다.
가장 많은 참여를 얻은 트윗
- Claude 접근성 / 제품 출시: 모바일 및 웹용 Claude Cowork와 7월 12일까지 연장된 Fable 5 접근성은 기술적으로 가장 관련성이 높은 제품 발표였습니다.
- 오픈소스 개발자 프로그램: @ClaudeDevs가 오픈소스 유지보수 담당자에게 6개월간 Claude Max 20x를 제공하는 것은 엄청난 참여를 이끌어냈으며, OSS 생태계에서 도구 채택에 중요하게 작용할 가능성이 높습니다.
- Meta 미디어 생성: Muse Image 출시와 Arena의 Muse Image #2 순위는 가장 큰 멀티모달 제품 소식이었습니다.
- 추론 신뢰성: Liquid AI의 Antidoom 출시는 그날의 가장 주목할 만한 학습 기술 게시물이었습니다.
- 해석 가능성: 38개 오픈 모델에 걸친 교차 모델 J-렌즈 보편성은 J-스페이스 담론에 대한 가장 강력한 기술적 후속 조치였습니다.

---

# AI Reddit Recap

## /r/LocalLlama + /r/localLLM Recap

### 1. 오픈 모델 출시 및 인퍼런스 효율성
- Tencent Hy의 새로운 오픈 모델: Hy3 (총 295B, 활성 21B - apache 2.0) (활동: 653): Tencent는 Hugging Face에 비-프리뷰 Hy3 오픈 모델 컬렉션을 출시했습니다. 이는 21B 활성 파라미터를 가진 295B 파라미터 MoE로 설명되며, 이전의 제한적인 커뮤니티 라이선스 대신 Apache 2.0 라이선스 하에 제공됩니다. 이 게시물은 이전 라이선스가 한국, 영국, EU를 포함한 지역에서의 사용을 배제했다고 보고되었음을 강조하며, 상위 댓글들은 HY3-Preview 대비 주장된 벤치마크 이득을 지적하고 이를 고성능 로컬/가정용 인퍼런스 설정에 잠재적으로 관련성이 있는 것으로 평가했습니다. 댓글 작성자들은 Apache 2.0 재라이선싱을 가장 중요한 변화로 보았는데, 특히 Tencent의 최근 번역 모델들도 Apache 라이선스를 사용하고 있다는 점을 고려했습니다. 보고된 벤치마크 개선이 실제 유용성으로 이어질 수 있다는 신중한 낙관론이 있었지만, 공급업체 차트 외부에서 테스트될 때까지는 암묵적인 회의론이 있었습니다. 댓글 작성자들은 Hunyuan/HY3가 이제 Apache 2.0으로 등재되어 있으며, 한국, 영국, EU와 같은 지역에서의 사용을 제한했다고 알려진 이전 "커뮤니티" 라이선스와 대조된다는 점을 강조했습니다. 이는 Apache 2.0이 많은 상업적 및 지리적 사용 장벽을 제거하기 때문에 배포에 기술적으로 중요하다고 여겨졌습니다. 여러 사용자는 Tencent가 HY3-Preview 대비 주장하는 벤치마크 개선이 실제 워크로드로 이어질지 여부에 초점을 맞췄습니다. 보고된 총 295B / 활성 21B MoE 스타일 구성을 고려할 때, 댓글 작성자들은 GGUF와 같은 인퍼런스 형식을 사용할 수 있게 되면 "고성능 가정용 설정"에 관련성이 있을 수 있다고 제안했습니다. HY3가 로컬/오픈 웨이트 워크플로우에서 Qwen 및 MiniMax 모델의 대안이 될 수 있다는 초기 추측이 있었지만, 댓글 작성자들은 결론을 내리기 전에 양자화된 릴리스와 독립적인 테스트를 기다리고 있었습니다.

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-lilian-weng-summarizes-35&utm_source=paywall-free-trial&utm_medium=web&utm_content=205984146&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-lilian-weng-summarizes-35&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
