# Founders and Forward Deployed Engineers

**원문 URL**: https://www.latent.space/p/ainews-founders-and-forward-deployed
**번역일**: 2026-05-30 06:18
**발행일**: 2026-05-30

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 파운더스 및 포워드 디플로이드 엔지니어

### 조용한 하루 덕분에 새로운 AIE WF의 초점을 강조할 수 있었습니다.
대부분의 사람들은 어제 발표된 Anthropic의 대규모 소식을 여전히 소화하고 있습니다.
저희는 OpenAI DeployCo와 Anthropic DeployCo의 유사한 추진을 반영하여, AIE의 새로운 포워드 디플로이드 엔지니어 트랙을 위해 세계 최고의 AI FDE를 모집하는 기회로 삼고 있습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/b92541e3-151a-4f10-8226-b86cb12eaca0_2332x1344.png)
또한 AIE의 새로운 파운더스 프로그램도 진행하고 있습니다. 이 프로그램에서는 YCombinator의 Garry Tan과 Howie Lu의 1천만 달러 규모 Hyperagent 콘테스트를 주최로 하는 경쟁 피치 콘테스트인 저희 버전의 스타트업 배틀필드를 개최합니다. 관심 있으신 분은 오늘 바로 등록(및 호텔 예약!)하여 자세한 내용을 확인하십시오.

![](https://substack-post-media.s3.amazonaws.com/public/images/aa6ef073-049b-4bd8-b183-4a49f1a913f8_2276x1306.png)
> 2026년 5월 28일~2026년 5월 29일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터를 확인했으며 추가 Discord는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Claude Opus 4.8 출시, 벤치마크 마찰 및 API 인체공학
- Opus 4.8은 시끄럽고 혼합된 평가 환경에 출시되었습니다. 여러 독립 벤치마크는 "점진적이지만 지배적이지는 않다"는 결론에 수렴했습니다. @arena는 Opus 4.8과 이전 Opus 변형, Gemini, GLM을 비교하는 200개 이상의 프론트엔드/코드 테스트를 진행했습니다. @theo는 CursorBench에서 4.7보다 더 효율적이지만 오차 범위 내에서 약간 더 나쁘다고 보고했습니다. @jerryjliu0와 @llama_index는 문서 파싱에서 테이블/레이아웃에서 작은 개선을 발견했지만, 콘텐츠 충실도/차트에서는 회귀를 발견했습니다. @scaling01은 ALE-Bench에서 진전이 없었으며 LisanBench에서 흥미로운 실패 모드를 별도로 지적했습니다. 긍정적인 측면에서는 @jeremyphoward가 코딩에서 4.8이 4.7/GPT-5.5보다 과도하게 에이전틱하지 않고 더 협력적이라고 발견했으며, @leo_linsky는 이를 이전 Anthropic 릴리스에 비해 실질적인 제품 개선이라고 평가했습니다.
- Anthropic은 또한 유용한 플랫폼 수준 변경 사항을 출시했습니다. @ClaudeDevs는 프롬프트 캐시를 깨뜨리지 않고 대화 중간 시스템 지침을 발표했으며, 장기 에이전트 세션 및 비용 제어에 중요한 권위 있는 대화 중간 시스템 역할 업데이트도 발표했습니다. 그러나 가격은 여전히 주요 불만 사항입니다. @jeremyphoward는 Anthropic이 API 경제성을 위해 거의 노력하지 않았으며, 구독/API 경제성이 정당화하기 더 쉽기 때문에 GPT-5.5를 선호한다고 주장했습니다. 전반적인 결론은 4.8이 깔끔한 벤치마크 리셋이 아니라 실제 사용을 위한 의미 있는 삶의 질 개선 릴리스라는 것입니다.
에이전트 하네스, 다중 턴 RL 버그 및 자율성 주변 인프라
- 미묘하지만 중요한 RL 실패 모드가 지적되었습니다. @ClementDelangue는 많은 도구 사용, 다중 턴 RL 학습 루프가 조용히 고장나는 이유에 대한 Hugging Face의 심층 분석을 강조했습니다. 핵심 버그는 모델 출력을 디코딩하고, 도구 호출을 파싱한 다음, 업데이트된 대화를 재토큰화하면 토큰화가 변경될 수 있으므로, 모델이 실제로 샘플링하지 않은 시퀀스에 그래디언트가 적용된다는 것입니다. 제안된 수정 사항은 엄격한 "토큰 인, 토큰 아웃" 규칙입니다. 샘플링된 토큰을 재인코딩하지 않고, 턴에 걸쳐 단일 토큰 버퍼를 유지하는 것입니다. @johnschulman2는 렌더러가 메시지와 토큰 사이의 기반 인프라이며, 학습/테스트 불일치, 캐싱 비효율성, 프롬프트 인젝션 위험에 이르는 실패 모드를 포함한다는 더 넓은 관점을 강조했습니다.
- 하네스 설계는 그 자체로 최적화 분야가 되고 있습니다. @omarsar0은 유효 피드백 컴퓨트(EFC)에 대한 작업을 표면화하며, 원시 토큰/도구 수가 에이전트 성공을 제대로 설명하지 못하는 반면 EFC는 R²가 0.99에 이르러 하네스 품질이 총 활동보다 더 중요함을 암시한다고 주장했습니다. 이는 @LangChain과 같은 제품화된 튜닝 노력과 일치합니다. LangChain의 Deep Agents v0.6은 Qwen/Kimi/DeepSeek에서 프론티어 API보다 20배 이상 낮은 비용으로 강력한 성능을 얻기 위해 하네스 프로필을 일급 객체로 만들고, @hwchase17은 "다른 모델에는 다른 프롬프트/도구가 필요하다"고 명시적으로 구성했습니다. @vllm_project는 네이티브 가중치 동기화 API와 비동기 RL을 위한 개선된 일시 정지/재개 기능을 출시했으며, 나중에 긴 컨텍스트/에이전틱 워크로드에서 CPU 토큰화 병목 현상을 줄이기 위해 Rust BPE 토크나이저인 패스트토큰을 추가했습니다.
- 논쟁은 "단일 에이전트 대 다중 에이전트"에서 추상화가 효과를 발휘하는 곳으로 전환되고 있습니다. @OfirPress는 현재 다중 에이전트 시스템이 주로 속도 향상이지 기능 잠금 해제가 아니라고 주장했습니다. @scaling01은 반대 견해를 취하며, 스웜 스타일 학습이 더 나은 계획과 초지능적 행동을 산출할 것으로 기대했습니다. 어느 쪽이든 실용적인 추세는 명확합니다. 더 많은 팀이 에이전트 관측성, 트레이스, 지속적인 개선 루프를 중심으로 구축하고 있습니다. 예를 들어, @Vtrivedy10은 SFT/디스틸레이션 및 장기 지속 학습을 위해 프로덕션 트레이스를 마이닝하는 작업을 진행하고 있습니다.
오픈 모델, 로컬 AI 및 OSS 툴체인 강화
- 로컬 우선 및 오픈 웨이트 모멘텀이 계속 상승하고 있습니다. @LangChain은 2026년 4월에 AI 팀 3곳 중 1곳이 오픈 웨이트 모델을 실행했으며, 이는 9개월 전 5곳 중 1곳에서 증가한 수치라고 밝혔습니다. @EpochAIResearch는 오픈 웨이트 모델이 이제 프론티어 독점 모델보다 약 4개월 뒤처진다고 추정했습니다. 툴체인 측면에서는 @ggerganov가 llama.app을 출시하여 llama.cpp에 공식 웹사이트, 통합 설치 프로그램, 더 쉬운 로컬 배포 및 타사 에이전트 통합을 목표로 하는 단일 llama 진입점을 제공했습니다. @ollama는 Ollama를 통해 로컬 우선 개인 AI인 OpenJarvis를 발표했으며, Stanford/Hazy의 "와트당 지능" 구성과 명시적으로 연결했습니다.
- 오픈 인프라가 더 엔터프라이즈 형태로 변모하고 있습니다. @ClementDelangue는 Hugging Face의 모델 및 데이터셋 중 약 50%가 이제 비공개이며, HF의 스토리지/버킷 제공과 함께 증가하고 있다고 언급했습니다. 이는 HF가 공개 OSS 인프라일 뿐이라는 생각에 대한 중요한 수정입니다. @abidlabs는 Hugging Face Jobs가 CPU/서버리스 GPU CI를 위해 GitHub 러너를 대체하는 것을 보여주었습니다. @DSPyOSS, @dbreunig 및 기타 개발자들은 순수 프롬프팅보다는 프로그래밍 가능한 AI 시스템 온보딩에 중점을 둔 다가오는 4.0에 앞서 재설계된 DSPy 문서/첫 페이지를 출시했습니다.
- 라이선싱 및 허용성이 전략적 지렛대가 되고 있습니다. @kimmonismus는 NVIDIA가 4개의 오픈 모델 제품군을 Linux Foundation OpenMDW-1.1로 이동하여 가중치/코드/문서/데이터 전반에 걸쳐 법적 파편화를 줄였다고 강조했습니다. 새로운 허용적인 데이터 릴리스도 중요합니다. @keshigeyan은 시각적 생성을 위한 1억 쌍 허용 이미지 코퍼스 및 100만 쌍 벤치마크인 GPIC를 소개했으며, 명시적인 연구 + 상업적 유용성을 강조했습니다.
Google/OpenAI 제품 표면 확장: 관리형 에이전트, Gemini Spark/Omni 및 Windows용 Codex
- Google은 "관리형 에이전트" 스택을 API에서 소비자 제품으로 확장하고 있습니다. @_philschmid는 Gemini API의 관리형 에이전트를 보여주었습니다. 이는 코드 실행, 웹 액세스 및 파일 I/O를 갖춘 샌드박스형 Linux 환경을 프로비저닝하는 단일 API 호출입니다. 소비자 측면에서는 @GeminiApp이 미국 AI Ultra 구독자에게 Gemini Spark를 출시했습니다. 이는 사용자의 디지털 생태계 전반에서 지시에 따라 작동할 수 있는 24/7 개인 에이전트입니다. Google은 또한 Gemini Omni 멀티모달 생성/편집 데모(예시, 제품 스레드)를 계속 추진했으며, 비디오/영화 제작의 창의적 워크플로우를 위한 Google Flow Agent를 발표했습니다(스레드).
- OpenAI의 Codex는 영구 원격 개발 운영자에 더 가까워지고 있습니다. @OpenAI와 @OpenAIDevs는 ChatGPT 모바일 앱에서 원격 제어를 포함하여 Windows 컴퓨터 사용을 추가했습니다. 후속 UX 개선 사항에는 백그라운드 에이전트용 안정적인 아이덴티콘과 이전 채팅 콘텐츠 검색이 포함되었습니다(@OpenAIDevs). @reach_vb는 Windows 제어, 모바일 원격 액세스, 프로필/작업 통계에 대한 광범위한 Codex 업데이트를 요약했습니다. 별도로 OpenAI는 @michpokrass에 따라 아첨, 사실성 및 다국어 성능을 개선하기 위해 gpt-5.5 instant를 업데이트했습니다.
- 이 모든 것은 모델 + 하네스 + 샌드박스 + UI + 원격 제어 + 가격/할당량으로 구성된 더 수직 통합된 에이전트 스택을 가리킵니다. Google은 Gemini의 할당량을 완화하고 있으며(@joshwoodward), OpenAI는 Codex의 운영 표면을 확장하고 있습니다. Cursor는 서브에이전트 기반 승인 라우팅을 통해 자동 검토 모드를 추가했습니다(트윗). 일반적인 패턴은 "챗봇"보다는 정책 및 메모리를 갖춘 관리형 실행 환경에 가깝습니다.
주목할 만한 연구 및 시스템 논문
- 검색, 리트리벌, 메모리: @TheTuringPost는 Harvard/MIT의 양방향 진화 검색(BES)을 강조했습니다. 이는 순방향 검색과 역방향 분해 및 진화 연산자를 결합한 것입니다. 보고된 개선 사항에는 MuSiQue에서 Llama-3.2-3B-Instruct가 4.0%에서 7.0%로 증가한 것이 포함됩니다. 리트리벌에서는 @_reachsumit이 Latent Terms를 지적하며, 희소 BM25-준비 기능이 SAE를 통해 고정된 밀집 리트리버에서 추출될 수 있음을 보여주었습니다. @topk_io는 더 효율적인 후기 상호작용 인퍼런스를 위해 Iso-ModernColBERT를 오픈소스화했습니다.
- 지속 학습 및 신념/상태 관리: @HuggingPapers는 BeliefTrack을 요약하며, 최적화된 신념 상태 관리가 장기 추론 실패를 70% 이상 줄인다고 주장했습니다. @AndrewLampinen은 지속 학습 분야가 긍정적 전이 대신 간섭에 과도하게 집중했다고 주장했습니다. @victor207755822는 자체 반복 및 CL에 중점을 둔 두 번째 DeliAutoResearch SKILL 논문을 발표했습니다.
- 멀티모달/월드 모델/로봇 공학: NVIDIA 관련 작업에는 24 FPS로 스트리밍되는 생성형 다중 에이전트 월드 모델인 γ-World(트윗)와 실시간 대화형 비디오 월드 모델 프레임워크인 minWM(트윗)이 포함되었습니다. 로봇 공학에서는 @_akhaliq이 Qwen-VLA를 공유했으며, @inventorOli는 Robostral의 언어 따르기 및 조작 개선 사항을 시연했습니다. 상시 작동 선제적 에이전트의 경우, @dair_ai는 LLM 깨우기 결정을 220MiB 시간 그래프 인코더로 대체하여 평균 F1을 +16.7 증가시키면서 4~83배 더 빠르게 실행되는 작업을 표면화했습니다.
(참여도 기준) 인기 트윗
- OpenAI / 생물학: @OpenAI는 Rosalind Biodefense에 대해 공중 보건 및 생물 방어를 위한 신뢰할 수 있는 액세스 생물학 도구를 발표했습니다.
- Google / 소비자 에이전트: @GeminiApp은 Spark에 대해 미국 AI Ultra 사용자에게 상시 작동 개인 에이전트를 출시했습니다.
- OpenAI / 개발 도구: @OpenAI는 Codex Windows 지원 및 @OpenAIDevs가 Windows 컴퓨터 사용 및 모바일 원격 제어로 확장했습니다.
- llama.cpp UX 이정표: @ggerganov는 로컬 AI를 위한 통합 설치 프로그램 및 CLI 진입점을 갖춘 llama.app을 출시했습니다.
- HF / RL 정확성: @ClementDelangue는 도구를 사용하는 다중 턴 RL에 대한 토큰 인, 토큰 아웃 경고를 증폭했습니다.
- 오픈 대 클로즈드 타이밍 격차: @EpochAIResearch는 오픈 웨이트 모델이 이제 프론티어 모델보다 약 4개월 뒤처진다고 추정했습니다.

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. 로컬 LLM 성능: MoE 릴리스, 퀀트, VRAM 절약
- StepFun 3.7 Flash (활동: 637): StepFun은 총 196B 파라미터, 활성 11B, 내장된 1.8B ViT를 갖춘 멀티모달 MoE인 Step 3.7 Flash를 출시했습니다. 이 모델은 최대 400 TPS의 고처리량 에이전트 워크플로우에 광고되었으며, 약 128GB RAM으로 로컬에서 실행 가능하다고 보고되었습니다. 보고된 벤치마크는 플래시 클래스/로컬 모델치고는 이례적으로 강력하게 평가합니다: SWE-Bench Pro 56.26%, DeepSearchQA F1 92.82%, 도구 사용 HLE 47.2, 그리고 Terminal-Bench, Toolathlon, ClawEval 및 기타 에이전틱/도구 사용 작업에서 Step 3.5 Flash에 비해 큰 개선을 보였습니다. 직접 모델 아티팩트는 Hugging Face에서 BF16, FP8, NVFP4, GGUF 형식으로 제공되며, llama.cpp 데이-0 지원 PR 및 llama.cpp#23274의 관련 MTP 작업과 함께 제공됩니다. 댓글 작성자들은 이 모델을 기술적으로 이상하다고 특징지었습니다. 숨겨진/사고 트레이스는 거의 비일관적이라고 설명되지만, 최종 답변은 "완벽"하며 훨씬 큰 1TB 이상 모델과 경쟁할 수 있습니다. 한 사용자는 이전 Step 3.5의 "무한 사고" 문제가 해결된 것으로 보인다고 말했습니다. 로컬 배포에 대한 신중한 열정이 있으며, 특히 4x3090급 하드웨어를 가진 사용자에게 그렇습니다. StepFun이 포크만 유지하는 대신 llama.cpp 지원을 업스트림한 것에 대한 감사도 있습니다. StepFun은 Hugging Face에 여러 Step-3.7-Flash 체크포인트를 출시했습니다: BF16 (Step-3.7-Flash), FP8 (Step-3.7-Flash-FP8), NVFP4 (Step-3.7-Flash-NVFP4), GGUF (Step-3.7-Flash-GGUF). 한 사용자는 이전 Step 3.5 Flash의 "무한 사고" 문제가 해결된 것으로 보이며, 여전히 이상한 중간 추론 스타일을 가지고 있음에도 불구하고 3.7이 더 유용해졌다고 보고합니다. StepFun의 업스트림 PR인 ggml-org/llama.cpp#23845를 통해 llama.cpp 데이-0 활성화가 이루어졌으며, 이는 Step 3.5의 포크 기반 지원과 대조적입니다. MTP 지원을 위한 별도의 커뮤니티 PR이 ggml-org/llama.cpp#23274에 존재하지만, 댓글 작성자들은 Step 3.7 및 현재 마스터에 맞게 업데이트가 필요하다고 언급합니다. 2x Pro 6k에서 64개의 동시 얕은 컨텍스트 요청을 사용한 NVFP4 체크포인트의 vLLM 야간 테스트는 약 2200 tok/s에 도달했습니다. 보고된 구성은 tensor-parallel-size 2, --enable-expert-parallel, --quantization modelopt, --kv-cache-dtype fp8, --reasoning-parser step3p5, 그리고 StepFun 도구 호출 파싱을 사용했습니다. vLLM은 GPU KV 캐시 크기가 1,667,645 토큰이고 262,144 토큰/요청당 최대 동시성이 6.36배라고 보고했습니다.

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 무료 액세스하십시오.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-founders-and-forward-deployed&utm_source=paywall-free-trial&utm_medium=web&utm_content=199815243&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-founders-and-forward-deployed&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
