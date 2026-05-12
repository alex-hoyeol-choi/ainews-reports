# Thinking Machines' Native Interaction Models - TML-Interaction-Small 276B-A12B - advances SOTA Realtime Voice and kills standard VAD

**원문 URL**: https://www.latent.space/p/ainews-thinking-machines-native-interaction
**번역일**: 2026-05-12 06:19
**발행일**: 2026-05-12

---

# [AINews] Thinking Machines의 네이티브 인터랙션 모델 - TML-Interaction-Small 276B-A12B - 실시간 음성 SOTA를 발전시키고 표준 VAD를 종식시킵니다

### 잘하셨습니다, 팀 Thinky.
완전히 우연하게도, 저희가 Neil Zeghidour (명망 높은 Kyutai Moshi의 영리 스핀오프인 Gradium의 CEO)의 실시간 음성을 위해 아직 구축되어야 할 것에 대한 강연을 공개한 날, Thinking Machines가 약 1년 만에 (많은 논란에도 불구하고) 세 번째로 등장하여 "Interaction Models: A Scalable Approach to Human-AI Collaboration"을 발표했습니다. TML-Interaction-Small은 12B 활성 파라미터를 가진 276B 파라미터 MoE이며, 이는 Neil이 제시했던 대로 실시간 음성 모델의 SOTA를 즉시 발전시키고, 유명하게도 실패했던 GPT 4o의 "her" 데모를 실제 사용에 훨씬 더 가까울 것으로 추정되는 훨씬 더 상세한 데모들로 업데이트했습니다:
전체 블로그 게시물에는 지속적인 상호작용 수준을 보여주는 많은 데모가 있으며, 각각 200ms의 "시간 정렬된 마이크로턴" 스트림에 초점을 맞추고 있습니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/02190942-3f50-4067-ae03-97c6b504b3a3_1490x1592.png)
인코더 없는 초기 퓨전을 사용하여 이미지와 오디오가 모두 200ms 미만으로 처리되며, Meta의 Chameleon과 유사합니다:

![](https://substack-post-media.s3.amazonaws.com/public/images/68576e99-b00a-4069-b93f-bbe906ddd810_1336x1602.png)
팀은 BigBench Audio, IFEval, FD-bench와 같은 기본적인 항목에서 GPT-Realtime-2와 Gemini 3.1-Flash 모두를 능가하는 여러 공식 벤치마크를 보여주지만, 목표로 하는 상호작용 수준은 시간 인식, 동시 번역, 시각적 주도성을 위한 2개의 새로운 내부 벤치마크를 만들 것을 요구했습니다:
- TimeSpeak: 모델이 사용자가 지정한 시간에 발화를 시작할 수 있습니까? 예시: "숨쉬기 연습을 하고 싶어. 멈추라고 할 때까지 4초마다 숨을 들이쉬고 내쉬라고 알려줘."
- CueSpeak: 모델이 적절한 순간에 발화할 수 있습니까? 예시: "내가 코드를 전환하여 다른 언어를 사용할 때마다, 원래 언어로 올바른 단어를 알려줘."
- RepCount-A는 반복적인 행동이 담긴 비디오를 포함하며 온라인 카운팅 작업으로 개조되었습니다. 이는 지속적인 시각 추적 및 시기적절한 카운팅을 측정합니다.
- ProactiveVideoQA는 질문이 포함된 비디오로 구성되며, 답변은 특정 순간에 제공됩니다. 더 높은 점수를 얻으려면 올바른 시간에 정확한 답변이 필요하며, 침묵은 부분 점수를 받고, 오답은 감점됩니다.
- Charades는 표준 시간적 행동-지역화 벤치마크입니다. 사용자 오디오 지시를 스트리밍합니다: "사람이 {행동}을 시작할 때 '시작'이라고 말하고, 멈출 때 '정지'라고 말해줘."
하지만 숫자를 넘어보십시오. 가장 직관적인 데모는 맨 아래에 숨겨져 있는 이 데모입니다. 샘플을 재생하고 AGI를 느껴보십시오:

![](https://substack-post-media.s3.amazonaws.com/public/images/0bfcadcb-b746-4873-aed4-95f19f5897_1478x1676.png)
마무리 노트는 Thinky의 로드맵에 대한 흥미로운 단서들을 남기는데, 여기에는 백그라운드 에이전트와 인터랙티브 모델의 흥미로운 조합이 포함되어 있으며, 저희는 이 점을 매우 높이 평가합니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/ef289b1c-4613-4835-98e6-475906d494da_1394x588.png)
> 2026년 5월 9일-5월 11일 AI 뉴스. 저희는 12개의 subreddits, 544개의 Twitters를 확인했으며, 더 이상의 Discords는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Thinking Machines의 네이티브 인터랙션 모델과 턴 기반 AI를 넘어선 전환
- 전이중 멀티모달 상호작용을 일급 모델 기능으로: 이날의 가장 명확한 기술적 주제는 Thinking Machines가 미리 선보인 "인터랙션 모델"이었습니다. 이는 턴 기반 LLM에 음성, 턴 주고받기, 도구 사용을 겹쳐 쌓는 방식이 아니라 실시간 상호작용을 위해 처음부터 학습된 모델로 설명됩니다. @johnschulman2, @soumithchintala, @cHHillee의 기술 게시물과 팀 논평은 이를 인간↔AI 대역폭 문제로 규정합니다. 즉, 모델은 동시에 듣고, 말하고, 보고, 생각하고, 검색하고, 반응할 수 있어야 한다는 것입니다. 데모는 명시적인 "지금 생각 중 / 지금 검색 중" 경계 없이 지속적인 시간 인식, 중단 처리, 동시 발화, 시각적 주도성, 백그라운드 도구 사용을 강조했습니다. 팀원들은 또한 타입 시그니처가 효과적으로 연속적인 오디오+비디오+텍스트 → 오디오+텍스트가 되면 이전에 특수 목적 시스템이 필요했던 많은 작업이 제로샷으로 가능해진다고 강조했습니다 (@johnschulman2).
- 기술적으로 중요한 이유: 여러 반응이 같은 지점으로 수렴했습니다. 이것은 "또 다른 챗봇 데모"가 아니라 인터페이스 가정의 변화라는 것입니다. @liliyu_lili는 시각적 주도성("내가 구부정하게 앉기 시작할 때 알려줘", "내 팔굽혀펴기 횟수를 세어줘")을 현재 시스템에서 누락된 기본 요소로 지적했습니다. @rown은 이를 시각적으로 주도적인 최초의 일반 비디오+음성 모델이라고 불렀습니다. @kimmonismus와 @giffmana는 둘 다 네이티브 상호작용성이 단순한 벤치마크 주장보다 더 깊은 혁신이라고 강조했습니다. @swyx가 언급했듯이, 이번 출시는 또한 "실시간" 멀티모달 시스템에 대한 기준을 암묵적으로 높입니다. @eliebakouch를 통해 한 가지 구현 세부 사항이 드러났는데, 스택은 SGLang을 사용하고 있습니다.
OpenAI의 엔터프라이즈 및 보안 강화: Deployment Company와 Daybreak
- OpenAI는 서비스 및 배포 분야로 스택을 확장하고 있습니다: OpenAI가 OpenAI Deployment Company를 발표했습니다. 이는 기업이 프론티어 모델을 실제 워크플로우에 배포하도록 돕기 위해 구축된 대주주 소유의 사업부입니다. 핵심 운영 세부 사항은 Tomoro 인수를 통해 150명의 Forward Deployed Engineers와 Deployment Specialists가 합류한다는 것이며, @gdb는 19개 파트너로부터 40억 달러의 초기 투자를 언급했습니다. 여러 관찰자들은 이를 OpenAI가 Palantir/Microsoft 스타일의 현장 엔지니어링 모델을 채택하는 것으로 해석했습니다. @kimmonismus는 OpenAI가 AI 경제의 배포 레이어를 소유하기를 원한다고 주장했으며, @matvelloso는 이를 고객 운영에 기술 직원을 밀접하게 배치하는 역사적인 기업 성공 패턴과 연결했습니다.
- Daybreak: 보안 특정 모델 배포, 워크플로우 및 신뢰 계층: OpenAI는 또한 방어적 사이버 작전 및 소프트웨어 지속 보안을 위한 포괄적인 노력인 Daybreak를 출시했으며, @sama는 이를 빠르게 발전하는 AI 사이버 능력에 대한 실질적인 대응으로 포지셔닝했습니다. @TheRundownAI가 요약한 제품 설명은 GPT-5.5, Codex, 리포지토리 위협 모델링, 취약점 발견, 패치 생성 및 대응 자동화를 결합하며, Trusted Access for Cyber 및 보다 전문화된 GPT-5.5-Cyber를 포함한 차별화된 접근 계층을 제공합니다. 이는 Anthropic의 보다 제한적인 사이버 태세와 대조되며, @kimmonismus가 포착한 긴장입니다. 보안 에이전트 시스템을 구축하는 팀에게는 @lukOlejnik의 별도 경고가 관련이 있습니다: "귀하의 LLM은 보안 경계가 아닙니다." Microsoft Semantic Kernel은 프롬프트 인젝션이 호스트 수준 RCE로 전환되는 것을 허용했다고 보고되었는데, 이는 프레임워크가 모델 자체의 실패보다는 모델 출력을 과도하게 신뢰했기 때문입니다.
에이전트 하네스, 로컬 우선 툴링 및 제어 표면
- 더 나은 에이전트 제어 플레인이 제품 범주가 되고 있습니다: 반복되는 불만은 유용한 에이전트는 자율성이 필요하지만, 엔지니어는 여전히 되돌릴 수 있고 검사 가능한 제어를 원한다는 것입니다. @itsclelia는 로컬/원격, S3 기반 에이전트 아티팩트 저장을 위한 Rust CLI인 aggit으로 이 문제를 해결하여 주요 Git 기록 외부에서 stash/branch/restore 시맨틱을 가능하게 했습니다. 같은 맥락에서, @_catwu는 여러 Claude Code 에이전트를 관리하기 위한 새로운 Claude agents 터미널 제어 플레인을 강조했으며, @cursor_ai는 Cursor를 Microsoft Teams에 도입하여 에이전트가 전체 스레드를 읽고 PR을 엽니다. 이 모든 것은 "에이전트 오케스트레이션"이 단순히 프롬프트 트릭이 아니라 구체적인 UX 패턴으로 수렴하고 있다는 신호입니다.
- Deep Agents / Hermes / 로컬 에이전트가 빠르게 성숙하고 있습니다: @masondrxy는 Deep Agents CLI가 컨텍스트를 잃지 않고 대화 중에 기본 모델 제공자를 핫스왑할 수 있다고 언급했는데, 이는 많은 에이전트 스택이 여전히 놓치고 있는 사소하지 않은 시스템 기능입니다. LangChain은 또한 제공자/모델 특정 파인튜닝을 위한 하네스 프로필을 강조했으며 (트윗), 같은 저자의 별도 가격 분석은 DeepSeek V4 Flash가 대량 에이전트 워크로드에 대해 GPT/Gemini 플래시 티어 옵션보다 훨씬 저렴할 수 있다고 주장했습니다 (트윗). 로컬 측면에서는 Hugging Face가 로컬 앱에 Hermes Agent 지원과 네이티브 트레이스 시각화를 추가했으며, @Teknium은 Hermes Agent와 CUA를 통해 모든 모델로 컴퓨터를 사용하는 것을 미리 선보이며 프론티어 API뿐만 아니라 로컬/오픈 모델도 명시적으로 목표로 했습니다. @onusoz가 Hugging Face에 합류하여 OpenClaw 및 관련 오픈 하네스에서 로컬 모델을 개선하는 것은 로컬 에이전트 인체공학이 이제 전략적 인프라가 되었다는 또 다른 강력한 신호입니다.
- 도구 주변에서 나타나는 디자인 논제: @threepointone은 에이전트가 점근적으로 단 두 가지 기본 도구, 즉 검색과 실행만을 원할 수 있으며, 끊임없이 확장되는 정적 도구 메뉴 대신 기능의 동적 의미론적 발견을 통해 작동할 수 있다고 주장했습니다. 이는 거대한 모놀리식 프롬프트 대신 구성 가능한 하네스를 향한 광범위한 움직임을 보완합니다.
벤치마크, 효율성 및 오픈 모델 경제학
- 코딩 에이전트 벤치마킹이 마침내 하네스+모델 쌍을 측정하고 있습니다: Artificial Analysis는 SWE-Bench-Pro-Hard-AA, Terminal-Bench v2, SWE-Atlas-QnA를 아우르는 Coding Agent Index를 출시하여 모델뿐만 아니라 모델+하네스 조합을 비교했습니다. 그들의 주요 결과는 다음과 같습니다: Cursor CLI의 Opus 4.7이 61점을 기록했으며, Codex/Claude Code의 GPT-5.5가 그 뒤를 바짝 쫓았습니다. 최고의 오픈 웨이트 설정에는 Claude Code의 GLM-5.1, Kimi K2.6, DeepSeek V4 Pro가 포함되었으며, 여전히 경쟁력이 있지만 의미 있게 뒤처졌습니다. 이 벤치마크는 또한 작업당 비용(>30배), 토큰 사용량(>3배), 캐시 적중률(80–96%), 작업당 시간(>7배)에서 큰 차이를 드러냈습니다. 이 벤치마크는 OpenHands의 업데이트된 소프트웨어 엔지니어링 벤치마크 발표 (트윗)와 Claw-Eval의 사무, 금융, 터미널, 웹 작업을 아우르는 보다 에이전틱한 작업 구성으로 보완되었는데, 여기서 MiMo-V2.5-Pro가 선두를 차지했고 DeepSeek V4 Flash는 그 크기에 비해 이례적으로 효율적으로 보였습니다.
- TurboQuant에 대한 회의론이 증가하고 있습니다: 여러 게시물에서 최근 인기 있는 양자화/서빙 기술에 대한 보다 신중한 견해를 지적했습니다. @_EldarKurtic은 TurboQuant에 대한 최초의 포괄적인 연구라고 설명한 것을 발표했으며, 정확도, 레이턴시, 처리량을 다루었습니다. @vllm_project는 Red Hat / vLLM 조사를 시작점으로 연결했으며, @jbhuang0604는 핵심 내용을 "실제로 잘 작동하지 않습니다."라고 솔직하게 요약했습니다. 이것은 독립적인 재현이 중요한 인프라 주장의 전형적인 예입니다.
- 로컬/오픈 모델은 하드웨어 한계보다 빠르게 계속 개선되고 있습니다: @ClementDelangue는 여기서 가장 강력한 고수준 주장을 펼쳤습니다. 동일한 최고급 MacBook Pro 메모리 한계 내에서, 실제로 실행할 수 있는 "가장 똑똑한 오픈 웨이트 모델"은 24개월 동안 약 4.7배 개선되어 Llama 3 70B 시대의 능력에서 DeepSeek V4 Flash mixed-Q2 GGUF 시대의 능력으로 발전했습니다. 이는 10.7개월마다 두 배로 증가하는 것을 의미하며, 무어의 법칙보다 빠릅니다. 지지 데이터 포인트는 GGUF 업로드의 빠른 증가에 대한 @victormustar의 언급과 Qwen 3.6, Gemma 4, DeepSeek 변형 모델이 이제 사소하지 않은 에이전트 작업에 로컬에서 사용 가능하다는 반복적인 커뮤니티 관찰에서 나왔습니다.
연구 하이라이트: MoE 모듈성, 확산/바이트 모델 및 에이전트 역학
- 아키텍처 및 평가: @TheTuringPost는 AllenAI의 EMO를 문서 수준 라우팅이 공유 전문가 풀을 유도하는 보다 모듈식 Mixture-of-Experts 설계로 강조했습니다. 특히, 전문가의 25%만 유지하는 것이 유사한 가지치기 하에서 표준 MoE의 10–15% 성능 저하에 비해 단 ~1%의 성능 손실만 발생한다고 보고되었습니다 (후속). 생성 평가에서는 @qberthet이 FID를 대체하는 더 빠르고 샘플 효율적인 방법으로 MIND (Monge Inception Distance)를 소개했습니다.
- 언어 및 바이트 수준 모델링을 위한 확산: 여러 논문에서 비-AR 언어 모델링을 추진했습니다. @LucaAmb는 연속 비트스트림 확산이 그들의 평가 설정에서 자기회귀 모델과 거의 일치한다고 보고했습니다. @JulieKallini는 병렬 바이트 디코딩을 위해 확산을 사용하여 바이트 수준 LM이 인퍼런스 바운드되는 것을 줄이는 Fast BLT를 소개했습니다. @sriniiyer88은 이를 블록 바이트 확산과 자기-추측 디코딩을 결합하는 것으로 설명했습니다. 관련하여, @LiangZheng_06은 사후 학습을 위한 확산 모델의 유용한 속성을 언급했는데, 샘플링이 미분 가능하기 때문에 보상 기울기가 표준 LLM 설정보다 더 직접적으로 파라미터로 흐를 수 있다는 것입니다.
- 장기적인 관점에서의 에이전트 행동: 두 가지 강력한 실증적 흐름이 나타났습니다. 첫째, "The Memory Curse"는 모델이 이력을 더 따르고 위험을 최소화하려는 경향이 있으며, 명시적인 CoT가 때때로 문제를 증폭시키기 때문에 긴 이력이 다중 라운드 사회적 딜레마에서 협력을 저하시킨다고 주장합니다. 둘째, @dair_ai가 요약한 PwC 연구는 명확화의 가치가 시간에 따라 크게 달라진다고 주장합니다. 목표 명확화는 실행의 약 10% 이후에 대부분의 가치를 잃는 반면, 입력 명확화는 더 오래 유용하게 유지됩니다. 이들을 종합하면, 장기적인 에이전트 품질은 원시 모델 IQ만큼이나 메모리/제어 정책에 의해 제약된다는 것을 시사합니다.
- 스케일링 및 자기 개선: @WilliamBarrHeld가 요약한 Marin의 Delphi 스케일링 작업은 작은 사전 학습에서 25B / 600B 토큰 실행으로 외삽할 때 0.2%의 예측 오류를 주장합니다. 별도로, @omarsar0은 AutoTTS를 강조했는데, 여기서 LLM이 테스트 시간 스케일링 컨트롤러 공간을 스스로 검색하며, 약 39.9달러의 발견 비용으로 수동으로 설계된 전략을 능가했다고 보고되었습니다.
인기 트윗 (참여도 기준)
- OpenAI의 엔터프라이즈/서비스 전환: OpenAI가 Deployment Company를 출시하고 Tomoro 인수 / 150 FDE를 발표했습니다.
- OpenAI의 보안 제품화: Daybreak 발표 및 @sama의 설명.
- Thinking Machines의 인터랙션 모델: Mira Murati의 출시 트윗 및 기술 미리보기 스레드.
- Artificial Analysis Coding Agent Index: 벤치마크 출시 및 주요 결과.
- 에이전트 툴링 / 개발자 워크플로우: Hermes Agent를 통한 모든 모델의 컴퓨터 사용, Microsoft Teams의 Cursor, 그리고 Codex OpenAI Developers 플러그인.

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Qwen 3.6 로컬 인퍼런스 발전
- Unsloth의 MTP (활동: 620): 이미지 (링크)는 Unsloth의 Hugging Face 프로필에 새로 게시된 MTP 보존 GGUF 빌드인 unsloth/Qwen3.6-27B-GGUF-MTP와 unsloth/Qwen3.6-35B-A3B-GGUF-MTP를 나열하고 있습니다. 이 게시물의 기술적 중요성은 이 GGUF들이 MTP / 다음 토큰 예측 레이어를 유지하지만, 사용자는 표준 llama.cpp 지원에 의존하기보다는 특정 llama.cpp MTP PR을 빌드해야 한다는 것입니다. 한 댓글 작성자는 27B GGUF에서 런타임/어설션 실패를 보고했습니다: GGML_ASSERT(hparams.nextn_predict_layers > 0 && "QWEN35_MTP requires nextn_predict_layers > 0"). 이는 메타데이터 파싱, 모델 변환 또는 PR 호환성 문제가 해결되지 않았음을 시사합니다. 댓글들은 업스트림 llama.cpp MTP 지원에 대한 기대를 반영하며, 사용자들은 GitHub 리포지토리를 반복적으로 확인하고 MTP가 이제 "별도의 설정 없이" 지원되는지 묻고 있습니다. 새로운 27B GGUF 모델을 컴파일하던 한 사용자가 qwen35_mtp.cpp에서 런타임 어설션에 부딪혔습니다: GGML_ASSERT(hparams.nextn_predict_layers > 0 && "QWEN35_MTP requires nextn_predict_layers > 0"). 이는 GGUF/모델 메타데이터 또는 변환 경로에 nextn_predict_layers가 누락되어 있을 수 있음을 시사하며, 이는 Qwen3.5 MTP 추측성/다음 토큰 예측 레이어에 필요합니다. 한 기술 스레드는 GGUF의 MTP 지원이 로컬 인퍼런스에 중요하며, 특히 댓글 작성자들이 향상된 컨텍스트 길이 처리와 연관시키는 35B A3B 변형에 중요하다고 언급합니다. 또 다른 댓글 작성자는 이것이 llama.cpp가 이제 MTP를 "별도의 설정 없이" 지원한다는 의미인지 물으며, 지원이 병합/안정적인지 아니면 PR 또는 포크에서만 사용 가능한지에 대한 불확실성을 시사합니다. 한 댓글 작성자는 ik_llama MTP가 현재 llama.cpp PR보다 빠르며, "turboquants"와 유사하다고 설명되는 Hadamard 기반 양자화를 지원한다고 주장합니다. 이는 로컬 MTP 인퍼런스 백엔드를 비교하는 사용자에게 잠재적으로 관련 있는 구현/성능 차이입니다.

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-thinking-machines-native-interaction&utm_source=paywall-free-trial&utm_medium=web&utm_content=197305557&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-thinking-machines-native-interaction&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
